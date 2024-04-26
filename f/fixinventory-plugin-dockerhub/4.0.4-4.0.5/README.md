# Comparing `tmp/fixinventory_plugin_dockerhub-4.0.4.tar.gz` & `tmp/fixinventory_plugin_dockerhub-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory_plugin_dockerhub-4.0.4.tar", last modified: Wed Apr 24 19:30:59 2024, max compression
+gzip compressed data, was "fixinventory_plugin_dockerhub-4.0.5.tar", last modified: Fri Apr 26 20:22:02 2024, max compression
```

## Comparing `fixinventory_plugin_dockerhub-4.0.4.tar` & `fixinventory_plugin_dockerhub-4.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:59.349605 fixinventory_plugin_dockerhub-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:27:59.000000 fixinventory_plugin_dockerhub-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-24 19:30:59.349605 fixinventory_plugin_dockerhub-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-24 19:27:59.000000 fixinventory_plugin_dockerhub-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:59.349605 fixinventory_plugin_dockerhub-4.0.4/fix_plugin_dockerhub/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-24 19:27:59.000000 fixinventory_plugin_dockerhub-4.0.4/fix_plugin_dockerhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-24 19:27:59.000000 fixinventory_plugin_dockerhub-4.0.4/fix_plugin_dockerhub/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-24 19:27:59.000000 fixinventory_plugin_dockerhub-4.0.4/fix_plugin_dockerhub/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:59.349605 fixinventory_plugin_dockerhub-4.0.4/fixinventory_plugin_dockerhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-24 19:30:59.000000 fixinventory_plugin_dockerhub-4.0.4/fixinventory_plugin_dockerhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 19:30:59.000000 fixinventory_plugin_dockerhub-4.0.4/fixinventory_plugin_dockerhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:30:59.000000 fixinventory_plugin_dockerhub-4.0.4/fixinventory_plugin_dockerhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 19:30:59.000000 fixinventory_plugin_dockerhub-4.0.4/fixinventory_plugin_dockerhub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:29:10.000000 fixinventory_plugin_dockerhub-4.0.4/fixinventory_plugin_dockerhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 19:30:59.000000 fixinventory_plugin_dockerhub-4.0.4/fixinventory_plugin_dockerhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 19:30:59.000000 fixinventory_plugin_dockerhub-4.0.4/fixinventory_plugin_dockerhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 19:27:59.000000 fixinventory_plugin_dockerhub-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 19:30:59.349605 fixinventory_plugin_dockerhub-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:59.349605 fixinventory_plugin_dockerhub-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-24 19:27:59.000000 fixinventory_plugin_dockerhub-4.0.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:01.998777 fixinventory_plugin_dockerhub-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:18:43.000000 fixinventory_plugin_dockerhub-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-26 20:22:01.998777 fixinventory_plugin_dockerhub-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-26 20:18:43.000000 fixinventory_plugin_dockerhub-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:01.994778 fixinventory_plugin_dockerhub-4.0.5/fix_plugin_dockerhub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-26 20:18:43.000000 fixinventory_plugin_dockerhub-4.0.5/fix_plugin_dockerhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-26 20:18:43.000000 fixinventory_plugin_dockerhub-4.0.5/fix_plugin_dockerhub/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-26 20:18:43.000000 fixinventory_plugin_dockerhub-4.0.5/fix_plugin_dockerhub/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:01.998777 fixinventory_plugin_dockerhub-4.0.5/fixinventory_plugin_dockerhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-26 20:22:01.000000 fixinventory_plugin_dockerhub-4.0.5/fixinventory_plugin_dockerhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-26 20:22:01.000000 fixinventory_plugin_dockerhub-4.0.5/fixinventory_plugin_dockerhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:22:01.000000 fixinventory_plugin_dockerhub-4.0.5/fixinventory_plugin_dockerhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 20:22:01.000000 fixinventory_plugin_dockerhub-4.0.5/fixinventory_plugin_dockerhub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:19:57.000000 fixinventory_plugin_dockerhub-4.0.5/fixinventory_plugin_dockerhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-26 20:22:01.000000 fixinventory_plugin_dockerhub-4.0.5/fixinventory_plugin_dockerhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-26 20:22:01.000000 fixinventory_plugin_dockerhub-4.0.5/fixinventory_plugin_dockerhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-26 20:18:43.000000 fixinventory_plugin_dockerhub-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 20:22:01.998777 fixinventory_plugin_dockerhub-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:01.998777 fixinventory_plugin_dockerhub-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-26 20:18:43.000000 fixinventory_plugin_dockerhub-4.0.5/test/test_config.py
```

### Comparing `fixinventory_plugin_dockerhub-4.0.4/PKG-INFO` & `fixinventory_plugin_dockerhub-4.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-dockerhub
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix Docker Hub Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/dockerhub
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
 
 # fix-plugin-dockerhub
 Docker Hub Collector Plugin for Fix
 
 This collector plugin is used to collect data from Docker Hub. It is used internally at Some Engineering to create metrics about image downloads.
```

### Comparing `fixinventory_plugin_dockerhub-4.0.4/README.md` & `fixinventory_plugin_dockerhub-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_dockerhub-4.0.4/fix_plugin_dockerhub/__init__.py` & `fixinventory_plugin_dockerhub-4.0.5/fix_plugin_dockerhub/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_dockerhub-4.0.4/fix_plugin_dockerhub/resources.py` & `fixinventory_plugin_dockerhub-4.0.5/fix_plugin_dockerhub/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_dockerhub-4.0.4/fixinventory_plugin_dockerhub.egg-info/PKG-INFO` & `fixinventory_plugin_dockerhub-4.0.5/fixinventory_plugin_dockerhub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-dockerhub
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix Docker Hub Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/dockerhub
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
 
 # fix-plugin-dockerhub
 Docker Hub Collector Plugin for Fix
 
 This collector plugin is used to collect data from Docker Hub. It is used internally at Some Engineering to create metrics about image downloads.
```

### Comparing `fixinventory_plugin_dockerhub-4.0.4/fixinventory_plugin_dockerhub.egg-info/SOURCES.txt` & `fixinventory_plugin_dockerhub-4.0.5/fixinventory_plugin_dockerhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_dockerhub-4.0.4/pyproject.toml` & `fixinventory_plugin_dockerhub-4.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-dockerhub"
 description = "Fix Docker Hub Collector Plugin"
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
 dockerhub = "fix_plugin_dockerhub:DockerHubCollectorPlugin"
```

