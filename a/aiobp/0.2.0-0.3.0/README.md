# Comparing `tmp/aiobp-0.2.0.tar.gz` & `tmp/aiobp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobp-0.2.0.tar", max compression
+gzip compressed data, was "aiobp-0.3.0.tar", max compression
```

## Comparing `aiobp-0.2.0.tar` & `aiobp-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1057 2024-01-29 17:17:42.453698 aiobp-0.2.0/LICENSE
--rw-r--r--   0        0        0     2455 2024-02-20 15:29:36.631957 aiobp-0.2.0/README.md
--rw-r--r--   0        0        0      177 2024-01-29 17:22:10.519225 aiobp-0.2.0/aiobp/__init__.py
--rw-r--r--   0        0        0      665 2024-01-29 16:50:33.893664 aiobp-0.2.0/aiobp/config/__init__.py
--rw-r--r--   0        0        0     3215 2024-02-20 16:08:04.633393 aiobp-0.2.0/aiobp/config/annotations.py
--rw-r--r--   0        0        0     1395 2024-02-20 15:49:52.311481 aiobp-0.2.0/aiobp/config/conf.py
--rw-r--r--   0        0        0      329 2024-01-29 15:02:53.137137 aiobp-0.2.0/aiobp/config/exceptions.py
--rw-r--r--   0        0        0     1182 2024-02-20 15:50:44.138554 aiobp-0.2.0/aiobp/config/json.py
--rw-r--r--   0        0        0      164 2024-01-29 17:01:49.865893 aiobp-0.2.0/aiobp/logging/__init__.py
--rw-r--r--   0        0        0     3228 2024-02-20 15:59:33.199374 aiobp-0.2.0/aiobp/logging/custom.py
--rw-r--r--   0        0        0      304 2024-01-29 14:10:35.443889 aiobp-0.2.0/aiobp/logging/log.py
--rw-r--r--   0        0        0     9043 2024-02-20 16:12:52.568989 aiobp-0.2.0/aiobp/runner.py
--rw-r--r--   0        0        0      567 2024-01-29 16:57:09.026915 aiobp-0.2.0/aiobp/task.py
--rw-r--r--   0        0        0      397 2024-02-20 15:47:05.016836 aiobp-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 aiobp-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-01-29 17:17:42.453698 aiobp-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2455 2024-02-20 15:29:36.631957 aiobp-0.3.0/README.md
+-rw-r--r--   0        0        0      177 2024-01-29 17:22:10.519225 aiobp-0.3.0/aiobp/__init__.py
+-rw-r--r--   0        0        0      665 2024-01-29 16:50:33.893664 aiobp-0.3.0/aiobp/config/__init__.py
+-rw-r--r--   0        0        0     3215 2024-02-20 16:08:04.633393 aiobp-0.3.0/aiobp/config/annotations.py
+-rw-r--r--   0        0        0     1395 2024-02-20 15:49:52.311481 aiobp-0.3.0/aiobp/config/conf.py
+-rw-r--r--   0        0        0      329 2024-01-29 15:02:53.137137 aiobp-0.3.0/aiobp/config/exceptions.py
+-rw-r--r--   0        0        0     1182 2024-02-20 15:50:44.138554 aiobp-0.3.0/aiobp/config/json.py
+-rw-r--r--   0        0        0      164 2024-01-29 17:01:49.865893 aiobp-0.3.0/aiobp/logging/__init__.py
+-rw-r--r--   0        0        0     3660 2024-04-26 15:53:53.276368 aiobp-0.3.0/aiobp/logging/custom.py
+-rw-r--r--   0        0        0      304 2024-01-29 14:10:35.443889 aiobp-0.3.0/aiobp/logging/log.py
+-rw-r--r--   0        0        0     9133 2024-04-26 13:26:30.776470 aiobp-0.3.0/aiobp/runner.py
+-rw-r--r--   0        0        0      989 2024-04-26 15:55:12.033670 aiobp-0.3.0/aiobp/task.py
+-rw-r--r--   0        0        0      397 2024-04-26 15:56:03.810755 aiobp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 aiobp-0.3.0/PKG-INFO
```

### Comparing `aiobp-0.2.0/LICENSE` & `aiobp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobp-0.2.0/README.md` & `aiobp-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aiobp-0.2.0/aiobp/config/__init__.py` & `aiobp-0.3.0/aiobp/config/__init__.py`

 * *Files identical despite different names*

### Comparing `aiobp-0.2.0/aiobp/config/annotations.py` & `aiobp-0.3.0/aiobp/config/annotations.py`

 * *Files identical despite different names*

### Comparing `aiobp-0.2.0/aiobp/config/conf.py` & `aiobp-0.3.0/aiobp/config/conf.py`

 * *Files identical despite different names*

### Comparing `aiobp-0.2.0/aiobp/config/json.py` & `aiobp-0.3.0/aiobp/config/json.py`

 * *Files identical despite different names*

### Comparing `aiobp-0.2.0/aiobp/logging/custom.py` & `aiobp-0.3.0/aiobp/logging/custom.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Customize Python logger"""
 
 import logging
 import logging.handlers
 import sys
 
-from typing import Optional
+from typing import Optional, Type, TracebackType
 
 
 class LoggingConfig:
     """Loging configuration"""
 
     level: str = 'DEBUG'
     filename: Optional[str] = None
@@ -78,23 +78,34 @@
 
 
 def add_devel_log_level():
     """Register new logging level for development purposes"""
     logging.addLevelName(1, "DEVEL")
 
 
+def log_unhandled_exception(type_: Type[BaseException], value: BaseException, traceback: TracebackType):
+    """Log unhandled exceptions"""
+    if issubclass(type_, KeyboardInterrupt):
+        sys.__excepthook__(type_, value, traceback)
+        return
+
+    logging.critical("Uncaught exception", exc_info=(type_, value, traceback))
+
+
 def setup_logging(config: Optional[LoggingConfig] = LoggingConfig()) -> None:
     """Setup Python logger"""
     console_handler = logging.StreamHandler(sys.stdout)
     console_handler.setFormatter(
         ColorFormatter(f"%(asctime)s [{Color.green}%(filename)s:%(lineno)d{Color.reset}] %(message)s"),
     )
     handlers = [console_handler]
 
-    if config.filename is not None:
+    if config and config.filename is not None:
         file_handler = logging.handlers.WatchedFileHandler(filename=config.filename)
         file_handler.setFormatter(
             PrefixExceptionFormatter("%(asctime)s %(levelname)s [%(filename)s:%(lineno)d] %(message)s"),
         )
         handlers.append(file_handler)
 
-    logging.basicConfig(level=config.level, handlers=handlers)
+    logging.basicConfig(level=config.level if config else None, handlers=handlers)
+
+    sys.excepthook = log_unhandled_exception
```

### Comparing `aiobp-0.2.0/aiobp/runner.py` & `aiobp-0.3.0/aiobp/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,18 @@
     coroutine finishes; otherwise the service is kept running.
     """
     loop = asyncio.get_event_loop()
     # main does:
     # 1. start given service coroutine as task
     # 2. add SIGTERM and SIGINT handlers
     # 3. waits for kill or KeyboardInterrupt
