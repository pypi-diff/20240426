# Comparing `tmp/parfor-2024.3.0.tar.gz` & `tmp/parfor-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parfor-2024.3.0.tar", max compression
+gzip compressed data, was "parfor-2024.4.0.tar", max compression
```

## Comparing `parfor-2024.3.0.tar` & `parfor-2024.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35128 2021-03-19 08:42:10.072818 parfor-2024.3.0/LICENSE
--rw-r--r--   0        0        0     5132 2023-09-08 15:19:34.988686 parfor-2024.3.0/README.md
--rw-r--r--   0        0        0    27278 2024-03-19 17:46:00.561359 parfor-2024.3.0/parfor/__init__.py
--rw-r--r--   0        0        0     4027 2023-10-31 13:23:53.429696 parfor-2024.3.0/parfor/pickler.py
--rw-r--r--   0        0        0      570 2024-03-19 17:43:51.493259 parfor-2024.3.0/pyproject.toml
--rw-r--r--   0        0        0     6014 1970-01-01 00:00:00.000000 parfor-2024.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35128 2021-03-19 08:42:10.072818 parfor-2024.4.0/LICENSE
+-rw-r--r--   0        0        0     5132 2023-09-08 15:19:34.988686 parfor-2024.4.0/README.md
+-rw-r--r--   0        0        0    27640 2024-04-26 16:29:27.585609 parfor-2024.4.0/parfor/__init__.py
+-rw-r--r--   0        0        0     4283 2024-04-15 13:16:29.130534 parfor-2024.4.0/parfor/pickler.py
+-rw-r--r--   0        0        0      603 2024-04-26 16:32:11.817505 parfor-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5915 1970-01-01 00:00:00.000000 parfor-2024.4.0/PKG-INFO
```

### Comparing `parfor-2024.3.0/LICENSE` & `parfor-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parfor-2024.3.0/README.md` & `parfor-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `parfor-2024.3.0/parfor/__init__.py` & `parfor-2024.4.0/parfor/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,101 @@
+from __future__ import annotations
+
 import multiprocessing
 from collections import UserDict
 from contextlib import ExitStack
 from functools import wraps
 from os import getpid
 from time import time
 from traceback import format_exc
+from typing import Any, Callable, Hashable, Iterable, Iterator, NoReturn, Optional, Protocol, Sized, TypeVar
 from warnings import warn
 
 from tqdm.auto import tqdm
 
 from .pickler import dumps, loads
 
 cpu_count = int(multiprocessing.cpu_count())
 
 
+Result = TypeVar('Result')
+Iteration = TypeVar('Iteration')
+Arg = TypeVar('Arg')
+Return = TypeVar('Return')
+
+
 class SharedMemory(UserDict):
-    def __init__(self, manager):
+    def __init__(self, manager: multiprocessing.Manager) -> None:
         super().__init__()
         self.data = manager.dict()  # item_id: dilled representation of object
         self.references = manager.dict()  # item_id: counter
         self.references_lock = manager.Lock()
         self.cache = {}  # item_id: object
         self.trash_can = {}
         self.pool_ids = {}  # item_id: {(pool_id, task_handle), ...}
 
-    def __getstate__(self):
+    def __getstate__(self) -> tuple[dict[int, bytes], dict[int, int], multiprocessing.Lock]:
         return self.data, self.references, self.references_lock
 
-    def __setitem__(self, item_id, value):
+    def __setitem__(self, item_id: int, value: Any) -> None:
         if item_id not in self:  # values will not be changed
             try:
                 self.data[item_id] = False, value
             except Exception:  # only use our pickler when necessary # noqa
                 self.data[item_id] = True, dumps(value, recurse=True)
             with self.references_lock:
                 try:
                     self.references[item_id] += 1
                 except KeyError:
                     self.references[item_id] = 1
             self.cache[item_id] = value  # the id of the object will not be reused as long as the object exists
 
-    def add_item(self, item, pool_id, task_handle):
+    def add_item(self, item: Any, pool_id: int, task_handle: Hashable) -> int:
         item_id = id(item)
         self[item_id] = item
         if item_id in self.pool_ids:
             self.pool_ids[item_id].add((pool_id, task_handle))
         else:
             self.pool_ids[item_id] = {(pool_id, task_handle)}
         return item_id
 
-    def remove_pool(self, pool_id):
+    def remove_pool(self, pool_id: int) -> None:
         """ remove objects used by a pool that won't be needed anymore """
         self.pool_ids = {key: v for key, value in self.pool_ids.items() if (v := {i for i in value if i[0] != pool_id})}
         for item_id in set(self.data.keys()) - set(self.pool_ids):
             del self[item_id]
         self.garbage_collect()
 
-    def remove_task(self, pool_id, task):
+    def remove_task(self, pool_id: int, task: Task) -> None:
         """ remove objects used by a task that won't be needed anymore """
         self.pool_ids = {key: v for key, value in self.pool_ids.items() if (v := value - {(pool_id, task.handle)})}
         for item_id in {task.fun, *task.args, *task.kwargs} - set(self.pool_ids):
             del self[item_id]
         self.garbage_collect()
 
     # worker functions
-    def __setstate__(self, state):
+    def __setstate__(self, state: dict) -> None:
         self.data, self.references, self.references_lock = state
         self.cache = {}
         self.trash_can = None
 
-    def __getitem__(self, item_id):
+    def __getitem__(self, item_id: int) -> Any:
         if item_id not in self.cache:
             dilled, value = self.data[item_id]
             if dilled:
                 value = loads(value)
             with self.references_lock:
                 if item_id in self.references:
                     self.references[item_id] += 1
                 else:
                     self.references[item_id] = 1
             self.cache[item_id] = value
         return self.cache[item_id]
 
-    def garbage_collect(self):
+    def garbage_collect(self) -> None:
         """ clean up the cache """
         for item_id in set(self.cache) - set(self.data.keys()):
             with self.references_lock:
                 try:
                     self.references[item_id] -= 1
                 except KeyError:
                     self.references[item_id] = 0
@@ -98,195 +107,190 @@
             for item_id in set(self.trash_can):
                 if self.references[item_id] == 0:
                     # make sure every process removed the object before removing it in the parent
                     del self.references[item_id]
                     del self.trash_can[item_id]
 
 
-class Chunks:
+class Chunks(Iterable):
     """ Yield successive chunks from lists.
         Usage: chunks(list0, list1, ...)
                chunks(list0, list1, ..., size=s)
                chunks(list0, list1, ..., number=n)
                chunks(list0, list1, ..., ratio=r)
         size:   size of chunks, might change to optimize division between chunks
         number: number of chunks, coerced to 1 <= n <= len(list0)
         ratio:  number of chunks / number of cpus, coerced to 1 <= n <= len(list0)
         both size and number or ratio are given: use number or ratio, unless the chunk size would be bigger than size
         both ratio and number are given: use ratio
     """
 
-    def __init__(self, *iterators, size=None, number=None, ratio=None, length=None, s=None, n=None, r=None):
-        # s, r and n are deprecated
-        if s is not None:
-            warn('parfor: use of \'s\' is deprecated, use \'size\' instead', DeprecationWarning, stacklevel=2)
-            warn('parfor: use of \'s\' is deprecated, use \'size\' instead', DeprecationWarning, stacklevel=3)
-            size = s
-        if n is not None:
-            warn('parfor: use of \'n\' is deprecated, use \'number\' instead', DeprecationWarning, stacklevel=2)
-            warn('parfor: use of \'n\' is deprecated, use \'number\' instead', DeprecationWarning, stacklevel=3)
-            number = n
-        if r is not None:
-            warn('parfor: use of \'r\' is deprecated, use \'ratio\' instead', DeprecationWarning, stacklevel=2)
-            warn('parfor: use of \'r\' is deprecated, use \'ratio\' instead', DeprecationWarning, stacklevel=3)
-            ratio = r
+    def __init__(self, *iterables: Iterable[Any] | Sized[Any], size: int = None, number: int = None,
+                 ratio: float = None, length: int = None) -> None:
         if length is None:
             try:
-                length = min(*[len(iterator) for iterator in iterators]) if len(iterators) > 1 else len(iterators[0])
+                length = min(*[len(iterable) for iterable in iterables]) if len(iterables) > 1 else len(iterables[0])
             except TypeError:
-                raise TypeError('Cannot determine the length of the iterator(s), so the length must be provided as an'
+                raise TypeError('Cannot determine the length of the iterables(s), so the length must be provided as an'
                                 ' argument.')
         if size is not None and (number is not None or ratio is not None):
             if number is None:
                 number = int(cpu_count * ratio)
             if length >= size * number:
                 number = round(length / size)
         elif size is not None:  # size of chunks
             number = round(length / size)
         elif ratio is not None:  # number of chunks
             number = int(cpu_count * ratio)
-        self.iterators = [iter(arg) for arg in iterators]
+        self.iterators = [iter(arg) for arg in iterables]
         self.number_of_items = length
         self.length = max(1, min(length, number))
         self.lengths = [((i + 1) * self.number_of_items // self.length) - (i * self.number_of_items // self.length)
                         for i in range(self.length)]
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Any]:
         for i in range(self.length):
             p, q = (i * self.number_of_items // self.length), ((i + 1) * self.number_of_items // self.length)
             if len(self.iterators) == 1:
                 yield [next(self.iterators[0]) for _ in range(q - p)]
             else:
                 yield [[next(iterator) for _ in range(q-p)] for iterator in self.iterators]
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self.length
 
 
-class ExternalBar:
-    def __init__(self, iterable=None, callback=None, total=0):
+class Bar(Protocol):
+    def update(self, n: int = 1) -> None: ...
+
+
+class ExternalBar(Iterable):
+    def __init__(self, iterable: Iterable = None, callback: Callable[[int], None] = None, total: int = 0) -> None:
         self.iterable = iterable
         self.callback = callback
         self.total = total
         self._n = 0
 
-    def __enter__(self):
+    def __enter__(self) -> ExternalBar:
         return self
 
-    def __exit__(self, *args, **kwargs):
+    def __exit__(self, *args: Any, **kwargs: Any) -> None:
         return
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Any]:
         for n, item in enumerate(self.iterable):
             yield item
             self.n = n + 1
 
-    def update(self, n=1):
+    def update(self, n: int = 1) -> None:
         self.n += n
 
     @property
-    def n(self):
+    def n(self) -> int:
         return self._n
 
     @n.setter
-    def n(self, n):
+    def n(self, n: int) -> None:
         if n != self._n:
             self._n = n
             if self.callback is not None:
                 self.callback(n)
 
 
 class Task:
-    def __init__(self, shared_memory: SharedMemory, pool_id: int, handle: int, fun=None, args=(), kwargs=None):
+    def __init__(self, shared_memory: SharedMemory, pool_id: int, handle: Hashable, fun: Callable[[Any, ...], Any],
+                 args: tuple[Any, ...] = (), kwargs: dict[str, Any] = None) -> None:
         self.pool_id = pool_id
         self.handle = handle
         self.fun = shared_memory.add_item(fun, pool_id, handle)
         self.args = [shared_memory.add_item(arg, pool_id, handle) for arg in args]
         self.kwargs = [] if kwargs is None else [shared_memory.add_item(item, pool_id, handle)
                                                  for item in kwargs.items()]
         self.name = fun.__name__ if hasattr(fun, '__name__') else None
         self.done = False
         self.result = None
         self.pid = None
 
-    def __getstate__(self):
+    def __getstate__(self) -> dict[str, Any]:
         state = self.__dict__
         if self.result is not None:
             state['result'] = dumps(self.result, recurse=True)
         return state
 
-    def __setstate__(self, state):
+    def __setstate__(self, state: dict[str, Any]) -> None:
         self.__dict__.update({key: value for key, value in state.items() if key != 'result'})
         if state['result'] is None:
             self.result = None
         else:
             self.result = loads(state['result'])
 
-    def __call__(self, shared_memory: SharedMemory):
+    def __call__(self, shared_memory: SharedMemory) -> Task:
         if not self.done:
             fun = shared_memory[self.fun] or (lambda *args, **kwargs: None)  # noqa
             args = [shared_memory[arg] for arg in self.args]
             kwargs = dict([shared_memory[kwarg] for kwarg in self.kwargs])
             self.result = fun(*args, **kwargs)  # noqa
             self.done = True
         return self
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         if self.done:
             return f'Task {self.handle}, result: {self.result}'
         else:
             return f'Task {self.handle}'
 
 
 class Context(multiprocessing.context.SpawnContext):
     """ Provide a context where child processes never are daemonic. """
     class Process(multiprocessing.context.SpawnProcess):
         @property
-        def daemon(self):
+        def daemon(self) -> bool:
             return False
 
         @daemon.setter
-        def daemon(self, value):
+        def daemon(self, value: bool) -> None:
             pass
 
 
 class ParPool:
     """ Parallel processing with addition of iterations at any time and request of that result any time after that.
         The target function and its argument can be changed at any time.
     """
-    def __init__(self, fun=None, args=None, kwargs=None, bar=None):
+    def __init__(self, fun: Callable[[Any, ...], Any] = None,
+                 args: tuple[Any] = None, kwargs: dict[str, Any] = None, bar: Bar = None):
         self.id = id(self)
         self.handle = 0
         self.tasks = {}
         self.bar = bar
         self.bar_lengths = {}
         self.spool = PoolSingleton(self)
         self.manager = self.spool.manager
         self.fun = fun
         self.args = args
         self.kwargs = kwargs
         self.is_started = False
         self.last_task = None
 
-    def __getstate__(self):
+    def __getstate__(self) -> NoReturn:
         raise RuntimeError(f'Cannot pickle {self.__class__.__name__} object.')
 
-    def __enter__(self, *args, **kwargs):
+    def __enter__(self) -> ParPool:
         return self
 
-    def __exit__(self, *args, **kwargs):
+    def __exit__(self, *args: Any, **kwargs: Any) -> None:
         self.close()
 
-    def close(self):
+    def close(self) -> None:
         self.spool.remove_pool(self.id)
 
-    def __call__(self, n, handle=None, barlength=1):
+    def __call__(self, n: Any, handle: Hashable = None, barlength: int = 1) -> None:
         self.add_task(args=(n, *(() if self.args is None else self.args)), handle=handle, barlength=barlength)
 
-    def add_task(self, fun=None, args=None, kwargs=None, handle=None, barlength=1):
+    def add_task(self, fun: Callable[[Any, ...], Any] = None, args: tuple[Any, ...] = None,
+                 kwargs: dict[str, Any] = None, handle: Hashable = None, barlength: int = 1) -> Optional[int]:
         if self.id not in self.spool.pools:
             raise ValueError(f'this pool is not registered (anymore) with the pool singleton')
         if handle is None:
             new_handle = self.handle
             self.handle += 1
         else:
             new_handle = handle
@@ -297,19 +301,19 @@
         self.tasks[new_handle] = task
         self.last_task = task
         self.spool.add_task(task)
         self.bar_lengths[new_handle] = barlength
         if handle is None:
             return new_handle
 
-    def __setitem__(self, handle, n):
+    def __setitem__(self, handle: Hashable, n: Any) -> None:
         """ Add new iteration. """
         self(n, handle=handle)
 
-    def __getitem__(self, handle):
+    def __getitem__(self, handle: Hashable) -> Any:
         """ Request result and delete its record. Wait if result not yet available. """
         if handle not in self:
             raise ValueError(f'No handle: {handle} in pool')
         while not self.tasks[handle].done:
             if not self.spool.get_from_queue() and not self.tasks[handle].done and self.is_started \
                     and not self.working:
                 for _ in range(10):  # wait some time while processing possible new messages
@@ -319,61 +323,64 @@
                     # retry a task if the process was killed while working on a task
                     self.spool.add_task(self.tasks[handle])
                     warn(f'Task {handle} was restarted because the process working on it was probably killed.')
         result = self.tasks[handle].result
         self.tasks.pop(handle)
         return result
 
-    def __contains__(self, handle):
+    def __contains__(self, handle: Hashable) -> bool:
         return handle in self.tasks
 
-    def __delitem__(self, handle):
+    def __delitem__(self, handle: Hashable) -> None:
         self.tasks.pop(handle)
 
-    def get_newest(self):
+    def get_newest(self) -> Any:
         return self.spool.get_newest_for_pool(self)
 
-    def process_queue(self):
+    def process_queue(self) -> None:
         self.spool.process_queue()
 
-    def task_error(self, handle, error):
+    def task_error(self, handle: Hashable, error: Exception) -> None:
         if handle in self:
             task = self.tasks[handle]
             print(f'Error from process working on iteration {handle}:\n')
             print(error)
             print('Retrying in main thread...')
             task(self.spool.shared_memory)
+            self.spool.shared_memory.remove_task(self.id, task)
             raise Exception(f'Function \'{task.name}\' cannot be executed by parfor, amend or execute in serial.')
-        self.spool.shared_memory.remove_task(self.id, self.tasks[handle])
 
-    def done(self, task):
+    def done(self, task: Task) -> None:
         if task.handle in self:  # if not, the task was restarted erroneously
             self.tasks[task.handle] = task
             if hasattr(self.bar, 'update'):
                 self.bar.update(self.bar_lengths.pop(task.handle))
         self.spool.shared_memory.remove_task(self.id, task)
 
-    def started(self, handle, pid):
+    def started(self, handle: Hashable, pid: int) -> None:
         self.is_started = True
         if handle in self:  # if not, the task was restarted erroneously
             self.tasks[handle].pid = pid
 
     @property
-    def working(self):
+    def working(self) -> bool:
         return not all([task.pid is None for task in self.tasks.values()])
 
 
 class PoolSingleton:
     """ There can be only one pool at a time, but the pool can be restarted by calling close() and then constructing a
         new pool. The pool will close itself after 10 minutes of idle time. """
-    def __new__(cls, *args, **kwargs):
-        if hasattr(cls, 'instance') and cls.instance is not None:  # noqa restart if any workers have shut down
+
+    instance = None
+
+    def __new__(cls, *args: Any, **kwargs: Any) -> PoolSingleton:
+        if cls.instance is not None:  # restart if any workers have shut down
             if cls.instance.n_workers.value < cls.instance.n_processes:
                 cls.instance.close()
-        if not hasattr(cls, 'instance') or cls.instance is None or not cls.instance.is_alive:  # noqa
+        if cls.instance is None or not cls.instance.is_alive:
             new = super().__new__(cls)
             new.n_processes = cpu_count
             new.instance = new
             new.is_started = False
             ctx = Context()
             new.n_workers = ctx.Value('i', new.n_processes)
             new.event = ctx.Event()
@@ -383,40 +390,40 @@
             new.shared_memory = SharedMemory(new.manager)
             new.pool = ctx.Pool(new.n_processes,
                                 Worker(new.shared_memory, new.queue_in, new.queue_out, new.n_workers, new.event))
             new.is_alive = True
             new.handle = 0
             new.pools = {}
             cls.instance = new
-        return cls.instance  # noqa
+        return cls.instance
 
-    def __init__(self, parpool=None):  # noqa
+    def __init__(self, parpool: Parpool = None) -> None:  # noqa
         if parpool is not None:
             self.pools[parpool.id] = parpool
 
-    def __getstate__(self):
+    def __getstate__(self) -> NoReturn:
         raise RuntimeError(f'Cannot pickle {self.__class__.__name__} object.')
 
     # def __del__(self):
     #     self.close()
 
-    def remove_pool(self, pool_id):
+    def remove_pool(self, pool_id: int) -> None:
         self.shared_memory.remove_pool(pool_id)
         if pool_id in self.pools:
             self.pools.pop(pool_id)
 
-    def error(self, error):
+    def error(self, error: Exception) -> NoReturn:
         self.close()
         raise Exception(f'Error occurred in worker: {error}')
 
-    def process_queue(self):
+    def process_queue(self) -> None:
         while self.get_from_queue():
             pass
 
-    def get_from_queue(self):
+    def get_from_queue(self) -> bool:
         """ Get an item from the queue and store it, return True if more messages are waiting. """
         try:
             code, pool_id, *args = self.queue_out.get(True, 0.02)
             if pool_id is None:
                 getattr(self, code)(*args)
             elif pool_id in self.pools:
                 getattr(self.pools[pool_id], code)(*args)
@@ -426,34 +433,34 @@
                 for handle, task in pool.tasks.items():  # retry a task if the process doing it was killed
                     if task.pid is not None \
                             and task.pid not in [child.pid for child in multiprocessing.active_children()]:
                         self.queue_in.put(task)
                         warn(f'Task {task.handle} was restarted because process {task.pid} was probably killed.')
             return False
 
-    def add_task(self, task):
+    def add_task(self, task: Task) -> None:
         """ Add new iteration, using optional manually defined handle."""
         if self.is_alive and not self.event.is_set():
             while self.queue_in.full():
                 self.get_from_queue()
             self.queue_in.put(task)
         self.shared_memory.garbage_collect()
 
-    def get_newest_for_pool(self, pool):
+    def get_newest_for_pool(self, pool: ParPool) -> tuple[Hashable, Any]:
         """ Request the newest key and result and delete its record. Wait if result not yet available. """
         while len(pool.tasks):
             self.get_from_queue()
             for task in pool.tasks.values():
                 if task.done:
                     handle, result = task.handle, task.result
                     pool.tasks.pop(handle)
                     return handle, result
 
     @classmethod
-    def close(cls):
+    def close(cls) -> None:
         if hasattr(cls, 'instance') and cls.instance is not None:
             instance = cls.instance
             cls.instance = None
 
             def empty_queue(queue):
                 try:
                     if not queue._closed:  # noqa
@@ -461,61 +468,63 @@
                             try:
                                 queue.get(True, 0.02)
                             except multiprocessing.queues.Empty:  # noqa
                                 pass
                 except OSError:
                     pass
 
-            def close_queue(queue):
-                empty_queue(queue)
+            def close_queue(queue: multiprocessing.queues.Queue) -> None:
+                empty_queue(queue)  # noqa
                 if not queue._closed:  # noqa
                     queue.close()
                 queue.join_thread()
 
             if instance.is_alive:
-                instance.is_alive = False  # noqa
+                instance.is_alive = False
                 instance.event.set()
                 instance.pool.close()
                 t = time()
-                while instance.n_workers.value:  # noqa
-                    empty_queue(instance.queue_in)  # noqa
-                    empty_queue(instance.queue_out)  # noqa
+                while instance.n_workers.value:
+                    empty_queue(instance.queue_in)
+                    empty_queue(instance.queue_out)
                     if time() - t > 10:
-                        warn(f'Parfor: Closing pool timed out, {instance.n_workers.value} processes still alive.')  # noqa
+                        warn(f'Parfor: Closing pool timed out, {instance.n_workers.value} processes still alive.')
                         instance.pool.terminate()
                         break
-                empty_queue(instance.queue_in)  # noqa
-                empty_queue(instance.queue_out)  # noqa
+                empty_queue(instance.queue_in)
+                empty_queue(instance.queue_out)
                 instance.pool.join()
-                close_queue(instance.queue_in)  # noqa
-                close_queue(instance.queue_out)  # noqa
+                close_queue(instance.queue_in)
+                close_queue(instance.queue_out)
                 instance.manager.shutdown()
-                instance.handle = 0  # noqa
+                instance.handle = 0
 
 
 class Worker:
     """ Manages executing the target function which will be executed in different processes. """
     nested = False
 
-    def __init__(self, shared_memory: SharedMemory, queue_in, queue_out, n_workers, event):
+    def __init__(self, shared_memory: SharedMemory, queue_in: multiprocessing.queues.Queue,
+                 queue_out: multiprocessing.queues.Queue, n_workers: multiprocessing.Value,
+                 event: multiprocessing.Event) -> None:
         self.shared_memory = shared_memory
         self.queue_in = queue_in
         self.queue_out = queue_out
         self.n_workers = n_workers
         self.event = event
 
-    def add_to_queue(self, *args):
+    def add_to_queue(self, *args: Any) -> None:
         while not self.event.is_set():
             try:
                 self.queue_out.put(args, timeout=0.1)
                 break
             except multiprocessing.queues.Full:  # noqa
                 continue
 
-    def __call__(self):
+    def __call__(self) -> None:
         Worker.nested = True
         pid = getpid()
         last_active_time = time()
         while not self.event.is_set() and time() - last_active_time < 600:
             try:
                 task = self.queue_in.get(True, 0.02)
                 try:
@@ -533,16 +542,18 @@
                 self.shared_memory.garbage_collect()
         for child in multiprocessing.active_children():
             child.kill()
         with self.n_workers:
             self.n_workers.value -= 1
 
 
-def pmap(fun, iterable=None, args=None, kwargs=None, total=None, desc=None, bar=True, terminator=None,
-         serial=None, length=None, **bar_kwargs):
+def pmap(fun: Callable[[Iteration, Any, ...], Result], iterable: Iterable[Iteration] = None,
+         args: tuple[Any, ...] = None, kwargs: dict[str, Any] = None, total: int = None, desc: str = None,
+         bar: Bar | bool = True, terminator: Callable[[], None] = None, serial: bool = None, length: int = None,
+         **bar_kwargs: Any) -> list[Result]:
     """ map a function fun to each iteration in iterable
         use as a function: pmap
         use as a decorator: parfor
         best use: iterable is a generator and length is given to this function as 'total'
 
         required:
             fun:    function taking arguments: iteration from  iterable, other arguments defined in args & kwargs
@@ -616,65 +627,46 @@
     is_chunked = isinstance(iterable, Chunks)
     if is_chunked:
         chunk_fun = fun
     else:
         iterable = Chunks(iterable, ratio=5, length=total)
 
         @wraps(fun)
-        def chunk_fun(iterator, *args, **kwargs):  # noqa
-            return [fun(i, *args, **kwargs) for i in iterator]  # noqa
+        def chunk_fun(iterable: Iterable, *args: Any, **kwargs: Any) -> list[Result]:  # noqa
+            return [fun(iteration, *args, **kwargs) for iteration in iterable]
 
     args = args or ()
     kwargs = kwargs or {}
 
     if 'total' not in bar_kwargs:
         bar_kwargs['total'] = sum(iterable.lengths)
     if 'desc' not in bar_kwargs:
         bar_kwargs['desc'] = desc
     if 'disable' not in bar_kwargs:
         bar_kwargs['disable'] = not bar
     if serial is True or (serial is None and len(iterable) < min(cpu_count, 4)) or Worker.nested:  # serial case
         if callable(bar):
             return sum([chunk_fun(c, *args, **kwargs) for c in ExternalBar(iterable, bar)], [])
         else:
-            return sum([chunk_fun(c, *args, **kwargs) for c in tqdm(iterable, **bar_kwargs)], [])  # noqa
+            return sum([chunk_fun(c, *args, **kwargs) for c in tqdm(iterable, **bar_kwargs)], [])
     else:   # parallel case
         with ExitStack() as stack:
             if callable(bar):
-                bar = stack.enter_context(ExternalBar(callback=bar))  # noqa
+                bar = stack.enter_context(ExternalBar(callback=bar))
             else:
-                bar = stack.enter_context(tqdm(**bar_kwargs))  # noqa
+                bar = stack.enter_context(tqdm(**bar_kwargs))
             with ParPool(chunk_fun, args, kwargs, bar) as p:
                 for i, (j, l) in enumerate(zip(iterable, iterable.lengths)):  # add work to the queue
                     p(j, handle=i, barlength=iterable.lengths[i])
                     if bar.total is None or bar.total < i+1:
                         bar.total = i+1
                 if is_chunked:
                     return [p[i] for i in range(len(iterable))]
                 else:
                     return sum([p[i] for i in range(len(iterable))], [])  # collect the results
 
 
 @wraps(pmap)
-def parfor(*args, **kwargs):
-    def decfun(fun):
+def parfor(*args: Any, **kwargs: Any) -> Callable[[Callable[[Iteration, Any, ...], Result]], list[Result]]:
+    def decfun(fun: Callable[[Iteration, Any, ...], Result]) -> list[Result]:
         return pmap(fun, *args, **kwargs)
     return decfun
-
-
-def deprecated(cls, name):
-    """ This is a decorator which can be used to mark functions and classes as deprecated. It will result in a warning
-        being emitted when the function or class is used."""
-    @wraps(cls)
-    def wrapper(*args, **kwargs):
-        warn(f'parfor: use of \'{name}\' is deprecated, use \'{cls.__name__}\' instead',
-             category=DeprecationWarning, stacklevel=2)
-        warn(f'parfor: use of \'{name}\' is deprecated, use \'{cls.__name__}\' instead',
-             category=DeprecationWarning, stacklevel=3)
-        return cls(*args, **kwargs)
-    return wrapper
-
-
-# backwards compatibility
-parpool = deprecated(ParPool, 'parpool')
-Parpool = deprecated(ParPool, 'Parpool')
-chunks = deprecated(Chunks, 'chunks')
```

