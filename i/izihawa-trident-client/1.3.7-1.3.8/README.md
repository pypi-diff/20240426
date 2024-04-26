# Comparing `tmp/izihawa_trident_client-1.3.7.tar.gz` & `tmp/izihawa_trident_client-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_trident_client-1.3.7.tar", max compression
+gzip compressed data, was "izihawa_trident_client-1.3.8.tar", max compression
```

## Comparing `izihawa_trident_client-1.3.7.tar` & `izihawa_trident_client-1.3.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.7/README.md
--rw-r--r--   0        0        0      423 2024-04-26 20:01:59.450012 izihawa_trident_client-1.3.7/pyproject.toml
--rw-r--r--   0        0        0       40 2024-04-26 19:52:25.445233 izihawa_trident_client-1.3.7/trident/__init__.py
--rw-r--r--   0        0        0      738 2024-04-26 19:54:39.941952 izihawa_trident_client-1.3.7/trident/cli.py
--rw-r--r--   0        0        0     6339 2024-04-26 20:01:48.911890 izihawa_trident_client-1.3.7/trident/client.py
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.8/README.md
+-rw-r--r--   0        0        0      423 2024-04-26 20:04:21.828569 izihawa_trident_client-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-04-26 19:52:25.445233 izihawa_trident_client-1.3.8/trident/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-26 19:54:39.941952 izihawa_trident_client-1.3.8/trident/cli.py
+-rw-r--r--   0        0        0     6490 2024-04-26 20:04:18.332037 izihawa_trident_client-1.3.8/trident/client.py
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.8/PKG-INFO
```

### Comparing `izihawa_trident_client-1.3.7/trident/cli.py` & `izihawa_trident_client-1.3.8/trident/cli.py`

 * *Files identical despite different names*

### Comparing `izihawa_trident_client-1.3.7/trident/client.py` & `izihawa_trident_client-1.3.8/trident/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import typing
 from typing import AsyncGenerator
 
 import aiofiles
 from aiobaseclient import BaseClient
 from aiobaseclient.exceptions import ExternalServiceError
+from izihawa_utils.common import filter_none
 
 
 class TridentClient(BaseClient):
     async def response_processor(self, response):
         if response.status == 404:
             return None
         elif response.status != 200:
@@ -39,15 +40,19 @@
         return await response.json()
 
     async def tables_create(self, table: str, storage: str | None = None) -> bytes:
         url = f"/tables/{table}/"
         params = {}
         if storage:
             params['storage'] = storage
-        response = await self.post(url, json=params)
+        response = await self.post(
+            url,
+            headers={'Content-Type': 'application/json'},
+            json=filter_none(params),
+        )
         return await response.read()
 
     async def tables_exists(self, table: str) -> bool:
         url = f"/tables/{table}/exists/"
         response = await self.get(url)
         if response is None:
             return False
```

### Comparing `izihawa_trident_client-1.3.7/PKG-INFO` & `izihawa_trident_client-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izihawa-trident-client
-Version: 1.3.7
+Version: 1.3.8
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

