# Comparing `tmp/api-nichotined-0.1.1.tar.gz` & `tmp/api-nichotined-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-nichotined-0.1.1.tar", last modified: Fri Apr 19 16:21:19 2024, max compression
+gzip compressed data, was "api-nichotined-0.1.2.tar", last modified: Fri Apr 26 10:37:13 2024, max compression
```

## Comparing `api-nichotined-0.1.1.tar` & `api-nichotined-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 16:21:19.263412 api-nichotined-0.1.1/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1112 2024-04-19 16:21:19.263195 api-nichotined-0.1.1/PKG-INFO
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      648 2024-04-19 16:19:11.000000 api-nichotined-0.1.1/README.md
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 16:21:19.261207 api-nichotined-0.1.1/api_nichotined/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       73 2024-04-19 16:18:53.000000 api-nichotined-0.1.1/api_nichotined/__init__.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 16:21:19.262300 api-nichotined-0.1.1/api_nichotined/core/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 04:53:46.000000 api-nichotined-0.1.1/api_nichotined/core/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1973 2024-04-19 14:43:50.000000 api-nichotined-0.1.1/api_nichotined/core/core.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 16:21:19.262977 api-nichotined-0.1.1/api_nichotined.egg-info/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1112 2024-04-19 16:21:19.000000 api-nichotined-0.1.1/api_nichotined.egg-info/PKG-INFO
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      324 2024-04-19 16:21:19.000000 api-nichotined-0.1.1/api_nichotined.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        1 2024-04-19 16:21:19.000000 api-nichotined-0.1.1/api_nichotined.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       17 2024-04-19 16:21:19.000000 api-nichotined-0.1.1/api_nichotined.egg-info/requires.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       20 2024-04-19 16:21:19.000000 api-nichotined-0.1.1/api_nichotined.egg-info/top_level.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       38 2024-04-19 16:21:19.263450 api-nichotined-0.1.1/setup.cfg
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      718 2024-04-19 16:18:53.000000 api-nichotined-0.1.1/setup.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 16:21:19.262712 api-nichotined-0.1.1/test/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 05:21:55.000000 api-nichotined-0.1.1/test/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      458 2024-04-19 16:18:53.000000 api-nichotined-0.1.1/test/main.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 10:37:13.150215 api-nichotined-0.1.2/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1112 2024-04-26 10:37:13.149887 api-nichotined-0.1.2/PKG-INFO
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      648 2024-04-19 16:19:11.000000 api-nichotined-0.1.2/README.md
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 10:37:13.148062 api-nichotined-0.1.2/api_nichotined/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       65 2024-04-26 10:16:58.000000 api-nichotined-0.1.2/api_nichotined/__init__.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 10:37:13.149122 api-nichotined-0.1.2/api_nichotined/core/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 04:53:46.000000 api-nichotined-0.1.2/api_nichotined/core/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1749 2024-04-26 10:30:30.000000 api-nichotined-0.1.2/api_nichotined/core/core.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 10:37:13.149622 api-nichotined-0.1.2/api_nichotined.egg-info/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1112 2024-04-26 10:37:13.000000 api-nichotined-0.1.2/api_nichotined.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      324 2024-04-26 10:37:13.000000 api-nichotined-0.1.2/api_nichotined.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        1 2024-04-26 10:37:13.000000 api-nichotined-0.1.2/api_nichotined.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       17 2024-04-26 10:37:13.000000 api-nichotined-0.1.2/api_nichotined.egg-info/requires.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       20 2024-04-26 10:37:13.000000 api-nichotined-0.1.2/api_nichotined.egg-info/top_level.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       38 2024-04-26 10:37:13.150282 api-nichotined-0.1.2/setup.cfg
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      718 2024-04-26 10:36:44.000000 api-nichotined-0.1.2/setup.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 10:37:13.149399 api-nichotined-0.1.2/test/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 05:21:55.000000 api-nichotined-0.1.2/test/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      451 2024-04-26 10:35:06.000000 api-nichotined-0.1.2/test/main.py
```

### Comparing `api-nichotined-0.1.1/PKG-INFO` & `api-nichotined-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-nichotined
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple lib for testing rest API
 Home-page: https://github.com/nichotined/simple-api
 Author: Nicholas Frederich
 Author-email: nicholas.frederich.lagaunne@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `api-nichotined-0.1.1/README.md` & `api-nichotined-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `api-nichotined-0.1.1/api_nichotined.egg-info/PKG-INFO` & `api-nichotined-0.1.2/api_nichotined.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-nichotined
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple lib for testing rest API
 Home-page: https://github.com/nichotined/simple-api
 Author: Nicholas Frederich
 Author-email: nicholas.frederich.lagaunne@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `api-nichotined-0.1.1/setup.py` & `api-nichotined-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="api-nichotined",
-    version="0.1.1",
+    version="0.1.2",
     author="Nicholas Frederich",
     author_email="nicholas.frederich.lagaunne@gmail.com",
     description="Simple lib for testing rest API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nichotined/simple-api",
     packages=setuptools.find_packages(),
```

