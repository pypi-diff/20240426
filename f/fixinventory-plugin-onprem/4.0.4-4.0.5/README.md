# Comparing `tmp/fixinventory_plugin_onprem-4.0.4.tar.gz` & `tmp/fixinventory_plugin_onprem-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory_plugin_onprem-4.0.4.tar", last modified: Wed Apr 24 19:30:10 2024, max compression
+gzip compressed data, was "fixinventory_plugin_onprem-4.0.5.tar", last modified: Fri Apr 26 20:21:55 2024, max compression
```

## Comparing `fixinventory_plugin_onprem-4.0.4.tar` & `fixinventory_plugin_onprem-4.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:10.178983 fixinventory_plugin_onprem-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:27:15.000000 fixinventory_plugin_onprem-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 19:30:10.178983 fixinventory_plugin_onprem-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 19:27:15.000000 fixinventory_plugin_onprem-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:10.178983 fixinventory_plugin_onprem-4.0.4/fix_plugin_onprem/
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-24 19:27:15.000000 fixinventory_plugin_onprem-4.0.4/fix_plugin_onprem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-24 19:27:15.000000 fixinventory_plugin_onprem-4.0.4/fix_plugin_onprem/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-24 19:27:15.000000 fixinventory_plugin_onprem-4.0.4/fix_plugin_onprem/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-24 19:27:15.000000 fixinventory_plugin_onprem-4.0.4/fix_plugin_onprem/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:10.178983 fixinventory_plugin_onprem-4.0.4/fixinventory_plugin_onprem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 19:30:10.000000 fixinventory_plugin_onprem-4.0.4/fixinventory_plugin_onprem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-24 19:30:10.000000 fixinventory_plugin_onprem-4.0.4/fixinventory_plugin_onprem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:30:10.000000 fixinventory_plugin_onprem-4.0.4/fixinventory_plugin_onprem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 19:30:10.000000 fixinventory_plugin_onprem-4.0.4/fixinventory_plugin_onprem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:28:23.000000 fixinventory_plugin_onprem-4.0.4/fixinventory_plugin_onprem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 19:30:10.000000 fixinventory_plugin_onprem-4.0.4/fixinventory_plugin_onprem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:30:10.000000 fixinventory_plugin_onprem-4.0.4/fixinventory_plugin_onprem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-24 19:27:15.000000 fixinventory_plugin_onprem-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 19:30:10.178983 fixinventory_plugin_onprem-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:30:10.178983 fixinventory_plugin_onprem-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-24 19:27:15.000000 fixinventory_plugin_onprem-4.0.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:55.161499 fixinventory_plugin_onprem-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:19:01.000000 fixinventory_plugin_onprem-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 20:21:55.161499 fixinventory_plugin_onprem-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-26 20:19:01.000000 fixinventory_plugin_onprem-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:55.161499 fixinventory_plugin_onprem-4.0.5/fix_plugin_onprem/
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-26 20:19:01.000000 fixinventory_plugin_onprem-4.0.5/fix_plugin_onprem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-26 20:19:01.000000 fixinventory_plugin_onprem-4.0.5/fix_plugin_onprem/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-26 20:19:01.000000 fixinventory_plugin_onprem-4.0.5/fix_plugin_onprem/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-26 20:19:01.000000 fixinventory_plugin_onprem-4.0.5/fix_plugin_onprem/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:55.161499 fixinventory_plugin_onprem-4.0.5/fixinventory_plugin_onprem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 20:21:55.000000 fixinventory_plugin_onprem-4.0.5/fixinventory_plugin_onprem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-26 20:21:55.000000 fixinventory_plugin_onprem-4.0.5/fixinventory_plugin_onprem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:21:55.000000 fixinventory_plugin_onprem-4.0.5/fixinventory_plugin_onprem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 20:21:55.000000 fixinventory_plugin_onprem-4.0.5/fixinventory_plugin_onprem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:20:04.000000 fixinventory_plugin_onprem-4.0.5/fixinventory_plugin_onprem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-26 20:21:55.000000 fixinventory_plugin_onprem-4.0.5/fixinventory_plugin_onprem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:21:55.000000 fixinventory_plugin_onprem-4.0.5/fixinventory_plugin_onprem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-26 20:19:01.000000 fixinventory_plugin_onprem-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 20:21:55.161499 fixinventory_plugin_onprem-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:55.161499 fixinventory_plugin_onprem-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-26 20:19:01.000000 fixinventory_plugin_onprem-4.0.5/test/test_config.py
```

### Comparing `fixinventory_plugin_onprem-4.0.4/PKG-INFO` & `fixinventory_plugin_onprem-4.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-onprem
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix On-Premises Collector Plugin
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
 Requires-Dist: paramiko
 
 # fix-plugin-onprem (WIP)
 On-Premises Collector Plugin for Fix
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory_plugin_onprem-4.0.4/fix_plugin_onprem/__init__.py` & `fixinventory_plugin_onprem-4.0.5/fix_plugin_onprem/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_onprem-4.0.4/fix_plugin_onprem/config.py` & `fixinventory_plugin_onprem-4.0.5/fix_plugin_onprem/config.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_onprem-4.0.4/fix_plugin_onprem/resources.py` & `fixinventory_plugin_onprem-4.0.5/fix_plugin_onprem/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_onprem-4.0.4/fix_plugin_onprem/ssh.py` & `fixinventory_plugin_onprem-4.0.5/fix_plugin_onprem/ssh.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_onprem-4.0.4/fixinventory_plugin_onprem.egg-info/PKG-INFO` & `fixinventory_plugin_onprem-4.0.5/fixinventory_plugin_onprem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-onprem
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix On-Premises Collector Plugin
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
 Requires-Dist: paramiko
 
 # fix-plugin-onprem (WIP)
 On-Premises Collector Plugin for Fix
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory_plugin_onprem-4.0.4/fixinventory_plugin_onprem.egg-info/SOURCES.txt` & `fixinventory_plugin_onprem-4.0.5/fixinventory_plugin_onprem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_onprem-4.0.4/pyproject.toml` & `fixinventory_plugin_onprem-4.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-onprem"
 description = "Fix On-Premises Collector Plugin"
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
     "paramiko",
 ]
 
 [project.entry-points."fix.plugins"]
 onprem = "fix_plugin_onprem:OnpremCollectorPlugin"
 
 [project.urls]
```

### Comparing `fixinventory_plugin_onprem-4.0.4/test/test_config.py` & `fixinventory_plugin_onprem-4.0.5/test/test_config.py`

 * *Files identical despite different names*

