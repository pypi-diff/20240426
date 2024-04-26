# Comparing `tmp/yamlscript-0.1.57.tar.gz` & `tmp/yamlscript-0.1.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamlscript-0.1.57.tar", last modified: Mon Apr 22 17:56:48 2024, max compression
+gzip compressed data, was "yamlscript-0.1.58.tar", last modified: Fri Apr 26 11:24:07 2024, max compression
```

## Comparing `yamlscript-0.1.57.tar` & `yamlscript-0.1.58.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-22 17:56:48.738556 yamlscript-0.1.57/
--rw-r--r--   0 ingy      (1000) ingy      (1000)        0 2024-04-22 17:56:48.000000 yamlscript-0.1.57/.long_description.md
--rw-r--r--   0 ingy      (1000) ingy      (1000)       47 2024-04-22 17:56:48.000000 yamlscript-0.1.57/MANIFEST.in
--rw-r--r--   0 ingy      (1000) ingy      (1000)      757 2024-04-22 17:56:48.738556 yamlscript-0.1.57/PKG-INFO
--rw-r--r--   0 ingy      (1000) ingy      (1000)     3082 2024-04-15 14:33:02.000000 yamlscript-0.1.57/ReadMe.md
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-22 17:56:48.738556 yamlscript-0.1.57/lib/
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-22 17:56:48.738556 yamlscript-0.1.57/lib/yamlscript/
--rw-r--r--   0 ingy      (1000) ingy      (1000)     4365 2024-04-22 17:39:33.000000 yamlscript-0.1.57/lib/yamlscript/__init__.py
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-22 17:56:48.738556 yamlscript-0.1.57/lib/yamlscript.egg-info/
--rw-r--r--   0 ingy      (1000) ingy      (1000)      757 2024-04-22 17:56:48.000000 yamlscript-0.1.57/lib/yamlscript.egg-info/PKG-INFO
--rw-r--r--   0 ingy      (1000) ingy      (1000)      290 2024-04-22 17:56:48.000000 yamlscript-0.1.57/lib/yamlscript.egg-info/SOURCES.txt
--rw-r--r--   0 ingy      (1000) ingy      (1000)        1 2024-04-22 17:56:48.000000 yamlscript-0.1.57/lib/yamlscript.egg-info/dependency_links.txt
--rw-r--r--   0 ingy      (1000) ingy      (1000)        7 2024-04-22 17:56:48.000000 yamlscript-0.1.57/lib/yamlscript.egg-info/requires.txt
--rw-r--r--   0 ingy      (1000) ingy      (1000)       11 2024-04-22 17:56:48.000000 yamlscript-0.1.57/lib/yamlscript.egg-info/top_level.txt
--rw-rw-r--   0 ingy      (1000) ingy      (1000)       79 2024-04-22 17:56:48.738556 yamlscript-0.1.57/setup.cfg
--rw-r--r--   0 ingy      (1000) ingy      (1000)     1146 2024-04-22 17:39:33.000000 yamlscript-0.1.57/setup.py
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-22 17:56:48.738556 yamlscript-0.1.57/test/
--rw-rw-r--   0 ingy      (1000) ingy      (1000)      144 2024-03-28 18:44:00.000000 yamlscript-0.1.57/test/test.py
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-26 11:24:07.815644 yamlscript-0.1.58/
+-rw-r--r--   0 ingy      (1000) ingy      (1000)        0 2024-04-26 11:24:07.000000 yamlscript-0.1.58/.long_description.md
+-rw-r--r--   0 ingy      (1000) ingy      (1000)       47 2024-04-26 11:24:07.000000 yamlscript-0.1.58/MANIFEST.in
+-rw-r--r--   0 ingy      (1000) ingy      (1000)      757 2024-04-26 11:24:07.815644 yamlscript-0.1.58/PKG-INFO
+-rw-r--r--   0 ingy      (1000) ingy      (1000)     3082 2024-04-15 14:33:02.000000 yamlscript-0.1.58/ReadMe.md
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-26 11:24:07.815644 yamlscript-0.1.58/lib/
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-26 11:24:07.815644 yamlscript-0.1.58/lib/yamlscript/
+-rw-r--r--   0 ingy      (1000) ingy      (1000)     4365 2024-04-26 10:57:22.000000 yamlscript-0.1.58/lib/yamlscript/__init__.py
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-26 11:24:07.815644 yamlscript-0.1.58/lib/yamlscript.egg-info/
+-rw-r--r--   0 ingy      (1000) ingy      (1000)      757 2024-04-26 11:24:07.000000 yamlscript-0.1.58/lib/yamlscript.egg-info/PKG-INFO
+-rw-r--r--   0 ingy      (1000) ingy      (1000)      290 2024-04-26 11:24:07.000000 yamlscript-0.1.58/lib/yamlscript.egg-info/SOURCES.txt
+-rw-r--r--   0 ingy      (1000) ingy      (1000)        1 2024-04-26 11:24:07.000000 yamlscript-0.1.58/lib/yamlscript.egg-info/dependency_links.txt
+-rw-r--r--   0 ingy      (1000) ingy      (1000)        7 2024-04-26 11:24:07.000000 yamlscript-0.1.58/lib/yamlscript.egg-info/requires.txt
+-rw-r--r--   0 ingy      (1000) ingy      (1000)       11 2024-04-26 11:24:07.000000 yamlscript-0.1.58/lib/yamlscript.egg-info/top_level.txt
+-rw-rw-r--   0 ingy      (1000) ingy      (1000)       79 2024-04-26 11:24:07.815644 yamlscript-0.1.58/setup.cfg
+-rw-r--r--   0 ingy      (1000) ingy      (1000)     1146 2024-04-26 10:57:22.000000 yamlscript-0.1.58/setup.py
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-26 11:24:07.815644 yamlscript-0.1.58/test/
+-rw-rw-r--   0 ingy      (1000) ingy      (1000)      144 2024-03-28 18:44:00.000000 yamlscript-0.1.58/test/test.py
```

### Comparing `yamlscript-0.1.57/PKG-INFO` & `yamlscript-0.1.58/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlscript
-Version: 0.1.57
+Version: 0.1.58
 Summary: Program in YAML
 Home-page: https://github.com/ingydotnet/yamlscript
 Author: Ingy döt Net
 Author-email: ingy@ingy.net
 License: MIT
 Keywords: yaml,language
 Platform: UNKNOWN
