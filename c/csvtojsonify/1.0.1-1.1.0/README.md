# Comparing `tmp/csvtojsonify-1.0.1.tar.gz` & `tmp/csvtojsonify-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvtojsonify-1.0.1.tar", last modified: Thu Apr 25 13:45:56 2024, max compression
+gzip compressed data, was "csvtojsonify-1.1.0.tar", last modified: Fri Apr 26 03:00:32 2024, max compression
```

## Comparing `csvtojsonify-1.0.1.tar` & `csvtojsonify-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-25 13:45:56.399991 csvtojsonify-1.0.1/
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      116 2024-04-25 04:37:39.000000 csvtojsonify-1.0.1/MANIFEST.in
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      894 2024-04-25 13:45:56.399806 csvtojsonify-1.0.1/PKG-INFO
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      436 2024-04-25 13:37:57.000000 csvtojsonify-1.0.1/README.md
-drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-25 13:45:56.399650 csvtojsonify-1.0.1/csvtojsonify.egg-info/
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      894 2024-04-25 13:45:56.000000 csvtojsonify-1.0.1/csvtojsonify.egg-info/PKG-INFO
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      225 2024-04-25 13:45:56.000000 csvtojsonify-1.0.1/csvtojsonify.egg-info/SOURCES.txt
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)        1 2024-04-25 13:45:56.000000 csvtojsonify-1.0.1/csvtojsonify.egg-info/dependency_links.txt
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)        7 2024-04-25 13:45:56.000000 csvtojsonify-1.0.1/csvtojsonify.egg-info/requires.txt
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)        1 2024-04-25 13:45:56.000000 csvtojsonify-1.0.1/csvtojsonify.egg-info/top_level.txt
--rwxr-xr-x   0 sriramsreedhar   (501) staff       (20)      749 2024-04-25 03:20:55.000000 csvtojsonify-1.0.1/csvtojsonify.py
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)       38 2024-04-25 13:45:56.400030 csvtojsonify-1.0.1/setup.cfg
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      665 2024-04-25 13:33:11.000000 csvtojsonify-1.0.1/setup.py
+drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 03:00:32.479638 csvtojsonify-1.1.0/
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      116 2024-04-25 04:37:39.000000 csvtojsonify-1.1.0/MANIFEST.in
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      728 2024-04-26 03:00:32.479468 csvtojsonify-1.1.0/PKG-INFO
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      436 2024-04-25 13:37:57.000000 csvtojsonify-1.1.0/README.md
+drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 03:00:32.478676 csvtojsonify-1.1.0/csvtojsonify/
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 02:50:35.000000 csvtojsonify-1.1.0/csvtojsonify/__init__.py
+drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-26 03:00:32.479305 csvtojsonify-1.1.0/csvtojsonify.egg-info/
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      728 2024-04-26 03:00:32.000000 csvtojsonify-1.1.0/csvtojsonify.egg-info/PKG-INFO
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      254 2024-04-26 03:00:32.000000 csvtojsonify-1.1.0/csvtojsonify.egg-info/SOURCES.txt
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)        1 2024-04-26 03:00:32.000000 csvtojsonify-1.1.0/csvtojsonify.egg-info/dependency_links.txt
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)       64 2024-04-26 03:00:32.000000 csvtojsonify-1.1.0/csvtojsonify.egg-info/entry_points.txt
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)       13 2024-04-26 03:00:32.000000 csvtojsonify-1.1.0/csvtojsonify.egg-info/top_level.txt
+-rwxr-xr-x   0 sriramsreedhar   (501) staff       (20)      749 2024-04-25 03:20:55.000000 csvtojsonify-1.1.0/csvtojsonify.py
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)       38 2024-04-26 03:00:32.479679 csvtojsonify-1.1.0/setup.cfg
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      587 2024-04-26 02:59:07.000000 csvtojsonify-1.1.0/setup.py
```

### Comparing `csvtojsonify-1.0.1/PKG-INFO` & `csvtojsonify-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: csvtojsonify
-Version: 1.0.1
-Summary: A Python script to convert CSV to JSON
+Version: 1.1.0
+Summary: A tool to convert CSV files to JSON.
 Home-page: https://github.com/sriramsreedhar/csvtojsonify
-Author: csvtojsonify
+Author: Sriram Sreedhar
 Author-email: sriramsreedhar003@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
 
 # csvtojsonify
 
 A simple tool to convert CSV files to JSON format.
 
 ## Usage
```

### Comparing `csvtojsonify-1.0.1/csvtojsonify.egg-info/PKG-INFO` & `csvtojsonify-1.1.0/csvtojsonify.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: csvtojsonify
-Version: 1.0.1
-Summary: A Python script to convert CSV to JSON
+Version: 1.1.0
+Summary: A tool to convert CSV files to JSON.
 Home-page: https://github.com/sriramsreedhar/csvtojsonify
-Author: csvtojsonify
+Author: Sriram Sreedhar
 Author-email: sriramsreedhar003@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
 
 # csvtojsonify
 
 A simple tool to convert CSV files to JSON format.
 
 ## Usage
```

### Comparing `csvtojsonify-1.0.1/csvtojsonify.py` & `csvtojsonify-1.1.0/csvtojsonify.py`

 * *Files identical despite different names*

### Comparing `csvtojsonify-1.0.1/setup.py` & `csvtojsonify-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
     name='csvtojsonify',
-    version='1.0.1',
-    author='csvtojsonify',
+    version='1.1.0',
+    packages=['csvtojsonify'],
+    entry_points={
+        'console_scripts': [
+            'csvtojsonify=csvtojsonify.csvtojsonify:main',
+        ],
+    },
+    install_requires=[],
+    python_requires='>=3.9.6',
+    author='Sriram Sreedhar',
     author_email='sriramsreedhar003@gmail.com',
-    description='A Python script to convert CSV to JSON',
+    description='A tool to convert CSV files to JSON.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sriramsreedhar/csvtojsonify',
-    packages=find_packages(),
-    install_requires=[
-        'pandas',
-    ],
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-    python_requires='>=3.10',
 )
```

