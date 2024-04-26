# Comparing `tmp/GaiaScript-0.1.1.6.tar.gz` & `tmp/GaiaScript-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GaiaScript-0.1.1.6.tar", last modified: Fri Apr 26 07:00:21 2024, max compression
+gzip compressed data, was "GaiaScript-0.1.2.tar", last modified: Fri Apr 26 08:21:45 2024, max compression
```

## Comparing `GaiaScript-0.1.1.6.tar` & `GaiaScript-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/GaiaScript.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 07:00:21.000000 GaiaScript-0.1.1.6/GaiaScript.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      233 2024-04-26 07:00:21.000000 GaiaScript-0.1.1.6/GaiaScript.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 07:00:21.000000 GaiaScript-0.1.1.6/GaiaScript.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 07:00:21.000000 GaiaScript-0.1.1.6/GaiaScript.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.1.6/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/gaia/
--rw-rw-r--   0 mark      (1000) mark      (1000)      544 2024-04-26 06:10:01.000000 GaiaScript-0.1.1.6/gaia/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      306 2024-04-26 02:08:44.000000 GaiaScript-0.1.1.6/gaia/_exceptions.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2305 2024-04-26 07:00:17.000000 GaiaScript-0.1.1.6/gaia/_template.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      658 2024-04-26 07:00:17.000000 GaiaScript-0.1.1.6/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.1.6/tests/test__template.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:21:45.475609 GaiaScript-0.1.2/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:21:45.471608 GaiaScript-0.1.2/GaiaScript.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-26 08:21:45.000000 GaiaScript-0.1.2/GaiaScript.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      248 2024-04-26 08:21:45.000000 GaiaScript-0.1.2/GaiaScript.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 08:21:45.000000 GaiaScript-0.1.2/GaiaScript.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 08:21:45.000000 GaiaScript-0.1.2/GaiaScript.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-26 08:21:45.471608 GaiaScript-0.1.2/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.2/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:21:45.471608 GaiaScript-0.1.2/gaia/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      544 2024-04-26 06:10:01.000000 GaiaScript-0.1.2/gaia/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3161 2024-04-26 08:21:37.000000 GaiaScript-0.1.2/gaia/_debug.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      816 2024-04-26 08:21:37.000000 GaiaScript-0.1.2/gaia/_exceptions.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2826 2024-04-26 08:21:37.000000 GaiaScript-0.1.2/gaia/_template.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 08:21:45.475609 GaiaScript-0.1.2/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      656 2024-04-26 07:52:27.000000 GaiaScript-0.1.2/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 08:21:45.471608 GaiaScript-0.1.2/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.2/tests/test__template.py
```

### Comparing `GaiaScript-0.1.1.6/gaia/__init__.py` & `GaiaScript-0.1.2/gaia/__init__.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.1.6/gaia/_template.py` & `GaiaScript-0.1.2/gaia/_template.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 
-from gaia._exceptions import TemplateNotFoundException, TemplateAlreadyExistsException
+from gaia._exceptions import TemplateNotFoundException, TemplateAlreadyExistsException, \
+    ReplaceDictMustStartWithDollarSignException
 
 
 class TemplateManager:
     @staticmethod
     def check_template_exists(func):
         def wrapper(self, *args, **kwargs):
             if not self.__is_template_exists(args[0]):
@@ -58,7 +59,18 @@
         template_path = os.path.join(self.template_dir, template_name)
         os.remove(template_path)
         return self.get_all_templates()
 
     @check_template_exists
     def get_template_path(self, template_name) -> str:
         return str(os.path.join(self.template_dir, template_name))
+
+    @check_template_exists
+    def get_replaced_template_content(
+            self, template_name, replace_dict: dict[str, str]
+    ) -> str:
+        template_content = self.get_template_content(template_name)
+        for key, value in replace_dict.items():
+            if not key.startswith('$'):
+                raise ReplaceDictMustStartWithDollarSignException(key)
+            template_content = template_content.replace(key, value)
+        return template_content
```

### Comparing `GaiaScript-0.1.1.6/setup.py` & `GaiaScript-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name='GaiaScript',
-    version='0.1.1.6',
+    version='0.1.2',
     author='369',
     author_email='luck.yangbo@gmail.com',
     long_description=read_readme(),
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `GaiaScript-0.1.1.6/tests/test__template.py` & `GaiaScript-0.1.2/tests/test__template.py`

 * *Files identical despite different names*