```

### Comparing `yamlscript-0.1.57/ReadMe.md` & `yamlscript-0.1.58/ReadMe.md`

 * *Files identical despite different names*

### Comparing `yamlscript-0.1.57/lib/yamlscript/__init__.py` & `yamlscript-0.1.58/lib/yamlscript/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 The load() method takes a YAMLScript string as input and returns the Python
 object that the YAMLScript code evaluates to.
 """
 
 # This value is automatically updated by 'make bump'.
 # The version number is used to find the correct shared library file.
 # We currently only support binding to an exact version of libyamlscript.
-yamlscript_version = '0.1.57'
+yamlscript_version = '0.1.58'
 
 import os, sys
 import ctypes
 import json
 
 # Require Python 3.6 or greater:
 assert sys.version_info >= (3, 6), \
```

### Comparing `yamlscript-0.1.57/lib/yamlscript.egg-info/PKG-INFO` & `yamlscript-0.1.58/lib/yamlscript.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlscript
-Version: 0.1.57
+Version: 0.1.58
 Summary: Program in YAML
 Home-page: https://github.com/ingydotnet/yamlscript
 Author: Ingy döt Net
 Author-email: ingy@ingy.net
 License: MIT
 Keywords: yaml,language
 Platform: UNKNOWN
```

### Comparing `yamlscript-0.1.57/setup.py` & `yamlscript-0.1.58/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version = '0.1.57'
+version = '0.1.58'
 
 from setuptools import setup
 import pathlib
 
 root = pathlib.Path(__file__).parent.resolve()
 
 long_description = \
```

