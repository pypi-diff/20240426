# Comparing `tmp/GaiaScript-0.1.0.tar.gz` & `tmp/GaiaScript-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GaiaScript-0.1.0.tar", last modified: Fri Apr 26 02:09:56 2024, max compression
+gzip compressed data, was "GaiaScript-0.1.1.tar", last modified: Fri Apr 26 06:10:06 2024, max compression
```

## Comparing `GaiaScript-0.1.0.tar` & `GaiaScript-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 02:09:56.658536 GaiaScript-0.1.0/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 02:09:56.658536 GaiaScript-0.1.0/GaiaScript.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-26 02:09:56.000000 GaiaScript-0.1.0/GaiaScript.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      233 2024-04-26 02:09:56.000000 GaiaScript-0.1.0/GaiaScript.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 02:09:56.000000 GaiaScript-0.1.0/GaiaScript.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 02:09:56.000000 GaiaScript-0.1.0/GaiaScript.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-26 02:09:56.658536 GaiaScript-0.1.0/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.0/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 02:09:56.658536 GaiaScript-0.1.0/gaia/
--rw-rw-r--   0 mark      (1000) mark      (1000)      385 2024-04-26 01:50:31.000000 GaiaScript-0.1.0/gaia/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      306 2024-04-26 02:08:44.000000 GaiaScript-0.1.0/gaia/_exceptions.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2130 2024-04-26 02:08:44.000000 GaiaScript-0.1.0/gaia/_template.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 02:09:56.658536 GaiaScript-0.1.0/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      656 2024-04-26 01:10:27.000000 GaiaScript-0.1.0/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 02:09:56.658536 GaiaScript-0.1.0/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.0/tests/test__template.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/GaiaScript.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-26 06:10:06.000000 GaiaScript-0.1.1/GaiaScript.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      233 2024-04-26 06:10:06.000000 GaiaScript-0.1.1/GaiaScript.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 06:10:06.000000 GaiaScript-0.1.1/GaiaScript.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 06:10:06.000000 GaiaScript-0.1.1/GaiaScript.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      356 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)       43 2024-04-26 01:07:00.000000 GaiaScript-0.1.1/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/gaia/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      544 2024-04-26 06:10:01.000000 GaiaScript-0.1.1/gaia/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      306 2024-04-26 02:08:44.000000 GaiaScript-0.1.1/gaia/_exceptions.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2130 2024-04-26 02:08:44.000000 GaiaScript-0.1.1/gaia/_template.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      656 2024-04-26 06:10:01.000000 GaiaScript-0.1.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 06:10:06.641726 GaiaScript-0.1.1/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2025 2024-04-26 02:09:35.000000 GaiaScript-0.1.1/tests/test__template.py
```

### Comparing `GaiaScript-0.1.0/gaia/_template.py` & `GaiaScript-0.1.1/gaia/_template.py`

 * *Files identical despite different names*

### Comparing `GaiaScript-0.1.0/setup.py` & `GaiaScript-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name='GaiaScript',
-    version='0.1.0',
+    version='0.1.1',
     author='369',
     author_email='luck.yangbo@gmail.com',
     long_description=read_readme(),
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `GaiaScript-0.1.0/tests/test__template.py` & `GaiaScript-0.1.1/tests/test__template.py`

 * *Files identical despite different names*

