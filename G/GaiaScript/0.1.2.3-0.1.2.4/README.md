# Comparing `tmp/GaiaScript-0.1.2.3.tar.gz` & `tmp/GaiaScript-0.1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GaiaScript-0.1.2.3.tar", last modified: Fri Apr 26 08:31:47 2024, max compression
+gzip compressed data, was "GaiaScript-0.1.2.4.tar", last modified: Fri Apr 26 08:33:06 2024, max compression
```

## Comparing `GaiaScript-0.1.2.3.tar` & `GaiaScript-0.1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:31:47.371835 GaiaScript-0.1.2.3/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:31:47.371835 GaiaScript-0.1.2.3/GaiaScript.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 08:31:47.000000 GaiaScript-0.1.2.3/GaiaScript.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      248 2024-04-26 08:31:47.000000 GaiaScript-0.1.2.3/GaiaScript.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 08:31:47.000000 GaiaScript-0.1.2.3/GaiaScript.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 08:31:47.000000 GaiaScript-0.1.2.3/GaiaScript.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 08:31:47.371835 GaiaScript-0.1.2.3/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.2.3/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:31:47.371835 GaiaScript-0.1.2.3/gaia/
--rw-rw-r--   0 mark      (1000) mark      (1000)      733 2024-04-26 08:28:57.000000 GaiaScript-0.1.2.3/gaia/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3186 2024-04-26 08:31:37.000000 GaiaScript-0.1.2.3/gaia/_debug.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      816 2024-04-26 08:21:37.000000 GaiaScript-0.1.2.3/gaia/_exceptions.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2826 2024-04-26 08:21:37.000000 GaiaScript-0.1.2.3/gaia/_template.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 08:31:47.371835 GaiaScript-0.1.2.3/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      658 2024-04-26 08:31:45.000000 GaiaScript-0.1.2.3/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:31:47.371835 GaiaScript-0.1.2.3/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.2.3/tests/test__template.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:33:06.645450 GaiaScript-0.1.2.4/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:33:06.645450 GaiaScript-0.1.2.4/GaiaScript.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 08:33:06.000000 GaiaScript-0.1.2.4/GaiaScript.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      248 2024-04-26 08:33:06.000000 GaiaScript-0.1.2.4/GaiaScript.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 08:33:06.000000 GaiaScript-0.1.2.4/GaiaScript.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 08:33:06.000000 GaiaScript-0.1.2.4/GaiaScript.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 08:33:06.645450 GaiaScript-0.1.2.4/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.2.4/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:33:06.645450 GaiaScript-0.1.2.4/gaia/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      733 2024-04-26 08:28:57.000000 GaiaScript-0.1.2.4/gaia/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3194 2024-04-26 08:33:05.000000 GaiaScript-0.1.2.4/gaia/_debug.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      816 2024-04-26 08:21:37.000000 GaiaScript-0.1.2.4/gaia/_exceptions.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2826 2024-04-26 08:21:37.000000 GaiaScript-0.1.2.4/gaia/_template.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 08:33:06.645450 GaiaScript-0.1.2.4/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      658 2024-04-26 08:33:05.000000 GaiaScript-0.1.2.4/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:33:06.645450 GaiaScript-0.1.2.4/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.2.4/tests/test__template.py
```

### Comparing `GaiaScript-0.1.2.3/gaia/__init__.py` & `GaiaScript-0.1.2.4/gaia/__init__.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.2.3/gaia/_debug.py` & `GaiaScript-0.1.2.4/gaia/_debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os.path
 
 from gaia._exceptions import DebugScriptNotFoundException, \
     DebugScriptAlreadyExistsException
-from . import get_template_script_manager
 
 
 class DebugScriptManager:
 
     @staticmethod
     def check_debug_script_exists(func):
         def wrapper(self, *args, **kwargs):
@@ -38,14 +37,15 @@
         return self.__save_debug_script(debug_script_name, content)
 
     def create_debug_script_from_template(
             self, debug_script_name, template_name, replace_dict: dict[str, str] = None
     ):
         if self.__is_debug_script_exists(debug_script_name):
             raise DebugScriptAlreadyExistsException(debug_script_name)
+        from . import get_template_script_manager
         if replace_dict:
             content = get_template_script_manager().get_replaced_template_content(
                 template_name, replace_dict
             )
         else:
             content = get_template_script_manager().get_template_content(template_name)
         return self.__save_debug_script(debug_script_name, content)
```

### Comparing `GaiaScript-0.1.2.3/gaia/_exceptions.py` & `GaiaScript-0.1.2.4/gaia/_exceptions.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.2.3/gaia/_template.py` & `GaiaScript-0.1.2.4/gaia/_template.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.2.3/setup.py` & `GaiaScript-0.1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name='GaiaScript',
-    version='0.1.2.3',
+    version='0.1.2.4',
     author='369',
     author_email='luck.yangbo@gmail.com',
     long_description=read_readme(),
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `GaiaScript-0.1.2.3/tests/test__template.py` & `GaiaScript-0.1.2.4/tests/test__template.py`

 * *Files identical despite different names*

