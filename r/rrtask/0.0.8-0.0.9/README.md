# Comparing `tmp/rrtask-0.0.8.tar.gz` & `tmp/rrtask-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrtask-0.0.8.tar", max compression
+gzip compressed data, was "rrtask-0.0.9.tar", max compression
```

## Comparing `rrtask-0.0.8.tar` & `rrtask-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.8/LICENSE
--rw-r--r--   0        0        0      210 2024-04-24 08:52:17.584490 rrtask-0.0.8/README.md
--rw-r--r--   0        0        0      624 2024-04-24 16:52:59.664139 rrtask-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      133 2024-04-24 09:02:58.172982 rrtask-0.0.8/rrtask/__init__.py
--rw-r--r--   0        0        0      195 2024-04-24 12:06:28.840639 rrtask-0.0.8/rrtask/enums.py
--rw-r--r--   0        0        0     6401 2024-04-24 16:52:08.508061 rrtask-0.0.8/rrtask/rrtask.py
--rw-r--r--   0        0        0      394 2024-04-24 08:50:30.008555 rrtask-0.0.8/rrtask/signals.py
--rw-r--r--   0        0        0      179 2024-04-24 16:38:09.798808 rrtask-0.0.8/rrtask/utils.py
--rw-r--r--   0        0        0       18 2024-04-24 16:53:29.008184 rrtask-0.0.8/rrtask/version.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 rrtask-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.9/LICENSE
+-rw-r--r--   0        0        0      210 2024-04-24 08:52:17.584490 rrtask-0.0.9/README.md
+-rw-r--r--   0        0        0      624 2024-04-26 14:43:58.123661 rrtask-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      133 2024-04-24 09:02:58.172982 rrtask-0.0.9/rrtask/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-24 12:06:28.840639 rrtask-0.0.9/rrtask/enums.py
+-rw-r--r--   0        0        0     6735 2024-04-26 14:04:37.278862 rrtask-0.0.9/rrtask/rrtask.py
+-rw-r--r--   0        0        0      394 2024-04-24 08:50:30.008555 rrtask-0.0.9/rrtask/signals.py
+-rw-r--r--   0        0        0      179 2024-04-26 13:53:35.643854 rrtask-0.0.9/rrtask/utils.py
+-rw-r--r--   0        0        0       18 2024-04-26 14:46:58.627948 rrtask-0.0.9/rrtask/version.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 rrtask-0.0.9/PKG-INFO
```

### Comparing `rrtask-0.0.8/LICENSE` & `rrtask-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rrtask-0.0.8/pyproject.toml` & `rrtask-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rrtask"
-version = "0.0.8"
+version = "0.0.9"
 description = "Round Robin Task"
 authors = ["François Schmidts <francois@schmidts.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "==3.7.*"
```

### Comparing `rrtask-0.0.8/rrtask/rrtask.py` & `rrtask-0.0.9/rrtask/rrtask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from typing import Generator, Optional, Union
 
 from redis import Redis
 from celery import Celery, current_task  # type: ignore
+from pyrabbit.http import HTTPError
 
 from rrtask import signals
 from rrtask.enums import State
 from rrtask.utils import get_rabbitmq_client
 
 logger = logging.getLogger(__name__)
 
@@ -16,15 +17,15 @@
     _lock_expire = 10 * 60
     _encoding = "utf8"
 
     def __init__(
         self,
         celery: Celery,
         redis: Redis,
-        queue_prefix: str = "",
+        queue_prefix: Optional[str] = None,
     ):
         self._celery = celery
         self._redis = redis
         self._queue_prefix = queue_prefix
 
         logger.info("[%s] Initializing celery tasks", self.queue_name)
         self._recurring_task = self.__set_recuring_task()
@@ -40,42 +41,50 @@
         """This method should return an iterable. Each element of this iterable
         is a valid argument for the true task (aka self.recurring_task).
         """
         raise NotImplementedError("should be overridden")
 
     @property
     def queue_name(self):
-        if self._queue_prefix:
+        if self._queue_prefix is not None:
             return f"{self._queue_prefix}.{self.__class__.__name__}"
         return self.__class__.__name__
 
     @property
     def is_queue_empty(self) -> int:
         rabbitmq_conn = self._celery.broker_connection()
         rabbitmq_client = get_rabbitmq_client(
             rabbitmq_conn.host, rabbitmq_conn.userid, rabbitmq_conn.password
         )
-        queue_depth = rabbitmq_client.get_queue_depth(
-            rabbitmq_conn.virtual_host, self.queue_name
-        )
+        try:
+            queue_depth = rabbitmq_client.get_queue_depth(
+                rabbitmq_conn.virtual_host, self.queue_name
+            )
+        except HTTPError as error:
+            if getattr(error, "reason", "") == "Object Not Found":
+                return True
+            queue_depth = 1
         return queue_depth == 0
 
+    @property
+    def scheduler_key(self):
+        return f"rrtask.{self.queue_name}.scheduler_id"
+
     def can_reschedule(self, force: bool = False) -> bool:
         lock_key = f"rrtask.{self.queue_name}.lock"
-        scheduler_key = f"rrtask.{self.queue_name}.scheduler_id"
         if not self._redis.setnx(lock_key, 1) and not force:
             logger.debug("[%s] scheduling forbidden: locked")
             return False
         self._redis.expire(lock_key, self._lock_expire)
         try:
             scheduler_id = current_task.request.id.encode(self._encoding)
         except AttributeError:
             scheduler_id = None
         allowed = True
-        existing_scheduler_id = self._redis.get(scheduler_key)
+        existing_scheduler_id = self._redis.get(self.scheduler_key)
         if scheduler_id and existing_scheduler_id == scheduler_id:
             logger.debug("[%s] can reschedule: matching id", self.queue_name)
         elif existing_scheduler_id is None:
             logger.debug(
                 "[%s] can reschedule: no registered scheduler",
                 self.queue_name,
             )
@@ -139,14 +148,15 @@
                 "force": force,
             }
             signals.task.send(current_task, status=State.STARTING, **sigload)
             if not self.can_reschedule(force):
                 status = State.SKIPPED
                 signals.task.send(current_task, status=status, **sigload)
                 return status
+            self._redis.delete(self.scheduler_key)
 
             # Push all other stuff in queue
             params_list = list(self.reschedule_params())
             task_count = len(params_list)
             delay_between_task = 0.0
             if self.shall_loop_in and params_list:
                 delay_between_task = self.shall_loop_in / task_count
```

### Comparing `rrtask-0.0.8/PKG-INFO` & `rrtask-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrtask
-Version: 0.0.8
+Version: 0.0.9
 Summary: Round Robin Task
 License: MIT
 Author: François Schmidts
 Author-email: francois@schmidts.fr
 Requires-Python: ==3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

