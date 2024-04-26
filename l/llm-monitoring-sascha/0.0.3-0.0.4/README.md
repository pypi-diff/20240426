# Comparing `tmp/llm_monitoring_sascha-0.0.3.tar.gz` & `tmp/llm_monitoring_sascha-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_monitoring_sascha-0.0.3.tar", last modified: Fri Apr 26 08:13:09 2024, max compression
+gzip compressed data, was "llm_monitoring_sascha-0.0.4.tar", last modified: Fri Apr 26 08:28:02 2024, max compression
```

## Comparing `llm_monitoring_sascha-0.0.3.tar` & `llm_monitoring_sascha-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:13:09.530879 llm_monitoring_sascha-0.0.3/
--rw-r--r--   0 sascha     (501) staff       (20)        8 2024-04-26 07:51:08.000000 llm_monitoring_sascha-0.0.3/LICENSE
--rw-r--r--   0 sascha     (501) staff       (20)      549 2024-04-26 08:13:09.530606 llm_monitoring_sascha-0.0.3/PKG-INFO
--rw-r--r--   0 sascha     (501) staff       (20)       10 2023-12-21 09:09:33.000000 llm_monitoring_sascha-0.0.3/README.md
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:13:09.530135 llm_monitoring_sascha-0.0.3/llm_monitoring_sascha.egg-info/
--rw-r--r--   0 sascha     (501) staff       (20)      549 2024-04-26 08:13:09.000000 llm_monitoring_sascha-0.0.3/llm_monitoring_sascha.egg-info/PKG-INFO
--rw-r--r--   0 sascha     (501) staff       (20)      256 2024-04-26 08:13:09.000000 llm_monitoring_sascha-0.0.3/llm_monitoring_sascha.egg-info/SOURCES.txt
--rw-r--r--   0 sascha     (501) staff       (20)        1 2024-04-26 08:13:09.000000 llm_monitoring_sascha-0.0.3/llm_monitoring_sascha.egg-info/dependency_links.txt
--rw-r--r--   0 sascha     (501) staff       (20)       11 2024-04-26 08:13:09.000000 llm_monitoring_sascha-0.0.3/llm_monitoring_sascha.egg-info/top_level.txt
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:13:09.529720 llm_monitoring_sascha-0.0.3/monitoring/
--rw-r--r--   0 sascha     (501) staff       (20)     2113 2024-04-25 14:07:28.000000 llm_monitoring_sascha-0.0.3/monitoring/__init__.py
--rw-r--r--   0 sascha     (501) staff       (20)     4629 2024-04-26 07:28:16.000000 llm_monitoring_sascha-0.0.3/monitoring/client.py
--rw-r--r--   0 sascha     (501) staff       (20)      627 2024-04-26 08:13:04.000000 llm_monitoring_sascha-0.0.3/pyproject.toml
--rw-r--r--   0 sascha     (501) staff       (20)       38 2024-04-26 08:13:09.530952 llm_monitoring_sascha-0.0.3/setup.cfg
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:28:02.635837 llm_monitoring_sascha-0.0.4/
+-rw-r--r--   0 sascha     (501) staff       (20)        8 2024-04-26 07:51:08.000000 llm_monitoring_sascha-0.0.4/LICENSE
+-rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:28:02.635605 llm_monitoring_sascha-0.0.4/PKG-INFO
+-rw-r--r--   0 sascha     (501) staff       (20)       10 2023-12-21 09:09:33.000000 llm_monitoring_sascha-0.0.4/README.md
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:28:02.635290 llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/
+-rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:28:02.000000 llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/PKG-INFO
+-rw-r--r--   0 sascha     (501) staff       (20)      256 2024-04-26 08:28:02.000000 llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/SOURCES.txt
+-rw-r--r--   0 sascha     (501) staff       (20)        1 2024-04-26 08:28:02.000000 llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/dependency_links.txt
+-rw-r--r--   0 sascha     (501) staff       (20)       11 2024-04-26 08:28:02.000000 llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/top_level.txt
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:28:02.634524 llm_monitoring_sascha-0.0.4/monitoring/
+-rw-r--r--   0 sascha     (501) staff       (20)     2113 2024-04-25 14:07:28.000000 llm_monitoring_sascha-0.0.4/monitoring/__init__.py
+-rw-r--r--   0 sascha     (501) staff       (20)     4629 2024-04-26 07:28:16.000000 llm_monitoring_sascha-0.0.4/monitoring/client.py
+-rw-r--r--   0 sascha     (501) staff       (20)      601 2024-04-26 08:27:54.000000 llm_monitoring_sascha-0.0.4/pyproject.toml
+-rw-r--r--   0 sascha     (501) staff       (20)       38 2024-04-26 08:28:02.635900 llm_monitoring_sascha-0.0.4/setup.cfg
```

### Comparing `llm_monitoring_sascha-0.0.3/PKG-INFO` & `llm_monitoring_sascha-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: llm_monitoring_sascha
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Author-email: Sascha Heyer <mail@saschaheyer.de>, Sascha Heyer <sascha@doit.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Plenoria
```

### Comparing `llm_monitoring_sascha-0.0.3/llm_monitoring_sascha.egg-info/PKG-INFO` & `llm_monitoring_sascha-0.0.4/llm_monitoring_sascha.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: llm_monitoring_sascha
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Author-email: Sascha Heyer <mail@saschaheyer.de>, Sascha Heyer <sascha@doit.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Plenoria
```

### Comparing `llm_monitoring_sascha-0.0.3/monitoring/__init__.py` & `llm_monitoring_sascha-0.0.4/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_monitoring_sascha-0.0.3/monitoring/client.py` & `llm_monitoring_sascha-0.0.4/monitoring/client.py`

 * *Files identical despite different names*

### Comparing `llm_monitoring_sascha-0.0.3/pyproject.toml` & `llm_monitoring_sascha-0.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm_monitoring_sascha"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Sascha Heyer", email="mail@saschaheyer.de" },
   { name="Sascha Heyer", email="sascha@doit.com" },
 ]
 description = "A small example package"
 readme = "README.md"
-requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

