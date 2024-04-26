# Comparing `tmp/rwthcolors-0.2.5.tar.gz` & `tmp/rwthcolors-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwthcolors-0.2.5.tar", max compression
+gzip compressed data, was "rwthcolors-0.2.6.tar", max compression
```

## Comparing `rwthcolors-0.2.5.tar` & `rwthcolors-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      804 2024-01-04 15:24:42.395137 rwthcolors-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-02-01 16:21:46.097203 rwthcolors-0.2.5/README.md
--rw-r--r--   0        0        0      933 2023-04-24 14:29:37.538409 rwthcolors-0.2.5/RWTHColors/__init__.py
--rw-r--r--   0        0        0     7978 2024-01-04 15:22:26.806107 rwthcolors-0.2.5/RWTHColors/cm.py
--rw-r--r--   0        0        0       21 2022-02-01 10:44:53.069840 rwthcolors-0.2.5/RWTHColors/colors/__init__.py
--rw-r--r--   0        0        0      232 2024-01-04 14:49:40.932935 rwthcolors-0.2.5/RWTHColors/colors/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      221 2023-04-24 13:39:59.918195 rwthcolors-0.2.5/RWTHColors/colors/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6564 2024-01-04 15:22:27.762790 rwthcolors-0.2.5/RWTHColors/colors/__pycache__/colors.cpython-312.pyc
--rw-r--r--   0        0        0     5526 2023-04-24 13:39:59.930905 rwthcolors-0.2.5/RWTHColors/colors/__pycache__/colors.cpython-39.pyc
--rw-r--r--   0        0        0     5390 2024-01-04 15:22:26.820094 rwthcolors-0.2.5/RWTHColors/colors/colors.py
--rw-r--r--   0        0        0      137 2023-09-11 11:46:16.735408 rwthcolors-0.2.5/RWTHColors/mpl-styles/rwth-dark.mplstyle
--rw-r--r--   0        0        0      535 2023-04-24 15:40:42.132533 rwthcolors-0.2.5/RWTHColors/mpl-styles/rwth-full.mplstyle
--rw-r--r--   0        0        0      137 2023-04-24 15:37:41.325630 rwthcolors-0.2.5/RWTHColors/mpl-styles/rwth.mplstyle
--rw-r--r--   0        0        0     1037 1970-01-01 00:00:00.000000 rwthcolors-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      808 2024-04-26 13:29:38.551745 rwthcolors-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-02-01 16:21:46.097203 rwthcolors-0.2.6/README.md
+-rw-r--r--   0        0        0      933 2023-04-24 14:29:37.538409 rwthcolors-0.2.6/RWTHColors/__init__.py
+-rw-r--r--   0        0        0     7978 2024-01-04 15:22:26.806107 rwthcolors-0.2.6/RWTHColors/cm.py
+-rw-r--r--   0        0        0       21 2022-02-01 10:44:53.069840 rwthcolors-0.2.6/RWTHColors/colors/__init__.py
+-rw-r--r--   0        0        0      232 2024-01-04 14:49:40.932935 rwthcolors-0.2.6/RWTHColors/colors/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      221 2023-04-24 13:39:59.918195 rwthcolors-0.2.6/RWTHColors/colors/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6564 2024-01-04 15:22:27.762790 rwthcolors-0.2.6/RWTHColors/colors/__pycache__/colors.cpython-312.pyc
+-rw-r--r--   0        0        0     5526 2023-04-24 13:39:59.930905 rwthcolors-0.2.6/RWTHColors/colors/__pycache__/colors.cpython-39.pyc
+-rw-r--r--   0        0        0     5390 2024-01-04 15:22:26.820094 rwthcolors-0.2.6/RWTHColors/colors/colors.py
+-rw-r--r--   0        0        0      137 2023-09-11 11:46:16.735408 rwthcolors-0.2.6/RWTHColors/mpl-styles/rwth-dark.mplstyle
+-rw-r--r--   0        0        0      535 2023-04-24 15:40:42.132533 rwthcolors-0.2.6/RWTHColors/mpl-styles/rwth-full.mplstyle
+-rw-r--r--   0        0        0      137 2023-04-24 15:37:41.325630 rwthcolors-0.2.6/RWTHColors/mpl-styles/rwth.mplstyle
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 rwthcolors-0.2.6/PKG-INFO
```

### Comparing `rwthcolors-0.2.5/pyproject.toml` & `rwthcolors-0.2.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "RWTHColors"
-version = "0.2.5"
+version = "0.2.6"
 description = "Simple library that makes it easier to use RWTH CI colors in python projects"
 authors = ["Philipp Simon Leibner <philipp.leibner@ifs.rwth-aachen.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/ifs-rwth-aachen/RWTH-Colors"
 
 classifiers = [
@@ -16,17 +16,17 @@
 
 include = [
     "LICENSE",
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4.0"
-pytest = "^7.4.2"
-matplotlib = "^3.5.3"
-cycler = "^0.12.1"
+python = ">=3.9,<3.13"
+pytest = ">=7.4.2"
+matplotlib = ">=3.5.3"
+cycler = ">=0.12.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rwthcolors-0.2.5/RWTHColors/__init__.py` & `rwthcolors-0.2.6/RWTHColors/__init__.py`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.5/RWTHColors/cm.py` & `rwthcolors-0.2.6/RWTHColors/cm.py`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.5/RWTHColors/colors/__pycache__/colors.cpython-312.pyc` & `rwthcolors-0.2.6/RWTHColors/colors/__pycache__/colors.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.5/RWTHColors/colors/__pycache__/colors.cpython-39.pyc` & `rwthcolors-0.2.6/RWTHColors/colors/__pycache__/colors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.5/RWTHColors/colors/colors.py` & `rwthcolors-0.2.6/RWTHColors/colors/colors.py`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.5/RWTHColors/mpl-styles/rwth-full.mplstyle` & `rwthcolors-0.2.6/RWTHColors/mpl-styles/rwth-full.mplstyle`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.5/PKG-INFO` & `rwthcolors-0.2.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: RWTHColors
-Version: 0.2.5
+Version: 0.2.6
 Summary: Simple library that makes it easier to use RWTH CI colors in python projects
 Home-page: https://github.com/ifs-rwth-aachen/RWTH-Colors
 License: Apache-2.0
 Keywords: rwth,aachen,rwth aachen,farbwelt
 Author: Philipp Simon Leibner
 Author-email: philipp.leibner@ifs.rwth-aachen.de
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Dist: cycler (>=0.12.1,<0.13.0)
-Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
-Requires-Dist: pytest (>=7.4.2,<8.0.0)
+Requires-Dist: cycler (>=0.12.1)
+Requires-Dist: matplotlib (>=3.5.3)
+Requires-Dist: pytest (>=7.4.2)
 Project-URL: Repository, https://github.com/ifs-rwth-aachen/RWTH-Colors
 Description-Content-Type: text/markdown
```

