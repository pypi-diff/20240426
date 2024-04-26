# Comparing `tmp/izihawa_trident_client-1.3.8.tar.gz` & `tmp/izihawa_trident_client-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_trident_client-1.3.8.tar", max compression
+gzip compressed data, was "izihawa_trident_client-1.3.9.tar", max compression
```

## Comparing `izihawa_trident_client-1.3.8.tar` & `izihawa_trident_client-1.3.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.8/README.md
--rw-r--r--   0        0        0      423 2024-04-26 20:04:21.828569 izihawa_trident_client-1.3.8/pyproject.toml
--rw-r--r--   0        0        0       40 2024-04-26 19:52:25.445233 izihawa_trident_client-1.3.8/trident/__init__.py
--rw-r--r--   0        0        0      738 2024-04-26 19:54:39.941952 izihawa_trident_client-1.3.8/trident/cli.py
--rw-r--r--   0        0        0     6490 2024-04-26 20:04:18.332037 izihawa_trident_client-1.3.8/trident/client.py
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.9/README.md
+-rw-r--r--   0        0        0      423 2024-04-26 20:08:59.693239 izihawa_trident_client-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-04-26 19:52:25.445233 izihawa_trident_client-1.3.9/trident/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-26 20:08:12.317855 izihawa_trident_client-1.3.9/trident/cli.py
+-rw-r--r--   0        0        0     6514 2024-04-26 20:07:18.615566 izihawa_trident_client-1.3.9/trident/client.py
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.9/PKG-INFO
```

### Comparing `izihawa_trident_client-1.3.8/trident/cli.py` & `izihawa_trident_client-1.3.9/trident/cli.py`

 * *Files identical despite different names*

### Comparing `izihawa_trident_client-1.3.8/trident/client.py` & `izihawa_trident_client-1.3.9/trident/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 import typing
 from typing import AsyncGenerator
 
 import aiofiles
 from aiobaseclient import BaseClient
 from aiobaseclient.exceptions import ExternalServiceError
@@ -43,15 +44,15 @@
         url = f"/tables/{table}/"
         params = {}
         if storage:
             params['storage'] = storage
         response = await self.post(
             url,
             headers={'Content-Type': 'application/json'},
-            json=filter_none(params),
+            data=json.dumps(filter_none(params)),
         )
         return await response.read()
 
     async def tables_exists(self, table: str) -> bool:
         url = f"/tables/{table}/exists/"
         response = await self.get(url)
         if response is None:
```

### Comparing `izihawa_trident_client-1.3.8/PKG-INFO` & `izihawa_trident_client-1.3.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izihawa-trident-client
-Version: 1.3.8
+Version: 1.3.9
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

