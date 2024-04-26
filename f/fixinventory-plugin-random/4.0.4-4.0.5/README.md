# Comparing `tmp/fixinventory_plugin_random-4.0.4.tar.gz` & `tmp/fixinventory_plugin_random-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory_plugin_random-4.0.4.tar", last modified: Wed Apr 24 19:34:17 2024, max compression
+gzip compressed data, was "fixinventory_plugin_random-4.0.5.tar", last modified: Fri Apr 26 20:22:33 2024, max compression
```

## Comparing `fixinventory_plugin_random-4.0.4.tar` & `fixinventory_plugin_random-4.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:17.296203 fixinventory_plugin_random-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:31:20.000000 fixinventory_plugin_random-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-24 19:34:17.296203 fixinventory_plugin_random-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-24 19:31:20.000000 fixinventory_plugin_random-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:17.296203 fixinventory_plugin_random-4.0.4/fix_plugin_random/
--rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-04-24 19:31:20.000000 fixinventory_plugin_random-4.0.4/fix_plugin_random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-24 19:31:20.000000 fixinventory_plugin_random-4.0.4/fix_plugin_random/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-24 19:31:20.000000 fixinventory_plugin_random-4.0.4/fix_plugin_random/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:17.296203 fixinventory_plugin_random-4.0.4/fixinventory_plugin_random.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-24 19:34:17.000000 fixinventory_plugin_random-4.0.4/fixinventory_plugin_random.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-24 19:34:17.000000 fixinventory_plugin_random-4.0.4/fixinventory_plugin_random.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:34:17.000000 fixinventory_plugin_random-4.0.4/fixinventory_plugin_random.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 19:34:17.000000 fixinventory_plugin_random-4.0.4/fixinventory_plugin_random.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:32:27.000000 fixinventory_plugin_random-4.0.4/fixinventory_plugin_random.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 19:34:17.000000 fixinventory_plugin_random-4.0.4/fixinventory_plugin_random.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:34:17.000000 fixinventory_plugin_random-4.0.4/fixinventory_plugin_random.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-24 19:31:20.000000 fixinventory_plugin_random-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 19:34:17.296203 fixinventory_plugin_random-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:17.296203 fixinventory_plugin_random-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-24 19:31:20.000000 fixinventory_plugin_random-4.0.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:33.326582 fixinventory_plugin_random-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:19:34.000000 fixinventory_plugin_random-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-26 20:22:33.326582 fixinventory_plugin_random-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-26 20:19:34.000000 fixinventory_plugin_random-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:33.326582 fixinventory_plugin_random-4.0.5/fix_plugin_random/
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-04-26 20:19:34.000000 fixinventory_plugin_random-4.0.5/fix_plugin_random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-26 20:19:34.000000 fixinventory_plugin_random-4.0.5/fix_plugin_random/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-26 20:19:34.000000 fixinventory_plugin_random-4.0.5/fix_plugin_random/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:33.326582 fixinventory_plugin_random-4.0.5/fixinventory_plugin_random.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-26 20:22:33.000000 fixinventory_plugin_random-4.0.5/fixinventory_plugin_random.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-26 20:22:33.000000 fixinventory_plugin_random-4.0.5/fixinventory_plugin_random.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:22:33.000000 fixinventory_plugin_random-4.0.5/fixinventory_plugin_random.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 20:22:33.000000 fixinventory_plugin_random-4.0.5/fixinventory_plugin_random.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:20:43.000000 fixinventory_plugin_random-4.0.5/fixinventory_plugin_random.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 20:22:33.000000 fixinventory_plugin_random-4.0.5/fixinventory_plugin_random.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:22:33.000000 fixinventory_plugin_random-4.0.5/fixinventory_plugin_random.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-26 20:19:34.000000 fixinventory_plugin_random-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 20:22:33.326582 fixinventory_plugin_random-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:33.326582 fixinventory_plugin_random-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-26 20:19:34.000000 fixinventory_plugin_random-4.0.5/test/test_config.py
```

### Comparing `fixinventory_plugin_random-4.0.4/PKG-INFO` & `fixinventory_plugin_random-4.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-random
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix Random Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/random
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
 
 # fix-plugin-random
 Random Cloud Collector for Fix
 
 Creates a plausible pseudo-random cloud based on a configurable seed.
 
 The base infrastructure stays the same, but the number of instances vary slightly from run to run so that metrics show some more interesting up/down lines.
```

### Comparing `fixinventory_plugin_random-4.0.4/README.md` & `fixinventory_plugin_random-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_random-4.0.4/fix_plugin_random/__init__.py` & `fixinventory_plugin_random-4.0.5/fix_plugin_random/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_random-4.0.4/fix_plugin_random/resources.py` & `fixinventory_plugin_random-4.0.5/fix_plugin_random/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_random-4.0.4/fixinventory_plugin_random.egg-info/PKG-INFO` & `fixinventory_plugin_random-4.0.5/fixinventory_plugin_random.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-random
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix Random Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/random
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
 
 # fix-plugin-random
 Random Cloud Collector for Fix
 
 Creates a plausible pseudo-random cloud based on a configurable seed.
 
 The base infrastructure stays the same, but the number of instances vary slightly from run to run so that metrics show some more interesting up/down lines.
```

### Comparing `fixinventory_plugin_random-4.0.4/pyproject.toml` & `fixinventory_plugin_random-4.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-random"
 description = "Fix Random Collector Plugin"
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
 ]
 
 [project.entry-points."fix.plugins"]
 random = "fix_plugin_random:RandomCollectorPlugin"
 
 [project.urls]
 Documentation = "https://inventory.fix.security"
```

