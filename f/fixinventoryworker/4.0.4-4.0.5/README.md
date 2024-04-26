# Comparing `tmp/fixinventoryworker-4.0.4.tar.gz` & `tmp/fixinventoryworker-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventoryworker-4.0.4.tar", last modified: Wed Apr 24 19:31:00 2024, max compression
+gzip compressed data, was "fixinventoryworker-4.0.5.tar", last modified: Fri Apr 26 20:23:17 2024, max compression
```

## Comparing `fixinventoryworker-4.0.4.tar` & `fixinventoryworker-4.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:00.822734 fixinventoryworker-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-24 19:31:00.822734 fixinventoryworker-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:00.818734 fixinventoryworker-4.0.4/fixinventoryworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-24 19:31:00.000000 fixinventoryworker-4.0.4/fixinventoryworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-24 19:31:00.000000 fixinventoryworker-4.0.4/fixinventoryworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:31:00.000000 fixinventoryworker-4.0.4/fixinventoryworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 19:31:00.000000 fixinventoryworker-4.0.4/fixinventoryworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:28:16.000000 fixinventoryworker-4.0.4/fixinventoryworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 19:31:00.000000 fixinventoryworker-4.0.4/fixinventoryworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 19:31:00.000000 fixinventoryworker-4.0.4/fixinventoryworker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:00.818734 fixinventoryworker-4.0.4/fixworker/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/fixworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13357 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/fixworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/fixworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/fixworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/fixworker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/fixworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/fixworker/fixcore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/fixworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/fixworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/fixworker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 19:31:00.822734 fixinventoryworker-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:00.818734 fixinventoryworker-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/test/test_fixcore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-24 19:27:10.000000 fixinventoryworker-4.0.4/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:23:17.634917 fixinventoryworker-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-26 20:23:17.634917 fixinventoryworker-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:23:17.634917 fixinventoryworker-4.0.5/fixinventoryworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-26 20:23:17.000000 fixinventoryworker-4.0.5/fixinventoryworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-26 20:23:17.000000 fixinventoryworker-4.0.5/fixinventoryworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:23:17.000000 fixinventoryworker-4.0.5/fixinventoryworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-26 20:23:17.000000 fixinventoryworker-4.0.5/fixinventoryworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:20:18.000000 fixinventoryworker-4.0.5/fixinventoryworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 20:23:17.000000 fixinventoryworker-4.0.5/fixinventoryworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 20:23:17.000000 fixinventoryworker-4.0.5/fixinventoryworker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:23:17.630917 fixinventoryworker-4.0.5/fixworker/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/fixworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13357 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/fixworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/fixworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/fixworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/fixworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/fixworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/fixworker/fixcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/fixworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/fixworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/fixworker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 20:23:17.634917 fixinventoryworker-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:23:17.634917 fixinventoryworker-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/test/test_fixcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-26 20:19:08.000000 fixinventoryworker-4.0.5/test/test_utils.py
```

### Comparing `fixinventoryworker-4.0.4/PKG-INFO` & `fixinventoryworker-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fixinventoryworker
-Version: 4.0.4
+Version: 4.0.5
 Summary: Runs collector plugins and sends the result to fixcore.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: tenacity
 Requires-Dist: CherryPy
 
 # `fixworker`
 Fix worker daemon
```

### Comparing `fixinventoryworker-4.0.4/README.md` & `fixinventoryworker-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/fixinventoryworker.egg-info/PKG-INFO` & `fixinventoryworker-4.0.5/fixinventoryworker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fixinventoryworker
-Version: 4.0.4
+Version: 4.0.5
 Summary: Runs collector plugins and sends the result to fixcore.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: tenacity
 Requires-Dist: CherryPy
 
 # `fixworker`
 Fix worker daemon
```

### Comparing `fixinventoryworker-4.0.4/fixinventoryworker.egg-info/SOURCES.txt` & `fixinventoryworker-4.0.5/fixinventoryworker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/fixworker/__main__.py` & `fixinventoryworker-4.0.5/fixworker/__main__.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/fixworker/cleanup.py` & `fixinventoryworker-4.0.5/fixworker/cleanup.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/fixworker/collect.py` & `fixinventoryworker-4.0.5/fixworker/collect.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/fixworker/config.py` & `fixinventoryworker-4.0.5/fixworker/config.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/fixworker/fixcore.py` & `fixinventoryworker-4.0.5/fixworker/fixcore.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/fixworker/pluginloader.py` & `fixinventoryworker-4.0.5/fixworker/pluginloader.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/fixworker/tag.py` & `fixinventoryworker-4.0.5/fixworker/tag.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/fixworker/utils.py` & `fixinventoryworker-4.0.5/fixworker/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/pyproject.toml` & `fixinventoryworker-4.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "fixinventoryworker"
-version = "4.0.4"
+version = "4.0.5"
 authors = [{ name = "Some Engineering Inc." }]
 description = "Runs collector plugins and sends the result to fixcore."
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = ["Programming Language :: Python :: 3"]
 readme = { file = "README.md", content-type = "text/markdown" }
 
 dependencies = [
-    "fixinventorylib==4.0.4",
+    "fixinventorylib==4.0.5",
     "tenacity",
     "CherryPy",
 ]
 
 [project.scripts]
 fixworker = "fixworker.__main__:main"
 resotoworker = "fixworker.__main__:main"
```

### Comparing `fixinventoryworker-4.0.4/test/test_args.py` & `fixinventoryworker-4.0.5/test/test_args.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/test/test_collect.py` & `fixinventoryworker-4.0.5/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/test/test_fixcore.py` & `fixinventoryworker-4.0.5/test/test_fixcore.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.4/test/test_utils.py` & `fixinventoryworker-4.0.5/test/test_utils.py`

 * *Files identical despite different names*

