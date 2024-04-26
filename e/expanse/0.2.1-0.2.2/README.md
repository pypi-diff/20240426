# Comparing `tmp/expanse-0.2.1.tar.gz` & `tmp/expanse-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expanse-0.2.1.tar", last modified: Fri Apr 26 10:46:15 2024, max compression
+gzip compressed data, was "expanse-0.2.2.tar", last modified: Fri Apr 26 11:01:39 2024, max compression
```

## Comparing `expanse-0.2.1.tar` & `expanse-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:46:15.542823 expanse-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 10:46:09.000000 expanse-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-26 10:46:15.542823 expanse-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-26 10:46:09.000000 expanse-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:46:15.538823 expanse-0.2.1/expanse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:46:09.000000 expanse-0.2.1/expanse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 10:46:09.000000 expanse-0.2.1/expanse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-26 10:46:09.000000 expanse-0.2.1/expanse/apple_health.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-26 10:46:09.000000 expanse-0.2.1/expanse/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:46:15.542823 expanse-0.2.1/expanse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-26 10:46:15.000000 expanse-0.2.1/expanse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-26 10:46:15.000000 expanse-0.2.1/expanse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:46:15.000000 expanse-0.2.1/expanse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 10:46:15.000000 expanse-0.2.1/expanse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 10:46:15.000000 expanse-0.2.1/expanse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-26 10:46:09.000000 expanse-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:46:15.542823 expanse-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:46:15.542823 expanse-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 10:46:09.000000 expanse-0.2.1/tests/test_expanse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:01:39.428463 expanse-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 11:01:31.000000 expanse-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-26 11:01:39.428463 expanse-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-26 11:01:31.000000 expanse-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:01:39.424463 expanse-0.2.2/expanse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:01:31.000000 expanse-0.2.2/expanse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 11:01:31.000000 expanse-0.2.2/expanse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-26 11:01:31.000000 expanse-0.2.2/expanse/apple_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-26 11:01:31.000000 expanse-0.2.2/expanse/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:01:39.428463 expanse-0.2.2/expanse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 11:01:39.000000 expanse-0.2.2/expanse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-26 11:01:31.000000 expanse-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:01:39.428463 expanse-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:01:39.424463 expanse-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 11:01:31.000000 expanse-0.2.2/tests/test_expanse.py
```

### Comparing `expanse-0.2.1/LICENSE` & `expanse-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `expanse-0.2.1/PKG-INFO` & `expanse-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expanse
-Version: 0.2.1
+Version: 0.2.2
 Summary: turn apple health export.xml into parquet
 Author: Thomas Schranz
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tosh/expanse
 Project-URL: Changelog, https://github.com/tosh/expanse/releases
 Project-URL: Issues, https://github.com/tosh/expanse/issues
 Project-URL: CI, https://github.com/tosh/expanse/actions
@@ -32,13 +32,13 @@
 Install expanse using `pipx`:
 ```bash
 brew install pipx
 pipx install expanse
 ```
 ## Usage
 
-Usage instructions go here.
+`expanse parquet export.xml`
 
 ## Features
 
 - turn export.xml into a simple parquet file
```

### Comparing `expanse-0.2.1/README.md` & `expanse-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 Install expanse using `pipx`:
 ```bash
 brew install pipx
 pipx install expanse
 ```
 ## Usage
 
-Usage instructions go here.
+`expanse parquet export.xml`
 
 ## Features
 
 - turn export.xml into a simple parquet file
```

### Comparing `expanse-0.2.1/expanse/apple_health.py` & `expanse-0.2.2/expanse/apple_health.py`

 * *Files identical despite different names*

### Comparing `expanse-0.2.1/expanse/cli.py` & `expanse-0.2.2/expanse/cli.py`

 * *Files identical despite different names*

### Comparing `expanse-0.2.1/expanse.egg-info/PKG-INFO` & `expanse-0.2.2/expanse.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expanse
-Version: 0.2.1
+Version: 0.2.2
 Summary: turn apple health export.xml into parquet
 Author: Thomas Schranz
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tosh/expanse
 Project-URL: Changelog, https://github.com/tosh/expanse/releases
 Project-URL: Issues, https://github.com/tosh/expanse/issues
 Project-URL: CI, https://github.com/tosh/expanse/actions
@@ -32,13 +32,13 @@
 Install expanse using `pipx`:
 ```bash
 brew install pipx
 pipx install expanse
 ```
 ## Usage
 
-Usage instructions go here.
+`expanse parquet export.xml`
 
 ## Features
 
 - turn export.xml into a simple parquet file
```

### Comparing `expanse-0.2.1/pyproject.toml` & `expanse-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "expanse"
-version = "0.2.1"
+version = "0.2.2"
 description = "turn apple health export.xml into parquet"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{name = "Thomas Schranz"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
@@ -15,16 +15,18 @@
     "polars>=0.20.22"
 ]
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
+[project.scripts]
+expanse = "expanse.cli:main"
+
 [project.urls]
 Homepage = "https://github.com/tosh/expanse"
 Changelog = "https://github.com/tosh/expanse/releases"
 Issues = "https://github.com/tosh/expanse/issues"
 CI = "https://github.com/tosh/expanse/actions"
 
-
 [project.optional-dependencies]
 test = ["pytest"]
```

