# Comparing `tmp/beta9-0.1.2rc1.tar.gz` & `tmp/beta9-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beta9-0.1.2rc1.tar", max compression
+gzip compressed data, was "beta9-0.1.3.tar", max compression
```

## Comparing `beta9-0.1.2rc1.tar` & `beta9-0.1.3.tar`

### file list

```diff
@@ -1,46 +1,82 @@
--rw-r--r--   0        0        0     1130 2024-04-17 13:23:37.995931 beta9-0.1.2rc1/pyproject.toml
--rw-r--r--   0        0        0      557 2024-04-17 13:13:37.445495 beta9-0.1.2rc1/src/beta9/__init__.py
--rw-r--r--   0        0        0        0 2024-01-23 23:38:59.669351 beta9-0.1.2rc1/src/beta9/abstractions/__init__.py
--rw-r--r--   0        0        0      606 2024-01-23 23:38:59.669478 beta9-0.1.2rc1/src/beta9/abstractions/base/__init__.py
--rw-r--r--   0        0        0     8509 2024-04-17 13:14:18.140772 beta9-0.1.2rc1/src/beta9/abstractions/base/runner.py
--rw-r--r--   0        0        0     3492 2024-04-17 13:14:18.141093 beta9-0.1.2rc1/src/beta9/abstractions/container.py
--rw-r--r--   0        0        0     3977 2024-04-17 13:14:18.141399 beta9-0.1.2rc1/src/beta9/abstractions/endpoint.py
--rw-r--r--   0        0        0     6175 2024-04-17 13:14:18.141584 beta9-0.1.2rc1/src/beta9/abstractions/function.py
--rw-r--r--   0        0        0     4264 2024-04-17 13:14:18.141720 beta9-0.1.2rc1/src/beta9/abstractions/image.py
--rw-r--r--   0        0        0     3237 2024-04-17 13:14:18.141834 beta9-0.1.2rc1/src/beta9/abstractions/map.py
--rw-r--r--   0        0        0     3183 2024-04-17 13:14:18.141940 beta9-0.1.2rc1/src/beta9/abstractions/queue.py
--rw-r--r--   0        0        0     6395 2024-04-17 13:14:18.142080 beta9-0.1.2rc1/src/beta9/abstractions/taskqueue.py
--rw-r--r--   0        0        0     1605 2024-04-17 13:14:18.142367 beta9-0.1.2rc1/src/beta9/abstractions/volume.py
--rw-r--r--   0        0        0      292 2024-04-15 21:13:39.880348 beta9-0.1.2rc1/src/beta9/aio.py
--rw-r--r--   0        0        0        0 2024-01-23 23:38:59.670190 beta9-0.1.2rc1/src/beta9/cli/__init__.py
--rw-r--r--   0        0        0      932 2024-04-17 13:14:18.142672 beta9-0.1.2rc1/src/beta9/cli/config.py
--rw-r--r--   0        0        0      824 2024-04-17 13:14:18.143012 beta9-0.1.2rc1/src/beta9/cli/contexts.py
--rw-r--r--   0        0        0     2422 2024-04-17 13:14:18.143206 beta9-0.1.2rc1/src/beta9/cli/deployment.py
--rw-r--r--   0        0        0     3197 2024-04-17 13:14:18.143457 beta9-0.1.2rc1/src/beta9/cli/extraclick.py
--rw-r--r--   0        0        0     1140 2024-04-17 13:14:18.143741 beta9-0.1.2rc1/src/beta9/cli/main.py
--rw-r--r--   0        0        0     3738 2024-04-17 13:14:18.144016 beta9-0.1.2rc1/src/beta9/cli/task.py
--rw-r--r--   0        0        0     8667 2024-04-17 13:14:18.144318 beta9-0.1.2rc1/src/beta9/cli/volume.py
--rw-r--r--   0        0        0        0 2024-04-16 19:32:37.403246 beta9-0.1.2rc1/src/beta9/clients/__init__.py
--rw-r--r--   0        0        0     2980 2024-04-17 13:14:18.144448 beta9-0.1.2rc1/src/beta9/clients/container/__init__.py
--rw-r--r--   0        0        0     2499 2024-04-17 13:14:18.144717 beta9-0.1.2rc1/src/beta9/clients/endpoint/__init__.py
--rw-r--r--   0        0        0     8023 2024-04-17 13:14:18.144848 beta9-0.1.2rc1/src/beta9/clients/function/__init__.py
--rw-r--r--   0        0        0    21023 2024-04-17 13:14:18.144938 beta9-0.1.2rc1/src/beta9/clients/gateway/__init__.py
--rw-r--r--   0        0        0     4773 2024-04-17 13:14:18.145074 beta9-0.1.2rc1/src/beta9/clients/image/__init__.py
--rw-r--r--   0        0        0     8003 2024-04-17 13:14:18.145188 beta9-0.1.2rc1/src/beta9/clients/map/__init__.py
--rw-r--r--   0        0        0     8687 2024-04-17 13:14:18.145328 beta9-0.1.2rc1/src/beta9/clients/simplequeue/__init__.py
--rw-r--r--   0        0        0     9665 2024-04-17 13:14:18.145458 beta9-0.1.2rc1/src/beta9/clients/taskqueue/__init__.py
--rw-r--r--   0        0        0     9482 2024-04-17 13:14:18.145732 beta9-0.1.2rc1/src/beta9/clients/volume/__init__.py
--rw-r--r--   0        0        0     7301 2024-04-17 13:14:18.145934 beta9-0.1.2rc1/src/beta9/config.py
--rw-r--r--   0        0        0      207 2024-01-23 23:38:59.671504 beta9-0.1.2rc1/src/beta9/exceptions.py
--rw-r--r--   0        0        0      886 2024-04-17 13:13:37.450038 beta9-0.1.2rc1/src/beta9/logging.py
--rw-r--r--   0        0        0        0 2024-01-23 23:38:59.671565 beta9-0.1.2rc1/src/beta9/runner/__init__.py
--rw-r--r--   0        0        0     2462 2024-04-17 13:14:18.146268 beta9-0.1.2rc1/src/beta9/runner/common.py
--rw-r--r--   0        0        0     2321 2024-04-17 13:14:18.146631 beta9-0.1.2rc1/src/beta9/runner/container.py
--rw-r--r--   0        0        0     4647 2024-04-17 13:14:18.146985 beta9-0.1.2rc1/src/beta9/runner/endpoint.py
--rw-r--r--   0        0        0     5905 2024-04-17 13:14:18.147159 beta9-0.1.2rc1/src/beta9/runner/function.py
--rw-r--r--   0        0        0     3910 2024-04-17 13:14:18.147410 beta9-0.1.2rc1/src/beta9/runner/serve.py
--rw-r--r--   0        0        0    10259 2024-04-17 13:14:18.147724 beta9-0.1.2rc1/src/beta9/runner/taskqueue.py
--rw-r--r--   0        0        0     5593 2024-04-17 13:14:18.148222 beta9-0.1.2rc1/src/beta9/sync.py
--rw-r--r--   0        0        0     2994 2024-04-17 13:14:18.148560 beta9-0.1.2rc1/src/beta9/terminal.py
--rw-r--r--   0        0        0     1399 2024-01-23 23:38:59.672017 beta9-0.1.2rc1/src/beta9/type.py
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 beta9-0.1.2rc1/PKG-INFO
+-rw-r--r--   0        0        0     1127 2024-04-26 16:59:00.312905 beta9-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      586 2024-04-26 16:58:18.488727 beta9-0.1.3/src/beta9/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.962074 beta9-0.1.3/src/beta9/abstractions/__init__.py
+-rw-r--r--   0        0        0      170 2024-01-27 18:19:06.888984 beta9-0.1.3/src/beta9/abstractions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5495 2024-04-21 16:47:13.563006 beta9-0.1.3/src/beta9/abstractions/__pycache__/container.cpython-311.pyc
+-rw-r--r--   0        0        0     7724 2024-04-26 06:05:25.284785 beta9-0.1.3/src/beta9/abstractions/__pycache__/endpoint.cpython-311.pyc
+-rw-r--r--   0        0        0    11097 2024-04-24 23:01:13.118744 beta9-0.1.3/src/beta9/abstractions/__pycache__/function.cpython-311.pyc
+-rw-r--r--   0        0        0     6226 2024-04-24 22:32:45.911483 beta9-0.1.3/src/beta9/abstractions/__pycache__/image.cpython-311.pyc
+-rw-r--r--   0        0        0     6188 2024-04-21 16:47:13.732114 beta9-0.1.3/src/beta9/abstractions/__pycache__/map.cpython-311.pyc
+-rw-r--r--   0        0        0     5648 2024-04-21 16:47:13.734715 beta9-0.1.3/src/beta9/abstractions/__pycache__/queue.cpython-311.pyc
+-rw-r--r--   0        0        0    12051 2024-04-25 22:07:33.858948 beta9-0.1.3/src/beta9/abstractions/__pycache__/taskqueue.cpython-311.pyc
+-rw-r--r--   0        0        0     2647 2024-04-21 16:47:13.714395 beta9-0.1.3/src/beta9/abstractions/__pycache__/volume.cpython-311.pyc
+-rw-r--r--   0        0        0      606 2024-01-27 16:13:22.962265 beta9-0.1.3/src/beta9/abstractions/base/__init__.py
+-rw-r--r--   0        0        0     1685 2024-01-27 18:19:06.984688 beta9-0.1.3/src/beta9/abstractions/base/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11644 2024-04-26 16:28:49.193305 beta9-0.1.3/src/beta9/abstractions/base/__pycache__/runner.cpython-311.pyc
+-rw-r--r--   0        0        0     8924 2024-04-26 16:58:18.488908 beta9-0.1.3/src/beta9/abstractions/base/runner.py
+-rw-r--r--   0        0        0     3492 2024-04-21 16:36:14.953861 beta9-0.1.3/src/beta9/abstractions/container.py
+-rw-r--r--   0        0        0     4574 2024-04-26 16:58:18.489070 beta9-0.1.3/src/beta9/abstractions/endpoint.py
+-rw-r--r--   0        0        0     6565 2024-04-26 16:58:18.489246 beta9-0.1.3/src/beta9/abstractions/function.py
+-rw-r--r--   0        0        0     4264 2024-04-24 22:31:23.870406 beta9-0.1.3/src/beta9/abstractions/image.py
+-rw-r--r--   0        0        0     3237 2024-04-21 16:36:14.954512 beta9-0.1.3/src/beta9/abstractions/map.py
+-rw-r--r--   0        0        0     3183 2024-04-21 16:36:14.955563 beta9-0.1.3/src/beta9/abstractions/queue.py
+-rw-r--r--   0        0        0     8548 2024-04-26 16:58:18.489543 beta9-0.1.3/src/beta9/abstractions/taskqueue.py
+-rw-r--r--   0        0        0     1605 2024-04-21 16:36:14.957214 beta9-0.1.3/src/beta9/abstractions/volume.py
+-rw-r--r--   0        0        0      292 2024-01-27 16:13:22.963762 beta9-0.1.3/src/beta9/aio.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.963872 beta9-0.1.3/src/beta9/cli/__init__.py
+-rw-r--r--   0        0        0      161 2024-02-07 17:33:34.585819 beta9-0.1.3/src/beta9/cli/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1786 2024-04-22 03:01:00.641942 beta9-0.1.3/src/beta9/cli/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     1433 2024-04-01 17:03:29.905084 beta9-0.1.3/src/beta9/cli/__pycache__/configure.cpython-311.pyc
+-rw-r--r--   0        0        0     2197 2024-04-22 03:01:00.644896 beta9-0.1.3/src/beta9/cli/__pycache__/contexts.cpython-311.pyc
+-rw-r--r--   0        0        0     2486 2024-04-01 17:03:29.905700 beta9-0.1.3/src/beta9/cli/__pycache__/deploy.cpython-311.pyc
+-rw-r--r--   0        0        0     4533 2024-04-22 03:01:00.644129 beta9-0.1.3/src/beta9/cli/__pycache__/deployment.cpython-311.pyc
+-rw-r--r--   0        0        0     6533 2024-04-22 03:01:00.643173 beta9-0.1.3/src/beta9/cli/__pycache__/extraclick.cpython-311.pyc
+-rw-r--r--   0        0        0     1531 2024-02-07 17:33:34.615345 beta9-0.1.3/src/beta9/cli/__pycache__/formatters.cpython-311.pyc
+-rw-r--r--   0        0        0     2634 2024-04-22 03:01:00.635557 beta9-0.1.3/src/beta9/cli/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0        0        0     6911 2024-04-22 03:01:00.646800 beta9-0.1.3/src/beta9/cli/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     6901 2024-04-10 01:00:13.874183 beta9-0.1.3/src/beta9/cli/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0        0        0    15122 2024-04-22 03:01:00.648559 beta9-0.1.3/src/beta9/cli/__pycache__/volume.cpython-311.pyc
+-rw-r--r--   0        0        0      932 2024-04-21 16:36:14.959066 beta9-0.1.3/src/beta9/cli/config.py
+-rw-r--r--   0        0        0      824 2024-04-21 16:36:14.962332 beta9-0.1.3/src/beta9/cli/contexts.py
+-rw-r--r--   0        0        0     2422 2024-04-21 16:36:14.964463 beta9-0.1.3/src/beta9/cli/deployment.py
+-rw-r--r--   0        0        0     3197 2024-04-21 16:36:14.964958 beta9-0.1.3/src/beta9/cli/extraclick.py
+-rw-r--r--   0        0        0     1140 2024-04-21 16:36:14.966489 beta9-0.1.3/src/beta9/cli/main.py
+-rw-r--r--   0        0        0     3738 2024-04-21 16:36:14.968025 beta9-0.1.3/src/beta9/cli/task.py
+-rw-r--r--   0        0        0     8667 2024-04-21 16:36:14.970907 beta9-0.1.3/src/beta9/cli/volume.py
+-rw-r--r--   0        0        0        0 2024-04-25 22:02:49.680323 beta9-0.1.3/src/beta9/clients/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-25 22:07:33.794285 beta9-0.1.3/src/beta9/clients/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2980 2024-04-25 22:02:49.680448 beta9-0.1.3/src/beta9/clients/container/__init__.py
+-rw-r--r--   0        0        0     5732 2024-04-25 22:07:33.847103 beta9-0.1.3/src/beta9/clients/container/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4275 2024-04-25 22:02:49.473122 beta9-0.1.3/src/beta9/clients/endpoint/__init__.py
+-rw-r--r--   0        0        0     7204 2024-04-25 22:07:33.849454 beta9-0.1.3/src/beta9/clients/endpoint/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8023 2024-04-25 22:02:48.559816 beta9-0.1.3/src/beta9/clients/function/__init__.py
+-rw-r--r--   0        0        0    13329 2024-04-25 22:07:33.853498 beta9-0.1.3/src/beta9/clients/function/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    21072 2024-04-26 16:58:18.489835 beta9-0.1.3/src/beta9/clients/gateway/__init__.py
+-rw-r--r--   0        0        0    35251 2024-04-25 22:07:33.796452 beta9-0.1.3/src/beta9/clients/gateway/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4773 2024-04-25 22:02:48.104339 beta9-0.1.3/src/beta9/clients/image/__init__.py
+-rw-r--r--   0        0        0     8254 2024-04-25 22:07:33.834827 beta9-0.1.3/src/beta9/clients/image/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8003 2024-04-25 22:02:48.322282 beta9-0.1.3/src/beta9/clients/map/__init__.py
+-rw-r--r--   0        0        0    13990 2024-04-25 22:07:33.855581 beta9-0.1.3/src/beta9/clients/map/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8687 2024-04-25 22:02:48.786327 beta9-0.1.3/src/beta9/clients/simplequeue/__init__.py
+-rw-r--r--   0        0        0    13538 2024-04-25 22:07:33.857419 beta9-0.1.3/src/beta9/clients/simplequeue/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    13315 2024-04-25 22:02:49.277977 beta9-0.1.3/src/beta9/clients/taskqueue/__init__.py
+-rw-r--r--   0        0        0    21218 2024-04-25 22:07:33.860493 beta9-0.1.3/src/beta9/clients/taskqueue/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9482 2024-04-25 22:02:49.031862 beta9-0.1.3/src/beta9/clients/volume/__init__.py
+-rw-r--r--   0        0        0    16586 2024-04-25 22:07:33.836911 beta9-0.1.3/src/beta9/clients/volume/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7301 2024-04-21 16:36:14.980146 beta9-0.1.3/src/beta9/config.py
+-rw-r--r--   0        0        0      492 2024-04-26 16:58:18.490032 beta9-0.1.3/src/beta9/env.py
+-rw-r--r--   0        0        0      207 2024-01-27 16:13:22.966808 beta9-0.1.3/src/beta9/exceptions.py
+-rw-r--r--   0        0        0      883 2024-04-26 16:58:18.490335 beta9-0.1.3/src/beta9/logging.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.966902 beta9-0.1.3/src/beta9/runner/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-26 05:59:09.072510 beta9-0.1.3/src/beta9/runner/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7724 2024-04-26 05:59:09.073289 beta9-0.1.3/src/beta9/runner/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0        0        0     4442 2024-04-26 16:58:18.490515 beta9-0.1.3/src/beta9/runner/common.py
+-rw-r--r--   0        0        0     2321 2024-04-21 16:36:14.980604 beta9-0.1.3/src/beta9/runner/container.py
+-rw-r--r--   0        0        0     7465 2024-04-26 16:58:18.490672 beta9-0.1.3/src/beta9/runner/endpoint.py
+-rw-r--r--   0        0        0     6006 2024-04-26 16:58:18.490846 beta9-0.1.3/src/beta9/runner/function.py
+-rw-r--r--   0        0        0     3910 2024-04-21 16:36:14.986354 beta9-0.1.3/src/beta9/runner/serve.py
+-rw-r--r--   0        0        0    11017 2024-04-26 16:58:18.491042 beta9-0.1.3/src/beta9/runner/taskqueue.py
+-rw-r--r--   0        0        0     5713 2024-04-26 16:58:18.491443 beta9-0.1.3/src/beta9/sync.py
+-rw-r--r--   0        0        0     2994 2024-04-21 16:36:14.997902 beta9-0.1.3/src/beta9/terminal.py
+-rw-r--r--   0        0        0     1460 2024-04-26 16:58:18.491680 beta9-0.1.3/src/beta9/type.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 beta9-0.1.3/PKG-INFO
```

### Comparing `beta9-0.1.2rc1/pyproject.toml` & `beta9-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beta9"
-version = "0.1.2rc1"
+version = "0.1.3"
 description = ""
 authors = ["beam.cloud <support@beam.cloud>"]
 packages = [
     { include = "beta9", from = "src" },
     { include = "beta9/**/*.py", from = "src" },
 ]
