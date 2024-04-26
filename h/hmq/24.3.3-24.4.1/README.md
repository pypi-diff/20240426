# Comparing `tmp/hmq-24.3.3.tar.gz` & `tmp/hmq-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmq-24.3.3.tar", last modified: Sun Mar 17 15:58:51 2024, max compression
+gzip compressed data, was "hmq-24.4.1.tar", last modified: Fri Apr 26 13:17:56 2024, max compression
```

## Comparing `hmq-24.3.3.tar` & `hmq-24.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ferchault  (1000) ferchault  (1000)        0 2024-03-17 15:58:51.650612 hmq-24.3.3/
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)      415 2024-03-17 15:58:51.650612 hmq-24.3.3/PKG-INFO
-drwxr-xr-x   0 ferchault  (1000) ferchault  (1000)        0 2024-03-17 15:58:51.650612 hmq-24.3.3/hmq/
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)       19 2023-06-29 17:44:11.000000 hmq-24.3.3/hmq/__init__.py
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)    27340 2024-03-17 15:54:00.000000 hmq-24.3.3/hmq/hmq.py
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)    22471 2023-11-14 12:41:24.000000 hmq-24.3.3/hmq/mod.py
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)     1622 2023-11-14 15:26:17.000000 hmq-24.3.3/hmq/tmptest.py
-drwxr-xr-x   0 ferchault  (1000) ferchault  (1000)        0 2024-03-17 15:58:51.650612 hmq-24.3.3/hmq.egg-info/
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)      415 2024-03-17 15:58:51.000000 hmq-24.3.3/hmq.egg-info/PKG-INFO
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)      251 2024-03-17 15:58:51.000000 hmq-24.3.3/hmq.egg-info/SOURCES.txt
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)        1 2024-03-17 15:58:51.000000 hmq-24.3.3/hmq.egg-info/dependency_links.txt
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)       32 2024-03-17 15:58:51.000000 hmq-24.3.3/hmq.egg-info/entry_points.txt
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)        1 2024-02-22 10:51:27.000000 hmq-24.3.3/hmq.egg-info/not-zip-safe
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)       64 2024-03-17 15:58:51.000000 hmq-24.3.3/hmq.egg-info/requires.txt
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)        4 2024-03-17 15:58:51.000000 hmq-24.3.3/hmq.egg-info/top_level.txt
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)       38 2024-03-17 15:58:51.650612 hmq-24.3.3/setup.cfg
--rw-r--r--   0 ferchault  (1000) ferchault  (1000)      579 2024-03-17 15:58:51.000000 hmq-24.3.3/setup.py
+drwxr-xr-x   0 ferchault  (1000) ferchault  (1000)        0 2024-04-26 13:17:55.988521 hmq-24.4.1/
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)      415 2024-04-26 13:17:55.988521 hmq-24.4.1/PKG-INFO
+drwxr-xr-x   0 ferchault  (1000) ferchault  (1000)        0 2024-04-26 13:17:55.988521 hmq-24.4.1/hmq/
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)       19 2023-06-29 17:44:11.000000 hmq-24.4.1/hmq/__init__.py
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)    28446 2024-04-26 13:16:37.000000 hmq-24.4.1/hmq/hmq.py
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)    22471 2023-11-14 12:41:24.000000 hmq-24.4.1/hmq/mod.py
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)     1622 2023-11-14 15:26:17.000000 hmq-24.4.1/hmq/tmptest.py
+drwxr-xr-x   0 ferchault  (1000) ferchault  (1000)        0 2024-04-26 13:17:55.988521 hmq-24.4.1/hmq.egg-info/
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)      415 2024-04-26 13:17:55.000000 hmq-24.4.1/hmq.egg-info/PKG-INFO
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)      251 2024-04-26 13:17:55.000000 hmq-24.4.1/hmq.egg-info/SOURCES.txt
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)        1 2024-04-26 13:17:55.000000 hmq-24.4.1/hmq.egg-info/dependency_links.txt
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)       32 2024-04-26 13:17:55.000000 hmq-24.4.1/hmq.egg-info/entry_points.txt
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)        1 2024-02-22 10:51:27.000000 hmq-24.4.1/hmq.egg-info/not-zip-safe
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)       64 2024-04-26 13:17:55.000000 hmq-24.4.1/hmq.egg-info/requires.txt
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)        4 2024-04-26 13:17:55.000000 hmq-24.4.1/hmq.egg-info/top_level.txt
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)       38 2024-04-26 13:17:55.988521 hmq-24.4.1/setup.cfg
+-rw-r--r--   0 ferchault  (1000) ferchault  (1000)      579 2024-04-26 13:17:55.000000 hmq-24.4.1/setup.py
```

### Comparing `hmq-24.3.3/hmq/hmq.py` & `hmq-24.4.1/hmq/hmq.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import json
 import hashlib
 import configparser
 import warnings
 import functools
 import numpy as np
 import pandas as pd