### Comparing `parfor-2024.3.0/parfor/pickler.py` & `parfor-2024.4.0/parfor/pickler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
+from __future__ import annotations
+
 import copyreg
 from io import BytesIO
 from pickle import PicklingError
+from typing import Any, Callable
 
 import dill
 
 loads = dill.loads
 
 
 class CouldNotBePickled:
-    def __init__(self, class_name):
+    def __init__(self, class_name: str) -> None:
         self.class_name = class_name
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"Item of type '{self.class_name}' could not be pickled and was omitted."
 
     @classmethod
-    def reduce(cls, item):
+    def reduce(cls, item: Any) -> tuple[Callable[[str], CouldNotBePickled], tuple[str]]:
         return cls, (type(item).__name__,)
 
 
 class Pickler(dill.Pickler):
     """ Overload dill to ignore unpicklable parts of objects.
         You probably didn't want to use these parts anyhow.
         However, if you did, you'll have to find some way to make them picklable.
     """
-    def save(self, obj, save_persistent_id=True):
+    def save(self, obj: Any, save_persistent_id: bool = True) -> None:
         """ Copied from pickle and amended. """
         self.framer.commit_frame()
 
         # Check for persistent id (defined by a subclass)
         pid = self.persistent_id(obj)
         if pid is not None and save_persistent_id:
             self.save_pers(pid)
