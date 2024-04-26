# Comparing `tmp/fixinventory_plugin_posthog-4.0.4.tar.gz` & `tmp/fixinventory_plugin_posthog-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory_plugin_posthog-4.0.4.tar", last modified: Wed Apr 24 19:34:36 2024, max compression
+gzip compressed data, was "fixinventory_plugin_posthog-4.0.5.tar", last modified: Fri Apr 26 20:21:38 2024, max compression
```

## Comparing `fixinventory_plugin_posthog-4.0.4.tar` & `fixinventory_plugin_posthog-4.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:36.845985 fixinventory_plugin_posthog-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:31:44.000000 fixinventory_plugin_posthog-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-24 19:34:36.845985 fixinventory_plugin_posthog-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-24 19:31:44.000000 fixinventory_plugin_posthog-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:36.845985 fixinventory_plugin_posthog-4.0.4/fix_plugin_posthog/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-24 19:31:44.000000 fixinventory_plugin_posthog-4.0.4/fix_plugin_posthog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 19:31:44.000000 fixinventory_plugin_posthog-4.0.4/fix_plugin_posthog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-24 19:31:44.000000 fixinventory_plugin_posthog-4.0.4/fix_plugin_posthog/posthog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-24 19:31:44.000000 fixinventory_plugin_posthog-4.0.4/fix_plugin_posthog/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:36.845985 fixinventory_plugin_posthog-4.0.4/fixinventory_plugin_posthog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-24 19:34:36.000000 fixinventory_plugin_posthog-4.0.4/fixinventory_plugin_posthog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-24 19:34:36.000000 fixinventory_plugin_posthog-4.0.4/fixinventory_plugin_posthog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:34:36.000000 fixinventory_plugin_posthog-4.0.4/fixinventory_plugin_posthog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 19:34:36.000000 fixinventory_plugin_posthog-4.0.4/fixinventory_plugin_posthog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:32:50.000000 fixinventory_plugin_posthog-4.0.4/fixinventory_plugin_posthog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 19:34:36.000000 fixinventory_plugin_posthog-4.0.4/fixinventory_plugin_posthog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 19:34:36.000000 fixinventory_plugin_posthog-4.0.4/fixinventory_plugin_posthog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-24 19:31:44.000000 fixinventory_plugin_posthog-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 19:34:36.845985 fixinventory_plugin_posthog-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:36.845985 fixinventory_plugin_posthog-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-24 19:31:44.000000 fixinventory_plugin_posthog-4.0.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:38.358506 fixinventory_plugin_posthog-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:18:44.000000 fixinventory_plugin_posthog-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-26 20:21:38.358506 fixinventory_plugin_posthog-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-26 20:18:44.000000 fixinventory_plugin_posthog-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:38.358506 fixinventory_plugin_posthog-4.0.5/fix_plugin_posthog/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-26 20:18:44.000000 fixinventory_plugin_posthog-4.0.5/fix_plugin_posthog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-26 20:18:44.000000 fixinventory_plugin_posthog-4.0.5/fix_plugin_posthog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-26 20:18:44.000000 fixinventory_plugin_posthog-4.0.5/fix_plugin_posthog/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-26 20:18:44.000000 fixinventory_plugin_posthog-4.0.5/fix_plugin_posthog/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:38.358506 fixinventory_plugin_posthog-4.0.5/fixinventory_plugin_posthog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-26 20:21:38.000000 fixinventory_plugin_posthog-4.0.5/fixinventory_plugin_posthog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-26 20:21:38.000000 fixinventory_plugin_posthog-4.0.5/fixinventory_plugin_posthog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:21:38.000000 fixinventory_plugin_posthog-4.0.5/fixinventory_plugin_posthog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 20:21:38.000000 fixinventory_plugin_posthog-4.0.5/fixinventory_plugin_posthog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:19:52.000000 fixinventory_plugin_posthog-4.0.5/fixinventory_plugin_posthog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-26 20:21:38.000000 fixinventory_plugin_posthog-4.0.5/fixinventory_plugin_posthog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 20:21:38.000000 fixinventory_plugin_posthog-4.0.5/fixinventory_plugin_posthog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-26 20:18:44.000000 fixinventory_plugin_posthog-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 20:21:38.358506 fixinventory_plugin_posthog-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:38.358506 fixinventory_plugin_posthog-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-26 20:18:44.000000 fixinventory_plugin_posthog-4.0.5/test/test_config.py
```

### Comparing `fixinventory_plugin_posthog-4.0.4/PKG-INFO` & `fixinventory_plugin_posthog-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-posthog
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix Posthog Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/posthog
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
 Requires-Dist: requests
 
 # fix-plugin-posthog
 Posthog Collector Plugin for Fix
 
 This collector plugin is used to collect data from Posthog. It is used internally at Some Engineering to create metrics about fix installations and usage.
```

### Comparing `fixinventory_plugin_posthog-4.0.4/README.md` & `fixinventory_plugin_posthog-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_posthog-4.0.4/fix_plugin_posthog/__init__.py` & `fixinventory_plugin_posthog-4.0.5/fix_plugin_posthog/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_posthog-4.0.4/fix_plugin_posthog/posthog.py` & `fixinventory_plugin_posthog-4.0.5/fix_plugin_posthog/posthog.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_posthog-4.0.4/fix_plugin_posthog/resources.py` & `fixinventory_plugin_posthog-4.0.5/fix_plugin_posthog/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_posthog-4.0.4/fixinventory_plugin_posthog.egg-info/PKG-INFO` & `fixinventory_plugin_posthog-4.0.5/fixinventory_plugin_posthog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-posthog
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix Posthog Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/posthog
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
 Requires-Dist: requests
 
 # fix-plugin-posthog
 Posthog Collector Plugin for Fix
 
 This collector plugin is used to collect data from Posthog. It is used internally at Some Engineering to create metrics about fix installations and usage.
```

### Comparing `fixinventory_plugin_posthog-4.0.4/fixinventory_plugin_posthog.egg-info/SOURCES.txt` & `fixinventory_plugin_posthog-4.0.5/fixinventory_plugin_posthog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_posthog-4.0.4/pyproject.toml` & `fixinventory_plugin_posthog-4.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-posthog"
 description = "Fix Posthog Collector Plugin"
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
     "requests",
 ]
 
 [project.entry-points."fix.plugins"]
 posthog = "fix_plugin_posthog:PosthogCollectorPlugin"
 
 [project.urls]
```

