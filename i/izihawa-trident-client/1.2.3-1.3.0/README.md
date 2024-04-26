# Comparing `tmp/izihawa_trident_client-1.2.3.tar.gz` & `tmp/izihawa_trident_client-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_trident_client-1.2.3.tar", max compression
+gzip compressed data, was "izihawa_trident_client-1.3.0.tar", max compression
```

## Comparing `izihawa_trident_client-1.2.3.tar` & `izihawa_trident_client-1.3.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.2.3/README.md
--rw-r--r--   0        0        0      348 2024-04-16 09:59:21.752554 izihawa_trident_client-1.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-19 06:00:51.101322 izihawa_trident_client-1.2.3/trident/__init__.py
--rw-r--r--   0        0        0     4980 2024-04-16 09:59:16.347631 izihawa_trident_client-1.2.3/trident/client.py
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 izihawa_trident_client-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.0/README.md
+-rw-r--r--   0        0        0      422 2024-04-26 19:42:19.359022 izihawa_trident_client-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-19 06:00:51.101322 izihawa_trident_client-1.3.0/trident/__init__.py
+-rw-r--r--   0        0        0      721 2024-04-26 19:24:10.303987 izihawa_trident_client-1.3.0/trident/cli.py
+-rw-r--r--   0        0        0     6196 2024-04-26 19:42:15.280047 izihawa_trident_client-1.3.0/trident/client.py
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.0/PKG-INFO
```

### Comparing `izihawa_trident_client-1.2.3/PKG-INFO` & `izihawa_trident_client-1.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: izihawa-trident-client
-Version: 1.2.3
+Version: 1.3.0
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiobaseclient (>=0.4.10,<0.5.0)
+Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Description-Content-Type: text/markdown
 
 # Trident
 
 ## Development
 
 ```bash
```

