# Comparing `tmp/pyhasura-1.0.5.tar.gz` & `tmp/pyhasura-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhasura-1.0.5.tar", last modified: Thu Apr 25 20:17:42 2024, max compression
+gzip compressed data, was "pyhasura-1.0.6.tar", last modified: Thu Apr 25 20:32:55 2024, max compression
```

## Comparing `pyhasura-1.0.5.tar` & `pyhasura-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:17:42.612037 pyhasura-1.0.5/
--rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.5/LICENSE
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 20:17:42.611825 pyhasura-1.0.5/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.5/README.md
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:17:42.610924 pyhasura-1.0.5/pyhasura/
--rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.5/pyhasura/__init__.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.5/pyhasura/flatten_dict.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.5/pyhasura/gql_client.py
--rw-r--r--   0 kennethstott   (501) staff       (20)    13573 2024-04-25 20:17:13.000000 pyhasura-1.0.5/pyhasura/hasura_client.py
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:17:42.611551 pyhasura-1.0.5/pyhasura.egg-info/
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 20:17:42.000000 pyhasura-1.0.5/pyhasura.egg-info/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-25 20:17:42.000000 pyhasura-1.0.5/pyhasura.egg-info/SOURCES.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-25 20:17:42.000000 pyhasura-1.0.5/pyhasura.egg-info/dependency_links.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-25 20:17:42.000000 pyhasura-1.0.5/pyhasura.egg-info/requires.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-25 20:17:42.000000 pyhasura-1.0.5/pyhasura.egg-info/top_level.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.5/pyproject.toml
--rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-25 20:17:42.612081 pyhasura-1.0.5/setup.cfg
--rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.5/setup.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:32:55.414354 pyhasura-1.0.6/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.6/LICENSE
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 20:32:55.414148 pyhasura-1.0.6/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.6/README.md
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:32:55.413232 pyhasura-1.0.6/pyhasura/
+-rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.6/pyhasura/__init__.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.6/pyhasura/flatten_dict.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.6/pyhasura/gql_client.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)    13578 2024-04-25 20:32:42.000000 pyhasura-1.0.6/pyhasura/hasura_client.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:32:55.413908 pyhasura-1.0.6/pyhasura.egg-info/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 20:32:55.000000 pyhasura-1.0.6/pyhasura.egg-info/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-25 20:32:55.000000 pyhasura-1.0.6/pyhasura.egg-info/SOURCES.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-25 20:32:55.000000 pyhasura-1.0.6/pyhasura.egg-info/dependency_links.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-25 20:32:55.000000 pyhasura-1.0.6/pyhasura.egg-info/requires.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-25 20:32:55.000000 pyhasura-1.0.6/pyhasura.egg-info/top_level.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.6/pyproject.toml
+-rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-25 20:32:55.414395 pyhasura-1.0.6/setup.cfg
+-rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.6/setup.py
```

### Comparing `pyhasura-1.0.5/LICENSE` & `pyhasura-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.5/PKG-INFO` & `pyhasura-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.5/README.md` & `pyhasura-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.5/pyhasura/flatten_dict.py` & `pyhasura-1.0.6/pyhasura/flatten_dict.py`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.5/pyhasura/hasura_client.py` & `pyhasura-1.0.6/pyhasura/hasura_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     _convert_output_format(output_format: str) -> Any:
         Convert the output format of the last query result.
 
     _write_to_file(output_dir: Optional[str] = None, output_format: Optional[str] = None) -> List[str]:
         Writes the last query result data to file(s) in the specified output format and directory.
     """
 
-    def __init__(self, uri, role=None, admin_secret=None, output_dir='.', headers=None):
+    def __init__(self, uri=None, role=None, admin_secret=None, output_dir='.', headers=None):
         if headers is None:
             headers = {}
         if role is not None:
             headers['x-hasura-role'] = role
         if admin_secret is not None:
             headers['x-hasura-admin-secret'] = admin_secret
         self.uri = uri
```

### Comparing `pyhasura-1.0.5/pyhasura.egg-info/PKG-INFO` & `pyhasura-1.0.6/pyhasura.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.5/pyproject.toml` & `pyhasura-1.0.6/pyproject.toml`

 * *Files identical despite different names*

