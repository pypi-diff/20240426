# Comparing `tmp/izihawa_trident_client-1.3.4.tar.gz` & `tmp/izihawa_trident_client-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_trident_client-1.3.4.tar", max compression
+gzip compressed data, was "izihawa_trident_client-1.3.5.tar", max compression
```

## Comparing `izihawa_trident_client-1.3.4.tar` & `izihawa_trident_client-1.3.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.4/README.md
--rw-r--r--   0        0        0      423 2024-04-26 19:54:44.950924 izihawa_trident_client-1.3.4/pyproject.toml
--rw-r--r--   0        0        0       40 2024-04-26 19:52:25.445233 izihawa_trident_client-1.3.4/trident/__init__.py
--rw-r--r--   0        0        0      738 2024-04-26 19:54:39.941952 izihawa_trident_client-1.3.4/trident/cli.py
--rw-r--r--   0        0        0     6323 2024-04-26 19:49:12.841636 izihawa_trident_client-1.3.4/trident/client.py
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.5/README.md
+-rw-r--r--   0        0        0      423 2024-04-26 19:57:40.806270 izihawa_trident_client-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-04-26 19:52:25.445233 izihawa_trident_client-1.3.5/trident/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-26 19:54:39.941952 izihawa_trident_client-1.3.5/trident/cli.py
+-rw-r--r--   0        0        0     6261 2024-04-26 19:57:30.892100 izihawa_trident_client-1.3.5/trident/client.py
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.5/PKG-INFO
```

### Comparing `izihawa_trident_client-1.3.4/trident/cli.py` & `izihawa_trident_client-1.3.5/trident/cli.py`

 * *Files identical despite different names*

### Comparing `izihawa_trident_client-1.3.4/trident/client.py` & `izihawa_trident_client-1.3.5/trident/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,18 +161,14 @@
                     element,
                     target_table,
                     remaining_path,
                 )
 
     def get_interface(self):
         return {
-            'table': {
-                'copy-files': self.table_copy_files,
-                'get': self.table_get,
-                'ls': self.table_ls,
-                'upload': self.table_upload,
-            },
-            'tables': {
-                'create': self.tables_create,
-                'drop': self.tables_drop,
-            }
+            'table-copy-files': self.table_copy_files,
+            'table-get': self.table_get,
+            'table-ls': self.table_ls,
+            'table-upload': self.table_upload,
+            'tables-create': self.tables_create,
+            'tables-drop': self.tables_drop,
         }
```

### Comparing `izihawa_trident_client-1.3.4/PKG-INFO` & `izihawa_trident_client-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izihawa-trident-client
-Version: 1.3.4
+Version: 1.3.5
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

