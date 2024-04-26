# Comparing `tmp/llm_monitoring_sascha-0.0.5.tar.gz` & `tmp/llm_monitoring_sascha-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_monitoring_sascha-0.0.5.tar", last modified: Fri Apr 26 08:42:34 2024, max compression
+gzip compressed data, was "llm_monitoring_sascha-0.0.6.tar", last modified: Fri Apr 26 08:46:53 2024, max compression
```

## Comparing `llm_monitoring_sascha-0.0.5.tar` & `llm_monitoring_sascha-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:42:34.828408 llm_monitoring_sascha-0.0.5/
--rw-r--r--   0 sascha     (501) staff       (20)        8 2024-04-26 07:51:08.000000 llm_monitoring_sascha-0.0.5/LICENSE
--rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:42:34.828160 llm_monitoring_sascha-0.0.5/PKG-INFO
--rw-r--r--   0 sascha     (501) staff       (20)       10 2023-12-21 09:09:33.000000 llm_monitoring_sascha-0.0.5/README.md
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:42:34.827872 llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/
--rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:42:34.000000 llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/PKG-INFO
--rw-r--r--   0 sascha     (501) staff       (20)      256 2024-04-26 08:42:34.000000 llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/SOURCES.txt
--rw-r--r--   0 sascha     (501) staff       (20)        1 2024-04-26 08:42:34.000000 llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/dependency_links.txt
--rw-r--r--   0 sascha     (501) staff       (20)       11 2024-04-26 08:42:34.000000 llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/top_level.txt
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:42:34.827286 llm_monitoring_sascha-0.0.5/monitoring/
--rw-r--r--   0 sascha     (501) staff       (20)     2113 2024-04-25 14:07:28.000000 llm_monitoring_sascha-0.0.5/monitoring/__init__.py
--rw-r--r--   0 sascha     (501) staff       (20)     4629 2024-04-26 07:28:16.000000 llm_monitoring_sascha-0.0.5/monitoring/client.py
--rw-r--r--   0 sascha     (501) staff       (20)      601 2024-04-26 08:42:31.000000 llm_monitoring_sascha-0.0.5/pyproject.toml
--rw-r--r--   0 sascha     (501) staff       (20)       38 2024-04-26 08:42:34.828477 llm_monitoring_sascha-0.0.5/setup.cfg
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:46:53.199233 llm_monitoring_sascha-0.0.6/
+-rw-r--r--   0 sascha     (501) staff       (20)        8 2024-04-26 07:51:08.000000 llm_monitoring_sascha-0.0.6/LICENSE
+-rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:46:53.198881 llm_monitoring_sascha-0.0.6/PKG-INFO
+-rw-r--r--   0 sascha     (501) staff       (20)       10 2023-12-21 09:09:33.000000 llm_monitoring_sascha-0.0.6/README.md
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:46:53.198356 llm_monitoring_sascha-0.0.6/llm_monitoring_sascha.egg-info/
+-rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:46:53.000000 llm_monitoring_sascha-0.0.6/llm_monitoring_sascha.egg-info/PKG-INFO
+-rw-r--r--   0 sascha     (501) staff       (20)      276 2024-04-26 08:46:53.000000 llm_monitoring_sascha-0.0.6/llm_monitoring_sascha.egg-info/SOURCES.txt
+-rw-r--r--   0 sascha     (501) staff       (20)        1 2024-04-26 08:46:53.000000 llm_monitoring_sascha-0.0.6/llm_monitoring_sascha.egg-info/dependency_links.txt
+-rw-r--r--   0 sascha     (501) staff       (20)       11 2024-04-26 08:46:53.000000 llm_monitoring_sascha-0.0.6/llm_monitoring_sascha.egg-info/top_level.txt
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:46:53.197929 llm_monitoring_sascha-0.0.6/monitoring/
+-rw-r--r--   0 sascha     (501) staff       (20)     2113 2024-04-25 14:07:28.000000 llm_monitoring_sascha-0.0.6/monitoring/__init__.py
+-rw-r--r--   0 sascha     (501) staff       (20)     4629 2024-04-26 07:28:16.000000 llm_monitoring_sascha-0.0.6/monitoring/client.py
+-rw-r--r--   0 sascha     (501) staff       (20)      204 2024-04-26 08:42:20.000000 llm_monitoring_sascha-0.0.6/monitoring/setup.py
+-rw-r--r--   0 sascha     (501) staff       (20)      601 2024-04-26 08:46:44.000000 llm_monitoring_sascha-0.0.6/pyproject.toml
+-rw-r--r--   0 sascha     (501) staff       (20)       38 2024-04-26 08:46:53.199319 llm_monitoring_sascha-0.0.6/setup.cfg
```

### Comparing `llm_monitoring_sascha-0.0.5/PKG-INFO` & `llm_monitoring_sascha-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_monitoring_sascha
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: Sascha Heyer <mail@saschaheyer.de>, Sascha Heyer <sascha@doit.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/PKG-INFO` & `llm_monitoring_sascha-0.0.6/llm_monitoring_sascha.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_monitoring_sascha
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: Sascha Heyer <mail@saschaheyer.de>, Sascha Heyer <sascha@doit.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm_monitoring_sascha-0.0.5/monitoring/__init__.py` & `llm_monitoring_sascha-0.0.6/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_monitoring_sascha-0.0.5/monitoring/client.py` & `llm_monitoring_sascha-0.0.6/monitoring/client.py`

 * *Files identical despite different names*

### Comparing `llm_monitoring_sascha-0.0.5/pyproject.toml` & `llm_monitoring_sascha-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm_monitoring_sascha"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Sascha Heyer", email="mail@saschaheyer.de" },
   { name="Sascha Heyer", email="sascha@doit.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 classifiers = [
```

