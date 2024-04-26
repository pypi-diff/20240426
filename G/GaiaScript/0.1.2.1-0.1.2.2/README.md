# Comparing `tmp/GaiaScript-0.1.2.1.tar.gz` & `tmp/GaiaScript-0.1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GaiaScript-0.1.2.1.tar", last modified: Fri Apr 26 08:25:46 2024, max compression
+gzip compressed data, was "GaiaScript-0.1.2.2.tar", last modified: Fri Apr 26 08:28:58 2024, max compression
```

## Comparing `GaiaScript-0.1.2.1.tar` & `GaiaScript-0.1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:25:46.528495 GaiaScript-0.1.2.1/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:25:46.528495 GaiaScript-0.1.2.1/GaiaScript.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 08:25:46.000000 GaiaScript-0.1.2.1/GaiaScript.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      248 2024-04-26 08:25:46.000000 GaiaScript-0.1.2.1/GaiaScript.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 08:25:46.000000 GaiaScript-0.1.2.1/GaiaScript.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 08:25:46.000000 GaiaScript-0.1.2.1/GaiaScript.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 08:25:46.528495 GaiaScript-0.1.2.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.2.1/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:25:46.528495 GaiaScript-0.1.2.1/gaia/
--rw-rw-r--   0 mark      (1000) mark      (1000)      729 2024-04-26 08:25:44.000000 GaiaScript-0.1.2.1/gaia/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3161 2024-04-26 08:21:37.000000 GaiaScript-0.1.2.1/gaia/_debug.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      816 2024-04-26 08:21:37.000000 GaiaScript-0.1.2.1/gaia/_exceptions.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2826 2024-04-26 08:21:37.000000 GaiaScript-0.1.2.1/gaia/_template.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 08:25:46.528495 GaiaScript-0.1.2.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      658 2024-04-26 08:25:44.000000 GaiaScript-0.1.2.1/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:25:46.528495 GaiaScript-0.1.2.1/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.2.1/tests/test__template.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:28:58.408395 GaiaScript-0.1.2.2/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:28:58.408395 GaiaScript-0.1.2.2/GaiaScript.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 08:28:58.000000 GaiaScript-0.1.2.2/GaiaScript.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      248 2024-04-26 08:28:58.000000 GaiaScript-0.1.2.2/GaiaScript.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 08:28:58.000000 GaiaScript-0.1.2.2/GaiaScript.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 08:28:58.000000 GaiaScript-0.1.2.2/GaiaScript.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 08:28:58.408395 GaiaScript-0.1.2.2/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.2.2/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:28:58.408395 GaiaScript-0.1.2.2/gaia/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      733 2024-04-26 08:28:57.000000 GaiaScript-0.1.2.2/gaia/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3189 2024-04-26 08:28:57.000000 GaiaScript-0.1.2.2/gaia/_debug.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      816 2024-04-26 08:21:37.000000 GaiaScript-0.1.2.2/gaia/_exceptions.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2826 2024-04-26 08:21:37.000000 GaiaScript-0.1.2.2/gaia/_template.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 08:28:58.408395 GaiaScript-0.1.2.2/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      654 2024-04-26 08:28:57.000000 GaiaScript-0.1.2.2/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:28:58.408395 GaiaScript-0.1.2.2/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.2.2/tests/test__template.py
```

### Comparing `GaiaScript-0.1.2.1/gaia/__init__.py` & `GaiaScript-0.1.2.2/gaia/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from gaia._template import TemplateManager
-from ._debug import DebugScriptManager
+from gaia._debug import DebugScriptManager
 from ._exceptions import *
 
 SCRIPTS_FOLDER = './scripts/'
 TEMPLATE_SCRIPTS_FOLDER = SCRIPTS_FOLDER + 'template/'
 DEBUG_SCRIPTS_FOLDER = SCRIPTS_FOLDER + 'debug/'
 WORK_SCRIPTS_FOLDER = SCRIPTS_FOLDER + 'work/'
```

### Comparing `GaiaScript-0.1.2.1/gaia/_debug.py` & `GaiaScript-0.1.2.2/gaia/_debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os.path
 
-from gaia import DebugScriptNotFoundException, DebugScriptAlreadyExistsException, \
-    get_template_script_manager
+from gaia._exceptions import DebugScriptNotFoundException, \
+    DebugScriptAlreadyExistsException
+from gaia import get_template_script_manager
 
 
 class DebugScriptManager:
 
     @staticmethod
     def check_debug_script_exists(func):
         def wrapper(self, *args, **kwargs):
```

### Comparing `GaiaScript-0.1.2.1/gaia/_exceptions.py` & `GaiaScript-0.1.2.2/gaia/_exceptions.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.2.1/gaia/_template.py` & `GaiaScript-0.1.2.2/gaia/_template.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.2.1/setup.py` & `GaiaScript-0.1.2.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name='GaiaScript',
-    version='0.1.2.1',
+version='0.1.2.2',
     author='369',
     author_email='luck.yangbo@gmail.com',
     long_description=read_readme(),
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `GaiaScript-0.1.2.1/tests/test__template.py` & `GaiaScript-0.1.2.2/tests/test__template.py`

 * *Files identical despite different names*