-    loop.run_until_complete(__main(service, endless))
+    try:
+        loop.run_until_complete(__main(service, endless))
+    except Exception:
+        log.critical("Unhandled exception in service")
     # graceful_shutdown does:
     # 1. calls one by one all registered coroutines via on_shutdown(...) in LIFO order
     # 2. cancel all tasks in parallel (via gather)
     # 3. await tasks to finish in specified shutdown_timeout
     # 4. calls all registered coroutines via on_shutdown(..., after_tasks_cancel=True) in LIFO order
     loop.run_until_complete(__graceful_shutdown(shutdown_timeout))
```

### Comparing `aiobp-0.2.0/aiobp/task.py` & `aiobp-0.3.0/aiobp/task.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 """Keep reference to running asyncio tasks"""
 
 import asyncio
 
+from aiobp import log
+
 from typing import Coroutine
 
 
 __tasks: set[asyncio.Task] = set()  # to avoid garbage collection by holding reference
 
 
+async def exception_handler(coroutine: Coroutine, name: str) -> Coroutine:
+    """Log unhandled exception in asyncio task
+
+    This is needed to get exceptions immediately (otherwise they are displayed on shutdown).
+    """
+    try:
+        await coroutine
+    except Exception as error:
+        log.critical('Unhandled exception in task "%s"', name, exc_info=error)
+
+
 def create_task(coroutine: Coroutine, name: str) -> asyncio.Task:
     """Creates task and keeps reference until the task is done
 
     Argument "name" is optional in asyncio.task(), however we require it
     to make our code easier to debug.
     """
-    task = asyncio.create_task(coroutine, name=name)
+    task = asyncio.create_task(exception_handler(coroutine, name=name), name=name)
     __tasks.add(task)
     task.add_done_callback(__tasks.discard)
     return task
```

### Comparing `aiobp-0.2.0/PKG-INFO` & `aiobp-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobp
-Version: 0.2.0
+Version: 0.3.0
 Summary: Boilerplate for asyncio service
 Author: INSOFT s.r.o.
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