```

### Comparing `beta9-0.1.2rc1/src/beta9/__init__.py` & `beta9-0.1.3/src/beta9/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from . import env
 from .abstractions.container import Container
 from .abstractions.endpoint import Endpoint as endpoint
 from .abstractions.function import Function as function
 from .abstractions.image import Image
 from .abstractions.map import Map
 from .abstractions.queue import SimpleQueue as Queue
 from .abstractions.taskqueue import TaskQueue as task_queue
@@ -14,8 +15,9 @@
     "Image",
     "Queue",
     "Volume",
     "task_queue",
     "function",
     "endpoint",
     "Container",
+    "env",
 ]
```

### Comparing `beta9-0.1.2rc1/src/beta9/abstractions/base/__init__.py` & `beta9-0.1.3/src/beta9/abstractions/base/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/abstractions/base/runner.py` & `beta9-0.1.3/src/beta9/abstractions/base/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ReplaceObjectContentRequest,
 )
 from ...sync import FileSyncer, SyncEventHandler
 
 CONTAINER_STUB_TYPE = "container"
 FUNCTION_STUB_TYPE = "function"
 TASKQUEUE_STUB_TYPE = "taskqueue"
-WEBSERVER_STUB_TYPE = "endpoint"
+ENDPOINT_STUB_TYPE = "endpoint"
 TASKQUEUE_DEPLOYMENT_STUB_TYPE = "taskqueue/deployment"
 ENDPOINT_DEPLOYMENT_STUB_TYPE = "endpoint/deployment"
 FUNCTION_DEPLOYMENT_STUB_TYPE = "function/deployment"
 TASKQUEUE_SERVE_STUB_TYPE = "taskqueue/serve"
 ENDPOINT_SERVE_STUB_TYPE = "endpoint/serve"
 FUNCTION_SERVE_STUB_TYPE = "function/serve"
 
