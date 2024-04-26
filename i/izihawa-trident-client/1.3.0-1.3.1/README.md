# Comparing `tmp/izihawa_trident_client-1.3.0.tar.gz` & `tmp/izihawa_trident_client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_trident_client-1.3.0.tar", max compression
+gzip compressed data, was "izihawa_trident_client-1.3.1.tar", max compression
```

## Comparing `izihawa_trident_client-1.3.0.tar` & `izihawa_trident_client-1.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.0/README.md
--rw-r--r--   0        0        0      422 2024-04-26 19:42:19.359022 izihawa_trident_client-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-19 06:00:51.101322 izihawa_trident_client-1.3.0/trident/__init__.py
--rw-r--r--   0        0        0      721 2024-04-26 19:24:10.303987 izihawa_trident_client-1.3.0/trident/cli.py
--rw-r--r--   0        0        0     6196 2024-04-26 19:42:15.280047 izihawa_trident_client-1.3.0/trident/client.py
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.1/README.md
+-rw-r--r--   0        0        0      422 2024-04-26 19:49:17.996953 izihawa_trident_client-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-19 06:00:51.101322 izihawa_trident_client-1.3.1/trident/__init__.py
+-rw-r--r--   0        0        0      721 2024-04-26 19:24:10.303987 izihawa_trident_client-1.3.1/trident/cli.py
+-rw-r--r--   0        0        0     6323 2024-04-26 19:49:12.841636 izihawa_trident_client-1.3.1/trident/client.py
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.1/PKG-INFO
```

### Comparing `izihawa_trident_client-1.3.0/trident/cli.py` & `izihawa_trident_client-1.3.1/trident/cli.py`

 * *Files identical despite different names*

### Comparing `izihawa_trident_client-1.3.0/trident/client.py` & `izihawa_trident_client-1.3.1/trident/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,9 +166,13 @@
     def get_interface(self):
         return {
             'table': {
                 'copy-files': self.table_copy_files,
                 'get': self.table_get,
                 'ls': self.table_ls,
                 'upload': self.table_upload,
+            },
+            'tables': {
+                'create': self.tables_create,
+                'drop': self.tables_drop,
             }
         }
```

### Comparing `izihawa_trident_client-1.3.0/PKG-INFO` & `izihawa_trident_client-1.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izihawa-trident-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