@@ -89,27 +92,28 @@
             return
 
         # Assert that reduce() returned a tuple
         if not isinstance(rv, tuple):
             raise PicklingError("%s must return string or tuple" % reduce)
 
         # Assert that it returned an appropriately sized tuple
-        l = len(rv)
-        if not (2 <= l <= 6):
+        length = len(rv)
+        if not (2 <= length <= 6):
             raise PicklingError("Tuple returned by %s must have "
                                 "two to six elements" % reduce)
 
         # Save the reduce() output and finally memoize the object
         try:
             self.save_reduce(obj=obj, *rv)
         except Exception:  # noqa
             self.save_reduce(obj=obj, *CouldNotBePickled.reduce(obj))
 
 
-def dumps(obj, protocol=None, byref=None, fmode=None, recurse=True, **kwds):
+def dumps(obj: Any, protocol: str = None, byref: bool = None, fmode: str = None, recurse: bool = True,
+          **kwds: Any) -> bytes:
     """pickle an object to a string"""
     protocol = dill.settings['protocol'] if protocol is None else int(protocol)
     _kwds = kwds.copy()
     _kwds.update(dict(byref=byref, fmode=fmode, recurse=recurse))
-    file = BytesIO()
-    Pickler(file, protocol, **_kwds).dump(obj)
-    return file.getvalue()
+    with BytesIO() as file:
+        Pickler(file, protocol, **_kwds).dump(obj)
+        return file.getvalue()
```

### Comparing `parfor-2024.3.0/PKG-INFO` & `parfor-2024.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: parfor
-Version: 2024.3.0
+Version: 2024.4.0
 Summary: A package to mimic the use of parfor as done in Matlab.
 Home-page: https://github.com/wimpomp/parfor
 License: GPLv3
 Keywords: parfor,concurrency,multiprocessing,parallel
 Author: Wim Pomp
 Author-email: wimpomp@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: test
 Requires-Dist: dill (>=0.3.0)
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: tqdm (>=4.50.0)
```