@@ -41,20 +41,24 @@
         concurrency: int = 1,
         max_containers: int = 1,
         keep_warm_seconds: float = 10.0,
         max_pending_tasks: int = 100,
         retries: int = 3,
         timeout: int = 3600,
         volumes: Optional[List[Volume]] = None,
+        on_start: Optional[Callable] = None,
     ) -> None:
         super().__init__()
 
         if image is None:
             image = Image()
 
+        if on_start is not None:
+            self._map_callable_to_attr(attr="on_start", func=on_start)
+
         self.image: Image = image
         self.image_available: bool = False
         self.files_synced: bool = False
         self.stub_created: bool = False
         self.runtime_ready: bool = False
         self.object_id: str = ""
         self.image_id: str = ""
@@ -108,27 +112,31 @@
                 raise ValueError(
                     "Invalid CPU string format. Must be a digit followed by 'm' (e.g., '1000m')."
                 )
 
         else:
             raise TypeError("CPU must be a float or a string.")
 
-    def _load_handler(self, func: Callable) -> None:
-        if self.handler or func is None:
+    def _map_callable_to_attr(self, *, attr: str, func: Callable):
+        """
+        Determine the module and function name of a callable function, and cache on the class.
+        This is used for passing callables to stub config.
+        """
+        if getattr(self, attr):
             return
 
         module = inspect.getmodule(func)  # Determine module / function name
         if module:
             module_file = os.path.basename(module.__file__)
             module_name = os.path.splitext(module_file)[0]
         else:
             module_name = "__main__"
 
         function_name = func.__name__
