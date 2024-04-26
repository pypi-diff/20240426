# Comparing `tmp/queue_api-0.1.4.tar.gz` & `tmp/queue_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_api-0.1.4.tar", last modified: Tue Apr 23 13:05:37 2024, max compression
+gzip compressed data, was "queue_api-0.1.5.tar", last modified: Fri Apr 26 06:54:30 2024, max compression
```

## Comparing `queue_api-0.1.4.tar` & `queue_api-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.250655 queue_api-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-23 13:05:37.250655 queue_api-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-04-21 17:59:12.000000 queue_api-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      565 2024-04-23 13:05:34.000000 queue_api-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-23 13:05:37.250655 queue_api-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.240655 queue_api-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.240655 queue_api-0.1.4/src/q/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.240655 queue_api-0.1.4/src/q/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      149 2024-04-21 18:00:51.000000 queue_api-0.1.4/src/q/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      228 2024-04-21 18:01:43.000000 queue_api-0.1.4/src/q/api/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.240655 queue_api-0.1.4/src/q/api/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      131 2024-04-21 18:01:20.000000 queue_api-0.1.4/src/q/api/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      649 2024-04-21 17:59:44.000000 queue_api-0.1.4/src/q/api/api/append.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      172 2024-04-15 16:36:13.000000 queue_api-0.1.4/src/q/api/api/queue.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5922 2024-04-23 13:05:32.000000 queue_api-0.1.4/src/q/api/api/read.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2723 2024-04-21 17:48:29.000000 queue_api-0.1.4/src/q/api/api/write.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.250655 queue_api-0.1.4/src/q/api/impl/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-04-15 16:36:13.000000 queue_api-0.1.4/src/q/api/impl/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      385 2024-04-15 16:36:13.000000 queue_api-0.1.4/src/q/api/impl/empty.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1180 2024-04-21 17:50:16.000000 queue_api-0.1.4/src/q/api/impl/simple.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.250655 queue_api-0.1.4/src/q/api/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 17:58:36.000000 queue_api-0.1.4/src/q/api/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      286 2024-04-21 17:59:26.000000 queue_api-0.1.4/src/q/api/ops/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1113 2024-04-21 17:58:13.000000 queue_api-0.1.4/src/q/api/ops/append_bounding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1105 2024-04-21 17:50:36.000000 queue_api-0.1.4/src/q/api/ops/bounding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1479 2024-04-21 17:50:49.000000 queue_api-0.1.4/src/q/api/ops/interleaving.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1735 2024-04-21 17:51:01.000000 queue_api-0.1.4/src/q/api/ops/merging.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1978 2024-04-21 17:51:05.000000 queue_api-0.1.4/src/q/api/ops/splitting.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.250655 queue_api-0.1.4/src/queue_api.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-23 13:05:37.000000 queue_api-0.1.4/src/queue_api.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      641 2024-04-23 13:05:37.000000 queue_api-0.1.4/src/queue_api.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-23 13:05:37.000000 queue_api-0.1.4/src/queue_api.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       23 2024-04-23 13:05:37.000000 queue_api-0.1.4/src/queue_api.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-23 13:05:37.000000 queue_api-0.1.4/src/queue_api.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.884412 queue_api-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      406 2024-04-26 06:54:30.884412 queue_api-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-04-24 13:02:36.000000 queue_api-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      570 2024-04-26 06:54:28.000000 queue_api-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-26 06:54:30.884412 queue_api-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.874412 queue_api-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.874412 queue_api-0.1.5/src/q/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.874412 queue_api-0.1.5/src/q/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      149 2024-04-24 13:02:36.000000 queue_api-0.1.5/src/q/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      228 2024-04-24 13:02:36.000000 queue_api-0.1.5/src/q/api/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.874412 queue_api-0.1.5/src/q/api/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      131 2024-04-24 13:02:36.000000 queue_api-0.1.5/src/q/api/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      660 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/api/append.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      183 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/api/queue.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5933 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/api/read.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3323 2024-04-26 06:53:43.000000 queue_api-0.1.5/src/q/api/api/write.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.874412 queue_api-0.1.5/src/q/api/impl/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-04-24 13:02:36.000000 queue_api-0.1.5/src/q/api/impl/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      396 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/impl/empty.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/impl/simple.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.884412 queue_api-0.1.5/src/q/api/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 13:02:36.000000 queue_api-0.1.5/src/q/api/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      317 2024-04-26 06:37:15.000000 queue_api-0.1.5/src/q/api/ops/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1124 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/ops/append_bounding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1116 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/ops/bounding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1490 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/ops/interleaving.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1746 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/ops/merging.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1989 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/ops/splitting.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      589 2024-04-26 06:52:51.000000 queue_api-0.1.5/src/q/api/ops/teeing.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.884412 queue_api-0.1.5/src/queue_api.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      406 2024-04-26 06:54:30.000000 queue_api-0.1.5/src/queue_api.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-04-26 06:54:30.000000 queue_api-0.1.5/src/queue_api.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-26 06:54:30.000000 queue_api-0.1.5/src/queue_api.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       23 2024-04-26 06:54:30.000000 queue_api-0.1.5/src/queue_api.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-26 06:54:30.000000 queue_api-0.1.5/src/queue_api.egg-info/top_level.txt
```

### Comparing `queue_api-0.1.4/pyproject.toml` & `queue_api-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "queue-api"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "API for an asynchronous, point-readable queue"
 dependencies = [
   "haskellian", "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
-repo = "https://github.com/moveread/python-kv.git"
+repo = "https://github.com/moveread/python-storage.git"
 
 # [project.optional-dependencies]
 # test = [
 #   "pytest < 5.0.0",
 #   "pytest-cov[all]"
 # ]
```

### Comparing `queue_api-0.1.4/src/q/api/api/append.py` & `queue_api-0.1.5/src/q/api/api/append.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, TypeVar, overload, Literal
+from typing_extensions import Generic, TypeVar, overload, Literal
 from abc import abstractmethod
 from . import WriteQueue, Queue
 
 T = TypeVar('T')
 
 class AppendQueue(WriteQueue[list[T]], Generic[T]):
   @overload
```

### Comparing `queue_api-0.1.4/src/q/api/api/read.py` & `queue_api-0.1.5/src/q/api/api/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, Never, TypeVar, Callable, Awaitable, overload, AsyncIterable, AsyncIterator, TypeGuard
+from typing_extensions import Generic, Never, TypeVar, Callable, Awaitable, overload, AsyncIterable, AsyncIterator, TypeGuard
 from haskellian import AsyncIter, promise as P
 from abc import ABC, abstractmethod
 
 A = TypeVar('A', covariant=True)
 B = TypeVar('B', covariant=True)
 
 class ReadQueue(ABC, AsyncIterator[tuple[str, A]], Generic[A]):
```

### Comparing `queue_api-0.1.4/src/q/api/api/write.py` & `queue_api-0.1.5/src/q/api/api/write.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, TypeVar, Callable, Awaitable, AsyncIterable
+from typing_extensions import Generic, TypeVar, Callable, Awaitable, AsyncIterable, TypeGuard, overload
 from haskellian import promise as P
 from abc import ABC, abstractmethod
 
 A = TypeVar('A', contravariant=True)
 B = TypeVar('B', contravariant=True)
 
 class WriteQueue(ABC, Generic[A]):
@@ -16,55 +16,72 @@
   async def push(self, key: str, value: A):
     ...
 
   def pusher(self, key: str) -> Callable[[A], Awaitable[None]]:
     """Partially applied `push`"""
     return lambda value: self.push(key, value)
   
+  @overload
+  def prefilter(self, pred: Callable[[A], TypeGuard[B]]) -> 'WriteQueue[B]': ...
+  @overload
+  def prefilter(self, pred: Callable[[A], bool]) -> 'WriteQueue[A]': ...
+  def prefilter(self, pred): # type: ignore
+    return prefilter(self, lambda kv: P.of(pred(kv[1])))
+  
   def premap(self, f: Callable[[B], A]) -> 'WriteQueue[B]':
-    return PremappedQueue(self, lambda kv: P.of((kv[0], f(kv[1]))))
+    return premap(self, lambda kv: P.of((kv[0], f(kv[1]))))
   
   def premap_kv(self, f: Callable[[str, B], A]) -> 'WriteQueue[B]':
     """Map but `f` receives both key and value"""
-    return PremappedQueue(self, lambda kv: P.of((kv[0], f(*kv))))
+    return premap(self, lambda kv: P.of((kv[0], f(*kv))))
   
   def premap_k(self, f: Callable[[str], A]) -> 'WriteQueue':
     """Map but `f` receives the key"""
-    return PremappedQueue(self, lambda kv: P.of((kv[0], f(kv[0]))))
+    return premap(self, lambda kv: P.of((kv[0], f(kv[0]))))
   
   def premap_kvt(self, f: Callable[[tuple[str, B]], A]) -> 'WriteQueue[B]':
     """Map but `f` receives both key and value as a tuple"""
-    return PremappedQueue(self, lambda kv: P.of((kv[0], f(kv))))
+    return premap(self, lambda kv: P.of((kv[0], f(kv))))
   
   def apremap(self, f: Callable[[B], Awaitable[A]]) -> 'WriteQueue[B]':
     """Map but `f` is asynchronous"""
     async def mapper(kv: tuple[str, B]):
       return kv[0], await f(kv[1])
-    return PremappedQueue(self, mapper)
+    return premap(self, mapper)
   
   def apremap_kv(self, f: Callable[[str, B], Awaitable[A]]) -> 'WriteQueue[B]':
     """Map but `f` is asynchronous and receives both key and value"""
     async def mapper(kv: tuple[str, B]):
       return kv[0], await f(*kv)
-    return PremappedQueue(self, mapper)
+    return premap(self, mapper)
   
   def apremap_k(self, f: Callable[[str], Awaitable[A]]) -> 'WriteQueue':
     """Map but `f` is asynchronous and receives the key"""
     async def mapper(kv: tuple[str, B]):
       return kv[0], await f(kv[0])
-    return PremappedQueue(self, mapper)
+    return premap(self, mapper)
   
   def apremap_kvt(self, f: Callable[[tuple[str, B]], Awaitable[A]]) -> 'WriteQueue[B]':
     """Map but `f` is asynchronous and receives both key and value as a tuple"""
     async def mapper(kv: tuple[str, B]):
       return kv[0], await f(kv)
-    return PremappedQueue(self, mapper)
+    return premap(self, mapper)
 
+class prefilter(WriteQueue[A], Generic[A]):
+  
+  def __init__(self, q: WriteQueue[A], p: Callable[[tuple[str, A]], Awaitable[bool]]):
+    self._wrapped = q
+    self._predicate = p
+    __name__ = f'Filtered{repr(self)}'
+
+  async def push(self, key: str, value: A):
+    if await self._predicate((key, value)):
+      return await self._wrapped.push(key, value)
 
-class PremappedQueue(WriteQueue[B], Generic[A, B]):
+class premap(WriteQueue[B], Generic[A, B]):
   
   def __init__(self, q: WriteQueue[A], f: Callable[[tuple[str, B]], Awaitable[tuple[str, A]]]):
     self._wrapped = q
     self._mapper = f
     __name__ = f'Mapped{repr(self)}'
 
   async def push(self, key: str, value: B):
```

### Comparing `queue_api-0.1.4/src/q/api/impl/simple.py` & `queue_api-0.1.5/src/q/api/impl/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, TypeVar, AsyncIterable
+from typing_extensions import Generic, TypeVar, AsyncIterable
 from collections import OrderedDict
 from ..api import ReadQueue, WriteQueue
 from haskellian import ManagedPromise
 
 A = TypeVar('A')
 B = TypeVar('B')
```

### Comparing `queue_api-0.1.4/src/q/api/ops/append_bounding.py` & `queue_api-0.1.5/src/q/api/ops/append_bounding.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Generic
+from typing_extensions import TypeVar, Generic
 import asyncio
 from haskellian import ManagedPromise
 from ..api.append import AppendableQueue
 from .bounding import Bounded
 
 T = TypeVar('T')
```

### Comparing `queue_api-0.1.4/src/q/api/ops/bounding.py` & `queue_api-0.1.5/src/q/api/ops/bounding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Generic
+from typing_extensions import TypeVar, Generic
 import asyncio
 from haskellian import ManagedPromise
 from ..api import Queue
 
 T = TypeVar('T')
 Q = TypeVar('Q', bound=Queue)
```

### Comparing `queue_api-0.1.4/src/q/api/ops/interleaving.py` & `queue_api-0.1.5/src/q/api/ops/interleaving.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Generic, AsyncIterable
+from typing_extensions import TypeVar, Generic, AsyncIterable
 import asyncio
 from haskellian import ManagedAsync
 from ..api import ReadQueue
 from ..impl import SimpleQueue
 
 A = TypeVar('A')
 B = TypeVar('B')
```

### Comparing `queue_api-0.1.4/src/q/api/ops/merging.py` & `queue_api-0.1.5/src/q/api/ops/merging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Generic, AsyncIterable, Callable, Awaitable
+from typing_extensions import TypeVar, Generic, AsyncIterable, Callable, Awaitable
 import asyncio
 import haskellian.promise as P
 from q.api import ReadQueue
 
 A = TypeVar('A')
 B = TypeVar('B')
 C = TypeVar('C')
```

### Comparing `queue_api-0.1.4/src/q/api/ops/splitting.py` & `queue_api-0.1.5/src/q/api/ops/splitting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Generic, AsyncIterable, Callable, Awaitable
+from typing_extensions import TypeVar, Generic, AsyncIterable, Callable, Awaitable
 import haskellian.promise as P
 from ..api import ReadQueue, WriteQueue
 from ..impl import SimpleQueue
 from .interleaving import interleave
 
 A = TypeVar('A')
 B = TypeVar('B')
```

### Comparing `queue_api-0.1.4/src/queue_api.egg-info/SOURCES.txt` & `queue_api-0.1.5/src/queue_api.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 src/q/api/ops/__init__.py
 src/q/api/ops/__init__.pyi
 src/q/api/ops/append_bounding.py
 src/q/api/ops/bounding.py
 src/q/api/ops/interleaving.py
 src/q/api/ops/merging.py
 src/q/api/ops/splitting.py
+src/q/api/ops/teeing.py
 src/queue_api.egg-info/PKG-INFO
 src/queue_api.egg-info/SOURCES.txt
 src/queue_api.egg-info/dependency_links.txt
 src/queue_api.egg-info/requires.txt
 src/queue_api.egg-info/top_level.txt
```

