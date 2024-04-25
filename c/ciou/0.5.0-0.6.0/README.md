# Comparing `tmp/ciou-0.5.0.tar.gz` & `tmp/ciou-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciou-0.5.0.tar", last modified: Wed Apr 24 22:13:24 2024, max compression
+gzip compressed data, was "ciou-0.6.0.tar", last modified: Thu Apr 25 22:50:47 2024, max compression
```

## Comparing `ciou-0.5.0.tar` & `ciou-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:13:24.098395 ciou-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 22:13:20.000000 ciou-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-24 22:13:24.098395 ciou-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-24 22:13:20.000000 ciou-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:13:24.094395 ciou-0.5.0/ciou/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:13:24.098395 ciou-0.5.0/ciou/color/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/color/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/color/_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/color/_dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:13:24.098395 ciou-0.5.0/ciou/progress/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/progress/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/progress/_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/progress/_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/progress/_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:13:24.098395 ciou-0.5.0/ciou/snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/snapshot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:13:24.098395 ciou-0.5.0/ciou/terminal/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/terminal/_windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:13:24.098395 ciou-0.5.0/ciou/time/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/time/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/time/_ticker.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/time/_timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:13:24.098395 ciou-0.5.0/ciou/types/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-24 22:13:20.000000 ciou-0.5.0/ciou/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:13:24.098395 ciou-0.5.0/ciou.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-24 22:13:24.000000 ciou-0.5.0/ciou.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-24 22:13:24.000000 ciou-0.5.0/ciou.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:13:24.000000 ciou-0.5.0/ciou.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 22:13:24.000000 ciou-0.5.0/ciou.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-24 22:13:20.000000 ciou-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:13:24.102395 ciou-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:50:47.738286 ciou-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 22:50:44.000000 ciou-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-25 22:50:47.738286 ciou-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-25 22:50:44.000000 ciou-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:50:47.734286 ciou-0.6.0/ciou/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:50:47.734286 ciou-0.6.0/ciou/color/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/color/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/color/_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/color/_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:50:47.738286 ciou-0.6.0/ciou/progress/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/progress/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/progress/_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/progress/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/progress/_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:50:47.738286 ciou-0.6.0/ciou/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/snapshot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:50:47.738286 ciou-0.6.0/ciou/terminal/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/terminal/_windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:50:47.738286 ciou-0.6.0/ciou/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/time/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/time/_ticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/time/_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:50:47.738286 ciou-0.6.0/ciou/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 22:50:44.000000 ciou-0.6.0/ciou/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:50:47.738286 ciou-0.6.0/ciou.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-25 22:50:47.000000 ciou-0.6.0/ciou.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-25 22:50:47.000000 ciou-0.6.0/ciou.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 22:50:47.000000 ciou-0.6.0/ciou.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 22:50:47.000000 ciou-0.6.0/ciou.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-25 22:50:44.000000 ciou-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 22:50:47.738286 ciou-0.6.0/setup.cfg
```

### Comparing `ciou-0.5.0/LICENSE` & `ciou-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ciou-0.5.0/PKG-INFO` & `ciou-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciou
-Version: 0.5.0
+Version: 0.6.0
 Summary: CLI input and output utils.
 Author: Toni Kangas
 License: MIT License
         
         Copyright (c) 2024 Toni Kangas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ciou-0.5.0/README.md` & `ciou-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ciou-0.5.0/ciou/color/__init__.py` & `ciou-0.6.0/ciou/color/__init__.py`

 * *Files identical despite different names*

### Comparing `ciou-0.5.0/ciou/color/_color.py` & `ciou-0.6.0/ciou/color/_color.py`

 * *Files identical despite different names*

### Comparing `ciou-0.5.0/ciou/progress/_config.py` & `ciou-0.6.0/ciou/progress/_config.py`

 * *Files identical despite different names*

### Comparing `ciou-0.5.0/ciou/progress/_message.py` & `ciou-0.6.0/ciou/progress/_message.py`

 * *Files identical despite different names*

### Comparing `ciou-0.5.0/ciou/progress/_progress.py` & `ciou-0.6.0/ciou/progress/_progress.py`

 * *Files identical despite different names*

### Comparing `ciou-0.5.0/ciou/progress/_renderer.py` & `ciou-0.6.0/ciou/progress/_renderer.py`

 * *Files identical despite different names*

### Comparing `ciou-0.5.0/ciou/snapshot/__init__.py` & `ciou-0.6.0/ciou/snapshot/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''Test utilities for validating output using snapshot files.
 '''
 
 import inspect
 from io import IOBase
-from os import getenv, makedirs, path
+import os
 import re
 from typing import List, Pattern, Tuple, Union
 
 
 from ciou.types import ensure_list
 
 
@@ -16,14 +16,17 @@
 
     See `snapshot` documentation for example usage.
     '''
     f.seek(0)
     return f.read()
 
 
+REPLACE_CWD = (re.escape(os.getcwd()), '<CWD>')
+'''Replace tuple for `snapshot` to remove dynamic durations from snapshots.
+For example, `0.673 ms` → `<DURATION>`'''
 REPLACE_DURATION = (r'[0-9]+\.[0-9]+.*s', '<DURATION>')
 '''Replace tuple for `snapshot` to remove dynamic durations from snapshots.
 For example, `0.673 ms` → `<DURATION>`'''
 REPLACE_TIMESTAMP = (
     r'[0-9]{4}-[0-9]{2}-[0-9]{2}T[0-9]{2}:[0-9]{2}:[0-9]{2}.[0-9]+Z',
     '<TIMESTAMP>')
 '''Replace tuple for `snapshot` to remove timestamps created with
@@ -73,25 +76,25 @@
         testfile = inspect.getsourcefile(inspect.stack()[1].frame)
 
     replaces = ensure_list(replace)
     for r in replaces:
         pattern, repl = r
         value = re.sub(pattern, repl, value)
 
-    filepath = path.join(
-        path.dirname(testfile),
+    filepath = os.path.join(
+        os.path.dirname(testfile),
         directory_name,
         f'{key}.snapshot')
 
     try:
         with open(filepath, "r") as f:
             prev = f.read()
     except FileNotFoundError:
         prev = None
 
-    if getenv("UPDATE_SNAPSHOTS") or prev is None:
-        makedirs(path.dirname(filepath), exist_ok=True)
+    if os.getenv("UPDATE_SNAPSHOTS") or prev is None:
+        os.makedirs(os.path.dirname(filepath), exist_ok=True)
         with open(filepath, "w+") as f:
             f.write(value)
             return value, value
 
     return prev, value
```

### Comparing `ciou-0.5.0/ciou/time/_ticker.py` & `ciou-0.6.0/ciou/time/_ticker.py`

 * *Files identical despite different names*

### Comparing `ciou-0.5.0/ciou/types/__init__.py` & `ciou-0.6.0/ciou/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ciou-0.5.0/ciou.egg-info/PKG-INFO` & `ciou-0.6.0/ciou.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciou
-Version: 0.5.0
+Version: 0.6.0
 Summary: CLI input and output utils.
 Author: Toni Kangas
 License: MIT License
         
         Copyright (c) 2024 Toni Kangas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ciou-0.5.0/ciou.egg-info/SOURCES.txt` & `ciou-0.6.0/ciou.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ciou-0.5.0/pyproject.toml` & `ciou-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ciou"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
     {name = "Toni Kangas"},
 ]
 description = "CLI input and output utils."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
```

