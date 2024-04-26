# Comparing `tmp/spark-metabase-api-0.1.8.tar.gz` & `tmp/spark_metabase_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark-metabase-api-0.1.8.tar", last modified: Thu Mar  7 10:58:14 2024, max compression
+gzip compressed data, was "spark_metabase_api-0.1.9.tar", last modified: Fri Apr 26 14:46:44 2024, max compression
```

## Comparing `spark-metabase-api-0.1.8.tar` & `spark_metabase_api-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 louisspark   (501) staff       (20)        0 2024-03-07 10:58:14.276891 spark-metabase-api-0.1.8/
--rw-r--r--   0 louisspark   (501) staff       (20)     1236 2024-03-07 10:58:14.276638 spark-metabase-api-0.1.8/PKG-INFO
--rw-r--r--   0 louisspark   (501) staff       (20)      764 2024-01-23 16:28:04.000000 spark-metabase-api-0.1.8/README.md
--rw-r--r--   0 louisspark   (501) staff       (20)       38 2024-03-07 10:58:14.276964 spark-metabase-api-0.1.8/setup.cfg
--rw-r--r--   0 louisspark   (501) staff       (20)      730 2024-03-07 10:57:44.000000 spark-metabase-api-0.1.8/setup.py
-drwxr-xr-x   0 louisspark   (501) staff       (20)        0 2024-03-07 10:58:14.275371 spark-metabase-api-0.1.8/spark_metabase_api/
--rw-r--r--   0 louisspark   (501) staff       (20)       39 2023-12-18 11:41:05.000000 spark-metabase-api-0.1.8/spark_metabase_api/__init__.py
--rw-r--r--   0 louisspark   (501) staff       (20)    17351 2024-03-07 10:38:43.000000 spark-metabase-api-0.1.8/spark_metabase_api/_helper_methods.py
--rw-r--r--   0 louisspark   (501) staff       (20)     1165 2023-12-15 13:14:41.000000 spark-metabase-api-0.1.8/spark_metabase_api/_rest_methods.py
--rw-r--r--   0 louisspark   (501) staff       (20)    14405 2024-01-23 16:28:04.000000 spark-metabase-api-0.1.8/spark_metabase_api/copy_methods.py
--rw-r--r--   0 louisspark   (501) staff       (20)    12248 2024-03-07 10:42:39.000000 spark-metabase-api-0.1.8/spark_metabase_api/create_methods.py
--rw-r--r--   0 louisspark   (501) staff       (20)    16262 2024-02-02 15:01:34.000000 spark-metabase-api-0.1.8/spark_metabase_api/main_methods.py
--rw-r--r--   0 louisspark   (501) staff       (20)     3800 2024-02-02 14:37:42.000000 spark-metabase-api-0.1.8/spark_metabase_api/modify_methods.py
-drwxr-xr-x   0 louisspark   (501) staff       (20)        0 2024-03-07 10:58:14.276233 spark-metabase-api-0.1.8/spark_metabase_api.egg-info/
--rw-r--r--   0 louisspark   (501) staff       (20)     1236 2024-03-07 10:58:14.000000 spark-metabase-api-0.1.8/spark_metabase_api.egg-info/PKG-INFO
--rw-r--r--   0 louisspark   (501) staff       (20)      476 2024-03-07 10:58:14.000000 spark-metabase-api-0.1.8/spark_metabase_api.egg-info/SOURCES.txt
--rw-r--r--   0 louisspark   (501) staff       (20)        1 2024-03-07 10:58:14.000000 spark-metabase-api-0.1.8/spark_metabase_api.egg-info/dependency_links.txt
--rw-r--r--   0 louisspark   (501) staff       (20)        9 2024-03-07 10:58:14.000000 spark-metabase-api-0.1.8/spark_metabase_api.egg-info/requires.txt
--rw-r--r--   0 louisspark   (501) staff       (20)       19 2024-03-07 10:58:14.000000 spark-metabase-api-0.1.8/spark_metabase_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:46:44.797189 spark_metabase_api-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-26 14:46:44.797189 spark_metabase_api-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-26 14:46:34.000000 spark_metabase_api-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:46:44.797189 spark_metabase_api-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 14:46:34.000000 spark_metabase_api-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:46:44.797189 spark_metabase_api-0.1.9/spark_metabase_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 14:46:34.000000 spark_metabase_api-0.1.9/spark_metabase_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17718 2024-04-26 14:46:34.000000 spark_metabase_api-0.1.9/spark_metabase_api/_helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-26 14:46:34.000000 spark_metabase_api-0.1.9/spark_metabase_api/_rest_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-04-26 14:46:34.000000 spark_metabase_api-0.1.9/spark_metabase_api/copy_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-26 14:46:34.000000 spark_metabase_api-0.1.9/spark_metabase_api/create_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-26 14:46:34.000000 spark_metabase_api-0.1.9/spark_metabase_api/main_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-26 14:46:34.000000 spark_metabase_api-0.1.9/spark_metabase_api/modify_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:46:44.797189 spark_metabase_api-0.1.9/spark_metabase_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-26 14:46:44.000000 spark_metabase_api-0.1.9/spark_metabase_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-26 14:46:44.000000 spark_metabase_api-0.1.9/spark_metabase_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:46:44.000000 spark_metabase_api-0.1.9/spark_metabase_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 14:46:44.000000 spark_metabase_api-0.1.9/spark_metabase_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 14:46:44.000000 spark_metabase_api-0.1.9/spark_metabase_api.egg-info/top_level.txt
```

### Comparing `spark-metabase-api-0.1.8/PKG-INFO` & `spark_metabase_api-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-metabase-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python wrapper for the Metabase API developed by the ⭐️ Spark Tech team
 Home-page: https://github.com/Spark-Data-Team/spark_metabase_api
 Author: Larry Page
 Author-email: tech@spark.do
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spark-metabase-api-0.1.8/README.md` & `spark_metabase_api-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `spark-metabase-api-0.1.8/setup.py` & `spark_metabase_api-0.1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spark-metabase-api",
-    version="0.1.8",
+    version="0.1.9",
     author="Larry Page",
     author_email="tech@spark.do",
     description="A Python wrapper for the Metabase API developed by the ⭐️ Spark Tech team",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Spark-Data-Team/spark_metabase_api",
     packages=setuptools.find_packages(),
```

