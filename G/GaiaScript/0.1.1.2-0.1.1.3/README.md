# Comparing `tmp/GaiaScript-0.1.1.2.tar.gz` & `tmp/GaiaScript-0.1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GaiaScript-0.1.1.2.tar", last modified: Fri Apr 26 06:16:45 2024, max compression
+gzip compressed data, was "GaiaScript-0.1.1.3.tar", last modified: Fri Apr 26 06:31:50 2024, max compression
```

## Comparing `GaiaScript-0.1.1.2.tar` & `GaiaScript-0.1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:16:45.807139 GaiaScript-0.1.1.2/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:16:45.807139 GaiaScript-0.1.1.2/GaiaScript.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 06:16:45.000000 GaiaScript-0.1.1.2/GaiaScript.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      233 2024-04-26 06:16:45.000000 GaiaScript-0.1.1.2/GaiaScript.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 06:16:45.000000 GaiaScript-0.1.1.2/GaiaScript.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 06:16:45.000000 GaiaScript-0.1.1.2/GaiaScript.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 06:16:45.807139 GaiaScript-0.1.1.2/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.1.2/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:16:45.807139 GaiaScript-0.1.1.2/gaia/
--rw-rw-r--   0 mark      (1000) mark      (1000)      544 2024-04-26 06:10:01.000000 GaiaScript-0.1.1.2/gaia/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      306 2024-04-26 02:08:44.000000 GaiaScript-0.1.1.2/gaia/_exceptions.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2065 2024-04-26 06:16:43.000000 GaiaScript-0.1.1.2/gaia/_template.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 06:16:45.807139 GaiaScript-0.1.1.2/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      658 2024-04-26 06:16:43.000000 GaiaScript-0.1.1.2/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:16:45.807139 GaiaScript-0.1.1.2/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.1.2/tests/test__template.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:31:50.102309 GaiaScript-0.1.1.3/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:31:50.102309 GaiaScript-0.1.1.3/GaiaScript.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 06:31:50.000000 GaiaScript-0.1.1.3/GaiaScript.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      233 2024-04-26 06:31:50.000000 GaiaScript-0.1.1.3/GaiaScript.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 06:31:50.000000 GaiaScript-0.1.1.3/GaiaScript.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 06:31:50.000000 GaiaScript-0.1.1.3/GaiaScript.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      358 2024-04-26 06:31:50.102309 GaiaScript-0.1.1.3/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.1.3/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:31:50.102309 GaiaScript-0.1.1.3/gaia/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      544 2024-04-26 06:10:01.000000 GaiaScript-0.1.1.3/gaia/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      306 2024-04-26 02:08:44.000000 GaiaScript-0.1.1.3/gaia/_exceptions.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2044 2024-04-26 06:31:47.000000 GaiaScript-0.1.1.3/gaia/_template.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 06:31:50.102309 GaiaScript-0.1.1.3/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      658 2024-04-26 06:31:47.000000 GaiaScript-0.1.1.3/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:31:50.102309 GaiaScript-0.1.1.3/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.1.3/tests/test__template.py
```

### Comparing `GaiaScript-0.1.1.2/gaia/__init__.py` & `GaiaScript-0.1.1.3/gaia/__init__.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.1.2/gaia/_template.py` & `GaiaScript-0.1.1.3/gaia/_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,29 +24,28 @@
         return os.path.exists(
             os.path.join(self.template_dir, template_name)
         )
 
     def create_template(self, template_name, content) -> str:
         if self.__is_template_exists(template_name):
             raise TemplateAlreadyExistsException(template_name)
-        return self.save_template(template_name, content)
+        return self.__save_template(template_name, content)
 
     @check_template_exists
     def get_template_content(self, template_name) -> str:
         template_path = os.path.join(self.template_dir, template_name)
         with open(template_path, 'r') as f:
             return f.read()
 
     @check_template_exists
     def update_template(self, template_name, content) -> str:
         self.delete_template(template_name)
-        return self.save_template(template_name, content)
+        return self.__save_template(template_name, content)
 
-    @check_template_exists
-    def save_template(self, template_name, content) -> str:
+    def __save_template(self, template_name, content) -> str:
         template_path = os.path.join(self.template_dir, template_name)
         with open(template_path, 'w') as f:
             f.write(content)
         return str(template_path)
 
     def delete_template(self, template_name) -> list[str]:
         template_path = os.path.join(self.template_dir, template_name)
```

### Comparing `GaiaScript-0.1.1.2/setup.py` & `GaiaScript-0.1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name='GaiaScript',
-    version='0.1.1.2',
+    version='0.1.1.3',
     author='369',
     author_email='luck.yangbo@gmail.com',
     long_description=read_readme(),
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `GaiaScript-0.1.1.2/tests/test__template.py` & `GaiaScript-0.1.1.3/tests/test__template.py`

 * *Files identical despite different names*

