# Comparing `tmp/GaiaScript-0.1.1.5.tar.gz` & `tmp/GaiaScript-0.1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GaiaScript-0.1.1.5.tar", last modified: Fri Apr 26 06:50:18 2024, max compression
+gzip compressed data, was "GaiaScript-0.1.1.6.tar", last modified: Fri Apr 26 07:00:21 2024, max compression
```

## Comparing `GaiaScript-0.1.1.5.tar` & `GaiaScript-0.1.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:50:18.075823 GaiaScript-0.1.1.5/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:50:18.075823 GaiaScript-0.1.1.5/GaiaScript.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 06:50:18.000000 GaiaScript-0.1.1.5/GaiaScript.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      233 2024-04-26 06:50:18.000000 GaiaScript-0.1.1.5/GaiaScript.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 06:50:18.000000 GaiaScript-0.1.1.5/GaiaScript.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 06:50:18.000000 GaiaScript-0.1.1.5/GaiaScript.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 06:50:18.075823 GaiaScript-0.1.1.5/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.1.5/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:50:18.075823 GaiaScript-0.1.1.5/gaia/
--rw-rw-r--   0 mark      (1000) mark      (1000)      544 2024-04-26 06:10:01.000000 GaiaScript-0.1.1.5/gaia/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      306 2024-04-26 02:08:44.000000 GaiaScript-0.1.1.5/gaia/_exceptions.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2428 2024-04-26 06:50:16.000000 GaiaScript-0.1.1.5/gaia/_template.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 06:50:18.075823 GaiaScript-0.1.1.5/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      658 2024-04-26 06:50:16.000000 GaiaScript-0.1.1.5/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:50:18.075823 GaiaScript-0.1.1.5/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.1.5/tests/test__template.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/GaiaScript.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 07:00:21.000000 GaiaScript-0.1.1.6/GaiaScript.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      233 2024-04-26 07:00:21.000000 GaiaScript-0.1.1.6/GaiaScript.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 07:00:21.000000 GaiaScript-0.1.1.6/GaiaScript.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 07:00:21.000000 GaiaScript-0.1.1.6/GaiaScript.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.1.6/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/gaia/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      544 2024-04-26 06:10:01.000000 GaiaScript-0.1.1.6/gaia/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      306 2024-04-26 02:08:44.000000 GaiaScript-0.1.1.6/gaia/_exceptions.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2305 2024-04-26 07:00:17.000000 GaiaScript-0.1.1.6/gaia/_template.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      658 2024-04-26 07:00:17.000000 GaiaScript-0.1.1.6/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 07:00:21.494793 GaiaScript-0.1.1.6/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.1.6/tests/test__template.py
```

### Comparing `GaiaScript-0.1.1.5/gaia/__init__.py` & `GaiaScript-0.1.1.6/gaia/__init__.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.1.5/gaia/_template.py` & `GaiaScript-0.1.1.6/gaia/_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import typing
 
 from gaia._exceptions import TemplateNotFoundException, TemplateAlreadyExistsException
 
 
 class TemplateManager:
     @staticmethod
     def check_template_exists(func):
@@ -22,43 +21,38 @@
         return os.listdir(self.template_dir)
 
     def __is_template_exists(self, template_name) -> bool:
         return os.path.exists(
             os.path.join(self.template_dir, template_name)
         )
 
-    def create_template(
-            self, template_name: str, content: str = None, file_path: str = None,
-            file_io: typing.IO = None
-    ) -> str:
+    @staticmethod
+    def __is_file_exists(file_path) -> bool:
+        return os.path.exists(file_path)
+
+    def create_template(self, template_name: str, content: str | bytes) -> str:
         if self.__is_template_exists(template_name):
             raise TemplateAlreadyExistsException(template_name)
-        if file_path:
-            with open(file_path, 'r') as f:
-                content = f.read()
-        elif file_io:
-            content = file_io.read()
-
-        if isinstance(content, bytes):
-            content = content.decode('utf-8')
         return self.__save_template(template_name, content)
 
     @check_template_exists
     def get_template_content(self, template_name) -> str:
         template_path = os.path.join(self.template_dir, template_name)
         with open(template_path, 'r') as f:
             return f.read()
 
     @check_template_exists
-    def update_template(self, template_name, content) -> str:
+    def update_template(self, template_name, content: str | bytes) -> str:
         self.delete_template(template_name)
         return self.__save_template(template_name, content)
 
-    def __save_template(self, template_name, content) -> str:
+    def __save_template(self, template_name, content: str | bytes) -> str:
         template_path = os.path.join(self.template_dir, template_name)
+        if isinstance(content, bytes):
+            content = content.decode('utf-8')
         with open(template_path, 'w') as f:
             f.write(content)
         return str(template_path)
 
     @check_template_exists
     def delete_template(self, template_name) -> list[str]:
         template_path = os.path.join(self.template_dir, template_name)
```

### Comparing `GaiaScript-0.1.1.5/setup.py` & `GaiaScript-0.1.1.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name='GaiaScript',
-    version='0.1.1.5',
+    version='0.1.1.6',
     author='369',
     author_email='luck.yangbo@gmail.com',
     long_description=read_readme(),
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `GaiaScript-0.1.1.5/tests/test__template.py` & `GaiaScript-0.1.1.6/tests/test__template.py`

 * *Files identical despite different names*

