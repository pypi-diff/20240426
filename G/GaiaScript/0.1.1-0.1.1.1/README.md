# Comparing `tmp/GaiaScript-0.1.1.tar.gz` & `tmp/GaiaScript-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GaiaScript-0.1.1.tar", last modified: Fri Apr 26 06:10:06 2024, max compression
+gzip compressed data, was "GaiaScript-0.1.1.1.tar", last modified: Fri Apr 26 06:15:18 2024, max compression
```

## Comparing `GaiaScript-0.1.1.tar` & `GaiaScript-0.1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/GaiaScript.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-26 06:10:06.000000 GaiaScript-0.1.1/GaiaScript.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      233 2024-04-26 06:10:06.000000 GaiaScript-0.1.1/GaiaScript.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 06:10:06.000000 GaiaScript-0.1.1/GaiaScript.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 06:10:06.000000 GaiaScript-0.1.1/GaiaScript.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.1/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/gaia/
--rw-rw-r--   0 mark      (1000) mark      (1000)      544 2024-04-26 06:10:01.000000 GaiaScript-0.1.1/gaia/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      306 2024-04-26 02:08:44.000000 GaiaScript-0.1.1/gaia/_exceptions.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2130 2024-04-26 02:08:44.000000 GaiaScript-0.1.1/gaia/_template.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      656 2024-04-26 06:10:01.000000 GaiaScript-0.1.1/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.1/tests/test__template.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:15:18.385839 GaiaScript-0.1.1.1/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:15:18.385839 GaiaScript-0.1.1.1/GaiaScript.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 06:15:18.000000 GaiaScript-0.1.1.1/GaiaScript.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      233 2024-04-26 06:15:18.000000 GaiaScript-0.1.1.1/GaiaScript.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 06:15:18.000000 GaiaScript-0.1.1.1/GaiaScript.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 06:15:18.000000 GaiaScript-0.1.1.1/GaiaScript.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 06:15:18.385839 GaiaScript-0.1.1.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.1.1/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:15:18.385839 GaiaScript-0.1.1.1/gaia/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      544 2024-04-26 06:10:01.000000 GaiaScript-0.1.1.1/gaia/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      306 2024-04-26 02:08:44.000000 GaiaScript-0.1.1.1/gaia/_exceptions.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2053 2024-04-26 06:15:14.000000 GaiaScript-0.1.1.1/gaia/_template.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 06:15:18.385839 GaiaScript-0.1.1.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      658 2024-04-26 06:15:14.000000 GaiaScript-0.1.1.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:15:18.385839 GaiaScript-0.1.1.1/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.1.1/tests/test__template.py
```

### Comparing `GaiaScript-0.1.1/gaia/__init__.py` & `GaiaScript-0.1.1.1/gaia/__init__.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.1/gaia/_template.py` & `GaiaScript-0.1.1.1/gaia/_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import os
 
-from gaia import TEMPLATE_SCRIPTS_FOLDER
-from gaia._exceptions import TemplateNotFoundException, TemplateAlreadyExistsException
+from gaia import TemplateNotFoundException, TemplateAlreadyExistsException
 
 
 class TemplateManager:
     @staticmethod
     def check_template_exists(func):
         def wrapper(self, *args, **kwargs):
             if not self.__is_template_exists(args[0]):
                 raise TemplateNotFoundException(args[0])
             return func(self, *args, **kwargs)
 
         return wrapper
 
-    def __init__(self, template_dir=TEMPLATE_SCRIPTS_FOLDER):
+    def __init__(self, template_dir):
         self.template_dir = template_dir
         os.makedirs(template_dir, exist_ok=True)
 
     def get_all_templates(self) -> list[str]:
         return os.listdir(self.template_dir)
 
     def __is_template_exists(self, template_name) -> bool:
```

### Comparing `GaiaScript-0.1.1/setup.py` & `GaiaScript-0.1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name='GaiaScript',
-    version='0.1.1',
+    version='0.1.1.1',
     author='369',
     author_email='luck.yangbo@gmail.com',
     long_description=read_readme(),
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `GaiaScript-0.1.1/tests/test__template.py` & `GaiaScript-0.1.1.1/tests/test__template.py`

 * *Files identical despite different names*

