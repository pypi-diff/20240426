# Comparing `tmp/izihawa_trident_client-1.3.5.tar.gz` & `tmp/izihawa_trident_client-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_trident_client-1.3.5.tar", max compression
+gzip compressed data, was "izihawa_trident_client-1.3.6.tar", max compression
```

## Comparing `izihawa_trident_client-1.3.5.tar` & `izihawa_trident_client-1.3.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.5/README.md
--rw-r--r--   0        0        0      423 2024-04-26 19:57:40.806270 izihawa_trident_client-1.3.5/pyproject.toml
--rw-r--r--   0        0        0       40 2024-04-26 19:52:25.445233 izihawa_trident_client-1.3.5/trident/__init__.py
--rw-r--r--   0        0        0      738 2024-04-26 19:54:39.941952 izihawa_trident_client-1.3.5/trident/cli.py
--rw-r--r--   0        0        0     6261 2024-04-26 19:57:30.892100 izihawa_trident_client-1.3.5/trident/client.py
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.6/README.md
+-rw-r--r--   0        0        0      423 2024-04-26 20:00:37.246847 izihawa_trident_client-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-04-26 19:52:25.445233 izihawa_trident_client-1.3.6/trident/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-26 19:54:39.941952 izihawa_trident_client-1.3.6/trident/cli.py
+-rw-r--r--   0        0        0     6341 2024-04-26 20:00:25.984867 izihawa_trident_client-1.3.6/trident/client.py
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.6/PKG-INFO
```

### Comparing `izihawa_trident_client-1.3.5/trident/cli.py` & `izihawa_trident_client-1.3.6/trident/cli.py`

 * *Files identical despite different names*

### Comparing `izihawa_trident_client-1.3.5/trident/client.py` & `izihawa_trident_client-1.3.6/trident/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,20 @@
         async for data, _ in response.content.iter_chunks():
             yield data
 
     async def tables_ls(self) -> dict:
         response = await self.get(f"/tables/")
         return await response.json()
 
-    async def tables_create(self, table: str, storage: str) -> bytes:
+    async def tables_create(self, table: str, storage: str | None = None) -> bytes:
         url = f"/tables/{table}/"
-        response = await self.post(url, params={'storage': storage})
+        params = {}
+        if storage:
+            params['storage'] = storage
+        response = await self.post(url, params=params)
         return await response.read()
 
     async def tables_exists(self, table: str) -> bool:
         url = f"/tables/{table}/exists/"
         response = await self.get(url)
         if response is None:
             return False
```

### Comparing `izihawa_trident_client-1.3.5/PKG-INFO` & `izihawa_trident_client-1.3.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izihawa-trident-client
-Version: 1.3.5
+Version: 1.3.6
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