+import secrets
 from pathlib import Path
 import nacl
 from nacl.secret import SecretBox
 from nacl.public import PrivateKey, SealedBox, PublicKey
 from nacl.signing import SigningKey, VerifyKey
 import tqdm
 from rq import Worker
@@ -226,15 +227,15 @@
                 self._computesecret = base64.b64decode(config["server"]["compute"])
             try:
                 self._adminkey = base64.b64decode(config["server"]["admin"])
             except:
                 pass
             self._box = SecretBox(self._computesecret)
 
-    def _encrypt(self, obj, raw=False):
+    def _encrypt(self, obj, raw=False) -> str:
         self._build_box()
 
         if raw:
             message = obj.encode("utf8")
         else:
             message = json.dumps(obj, cls=AutomaticEncoder).encode("utf8")
         message = base64.b64encode(self._box.encrypt(message)).decode("ascii")
@@ -371,33 +372,62 @@
         tag: str,
         digest: str,
         calls: list,
         ncores: int = 1,
         datacenters: list = None,
     ):
         calls = [self._encrypt(call) for call in calls]
-        callstr = json.dumps(calls)
-        calldigest = hashlib.sha256(callstr.encode("utf8")).hexdigest()
-        payload = {
-            "tag": tag,
-            "function": digest,
-            "calls": callstr,
-            "digest": calldigest,
-            "ncores": ncores,
-            "datacenters": datacenters,
-            "challenge": self._get_challenge(),
-        }
-        uuids = self._post("/tasks/submit", payload)
+
+        uuids = []
+        limit_mb = 14
+        limit = limit_mb * 1024 * 1024
+        while len(calls) > 0:
+            chunk = [calls.pop(0)]
+            chunk_length = len(chunk[0])
+            while chunk_length < limit and len(calls) > 0:
+                next_length = len(calls[0])
+                if chunk_length + next_length > limit:
+                    break
+                chunk.append(calls.pop(0))
+                chunk_length += len(chunk[-1])
+
+            if chunk_length > limit:
+                raise ValueError(
+                    f"Chunk size exceeded {limit_mb} MB limit: cannot submit task."
+                )
+
+            chunkstr = json.dumps(chunk)
+            chunk_digest = hashlib.sha256(chunkstr.encode("utf8")).hexdigest()
+            payload = {
+                "tag": tag,
+                "function": digest,
+                "calls": chunkstr,
+                "digest": chunk_digest,
+                "ncores": ncores,
+                "datacenters": datacenters,
+                "challenge": self._get_challenge(),
+            }
+            uuids += self._post("/tasks/submit", payload)
+
         return uuids
 
     def find_tasks(self, tag: str):
         payload = {"tag": tag, "challenge": self._get_challenge()}
         tasks = self._post("/tasks/find", payload)
         return tasks
 
+    def sync_tasks(self, datacenter: str, known: list[str]) -> list[str]:
+        payload = {
+            "datacenter": datacenter,
+            "known": known,
+            "challenge": self._get_challenge(),
+        }
+        stale = self._post("/tasks/sync", payload)
+        return stale
+
     def get_tasks_status(self, tasks: list[str]):
         payload = {
             "tasks": tasks,
             "challenge": self._get_challenge(),
         }
         return self._post("/tasks/inspect", payload)
 
@@ -792,14 +822,16 @@
     return api._worker(hmqid, call, function, api._box._key)
 
 
 class CachedWorker(Worker):
     def execute_job(self, job, queue):
         payload = self.connection.hget("hmq:functions", job.kwargs["function"])
         api.warm_cache(job.kwargs["function"], json.loads(payload.decode("ascii")))
+        # re-seed numpy random state
+        np.random.seed(int.from_bytes(secrets.token_bytes(4)))
         return super().execute_job(job, queue)
 
 
 def cli():
     if len(sys.argv) == 1:
         print(
             """Usage: hmq COMMAND [ARGS]
```

### Comparing `hmq-24.3.3/hmq/mod.py` & `hmq-24.4.1/hmq/mod.py`

 * *Files identical despite different names*

### Comparing `hmq-24.3.3/hmq/tmptest.py` & `hmq-24.4.1/hmq/tmptest.py`

 * *Files identical despite different names*

### Comparing `hmq-24.3.3/setup.py` & `hmq-24.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="hmq",
-    version="24.03.3",
+    version="24.04.1",
     description="Distributed computing.",
     url="https://github.com/NablaChem/hummingqueue",
     author="Guido Falk von Rudorff",
     author_email="guido@vonrudorff.de",
     license="AGPL-3.0",
     packages=["hmq"],
     zip_safe=False,
```

