# Comparing `tmp/psrecord-1.3.tar.gz` & `tmp/psrecord-1.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psrecord-1.3.tar", last modified: Fri Apr 26 11:05:04 2024, max compression
+gzip compressed data, was "psrecord-1.3.dev0.tar", last modified: Fri Apr 26 10:55:49 2024, max compression
```

## Comparing `psrecord-1.3.tar` & `psrecord-1.3.dev0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:05:04.683929 psrecord-1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:05:04.679929 psrecord-1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:05:04.683929 psrecord-1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-26 11:04:55.000000 psrecord-1.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-26 11:04:55.000000 psrecord-1.3/.github/workflows/update-changelog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-26 11:04:55.000000 psrecord-1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-26 11:04:55.000000 psrecord-1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-26 11:04:55.000000 psrecord-1.3/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-26 11:04:55.000000 psrecord-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 11:04:55.000000 psrecord-1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-26 11:05:04.683929 psrecord-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-26 11:04:55.000000 psrecord-1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:05:04.683929 psrecord-1.3/psrecord/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-26 11:04:55.000000 psrecord-1.3/psrecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-26 11:04:55.000000 psrecord-1.3/psrecord/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-26 11:05:04.000000 psrecord-1.3/psrecord/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-26 11:04:55.000000 psrecord-1.3/psrecord/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:05:04.683929 psrecord-1.3/psrecord/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:04:55.000000 psrecord-1.3/psrecord/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-26 11:04:55.000000 psrecord-1.3/psrecord/tests/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:05:04.683929 psrecord-1.3/psrecord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-26 11:05:04.000000 psrecord-1.3/psrecord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-26 11:05:04.000000 psrecord-1.3/psrecord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:05:04.000000 psrecord-1.3/psrecord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 11:05:04.000000 psrecord-1.3/psrecord.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 11:05:04.000000 psrecord-1.3/psrecord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 11:05:04.000000 psrecord-1.3/psrecord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:05:04.000000 psrecord-1.3/psrecord.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-26 11:04:55.000000 psrecord-1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    51707 2024-04-26 11:04:55.000000 psrecord-1.3/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:05:04.683929 psrecord-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-26 11:04:55.000000 psrecord-1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.621949 psrecord-1.3.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.621949 psrecord-1.3.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/psrecord/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/psrecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/psrecord/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/psrecord/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/psrecord/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/psrecord/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/psrecord/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/psrecord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:55:49.000000 psrecord-1.3.dev0/psrecord.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    51707 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:55:49.625949 psrecord-1.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-26 10:55:39.000000 psrecord-1.3.dev0/tox.ini
```

### Comparing `psrecord-1.3/.github/workflows/main.yml` & `psrecord-1.3.dev0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `psrecord-1.3/.github/workflows/update-changelog.yaml` & `psrecord-1.3.dev0/.github/workflows/update-changelog.yaml`

 * *Files identical despite different names*

### Comparing `psrecord-1.3/.gitignore` & `psrecord-1.3.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `psrecord-1.3/LICENSE` & `psrecord-1.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `psrecord-1.3/PKG-INFO` & `psrecord-1.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrecord
-Version: 1.3
+Version: 1.3.dev0
 Summary: Python package to record activity from processes
 Author-email: Thomas Robitaille <thomas.robitaille@gmail.com>
 License: Simplified BSD License
 Project-URL: Homepage, https://github.com/astrofrog/psrecord
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `psrecord-1.3/README.rst` & `psrecord-1.3.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `psrecord-1.3/psrecord/__init__.py` & `psrecord-1.3.dev0/psrecord/__init__.py`

 * *Files identical despite different names*

### Comparing `psrecord-1.3/psrecord/__main__.py` & `psrecord-1.3.dev0/psrecord/__main__.py`

 * *Files identical despite different names*

### Comparing `psrecord-1.3/psrecord/main.py` & `psrecord-1.3.dev0/psrecord/main.py`

 * *Files identical despite different names*

### Comparing `psrecord-1.3/psrecord/tests/test_main.py` & `psrecord-1.3.dev0/psrecord/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `psrecord-1.3/psrecord.egg-info/PKG-INFO` & `psrecord-1.3.dev0/psrecord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrecord
-Version: 1.3
+Version: 1.3.dev0
 Summary: Python package to record activity from processes
 Author-email: Thomas Robitaille <thomas.robitaille@gmail.com>
 License: Simplified BSD License
 Project-URL: Homepage, https://github.com/astrofrog/psrecord
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `psrecord-1.3/psrecord.egg-info/SOURCES.txt` & `psrecord-1.3.dev0/psrecord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psrecord-1.3/pyproject.toml` & `psrecord-1.3.dev0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 version_file = "psrecord/_version.py"
 
 [project]
 name = "psrecord"
-dynamic = [
-    "version"
-]
+version = "1.3.dev0"
 authors = [
     { name = "Thomas Robitaille", email = "thomas.robitaille@gmail.com" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
     "License :: OSI Approved :: BSD License",
```

### Comparing `psrecord-1.3/screenshot.png` & `psrecord-1.3.dev0/screenshot.png`

 * *Files identical despite different names*