### Comparing `spark-metabase-api-0.1.8/spark_metabase_api/_helper_methods.py` & `spark_metabase_api-0.1.9/spark_metabase_api/_helper_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,14 +362,28 @@
         raise ValueError(
             'There is no DB containing the table with the ID "{}"'.format(table_id)
         )
 
     return tables[0]
 
 
+def get_user_coll_id(self, user_id):
+    """
+    Return user's personnal collection.
+    """
+    collections = [user["personal_collection_id"] for user in self.get("/api/user/") if user["id"] == user_id]
+
+    if len(collections) == 0:
+        raise ValueError(
+            'There is no active user with ID "{}"'.format(user_id)
+        )
+
+    return collections[0]
+
+
 def get_db_info(self, db_name=None, db_id=None, params=None):
     """
     Return Database info. Use 'params' for providing arguments.
     For example to include tables in the result, use: params={'include':'tables'}
     """
     import warnings
```

### Comparing `spark-metabase-api-0.1.8/spark_metabase_api/_rest_methods.py` & `spark_metabase_api-0.1.9/spark_metabase_api/_rest_methods.py`

 * *Files identical despite different names*

### Comparing `spark-metabase-api-0.1.8/spark_metabase_api/copy_methods.py` & `spark_metabase_api-0.1.9/spark_metabase_api/copy_methods.py`

 * *Files identical despite different names*

### Comparing `spark-metabase-api-0.1.8/spark_metabase_api/create_methods.py` & `spark_metabase_api-0.1.9/spark_metabase_api/create_methods.py`

 * *Files identical despite different names*

### Comparing `spark-metabase-api-0.1.8/spark_metabase_api/main_methods.py` & `spark_metabase_api-0.1.9/spark_metabase_api/main_methods.py`

 * *Files identical despite different names*

### Comparing `spark-metabase-api-0.1.8/spark_metabase_api/modify_methods.py` & `spark_metabase_api-0.1.9/spark_metabase_api/modify_methods.py`

 * *Files identical despite different names*

### Comparing `spark-metabase-api-0.1.8/spark_metabase_api.egg-info/PKG-INFO` & `spark_metabase_api-0.1.9/spark_metabase_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-metabase-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python wrapper for the Metabase API developed by the ⭐️ Spark Tech team
 Home-page: https://github.com/Spark-Data-Team/spark_metabase_api
 Author: Larry Page
 Author-email: tech@spark.do
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

