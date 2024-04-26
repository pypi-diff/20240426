# Comparing `tmp/datasette_test-0.3.tar.gz` & `tmp/datasette_test-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_test-0.3.tar", last modified: Fri Apr 26 18:23:55 2024, max compression
+gzip compressed data, was "datasette_test-0.3.1.tar", last modified: Fri Apr 26 18:55:55 2024, max compression
```

## Comparing `datasette_test-0.3.tar` & `datasette_test-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:23:55.302247 datasette_test-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 18:23:46.000000 datasette_test-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-26 18:23:55.302247 datasette_test-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-26 18:23:46.000000 datasette_test-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:23:55.298247 datasette_test-0.3/datasette_test/
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-26 18:23:46.000000 datasette_test-0.3/datasette_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-26 18:23:46.000000 datasette_test-0.3/datasette_test/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:23:55.298247 datasette_test-0.3/datasette_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-26 18:23:46.000000 datasette_test-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:23:55.302247 datasette_test-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:23:55.298247 datasette_test-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-26 18:23:46.000000 datasette_test-0.3/tests/test_datasette_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:55:55.301807 datasette_test-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 18:55:49.000000 datasette_test-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-26 18:55:55.301807 datasette_test-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-26 18:55:49.000000 datasette_test-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:55:55.297807 datasette_test-0.3.1/datasette_test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-26 18:55:49.000000 datasette_test-0.3.1/datasette_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:55:55.301807 datasette_test-0.3.1/datasette_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-26 18:55:55.000000 datasette_test-0.3.1/datasette_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-26 18:55:55.000000 datasette_test-0.3.1/datasette_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:55:55.000000 datasette_test-0.3.1/datasette_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 18:55:55.000000 datasette_test-0.3.1/datasette_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 18:55:55.000000 datasette_test-0.3.1/datasette_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-26 18:55:49.000000 datasette_test-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:55:55.301807 datasette_test-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:55:55.301807 datasette_test-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-26 18:55:49.000000 datasette_test-0.3.1/tests/test_datasette_test.py
```

### Comparing `datasette_test-0.3/LICENSE` & `datasette_test-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_test-0.3/PKG-INFO` & `datasette_test-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: datasette-test
-Version: 0.3
+Version: 0.3.1
 Summary: Utilities to help write tests for Datasette plugins and applications
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-test
 Project-URL: Changelog, https://github.com/datasette/datasette-test/releases
 Project-URL: Issues, https://github.com/datasette/datasette-test/issues
 Project-URL: CI, https://github.com/datasette/datasette-test/actions
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datasette
 Requires-Dist: httpx
 Requires-Dist: packaging
+Requires-Dist: datasette-test-plugin
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 
 # datasette-test
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-test.svg)](https://pypi.org/project/datasette-test/)
```

### Comparing `datasette_test-0.3/README.md` & `datasette_test-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `datasette_test-0.3/datasette_test/__init__.py` & `datasette_test-0.3.1/datasette_test/__init__.py`

 * *Files identical despite different names*

### Comparing `datasette_test-0.3/datasette_test.egg-info/PKG-INFO` & `datasette_test-0.3.1/datasette_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: datasette-test
-Version: 0.3
+Version: 0.3.1
 Summary: Utilities to help write tests for Datasette plugins and applications
 Author: Datasette
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-test
 Project-URL: Changelog, https://github.com/datasette/datasette-test/releases
 Project-URL: Issues, https://github.com/datasette/datasette-test/issues
 Project-URL: CI, https://github.com/datasette/datasette-test/actions
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datasette
 Requires-Dist: httpx
 Requires-Dist: packaging
+Requires-Dist: datasette-test-plugin
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 
 # datasette-test
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-test.svg)](https://pypi.org/project/datasette-test/)
```

### Comparing `datasette_test-0.3/pyproject.toml` & `datasette_test-0.3.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [project]
 name = "datasette-test"
-version = "0.3"
+version = "0.3.1"
 description = "Utilities to help write tests for Datasette plugins and applications"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{name = "Datasette"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
     "datasette",
     "httpx",
-    "packaging"
+    "packaging",
+    "datasette-test-plugin"
 ]
 
 [project.urls]
 Homepage = "https://github.com/datasette/datasette-test"
 Changelog = "https://github.com/datasette/datasette-test/releases"
 Issues = "https://github.com/datasette/datasette-test/issues"
 CI = "https://github.com/datasette/datasette-test/actions"
 
-[project.entry-points.datasette]
-datasette_test = "datasette_test.plugin"
-
 [project.optional-dependencies]
 test = ["pytest", "pytest-asyncio"]
```

### Comparing `datasette_test-0.3/tests/test_datasette_test.py` & `datasette_test-0.3.1/tests/test_datasette_test.py`

 * *Files identical despite different names*

