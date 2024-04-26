# Comparing `tmp/llm_monitoring_sascha-0.0.4.tar.gz` & `tmp/llm_monitoring_sascha-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_monitoring_sascha-0.0.4.tar", last modified: Fri Apr 26 08:28:02 2024, max compression
+gzip compressed data, was "llm_monitoring_sascha-0.0.5.tar", last modified: Fri Apr 26 08:42:34 2024, max compression
```

## Comparing `llm_monitoring_sascha-0.0.4.tar` & `llm_monitoring_sascha-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:28:02.635837 llm_monitoring_sascha-0.0.4/
--rw-r--r--   0 sascha     (501) staff       (20)        8 2024-04-26 07:51:08.000000 llm_monitoring_sascha-0.0.4/LICENSE
--rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:28:02.635605 llm_monitoring_sascha-0.0.4/PKG-INFO
--rw-r--r--   0 sascha     (501) staff       (20)       10 2023-12-21 09:09:33.000000 llm_monitoring_sascha-0.0.4/README.md
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:28:02.635290 llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/
--rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:28:02.000000 llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/PKG-INFO
--rw-r--r--   0 sascha     (501) staff       (20)      256 2024-04-26 08:28:02.000000 llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/SOURCES.txt
--rw-r--r--   0 sascha     (501) staff       (20)        1 2024-04-26 08:28:02.000000 llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/dependency_links.txt
--rw-r--r--   0 sascha     (501) staff       (20)       11 2024-04-26 08:28:02.000000 llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/top_level.txt
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:28:02.634524 llm_monitoring_sascha-0.0.4/monitoring/
--rw-r--r--   0 sascha     (501) staff       (20)     2113 2024-04-25 14:07:28.000000 llm_monitoring_sascha-0.0.4/monitoring/__init__.py
--rw-r--r--   0 sascha     (501) staff       (20)     4629 2024-04-26 07:28:16.000000 llm_monitoring_sascha-0.0.4/monitoring/client.py
--rw-r--r--   0 sascha     (501) staff       (20)      601 2024-04-26 08:27:54.000000 llm_monitoring_sascha-0.0.4/pyproject.toml
--rw-r--r--   0 sascha     (501) staff       (20)       38 2024-04-26 08:28:02.635900 llm_monitoring_sascha-0.0.4/setup.cfg
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:42:34.828408 llm_monitoring_sascha-0.0.5/
+-rw-r--r--   0 sascha     (501) staff       (20)        8 2024-04-26 07:51:08.000000 llm_monitoring_sascha-0.0.5/LICENSE
+-rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:42:34.828160 llm_monitoring_sascha-0.0.5/PKG-INFO
+-rw-r--r--   0 sascha     (501) staff       (20)       10 2023-12-21 09:09:33.000000 llm_monitoring_sascha-0.0.5/README.md
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:42:34.827872 llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/
+-rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:42:34.000000 llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/PKG-INFO
+-rw-r--r--   0 sascha     (501) staff       (20)      256 2024-04-26 08:42:34.000000 llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/SOURCES.txt
+-rw-r--r--   0 sascha     (501) staff       (20)        1 2024-04-26 08:42:34.000000 llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/dependency_links.txt
+-rw-r--r--   0 sascha     (501) staff       (20)       11 2024-04-26 08:42:34.000000 llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/top_level.txt
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:42:34.827286 llm_monitoring_sascha-0.0.5/monitoring/
+-rw-r--r--   0 sascha     (501) staff       (20)     2113 2024-04-25 14:07:28.000000 llm_monitoring_sascha-0.0.5/monitoring/__init__.py
+-rw-r--r--   0 sascha     (501) staff       (20)     4629 2024-04-26 07:28:16.000000 llm_monitoring_sascha-0.0.5/monitoring/client.py
+-rw-r--r--   0 sascha     (501) staff       (20)      601 2024-04-26 08:42:31.000000 llm_monitoring_sascha-0.0.5/pyproject.toml
+-rw-r--r--   0 sascha     (501) staff       (20)       38 2024-04-26 08:42:34.828477 llm_monitoring_sascha-0.0.5/setup.cfg
```

### Comparing `llm_monitoring_sascha-0.0.4/PKG-INFO` & `llm_monitoring_sascha-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_monitoring_sascha
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Author-email: Sascha Heyer <mail@saschaheyer.de>, Sascha Heyer <sascha@doit.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/PKG-INFO` & `llm_monitoring_sascha-0.0.5/llm_monitoring_sascha.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_monitoring_sascha
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Author-email: Sascha Heyer <mail@saschaheyer.de>, Sascha Heyer <sascha@doit.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm_monitoring_sascha-0.0.4/monitoring/__init__.py` & `llm_monitoring_sascha-0.0.5/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_monitoring_sascha-0.0.4/monitoring/client.py` & `llm_monitoring_sascha-0.0.5/monitoring/client.py`

 * *Files identical despite different names*

### Comparing `llm_monitoring_sascha-0.0.4/pyproject.toml` & `llm_monitoring_sascha-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm_monitoring_sascha"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Sascha Heyer", email="mail@saschaheyer.de" },
   { name="Sascha Heyer", email="sascha@doit.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 classifiers = [
```

