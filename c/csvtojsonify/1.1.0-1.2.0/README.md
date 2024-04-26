# Comparing `tmp/csvtojsonify-1.1.0.tar.gz` & `tmp/csvtojsonify-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvtojsonify-1.1.0.tar", last modified: Fri Apr 26 03:00:32 2024, max compression
+gzip compressed data, was "csvtojsonify-1.2.0.tar", last modified: Fri Apr 26 03:19:07 2024, max compression
```

## Comparing `csvtojsonify-1.1.0.tar` & `csvtojsonify-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 03:00:32.479638 csvtojsonify-1.1.0/
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      116 2024-04-25 04:37:39.000000 csvtojsonify-1.1.0/MANIFEST.in
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      728 2024-04-26 03:00:32.479468 csvtojsonify-1.1.0/PKG-INFO
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      436 2024-04-25 13:37:57.000000 csvtojsonify-1.1.0/README.md
-drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 03:00:32.478676 csvtojsonify-1.1.0/csvtojsonify/
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 02:50:35.000000 csvtojsonify-1.1.0/csvtojsonify/__init__.py
-drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 03:00:32.479305 csvtojsonify-1.1.0/csvtojsonify.egg-info/
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      728 2024-04-26 03:00:32.000000 csvtojsonify-1.1.0/csvtojsonify.egg-info/PKG-INFO
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      254 2024-04-26 03:00:32.000000 csvtojsonify-1.1.0/csvtojsonify.egg-info/SOURCES.txt
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)        1 2024-04-26 03:00:32.000000 csvtojsonify-1.1.0/csvtojsonify.egg-info/dependency_links.txt
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)       64 2024-04-26 03:00:32.000000 csvtojsonify-1.1.0/csvtojsonify.egg-info/entry_points.txt
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)       13 2024-04-26 03:00:32.000000 csvtojsonify-1.1.0/csvtojsonify.egg-info/top_level.txt
--rwxr-xr-x   0 sriramsreedhar   (501) staff       (20)      749 2024-04-25 03:20:55.000000 csvtojsonify-1.1.0/csvtojsonify.py
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)       38 2024-04-26 03:00:32.479679 csvtojsonify-1.1.0/setup.cfg
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      587 2024-04-26 02:59:07.000000 csvtojsonify-1.1.0/setup.py
+drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 03:19:07.513084 csvtojsonify-1.2.0/
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      116 2024-04-25 04:37:39.000000 csvtojsonify-1.2.0/MANIFEST.in
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      728 2024-04-26 03:19:07.512911 csvtojsonify-1.2.0/PKG-INFO
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      436 2024-04-25 13:37:57.000000 csvtojsonify-1.2.0/README.md
+drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 03:19:07.512060 csvtojsonify-1.2.0/csvtojsonify/
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 02:50:35.000000 csvtojsonify-1.2.0/csvtojsonify/__init__.py
+drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 03:19:07.512735 csvtojsonify-1.2.0/csvtojsonify.egg-info/
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      728 2024-04-26 03:19:07.000000 csvtojsonify-1.2.0/csvtojsonify.egg-info/PKG-INFO
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      254 2024-04-26 03:19:07.000000 csvtojsonify-1.2.0/csvtojsonify.egg-info/SOURCES.txt
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)        1 2024-04-26 03:19:07.000000 csvtojsonify-1.2.0/csvtojsonify.egg-info/dependency_links.txt
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)       64 2024-04-26 03:19:07.000000 csvtojsonify-1.2.0/csvtojsonify.egg-info/entry_points.txt
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)       13 2024-04-26 03:19:07.000000 csvtojsonify-1.2.0/csvtojsonify.egg-info/top_level.txt
+-rwxr-xr-x   0 sriramsreedhar   (501) staff       (20)      956 2024-04-26 03:15:02.000000 csvtojsonify-1.2.0/csvtojsonify.py
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)       38 2024-04-26 03:19:07.513125 csvtojsonify-1.2.0/setup.cfg
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      587 2024-04-26 03:17:32.000000 csvtojsonify-1.2.0/setup.py
```

### Comparing `csvtojsonify-1.1.0/PKG-INFO` & `csvtojsonify-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvtojsonify
-Version: 1.1.0
+Version: 1.2.0
 Summary: A tool to convert CSV files to JSON.
 Home-page: https://github.com/sriramsreedhar/csvtojsonify
 Author: Sriram Sreedhar
 Author-email: sriramsreedhar003@gmail.com
 Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
```

### Comparing `csvtojsonify-1.1.0/csvtojsonify.egg-info/PKG-INFO` & `csvtojsonify-1.2.0/csvtojsonify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvtojsonify
-Version: 1.1.0
+Version: 1.2.0
 Summary: A tool to convert CSV files to JSON.
 Home-page: https://github.com/sriramsreedhar/csvtojsonify
 Author: Sriram Sreedhar
 Author-email: sriramsreedhar003@gmail.com
 Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
```

### Comparing `csvtojsonify-1.1.0/setup.py` & `csvtojsonify-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='csvtojsonify',
-    version='1.1.0',
+    version='1.2.0',
     packages=['csvtojsonify'],
     entry_points={
         'console_scripts': [
             'csvtojsonify=csvtojsonify.csvtojsonify:main',
         ],
     },
     install_requires=[],
```