-        self.handler = f"{module_name}:{function_name}"
+        setattr(self, attr, f"{module_name}:{function_name}")
 
     async def _object_iterator(self, *, dir: str, object_id: str, file_update_queue: Queue):
         while True:
             try:
                 operation, path = file_update_queue.get_nowait()
 
                 if operation == ReplaceObjectContentOperation.WRITE:
@@ -171,15 +179,15 @@
         *,
         func: Optional[Callable] = None,
         stub_type: str,
         force_create_stub: bool = False,
         name: Optional[str] = None,
     ) -> bool:
         if func is not None:
-            self._load_handler(func)
+            self._map_callable_to_attr(attr="handler", func=func)
 
         stub_name = f"{stub_type}/{self.handler}" if self.handler else stub_type
 
         if name:
             stub_name = f"{stub_name}/{name}"
 
         if self.runtime_ready:
@@ -218,14 +226,15 @@
                         stub_type=stub_type,
                         name=stub_name,
                         python_version=self.image.python_version,
                         cpu=self.cpu,
                         memory=self.memory,
                         gpu=self.gpu,
                         handler=self.handler,
+                        on_start=self.on_start,
                         retries=self.retries,
                         timeout=self.timeout,
                         keep_warm_seconds=self.keep_warm_seconds,
                         concurrency=self.concurrency,
                         max_containers=self.max_containers,
                         max_pending_tasks=self.max_pending_tasks,
                         volumes=[v.export() for v in self.volumes],
```

### Comparing `beta9-0.1.2rc1/src/beta9/abstractions/container.py` & `beta9-0.1.3/src/beta9/abstractions/container.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/abstractions/endpoint.py` & `beta9-0.1.3/src/beta9/abstractions/endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,75 @@
 import os
-from typing import Any, Callable, Union
+from typing import Any, Callable, Optional, Union
 
 from .. import terminal
 from ..abstractions.base.runner import (
     ENDPOINT_DEPLOYMENT_STUB_TYPE,
     ENDPOINT_SERVE_STUB_TYPE,
     RunnerAbstraction,
 )
 from ..abstractions.image import Image
-from ..clients.endpoint import EndpointServeRequest, EndpointServiceStub
+from ..clients.endpoint import (
+    EndpointServiceStub,
+    StartEndpointServeRequest,
+    StopEndpointServeRequest,
+)
 from ..clients.gateway import DeployStubRequest, DeployStubResponse
 from ..config import GatewayConfig, get_gateway_config
+from ..env import is_local
 
 
 class Endpoint(RunnerAbstraction):
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
         memory: int = 128,
         gpu: str = "",
         image: Image = Image(),
         timeout: int = 180,
         concurrency: int = 1,
         max_containers: int = 1,
         keep_warm_seconds: int = 300,
         max_pending_tasks: int = 100,
+        on_start: Optional[Callable] = None,
     ):
         super().__init__(
             cpu=cpu,
             memory=memory,
             gpu=gpu,
             image=image,
             concurrency=concurrency,
             max_containers=max_containers,
             timeout=timeout,
             retries=0,
             keep_warm_seconds=keep_warm_seconds,
             max_pending_tasks=max_pending_tasks,
+            on_start=on_start,
         )
 
         self.endpoint_stub: EndpointServiceStub = EndpointServiceStub(self.channel)
 
     def __call__(self, func):
         return _CallableWrapper(func, self)
 
 
 class _CallableWrapper:
     def __init__(self, func: Callable, parent: Endpoint):
         self.func: Callable = func
         self.parent: Endpoint = parent
 
     def __call__(self, *args, **kwargs) -> Any:
-        container_id = os.getenv("CONTAINER_ID")
-        if container_id is not None:
+        if not is_local():
             return self.local(*args, **kwargs)
 
         raise NotImplementedError("Direct calls to Endpoints are not supported.")
 
+    def local(self, *args, **kwargs) -> Any:
+        return self.func(*args, **kwargs)
+
     def deploy(self, name: str) -> bool:
         if not self.parent.prepare_runtime(
             func=self.func, stub_type=ENDPOINT_DEPLOYMENT_STUB_TYPE, force_create_stub=True
         ):
             return False
 
         terminal.header("Deploying endpoint")
@@ -89,23 +98,34 @@
 
         try:
             with terminal.progress("Serving endpoint..."):
                 return self.parent.run_sync(
                     self._serve(dir=os.getcwd(), object_id=self.parent.object_id)
                 )
         except KeyboardInterrupt:
-            terminal.prompt(text="Would you like to stop the container? (y/n)", default="y")
+            response = terminal.prompt(
+                text="Would you like to stop the container? (y/n)", default="y"
+            )
+            if response == "y":
+                terminal.header("Stopping serve container")
+                self.parent.run_sync(
+                    self.parent.endpoint_stub.stop_endpoint_serve(
+                        StopEndpointServeRequest(stub_id=self.parent.stub_id)
+                    )
+                )
+
+        terminal.print("Goodbye 👋")
 
     async def _serve(self, *, dir: str, object_id: str):
         sync_task = self.parent.loop.create_task(
             self.parent.sync_dir_to_workspace(dir=dir, object_id=object_id)
         )
         try:
-            async for r in self.parent.endpoint_stub.endpoint_serve(
-                EndpointServeRequest(
+            async for r in self.parent.endpoint_stub.start_endpoint_serve(
+                StartEndpointServeRequest(
                     stub_id=self.parent.stub_id,
                 )
             ):
                 if r.output != "":
                     terminal.detail(r.output.strip())
 
                 if r.done or r.exit_code != 0:
```

### Comparing `beta9-0.1.2rc1/src/beta9/abstractions/function.py` & `beta9-0.1.3/src/beta9/abstractions/function.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import os
 from typing import Any, Callable, Iterator, List, Optional, Sequence, Union
 
 import cloudpickle
 
 from .. import terminal
 from ..abstractions.base.runner import (
     FUNCTION_DEPLOYMENT_STUB_TYPE,
@@ -15,14 +14,15 @@
 from ..clients.function import (
     FunctionInvokeRequest,
     FunctionInvokeResponse,
     FunctionServiceStub,
 )
 from ..clients.gateway import DeployStubRequest, DeployStubResponse
 from ..config import GatewayConfig, get_gateway_config
+from ..env import is_local
 from ..sync import FileSyncer
 
 
 class Function(RunnerAbstraction):
     """
     Decorator which allows you to run the decorated function in a remote container.
 
@@ -59,34 +59,43 @@
     """
 
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
         memory: int = 128,
         gpu: str = "",
+        timeout: int = 3600,
+        retries: int = 3,
         image: Image = Image(),
         volumes: Optional[List[Volume]] = None,
     ) -> None:
-        super().__init__(cpu=cpu, memory=memory, gpu=gpu, image=image, volumes=volumes)
+        super().__init__(
+            cpu=cpu,
+            memory=memory,
+            gpu=gpu,
+            image=image,
+            volumes=volumes,
+            timeout=timeout,
+            retries=retries,
+        )
 
         self.function_stub: FunctionServiceStub = FunctionServiceStub(self.channel)
         self.syncer: FileSyncer = FileSyncer(self.gateway_stub)
 
     def __call__(self, func):
         return _CallableWrapper(func, self)
 
 
 class _CallableWrapper:
     def __init__(self, func: Callable, parent: Function) -> None:
         self.func: Callable = func
         self.parent: Function = parent
 
     def __call__(self, *args, **kwargs) -> Any:
-        container_id = os.getenv("CONTAINER_ID")
-        if container_id:
+        if not is_local():
             return self.local(*args, **kwargs)
 
         if not self.parent.prepare_runtime(
             func=self.func,
             stub_type=FUNCTION_STUB_TYPE,
         ):
             return
@@ -151,19 +160,28 @@
             terminal.header("Deployed 🎉")
             terminal.detail(
                 f"Call your deployment at: {gateway_url}/api/v1/function/{name}/v{deploy_response.version}"
             )
 
         return deploy_response.ok
 
+    def _format_args(self, args):
+        if isinstance(args, tuple):
+            return list(args)
+        elif not isinstance(args, list):
+            return [args]
+        return args
+
     def _gather_and_yield_results(self, inputs: Sequence) -> Iterator[Any]:
         container_count = len(inputs)
 
         async def _gather_async():
-            tasks = [asyncio.create_task(self._call_remote(input)) for input in inputs]
+            tasks = [
+                asyncio.create_task(self._call_remote(*self._format_args(args))) for args in inputs
+            ]
             for task in asyncio.as_completed(tasks):
                 yield await task
 
         async_gen = _gather_async()
         with terminal.progress(f"Running {container_count} containers..."):
             while True:
                 try:
```

### Comparing `beta9-0.1.2rc1/src/beta9/abstractions/image.py` & `beta9-0.1.3/src/beta9/abstractions/image.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/abstractions/map.py` & `beta9-0.1.3/src/beta9/abstractions/map.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/abstractions/queue.py` & `beta9-0.1.3/src/beta9/abstractions/queue.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/abstractions/taskqueue.py` & `beta9-0.1.3/src/beta9/abstractions/taskqueue.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import json
 import os
-from typing import Any, Callable, Union
+from typing import Any, Callable, Optional, Union
 
 from .. import terminal
 from ..abstractions.base.runner import (
     TASKQUEUE_DEPLOYMENT_STUB_TYPE,
+    TASKQUEUE_SERVE_STUB_TYPE,
     TASKQUEUE_STUB_TYPE,
     RunnerAbstraction,
 )
 from ..abstractions.image import Image
 from ..clients.gateway import DeployStubRequest, DeployStubResponse
-from ..clients.taskqueue import TaskQueuePutRequest, TaskQueuePutResponse, TaskQueueServiceStub
+from ..clients.taskqueue import (
+    StartTaskQueueServeRequest,
+    StopTaskQueueServeRequest,
+    TaskQueuePutRequest,
+    TaskQueuePutResponse,
+    TaskQueueServiceStub,
+)
 from ..config import GatewayConfig, get_gateway_config
+from ..env import is_local
 
 
 class TaskQueue(RunnerAbstraction):
     """
     Decorator which allows you to create a task queue out of the decorated function. The tasks are executed
     asynchronously, in remote containers. You can interact with the task queue either through an API (when deployed), or directly
     in python through the .put() method.
@@ -51,14 +59,17 @@
             The duration in seconds to keep the task queue warm even if there are no pending
             tasks. Keeping the queue warm helps to reduce the latency when new tasks arrive.
             Default is 10s.
         max_pending_tasks (int):
             The maximum number of tasks that can be pending in the queue. If the number of
             pending tasks exceeds this value, the task queue will stop accepting new tasks.
             Default is 100.
+        on_start (Optional[Callable]):
+            An optional function to run once (per process) when the container starts. Can be used for downloading data,
+            loading models, or anything else computationally expensive.
     Example:
         ```python
         from beta9 import task_queue, Image
 
         @task_queue(cpu=1.0, memory=128, gpu="T4", image=Image(python_packages=["torch"]), keep_warm_seconds=1000)
         def transcribe(filename: str):
             print(filename)
@@ -77,42 +88,43 @@
         image: Image = Image(),
         timeout: int = 3600,
         retries: int = 3,
         concurrency: int = 1,
         max_containers: int = 1,
         keep_warm_seconds: int = 10,
         max_pending_tasks: int = 100,
+        on_start: Optional[Callable] = None,
     ) -> None:
         super().__init__(
             cpu=cpu,
             memory=memory,
             gpu=gpu,
             image=image,
             concurrency=concurrency,
             max_containers=max_containers,
             timeout=timeout,
             retries=retries,
             keep_warm_seconds=keep_warm_seconds,
             max_pending_tasks=max_pending_tasks,
+            on_start=on_start,
         )
 
         self.taskqueue_stub: TaskQueueServiceStub = TaskQueueServiceStub(self.channel)
 
     def __call__(self, func):
         return _CallableWrapper(func, self)
 
 
 class _CallableWrapper:
     def __init__(self, func: Callable, parent: TaskQueue):
         self.func: Callable = func
         self.parent: TaskQueue = parent
 
     def __call__(self, *args, **kwargs) -> Any:
-        container_id = os.getenv("CONTAINER_ID")
-        if container_id is not None:
+        if not is_local():
             return self.local(*args, **kwargs)
 
         raise NotImplementedError(
             "Direct calls to TaskQueues are not yet supported."
             + " To enqueue items use .put(*args, **kwargs)"
         )
 
@@ -139,14 +151,61 @@
             terminal.header("Deployed 🎉")
             terminal.detail(
                 f"Call your deployment at: {gateway_url}/api/v1/taskqueue/{name}/v{deploy_response.version}"
             )
 
         return deploy_response.ok
 
+    def serve(self):
+        if not self.parent.prepare_runtime(
+            func=self.func, stub_type=TASKQUEUE_SERVE_STUB_TYPE, force_create_stub=True
+        ):
+            return False
+
+        try:
+            with terminal.progress("Serving taskqueue..."):
+                return self.parent.run_sync(
+                    self._serve(dir=os.getcwd(), object_id=self.parent.object_id)
+                )
+        except KeyboardInterrupt:
+            response = terminal.prompt(
+                text="Would you like to stop the container? (y/n)", default="y"
+            )
+            if response == "y":
+                terminal.header("Stopping serve container")
+                self.parent.run_sync(
+                    self.parent.taskqueue_stub.stop_task_queue_serve(
+                        StopTaskQueueServeRequest(stub_id=self.parent.stub_id)
+                    )
+                )
+
+        terminal.print("Goodbye 👋")
+
+    async def _serve(self, *, dir: str, object_id: str):
+        sync_task = self.parent.loop.create_task(
+            self.parent.sync_dir_to_workspace(dir=dir, object_id=object_id)
+        )
+        try:
+            async for r in self.parent.taskqueue_stub.start_task_queue_serve(
+                StartTaskQueueServeRequest(
+                    stub_id=self.parent.stub_id,
+                )
+            ):
+                if r.output != "":
+                    terminal.detail(r.output.strip())
+
+                if r.done or r.exit_code != 0:
+                    last_response = r
+                    break
+
+            if last_response is None or not last_response.done or last_response.exit_code != 0:
+                terminal.error("Serve container failed ☠️")
+        finally:
+            sync_task.cancel()
+
     def put(self, *args, **kwargs) -> bool:
         if not self.parent.prepare_runtime(
             func=self.func,
             stub_type=TASKQUEUE_STUB_TYPE,
         ):
             return False
```

### Comparing `beta9-0.1.2rc1/src/beta9/abstractions/volume.py` & `beta9-0.1.3/src/beta9/abstractions/volume.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/cli/config.py` & `beta9-0.1.3/src/beta9/cli/config.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/cli/contexts.py` & `beta9-0.1.3/src/beta9/cli/contexts.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/cli/deployment.py` & `beta9-0.1.3/src/beta9/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/cli/extraclick.py` & `beta9-0.1.3/src/beta9/cli/extraclick.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/cli/main.py` & `beta9-0.1.3/src/beta9/cli/main.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/cli/task.py` & `beta9-0.1.3/src/beta9/cli/task.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/cli/volume.py` & `beta9-0.1.3/src/beta9/cli/volume.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/clients/container/__init__.py` & `beta9-0.1.3/src/beta9/clients/container/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/clients/function/__init__.py` & `beta9-0.1.3/src/beta9/clients/function/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/clients/gateway/__init__.py` & `beta9-0.1.3/src/beta9/clients/gateway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,15 @@
     timeout: int = betterproto.int64_field(11)
     keep_warm_seconds: float = betterproto.float_field(12)
     concurrency: int = betterproto.uint32_field(13)
     max_containers: int = betterproto.uint32_field(14)
     max_pending_tasks: int = betterproto.uint32_field(15)
     volumes: List["Volume"] = betterproto.message_field(16)
     force_create: bool = betterproto.bool_field(17)
+    on_start: str = betterproto.string_field(18)
 
 
 @dataclass(eq=False, repr=False)
 class GetOrCreateStubResponse(betterproto.Message):
     ok: bool = betterproto.bool_field(1)
     stub_id: str = betterproto.string_field(2)
```

### Comparing `beta9-0.1.2rc1/src/beta9/clients/image/__init__.py` & `beta9-0.1.3/src/beta9/clients/image/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/clients/map/__init__.py` & `beta9-0.1.3/src/beta9/clients/map/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/clients/simplequeue/__init__.py` & `beta9-0.1.3/src/beta9/clients/simplequeue/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/clients/taskqueue/__init__.py` & `beta9-0.1.3/src/beta9/clients/taskqueue/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -84,14 +84,36 @@
 class TaskQueueMonitorResponse(betterproto.Message):
     ok: bool = betterproto.bool_field(1)
     cancelled: bool = betterproto.bool_field(2)
     complete: bool = betterproto.bool_field(3)
     timed_out: bool = betterproto.bool_field(4)
 
 
+@dataclass(eq=False, repr=False)
+class StartTaskQueueServeRequest(betterproto.Message):
+    stub_id: str = betterproto.string_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class StartTaskQueueServeResponse(betterproto.Message):
+    output: str = betterproto.string_field(1)
+    done: bool = betterproto.bool_field(2)
+    exit_code: int = betterproto.int32_field(3)
+
+
+@dataclass(eq=False, repr=False)
+class StopTaskQueueServeRequest(betterproto.Message):
+    stub_id: str = betterproto.string_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class StopTaskQueueServeResponse(betterproto.Message):
+    ok: bool = betterproto.bool_field(1)
+
+
 class TaskQueueServiceStub(betterproto.ServiceStub):
     async def task_queue_put(
         self,
         task_queue_put_request: "TaskQueuePutRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
@@ -171,14 +193,49 @@
             task_queue_length_request,
             TaskQueueLengthResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
+    async def start_task_queue_serve(
+        self,
+        start_task_queue_serve_request: "StartTaskQueueServeRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> AsyncIterator["StartTaskQueueServeResponse"]:
+        async for response in self._unary_stream(
+            "/taskqueue.TaskQueueService/StartTaskQueueServe",
+            start_task_queue_serve_request,
+            StartTaskQueueServeResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    async def stop_task_queue_serve(
+        self,
+        stop_task_queue_serve_request: "StopTaskQueueServeRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "StopTaskQueueServeResponse":
+        return await self._unary_unary(
+            "/taskqueue.TaskQueueService/StopTaskQueueServe",
+            stop_task_queue_serve_request,
+            StopTaskQueueServeResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
 
 class TaskQueueServiceBase(ServiceBase):
 
     async def task_queue_put(
         self, task_queue_put_request: "TaskQueuePutRequest"
     ) -> "TaskQueuePutResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
@@ -200,14 +257,25 @@
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def task_queue_length(
         self, task_queue_length_request: "TaskQueueLengthRequest"
     ) -> "TaskQueueLengthResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
+    async def start_task_queue_serve(
+        self, start_task_queue_serve_request: "StartTaskQueueServeRequest"
+    ) -> AsyncIterator["StartTaskQueueServeResponse"]:
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+        yield StartTaskQueueServeResponse()
+
+    async def stop_task_queue_serve(
+        self, stop_task_queue_serve_request: "StopTaskQueueServeRequest"
+    ) -> "StopTaskQueueServeResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
     async def __rpc_task_queue_put(
         self, stream: "grpclib.server.Stream[TaskQueuePutRequest, TaskQueuePutResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.task_queue_put(request)
         await stream.send_message(response)
 
@@ -241,14 +309,33 @@
         self,
         stream: "grpclib.server.Stream[TaskQueueLengthRequest, TaskQueueLengthResponse]",
     ) -> None:
         request = await stream.recv_message()
         response = await self.task_queue_length(request)
         await stream.send_message(response)
 
+    async def __rpc_start_task_queue_serve(
+        self,
+        stream: "grpclib.server.Stream[StartTaskQueueServeRequest, StartTaskQueueServeResponse]",
+    ) -> None:
+        request = await stream.recv_message()
+        await self._call_rpc_handler_server_stream(
+            self.start_task_queue_serve,
+            stream,
+            request,
+        )
+
+    async def __rpc_stop_task_queue_serve(
+        self,
+        stream: "grpclib.server.Stream[StopTaskQueueServeRequest, StopTaskQueueServeResponse]",
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.stop_task_queue_serve(request)
+        await stream.send_message(response)
+
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
             "/taskqueue.TaskQueueService/TaskQueuePut": grpclib.const.Handler(
                 self.__rpc_task_queue_put,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 TaskQueuePutRequest,
                 TaskQueuePutResponse,
@@ -273,8 +360,20 @@
             ),
             "/taskqueue.TaskQueueService/TaskQueueLength": grpclib.const.Handler(
                 self.__rpc_task_queue_length,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 TaskQueueLengthRequest,
                 TaskQueueLengthResponse,
             ),
+            "/taskqueue.TaskQueueService/StartTaskQueueServe": grpclib.const.Handler(
+                self.__rpc_start_task_queue_serve,
+                grpclib.const.Cardinality.UNARY_STREAM,
+                StartTaskQueueServeRequest,
+                StartTaskQueueServeResponse,
+            ),
+            "/taskqueue.TaskQueueService/StopTaskQueueServe": grpclib.const.Handler(
+                self.__rpc_stop_task_queue_serve,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                StopTaskQueueServeRequest,
+                StopTaskQueueServeResponse,
+            ),
         }
```

### Comparing `beta9-0.1.2rc1/src/beta9/clients/volume/__init__.py` & `beta9-0.1.3/src/beta9/clients/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/config.py` & `beta9-0.1.3/src/beta9/config.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/logging.py` & `beta9-0.1.3/src/beta9/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
-import sys
 import json
+import sys
+
 
 class StdoutJsonInterceptor(io.TextIOBase):
     def __init__(self, stream=sys.__stdout__, **ctx):
         self.ctx = ctx
         self.stream = stream
 
     def __enter__(self):
@@ -30,8 +31,7 @@
             self.stream.write(buf)
 
     def flush(self):
         return self.stream.flush()
 
     def fileno(self) -> int:
         return -1
-
```

### Comparing `beta9-0.1.2rc1/src/beta9/runner/container.py` & `beta9-0.1.3/src/beta9/runner/container.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/runner/function.py` & `beta9-0.1.3/src/beta9/runner/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     GatewayServiceStub,
     StartTaskRequest,
     StartTaskResponse,
 )
 from ..config import with_runner_context
 from ..exceptions import InvalidFunctionArgumentsException, RunnerException
 from ..logging import StdoutJsonInterceptor
-from ..runner.common import config, load_handler
+from ..runner.common import FunctionContext, FunctionHandler, config
 from ..type import TaskExitCode, TaskStatus
 
 
 def _load_args(args: bytes) -> dict:
     try:
         return cloudpickle.loads(args)
     except BaseException:
@@ -127,36 +127,39 @@
         if not start_task_response.ok:
             raise RunnerException("Unable to start task")
 
         # Kick off monitoring task
         monitor_task = loop.create_task(
             _monitor_task(
                 stub_id=config.stub_id,
-                task_id=config.task_id,
+                task_id=task_id,
                 container_id=config.container_id,
                 function_stub=function_stub,
             ),
         )
 
         task_status = TaskStatus.Complete
         error = None
 
         # Invoke function
         try:
-            handler = load_handler()
             get_args_resp: FunctionGetArgsResponse = run_sync(
                 function_stub.function_get_args(FunctionGetArgsRequest(task_id=task_id)),
             )
             if not get_args_resp.ok:
                 raise InvalidFunctionArgumentsException
 
+            handler = FunctionHandler()
+            context = FunctionContext.new(config=config, task_id=task_id)
+
             payload: dict = _load_args(get_args_resp.args)
             args = payload.get("args") or []
             kwargs = payload.get("kwargs") or {}
-            result = handler(*args, **kwargs)
+
+            result = handler(context, *args, **kwargs)
         except BaseException as exc:
             result = error = exc
             task_status = TaskStatus.Error
         finally:
             result = cloudpickle.dumps(result)
             set_result_resp: FunctionSetResultResponse = run_sync(
                 function_stub.function_set_result(
```

### Comparing `beta9-0.1.2rc1/src/beta9/runner/serve.py` & `beta9-0.1.3/src/beta9/runner/serve.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/runner/taskqueue.py` & `beta9-0.1.3/src/beta9/runner/taskqueue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import atexit
 import json
 import os
 import signal
 import sys
 import threading
 import time
 import traceback
@@ -26,58 +25,69 @@
     TaskQueuePopRequest,
     TaskQueuePopResponse,
     TaskQueueServiceStub,
 )
 from ..config import with_runner_context
 from ..exceptions import RunnerException
 from ..logging import StdoutJsonInterceptor
-from ..runner.common import config, load_handler
-from ..type import TaskExitCode, TaskStatus
+from ..runner.common import FunctionContext, FunctionHandler, config, execute_lifecycle_method
+from ..type import LifeCycleMethod, TaskExitCode, TaskStatus
 
 TASK_PROCESS_WATCHDOG_INTERVAL = 0.01
 TASK_POLLING_INTERVAL = 0.01
+TASK_MANAGER_INTERVAL = 0.1
 
 
 class TaskQueueManager:
     def __init__(self) -> None:
-        self._setup_signal_handlers()
-
-        set_start_method("spawn", force=True)
-
         # Manager attributes
         self.pid: int = os.getpid()
         self.exit_code: int = 0
+        self.shutdown_event = Event()
+
+        self._setup_signal_handlers()
+        set_start_method("spawn", force=True)
 
         # Task worker attributes
         self.task_worker_count: int = config.concurrency
         self.task_processes: List[Process] = []
         self.task_workers: List[TaskQueueWorker] = []
         self.task_worker_startup_events: List[Event] = [
             Event() for _ in range(self.task_worker_count)
         ]
         self.task_worker_watchdog_threads: List[threading.Thread] = []
 
     def _setup_signal_handlers(self):
-        signal.signal(signal.SIGTERM, self.shutdown)
+        if os.getpid() == self.pid:
+            signal.signal(signal.SIGTERM, self._init_shutdown)
+
+    def _init_shutdown(self, signum=None, frame=None):
+        self.shutdown_event.set()
 
     def run(self):
         for worker_index in range(self.task_worker_count):
             print(f"Starting task worker[{worker_index}]")
             self._start_worker(worker_index)
 
-        for task_process in self.task_processes:
-            task_process.join()
+        while not self.shutdown_event.is_set():
+            time.sleep(TASK_MANAGER_INTERVAL)
+
+        self.shutdown()
 
-    def shutdown(self, signum=None, frame=None):
+    def shutdown(self):
+        print("Spinning down taskqueue")
+
+        # Terminate all worker processes
         for task_process in self.task_processes:
             task_process.terminate()
-            task_process.join()
+            task_process.join(timeout=5)
 
         for task_process in self.task_processes:
             if task_process.is_alive():
+                print("Task process did not join within the timeout. Terminating...")
                 task_process.terminate()
                 task_process.join(timeout=0)
 
             if task_process.exitcode != 0:
                 self.exit_code = task_process.exitcode
 
     def _start_worker(self, worker_index: int):
@@ -225,43 +235,52 @@
                 print("Unexpected error occurred in task monitor")
                 os._exit(0)
 
     @with_runner_context
     def process_tasks(self, channel: Channel) -> None:
         self.worker_startup_event.set()
         loop = asyncio.get_event_loop()
-
-        taskqueue_stub: TaskQueueServiceStub = TaskQueueServiceStub(channel)
-
-        handler = load_handler()
         executor = ThreadPoolExecutor()
+        taskqueue_stub = TaskQueueServiceStub(channel)
+
+        # Load handler and execute on_start method
+        handler = FunctionHandler()
+        on_start_value = execute_lifecycle_method(name=LifeCycleMethod.OnStart)
 
         print(f"Worker[{self.worker_index}] ready")
         while True:
             task = self._get_next_task(taskqueue_stub, config.stub_id, config.container_id)
             if not task:
                 time.sleep(TASK_POLLING_INTERVAL)
                 continue
 
             async def _run_task():
                 with StdoutJsonInterceptor(task_id=task.id):
                     print(f"Running task <{task.id}>")
+
                     monitor_task = loop.create_task(
                         self._monitor_task(
                             config.stub_id, config.container_id, taskqueue_stub, task
                         ),
                     )
 
                     start_time = time.time()
                     task_status = TaskStatus.Complete
                     try:
                         args = task.args or []
                         kwargs = task.kwargs or {}
+
+                        context = FunctionContext.new(
+                            config=config,
+                            task_id=task.id,
+                            on_start_value=on_start_value,
+                        )
+
                         result = await loop.run_in_executor(
-                            executor, lambda: handler(*args, **kwargs)
+                            executor, lambda: handler(context, *args, **kwargs)
                         )
                         result = cloudpickle.dumps(result)
                     except BaseException as exc:
                         print(traceback.format_exc())
                         result = cloudpickle.dumps(exc)
                         task_status = TaskStatus.Error
                     finally:
@@ -286,13 +305,11 @@
                         monitor_task.cancel()
 
             loop.run_until_complete(_run_task())
 
 
 if __name__ == "__main__":
     tq = TaskQueueManager()
-    atexit.register(tq.shutdown)
-
     tq.run()
 
     if tq.exit_code != 0 and tq.exit_code != TaskExitCode.SigTerm:
         sys.exit(tq.exit_code)
```

### Comparing `beta9-0.1.2rc1/src/beta9/sync.py` & `beta9-0.1.3/src/beta9/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     HeadObjectRequest,
     HeadObjectResponse,
     ObjectMetadata,
     PutObjectRequest,
     PutObjectResponse,
     ReplaceObjectContentOperation,
 )
+from .env import is_local
 
 CHUNK_SIZE = 1024 * 1024 * 4
 IGNORE_FILE_NAME = ".beta9ignore"
 IGNORE_FILE_CONTENTS = """# Generated by Beta9 SDK
 .beta9ignore
 .git
 .idea
@@ -53,22 +54,28 @@
         self.gateway_stub: GatewayServiceStub = gateway_stub
 
     @property
     def ignore_file_path(self) -> Path:
         return self.root_dir / IGNORE_FILE_NAME
 
     def _init_ignore_file(self) -> None:
+        if not is_local():
+            return
+
         if self.ignore_file_path.exists():
             return
 
         terminal.detail(f"Writing {IGNORE_FILE_NAME} file")
         with self.ignore_file_path.open(mode="w") as f:
             f.writelines(IGNORE_FILE_CONTENTS)
 
     def _read_ignore_file(self) -> list:
+        if not is_local():
+            return
+
         terminal.detail(f"Reading {IGNORE_FILE_NAME} file")
 
         patterns = []
 
         if self.ignore_file_path.is_file():
             with self.ignore_file_path.open() as file:
                 patterns = [line.strip() for line in file.readlines() if line.strip()]
```

### Comparing `beta9-0.1.2rc1/src/beta9/terminal.py` & `beta9-0.1.3/src/beta9/terminal.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2rc1/src/beta9/type.py` & `beta9-0.1.3/src/beta9/type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from enum import Enum
 
 
+class LifeCycleMethod(str, Enum):
+    OnStart = "on_start"
+
+
 class TaskStatus(str, Enum):
     Complete = "COMPLETE"
     Error = "ERROR"
     Pending = "PENDING"
     Running = "RUNNING"
     Cancelled = "CANCELLED"
     Retry = "RETRY"
```

### Comparing `beta9-0.1.2rc1/PKG-INFO` & `beta9-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: beta9
-Version: 0.1.2rc1
+Version: 0.1.3
 Summary: 
 Author: beam.cloud
 Author-email: support@beam.cloud
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asgiref (>=3.7.2,<4.0.0)
 Requires-Dist: betterproto[compiler] (==2.0.0b6)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cloudpickle (>=3.0.0,<4.0.0)
 Requires-Dist: croniter (>=2.0.3,<3.0.0)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
```

