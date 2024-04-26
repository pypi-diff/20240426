# Comparing `tmp/fixinventory_plugin_onelogin-4.0.4.tar.gz` & `tmp/fixinventory_plugin_onelogin-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory_plugin_onelogin-4.0.4.tar", last modified: Wed Apr 24 19:30:12 2024, max compression
+gzip compressed data, was "fixinventory_plugin_onelogin-4.0.5.tar", last modified: Fri Apr 26 20:21:46 2024, max compression
```

## Comparing `fixinventory_plugin_onelogin-4.0.4.tar` & `fixinventory_plugin_onelogin-4.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:12.248603 fixinventory_plugin_onelogin-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:27:12.000000 fixinventory_plugin_onelogin-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-24 19:30:12.248603 fixinventory_plugin_onelogin-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-24 19:27:12.000000 fixinventory_plugin_onelogin-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:12.244603 fixinventory_plugin_onelogin-4.0.4/fix_plugin_onelogin/
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-24 19:27:12.000000 fixinventory_plugin_onelogin-4.0.4/fix_plugin_onelogin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-24 19:27:12.000000 fixinventory_plugin_onelogin-4.0.4/fix_plugin_onelogin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:12.244603 fixinventory_plugin_onelogin-4.0.4/fixinventory_plugin_onelogin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-24 19:30:12.000000 fixinventory_plugin_onelogin-4.0.4/fixinventory_plugin_onelogin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-24 19:30:12.000000 fixinventory_plugin_onelogin-4.0.4/fixinventory_plugin_onelogin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:30:12.000000 fixinventory_plugin_onelogin-4.0.4/fixinventory_plugin_onelogin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 19:30:12.000000 fixinventory_plugin_onelogin-4.0.4/fixinventory_plugin_onelogin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:28:24.000000 fixinventory_plugin_onelogin-4.0.4/fixinventory_plugin_onelogin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 19:30:12.000000 fixinventory_plugin_onelogin-4.0.4/fixinventory_plugin_onelogin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 19:30:12.000000 fixinventory_plugin_onelogin-4.0.4/fixinventory_plugin_onelogin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-24 19:27:12.000000 fixinventory_plugin_onelogin-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 19:30:12.248603 fixinventory_plugin_onelogin-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:12.244603 fixinventory_plugin_onelogin-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 19:27:12.000000 fixinventory_plugin_onelogin-4.0.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:46.431929 fixinventory_plugin_onelogin-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:18:46.000000 fixinventory_plugin_onelogin-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-26 20:21:46.431929 fixinventory_plugin_onelogin-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-26 20:18:46.000000 fixinventory_plugin_onelogin-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:46.427929 fixinventory_plugin_onelogin-4.0.5/fix_plugin_onelogin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-26 20:18:46.000000 fixinventory_plugin_onelogin-4.0.5/fix_plugin_onelogin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-26 20:18:46.000000 fixinventory_plugin_onelogin-4.0.5/fix_plugin_onelogin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:46.431929 fixinventory_plugin_onelogin-4.0.5/fixinventory_plugin_onelogin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-26 20:21:46.000000 fixinventory_plugin_onelogin-4.0.5/fixinventory_plugin_onelogin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-26 20:21:46.000000 fixinventory_plugin_onelogin-4.0.5/fixinventory_plugin_onelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:21:46.000000 fixinventory_plugin_onelogin-4.0.5/fixinventory_plugin_onelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-26 20:21:46.000000 fixinventory_plugin_onelogin-4.0.5/fixinventory_plugin_onelogin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:19:54.000000 fixinventory_plugin_onelogin-4.0.5/fixinventory_plugin_onelogin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 20:21:46.000000 fixinventory_plugin_onelogin-4.0.5/fixinventory_plugin_onelogin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 20:21:46.000000 fixinventory_plugin_onelogin-4.0.5/fixinventory_plugin_onelogin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-26 20:18:46.000000 fixinventory_plugin_onelogin-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 20:21:46.431929 fixinventory_plugin_onelogin-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:46.431929 fixinventory_plugin_onelogin-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-26 20:18:46.000000 fixinventory_plugin_onelogin-4.0.5/test/test_config.py
```

### Comparing `fixinventory_plugin_onelogin-4.0.4/PKG-INFO` & `fixinventory_plugin_onelogin-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-onelogin
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix OneLogin Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: onelogin==2.0.4
 
 # fix-plugin-onelogin
 OneLogin collector plugin for Fix
 
 This plugin collects OneLogin users as cloud resources and adds them to the Fix graph for use by other plugins.
```

### Comparing `fixinventory_plugin_onelogin-4.0.4/fix_plugin_onelogin/__init__.py` & `fixinventory_plugin_onelogin-4.0.5/fix_plugin_onelogin/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_onelogin-4.0.4/fixinventory_plugin_onelogin.egg-info/PKG-INFO` & `fixinventory_plugin_onelogin-4.0.5/fixinventory_plugin_onelogin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-onelogin
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix OneLogin Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: onelogin==2.0.4
 
 # fix-plugin-onelogin
 OneLogin collector plugin for Fix
 
 This plugin collects OneLogin users as cloud resources and adds them to the Fix graph for use by other plugins.
```

### Comparing `fixinventory_plugin_onelogin-4.0.4/pyproject.toml` & `fixinventory_plugin_onelogin-4.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-onelogin"
 description = "Fix OneLogin Plugin"
-version = "4.0.4"
+version = "4.0.5"
 authors = [{name="Some Engineering Inc."}]
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.4",
+    "fixinventorylib==4.0.5",
     "onelogin==2.0.4",
 ]
 
 [project.entry-points."fix.plugins"]
 onelogin = "fix_plugin_onelogin:OneLoginPlugin"
 
 [project.urls]
```

