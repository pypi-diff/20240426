# Comparing `tmp/metronomes-0.0.2.tar.gz` & `tmp/metronomes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metronomes-0.0.2.tar", last modified: Sun Apr 21 11:53:15 2024, max compression
+gzip compressed data, was "metronomes-0.0.3.tar", last modified: Fri Apr 26 19:23:25 2024, max compression
```

## Comparing `metronomes-0.0.2.tar` & `metronomes-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:53:15.186842 metronomes-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 11:53:02.000000 metronomes-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-04-21 11:53:15.186842 metronomes-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-04-21 11:53:02.000000 metronomes-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:53:15.186842 metronomes-0.0.2/metronomes/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-21 11:53:02.000000 metronomes-0.0.2/metronomes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-21 11:53:02.000000 metronomes-0.0.2/metronomes/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-21 11:53:02.000000 metronomes-0.0.2/metronomes/metronome.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:53:02.000000 metronomes-0.0.2/metronomes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:53:15.186842 metronomes-0.0.2/metronomes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-04-21 11:53:15.000000 metronomes-0.0.2/metronomes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-21 11:53:15.000000 metronomes-0.0.2/metronomes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:53:15.000000 metronomes-0.0.2/metronomes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-21 11:53:15.000000 metronomes-0.0.2/metronomes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 11:53:15.000000 metronomes-0.0.2/metronomes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-21 11:53:02.000000 metronomes-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:53:15.186842 metronomes-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:23:25.384494 metronomes-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 19:23:12.000000 metronomes-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10996 2024-04-26 19:23:25.384494 metronomes-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-04-26 19:23:12.000000 metronomes-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:23:25.384494 metronomes-0.0.3/metronomes/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 19:23:12.000000 metronomes-0.0.3/metronomes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-26 19:23:12.000000 metronomes-0.0.3/metronomes/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-26 19:23:12.000000 metronomes-0.0.3/metronomes/metronome.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:23:12.000000 metronomes-0.0.3/metronomes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:23:25.384494 metronomes-0.0.3/metronomes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10996 2024-04-26 19:23:25.000000 metronomes-0.0.3/metronomes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-26 19:23:25.000000 metronomes-0.0.3/metronomes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:23:25.000000 metronomes-0.0.3/metronomes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-26 19:23:25.000000 metronomes-0.0.3/metronomes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 19:23:25.000000 metronomes-0.0.3/metronomes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-26 19:23:12.000000 metronomes-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:23:25.384494 metronomes-0.0.3/setup.cfg
```

### Comparing `metronomes-0.0.2/LICENSE` & `metronomes-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metronomes-0.0.2/PKG-INFO` & `metronomes-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metronomes
-Version: 0.0.2
+Version: 0.0.3
 Summary: Endless tick-tock generators
 Author-email: Evgeniy Blinov <zheni-b@yandex.ru>
 Project-URL: Source, https://github.com/pomponchik/metronomes
 Project-URL: Tracker, https://github.com/pomponchik/metronomes/issues
 Keywords: metronome,task scheduling,callbacks runner
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
@@ -50,14 +50,15 @@
 
 - [**Quick start**](#quick-start)
 - [**Why?**](#why)
 - [**Logging**](#logging)
 - [**Error escaping**](#error-escaping)
 - [**Working with Cancellation Tokens**](#working-with-cancellation-tokens)
 - [**Limitations**](#limitations)
+- [**Use it as a context manager**](#use-it-as-a-context-manager)
 
 
 ## Quick start
 
 Install it:
 
 ```bash
@@ -220,7 +221,27 @@
 
 metronome.start()
 sleep(1)
 #> go!
 #> go!
 #> go!
 ```
+
+
+## Use it as a context manager
+
+We recommend using a metronome exclusively in the context manager mode, without "manual" start and stop:
+
+```python
+from time import sleep
+from metronomes import Metronome
+
+with Metronome(0.2, lambda: print('go!')):
+    sleep(1)
+#> go!
+#> go!
+#> go!
+#> go!
+#> go!
+```
+
+In this case, it is guaranteed that the metronome will be completed correctly after the end of the code block and will not remain "hanging" in a separate thread. Even if an error occurs in the block.
```

### Comparing `metronomes-0.0.2/README.md` & `metronomes-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 - [**Quick start**](#quick-start)
 - [**Why?**](#why)
 - [**Logging**](#logging)
 - [**Error escaping**](#error-escaping)
 - [**Working with Cancellation Tokens**](#working-with-cancellation-tokens)
 - [**Limitations**](#limitations)
+- [**Use it as a context manager**](#use-it-as-a-context-manager)
 
 
 ## Quick start
 
 Install it:
 
 ```bash
@@ -193,7 +194,27 @@
 
 metronome.start()
 sleep(1)
 #> go!
 #> go!
 #> go!
 ```
+
+
+## Use it as a context manager
+
+We recommend using a metronome exclusively in the context manager mode, without "manual" start and stop:
+
+```python
+from time import sleep
+from metronomes import Metronome
+
+with Metronome(0.2, lambda: print('go!')):
+    sleep(1)
+#> go!
+#> go!
+#> go!
+#> go!
+#> go!
+```
+
+In this case, it is guaranteed that the metronome will be completed correctly after the end of the code block and will not remain "hanging" in a separate thread. Even if an error occurs in the block.
```

### Comparing `metronomes-0.0.2/metronomes/metronome.py` & `metronomes-0.0.3/metronomes/metronome.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 from typing import Type, Callable, Union, Optional, Any
+
+try:
+    from typing import Literal  # type: ignore[attr-defined]
+except ImportError:  # pragma: no cover
+    from typing_extensions import Literal  # type: ignore[assignment, unused-ignore]
+
 from threading import Thread, RLock
 from time import perf_counter, sleep
 from functools import partial
+from types import TracebackType
 
 import escape
 from emptylog import EmptyLogger, LoggerProtocol
 from cantok import AbstractToken, SimpleToken, TimeoutToken
 from locklib import ContextLockProtocol
 
 from metronomes.errors import RunStoppedMetronomeError, RunAlreadyStartedMetronomeError, StopNotStartedMetronomeError, StopStoppedMetronomeError
@@ -29,14 +36,26 @@
             self.token = self.token + TimeoutToken(duration)
         self.thread: Optional[Thread] = None
         self.started: bool = False
         self.stopped: bool = False
         self.lock: ContextLockProtocol = lock_factory()
         self.sleeping_callback: Callable[[Union[int, float]], Any] = sleeping_callback
 
+    def __enter__(self) -> 'Metronome':
+        with self.lock:
+            with escape(RunAlreadyStartedMetronomeError):  # type: ignore[operator]
+                self.start()
+            return self
+
+    def __exit__(self, exception_type: Optional[Type[BaseException]], exception_value: Optional[BaseException], traceback: Optional[TracebackType]) -> Literal[True]:
+        with self.lock:
+            with escape(StopStoppedMetronomeError):  # type: ignore[operator]
+                self.stop()
+        return False
+
     def start(self) -> 'Metronome':
         with self.lock:
             if self.stopped:
                 raise RunStoppedMetronomeError('Metronomes are disposable, you cannot restart a stopped metronome.')
             if self.started:
                 raise RunAlreadyStartedMetronomeError('The metronome has already been launched.')
```

### Comparing `metronomes-0.0.2/metronomes.egg-info/PKG-INFO` & `metronomes-0.0.3/metronomes.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metronomes
-Version: 0.0.2
+Version: 0.0.3
 Summary: Endless tick-tock generators
 Author-email: Evgeniy Blinov <zheni-b@yandex.ru>
 Project-URL: Source, https://github.com/pomponchik/metronomes
 Project-URL: Tracker, https://github.com/pomponchik/metronomes/issues
 Keywords: metronome,task scheduling,callbacks runner
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
@@ -50,14 +50,15 @@
 
 - [**Quick start**](#quick-start)
 - [**Why?**](#why)
 - [**Logging**](#logging)
 - [**Error escaping**](#error-escaping)
 - [**Working with Cancellation Tokens**](#working-with-cancellation-tokens)
 - [**Limitations**](#limitations)
+- [**Use it as a context manager**](#use-it-as-a-context-manager)
 
 
 ## Quick start
 
 Install it:
 
 ```bash
@@ -220,7 +221,27 @@
 
 metronome.start()
 sleep(1)
 #> go!
 #> go!
 #> go!
 ```
+
+
+## Use it as a context manager
+
+We recommend using a metronome exclusively in the context manager mode, without "manual" start and stop:
+
+```python
+from time import sleep
+from metronomes import Metronome
+
+with Metronome(0.2, lambda: print('go!')):
+    sleep(1)
+#> go!
+#> go!
+#> go!
+#> go!
+#> go!
+```
+
+In this case, it is guaranteed that the metronome will be completed correctly after the end of the code block and will not remain "hanging" in a separate thread. Even if an error occurs in the block.
```

### Comparing `metronomes-0.0.2/pyproject.toml` & `metronomes-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ['setuptools==68.0.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'metronomes'
-version = '0.0.2'
+version = '0.0.3'
 authors = [
   { name='Evgeniy Blinov', email='zheni-b@yandex.ru' },
 ]
 description = 'Endless tick-tock generators'
 readme = 'README.md'
 requires-python = '>=3.7'
 dependencies = [
     'emptylog>=0.0.4',
     'cantok>=0.0.22',
     'escaping>=0.0.11',
     'locklib>=0.0.15',
+    'typing_extensions ; python_version < "3.8"',
 ]
 classifiers = [
     'Operating System :: OS Independent',
     'Operating System :: MacOS :: MacOS X',
     'Operating System :: Microsoft :: Windows',
     'Operating System :: POSIX',
     'Operating System :: POSIX :: Linux',
```

