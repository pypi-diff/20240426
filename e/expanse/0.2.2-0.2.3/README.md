# Comparing `tmp/expanse-0.2.2.tar.gz` & `tmp/expanse-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expanse-0.2.2.tar", last modified: Fri Apr 26 11:01:39 2024, max compression
+gzip compressed data, was "expanse-0.2.3.tar", last modified: Fri Apr 26 11:11:28 2024, max compression
```

## Comparing `expanse-0.2.2.tar` & `expanse-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:01:39.428463 expanse-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 11:01:31.000000 expanse-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-26 11:01:39.428463 expanse-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-26 11:01:31.000000 expanse-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:01:39.424463 expanse-0.2.2/expanse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:01:31.000000 expanse-0.2.2/expanse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 11:01:31.000000 expanse-0.2.2/expanse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-26 11:01:31.000000 expanse-0.2.2/expanse/apple_health.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-26 11:01:31.000000 expanse-0.2.2/expanse/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:01:39.428463 expanse-0.2.2/expanse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-26 11:01:31.000000 expanse-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:01:39.428463 expanse-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:01:39.424463 expanse-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 11:01:31.000000 expanse-0.2.2/tests/test_expanse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:11:28.673165 expanse-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 11:11:21.000000 expanse-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-26 11:11:28.669165 expanse-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-26 11:11:21.000000 expanse-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:11:28.669165 expanse-0.2.3/expanse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:11:21.000000 expanse-0.2.3/expanse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 11:11:21.000000 expanse-0.2.3/expanse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-26 11:11:21.000000 expanse-0.2.3/expanse/apple_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-26 11:11:21.000000 expanse-0.2.3/expanse/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:11:28.669165 expanse-0.2.3/expanse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-26 11:11:28.000000 expanse-0.2.3/expanse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-26 11:11:28.000000 expanse-0.2.3/expanse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:11:28.000000 expanse-0.2.3/expanse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 11:11:28.000000 expanse-0.2.3/expanse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 11:11:28.000000 expanse-0.2.3/expanse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 11:11:28.000000 expanse-0.2.3/expanse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-26 11:11:21.000000 expanse-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:11:28.673165 expanse-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:11:28.669165 expanse-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 11:11:21.000000 expanse-0.2.3/tests/test_expanse.py
```

### Comparing `expanse-0.2.2/LICENSE` & `expanse-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `expanse-0.2.2/PKG-INFO` & `expanse-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expanse
-Version: 0.2.2
+Version: 0.2.3
 Summary: turn apple health export.xml into parquet
 Author: Thomas Schranz
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tosh/expanse
 Project-URL: Changelog, https://github.com/tosh/expanse/releases
 Project-URL: Issues, https://github.com/tosh/expanse/issues
 Project-URL: CI, https://github.com/tosh/expanse/actions
```

### Comparing `expanse-0.2.2/README.md` & `expanse-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `expanse-0.2.2/expanse/apple_health.py` & `expanse-0.2.3/expanse/apple_health.py`

 * *Files identical despite different names*

### Comparing `expanse-0.2.2/expanse/cli.py` & `expanse-0.2.3/expanse/cli.py`

 * *Files identical despite different names*

### Comparing `expanse-0.2.2/expanse.egg-info/PKG-INFO` & `expanse-0.2.3/expanse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expanse
-Version: 0.2.2
+Version: 0.2.3
 Summary: turn apple health export.xml into parquet
 Author: Thomas Schranz
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tosh/expanse
 Project-URL: Changelog, https://github.com/tosh/expanse/releases
 Project-URL: Issues, https://github.com/tosh/expanse/issues
 Project-URL: CI, https://github.com/tosh/expanse/actions
```

### Comparing `expanse-0.2.2/pyproject.toml` & `expanse-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "expanse"
-version = "0.2.2"
+version = "0.2.3"
 description = "turn apple health export.xml into parquet"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{name = "Thomas Schranz"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
@@ -16,15 +16,16 @@
 ]
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
-expanse = "expanse.cli:main"
+expanse = "expanse:__main__"
+
 
 [project.urls]
 Homepage = "https://github.com/tosh/expanse"
 Changelog = "https://github.com/tosh/expanse/releases"
 Issues = "https://github.com/tosh/expanse/issues"
 CI = "https://github.com/tosh/expanse/actions"
```

