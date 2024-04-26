# Comparing `tmp/fixinventoryshell-4.0.4.tar.gz` & `tmp/fixinventoryshell-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventoryshell-4.0.4.tar", last modified: Wed Apr 24 19:35:17 2024, max compression
+gzip compressed data, was "fixinventoryshell-4.0.5.tar", last modified: Fri Apr 26 20:22:07 2024, max compression
```

## Comparing `fixinventoryshell-4.0.4.tar` & `fixinventoryshell-4.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:35:17.408051 fixinventoryshell-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-24 19:35:17.408051 fixinventoryshell-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:35:17.408051 fixinventoryshell-4.0.4/fixinventoryshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-24 19:35:17.000000 fixinventoryshell-4.0.4/fixinventoryshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-24 19:35:17.000000 fixinventoryshell-4.0.4/fixinventoryshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:35:17.000000 fixinventoryshell-4.0.4/fixinventoryshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 19:35:17.000000 fixinventoryshell-4.0.4/fixinventoryshell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:32:36.000000 fixinventoryshell-4.0.4/fixinventoryshell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 19:35:17.000000 fixinventoryshell-4.0.4/fixinventoryshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 19:35:17.000000 fixinventoryshell-4.0.4/fixinventoryshell.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:35:17.408051 fixinventoryshell-4.0.4/fixshell/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/fixshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/fixshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/fixshell/authorized_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    38726 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/fixshell/promptsession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/fixshell/protected_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/fixshell/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 19:35:17.408051 fixinventoryshell-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:35:17.408051 fixinventoryshell-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/test/test_promptsession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-24 19:31:34.000000 fixinventoryshell-4.0.4/test/test_protected_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:07.271144 fixinventoryshell-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-26 20:22:07.271144 fixinventoryshell-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:07.271144 fixinventoryshell-4.0.5/fixinventoryshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-26 20:22:07.000000 fixinventoryshell-4.0.5/fixinventoryshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-26 20:22:07.000000 fixinventoryshell-4.0.5/fixinventoryshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:22:07.000000 fixinventoryshell-4.0.5/fixinventoryshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 20:22:07.000000 fixinventoryshell-4.0.5/fixinventoryshell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:19:18.000000 fixinventoryshell-4.0.5/fixinventoryshell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-26 20:22:07.000000 fixinventoryshell-4.0.5/fixinventoryshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 20:22:07.000000 fixinventoryshell-4.0.5/fixinventoryshell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:07.267144 fixinventoryshell-4.0.5/fixshell/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/fixshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/fixshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/fixshell/authorized_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38726 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/fixshell/promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/fixshell/protected_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/fixshell/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-26 20:22:07.271144 fixinventoryshell-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:22:07.271144 fixinventoryshell-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/test/test_promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-26 20:18:09.000000 fixinventoryshell-4.0.5/test/test_protected_files.py
```

### Comparing `fixinventoryshell-4.0.4/PKG-INFO` & `fixinventoryshell-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventoryshell
-Version: 4.0.4
+Version: 4.0.5
 Summary: Commandline interpreter to interact with Fix Inventory.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixshell
 Keywords: cloud security
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: prompt-toolkit
 Requires-Dist: rich
 Requires-Dist: fixinventoryclient
 Requires-Dist: aiohttp[speedups]
 
 # `resh`
 Fix Shell
```

### Comparing `fixinventoryshell-4.0.4/README.md` & `fixinventoryshell-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.4/fixinventoryshell.egg-info/PKG-INFO` & `fixinventoryshell-4.0.5/fixinventoryshell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventoryshell
-Version: 4.0.4
+Version: 4.0.5
 Summary: Commandline interpreter to interact with Fix Inventory.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixshell
 Keywords: cloud security
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: prompt-toolkit
 Requires-Dist: rich
 Requires-Dist: fixinventoryclient
 Requires-Dist: aiohttp[speedups]
 
 # `resh`
 Fix Shell
```

### Comparing `fixinventoryshell-4.0.4/fixinventoryshell.egg-info/SOURCES.txt` & `fixinventoryshell-4.0.5/fixinventoryshell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.4/fixshell/__main__.py` & `fixinventoryshell-4.0.5/fixshell/__main__.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.4/fixshell/authorized_client.py` & `fixinventoryshell-4.0.5/fixshell/authorized_client.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.4/fixshell/promptsession.py` & `fixinventoryshell-4.0.5/fixshell/promptsession.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.4/fixshell/protected_files.py` & `fixinventoryshell-4.0.5/fixshell/protected_files.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.4/fixshell/shell.py` & `fixinventoryshell-4.0.5/fixshell/shell.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.4/pyproject.toml` & `fixinventoryshell-4.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixinventoryshell"
-version = "4.0.4"
+version = "4.0.5"
 authors = [{name="Some Engineering Inc."}]
 description = "Commandline interpreter to interact with Fix Inventory."
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 5 - Production/Stable",
@@ -24,15 +24,15 @@
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 keywords = ["cloud security"]
 
 dependencies = [
-    "fixinventorylib==4.0.4",
+    "fixinventorylib==4.0.5",
     "prompt-toolkit",
     "rich",
     "fixinventoryclient",
     "aiohttp[speedups]",
 ]
 
 [project.scripts]
```

### Comparing `fixinventoryshell-4.0.4/test/test_promptsession.py` & `fixinventoryshell-4.0.5/test/test_promptsession.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.4/test/test_protected_files.py` & `fixinventoryshell-4.0.5/test/test_protected_files.py`

 * *Files identical despite different names*

