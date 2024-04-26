# Comparing `tmp/fixinventory_plugin_vsphere-4.0.4.tar.gz` & `tmp/fixinventory_plugin_vsphere-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory_plugin_vsphere-4.0.4.tar", last modified: Wed Apr 24 19:31:39 2024, max compression
+gzip compressed data, was "fixinventory_plugin_vsphere-4.0.5.tar", last modified: Fri Apr 26 20:21:47 2024, max compression
```

## Comparing `fixinventory_plugin_vsphere-4.0.4.tar` & `fixinventory_plugin_vsphere-4.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:39.160911 fixinventory_plugin_vsphere-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-24 19:28:47.000000 fixinventory_plugin_vsphere-4.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:28:47.000000 fixinventory_plugin_vsphere-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-24 19:31:39.160911 fixinventory_plugin_vsphere-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 19:28:47.000000 fixinventory_plugin_vsphere-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:39.160911 fixinventory_plugin_vsphere-4.0.4/fix_plugin_vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-24 19:28:47.000000 fixinventory_plugin_vsphere-4.0.4/fix_plugin_vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-24 19:28:47.000000 fixinventory_plugin_vsphere-4.0.4/fix_plugin_vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-24 19:28:47.000000 fixinventory_plugin_vsphere-4.0.4/fix_plugin_vsphere/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-24 19:28:47.000000 fixinventory_plugin_vsphere-4.0.4/fix_plugin_vsphere/vsphere_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:39.160911 fixinventory_plugin_vsphere-4.0.4/fixinventory_plugin_vsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-24 19:31:39.000000 fixinventory_plugin_vsphere-4.0.4/fixinventory_plugin_vsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-24 19:31:39.000000 fixinventory_plugin_vsphere-4.0.4/fixinventory_plugin_vsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:31:39.000000 fixinventory_plugin_vsphere-4.0.4/fixinventory_plugin_vsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 19:31:39.000000 fixinventory_plugin_vsphere-4.0.4/fixinventory_plugin_vsphere.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:29:53.000000 fixinventory_plugin_vsphere-4.0.4/fixinventory_plugin_vsphere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 19:31:39.000000 fixinventory_plugin_vsphere-4.0.4/fixinventory_plugin_vsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 19:31:39.000000 fixinventory_plugin_vsphere-4.0.4/fixinventory_plugin_vsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-24 19:28:47.000000 fixinventory_plugin_vsphere-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 19:31:39.160911 fixinventory_plugin_vsphere-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:39.160911 fixinventory_plugin_vsphere-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-24 19:28:47.000000 fixinventory_plugin_vsphere-4.0.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:47.730500 fixinventory_plugin_vsphere-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-26 20:18:50.000000 fixinventory_plugin_vsphere-4.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:18:50.000000 fixinventory_plugin_vsphere-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-26 20:21:47.730500 fixinventory_plugin_vsphere-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 20:18:50.000000 fixinventory_plugin_vsphere-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:47.730500 fixinventory_plugin_vsphere-4.0.5/fix_plugin_vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-26 20:18:50.000000 fixinventory_plugin_vsphere-4.0.5/fix_plugin_vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-26 20:18:50.000000 fixinventory_plugin_vsphere-4.0.5/fix_plugin_vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-26 20:18:50.000000 fixinventory_plugin_vsphere-4.0.5/fix_plugin_vsphere/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-26 20:18:50.000000 fixinventory_plugin_vsphere-4.0.5/fix_plugin_vsphere/vsphere_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:47.730500 fixinventory_plugin_vsphere-4.0.5/fixinventory_plugin_vsphere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-26 20:21:47.000000 fixinventory_plugin_vsphere-4.0.5/fixinventory_plugin_vsphere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-26 20:21:47.000000 fixinventory_plugin_vsphere-4.0.5/fixinventory_plugin_vsphere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:21:47.000000 fixinventory_plugin_vsphere-4.0.5/fixinventory_plugin_vsphere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 20:21:47.000000 fixinventory_plugin_vsphere-4.0.5/fixinventory_plugin_vsphere.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:19:57.000000 fixinventory_plugin_vsphere-4.0.5/fixinventory_plugin_vsphere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-26 20:21:47.000000 fixinventory_plugin_vsphere-4.0.5/fixinventory_plugin_vsphere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 20:21:47.000000 fixinventory_plugin_vsphere-4.0.5/fixinventory_plugin_vsphere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-26 20:18:50.000000 fixinventory_plugin_vsphere-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 20:21:47.730500 fixinventory_plugin_vsphere-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:47.730500 fixinventory_plugin_vsphere-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-26 20:18:50.000000 fixinventory_plugin_vsphere-4.0.5/test/test_config.py
```

### Comparing `fixinventory_plugin_vsphere-4.0.4/LICENSE` & `fixinventory_plugin_vsphere-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_vsphere-4.0.4/PKG-INFO` & `fixinventory_plugin_vsphere-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-vsphere
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix VSphere Collector Plugin
 Author: Some Engineering Inc.
 License: 
                                       Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
@@ -217,15 +217,15 @@
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: pyvmomi
 
 # fix-plugin-vsphere
 VMWare VSphere Collector Plugin for Fix (Alpha)
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory_plugin_vsphere-4.0.4/fix_plugin_vsphere/__init__.py` & `fixinventory_plugin_vsphere-4.0.5/fix_plugin_vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_vsphere-4.0.4/fix_plugin_vsphere/config.py` & `fixinventory_plugin_vsphere-4.0.5/fix_plugin_vsphere/config.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_vsphere-4.0.4/fix_plugin_vsphere/resources.py` & `fixinventory_plugin_vsphere-4.0.5/fix_plugin_vsphere/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_vsphere-4.0.4/fix_plugin_vsphere/vsphere_client.py` & `fixinventory_plugin_vsphere-4.0.5/fix_plugin_vsphere/vsphere_client.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_vsphere-4.0.4/fixinventory_plugin_vsphere.egg-info/PKG-INFO` & `fixinventory_plugin_vsphere-4.0.5/fixinventory_plugin_vsphere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-vsphere
-Version: 4.0.4
+Version: 4.0.5
 Summary: Fix VSphere Collector Plugin
 Author: Some Engineering Inc.
 License: 
                                       Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
@@ -217,15 +217,15 @@
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: pyvmomi
 
 # fix-plugin-vsphere
 VMWare VSphere Collector Plugin for Fix (Alpha)
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory_plugin_vsphere-4.0.4/fixinventory_plugin_vsphere.egg-info/SOURCES.txt` & `fixinventory_plugin_vsphere-4.0.5/fixinventory_plugin_vsphere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_vsphere-4.0.4/pyproject.toml` & `fixinventory_plugin_vsphere-4.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-vsphere"
 description = "Fix VSphere Collector Plugin"
-version = "4.0.4"
+version = "4.0.5"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
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
     "pyvmomi",
 ]
 
 [project.entry-points."fix.plugins"]
 vsphere = "fix_plugin_vsphere:VSphereCollectorPlugin"
 
 [project.urls]
```

