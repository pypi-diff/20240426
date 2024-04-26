# Comparing `tmp/nue-0.0.3.tar.gz` & `tmp/nue-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nue-0.0.3.tar", last modified: Thu Apr 25 06:36:30 2024, max compression
+gzip compressed data, was "nue-0.0.4.tar", last modified: Fri Apr 26 21:31:36 2024, max compression
```

## Comparing `nue-0.0.3.tar` & `nue-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-25 06:36:30.845512 nue-0.0.3/
--rw-r--r--   0 juanvera   (501) staff       (20)     1062 2024-04-22 16:56:55.000000 nue-0.0.3/LICENSE
--rw-r--r--   0 juanvera   (501) staff       (20)     1776 2024-04-25 06:36:30.845224 nue-0.0.3/PKG-INFO
--rw-r--r--   0 juanvera   (501) staff       (20)     1212 2024-04-25 01:49:56.000000 nue-0.0.3/README.md
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-25 06:36:30.842839 nue-0.0.3/nue/
--rw-r--r--   0 juanvera   (501) staff       (20)       39 2024-04-25 06:35:25.000000 nue-0.0.3/nue/__init__.py
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-25 06:36:30.844714 nue-0.0.3/nue/models/
--rw-r--r--   0 juanvera   (501) staff       (20)       62 2024-04-25 06:35:48.000000 nue-0.0.3/nue/models/__init__.py
--rw-r--r--   0 juanvera   (501) staff       (20)     1731 2024-04-25 05:49:19.000000 nue-0.0.3/nue/models/linreg.py
--rw-r--r--   0 juanvera   (501) staff       (20)     1923 2024-04-25 05:49:19.000000 nue-0.0.3/nue/models/logreg.py
--rw-r--r--   0 juanvera   (501) staff       (20)     3455 2024-04-25 05:49:19.000000 nue-0.0.3/nue/models/nn.py
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-25 06:36:30.843642 nue-0.0.3/nue.egg-info/
--rw-r--r--   0 juanvera   (501) staff       (20)     1776 2024-04-25 06:36:30.000000 nue-0.0.3/nue.egg-info/PKG-INFO
--rw-r--r--   0 juanvera   (501) staff       (20)      258 2024-04-25 06:36:30.000000 nue-0.0.3/nue.egg-info/SOURCES.txt
--rw-r--r--   0 juanvera   (501) staff       (20)        1 2024-04-25 06:36:30.000000 nue-0.0.3/nue.egg-info/dependency_links.txt
--rw-r--r--   0 juanvera   (501) staff       (20)       24 2024-04-25 06:36:30.000000 nue-0.0.3/nue.egg-info/requires.txt
--rw-r--r--   0 juanvera   (501) staff       (20)        4 2024-04-25 06:36:30.000000 nue-0.0.3/nue.egg-info/top_level.txt
--rw-r--r--   0 juanvera   (501) staff       (20)       38 2024-04-25 06:36:30.845576 nue-0.0.3/setup.cfg
--rw-r--r--   0 juanvera   (501) staff       (20)      862 2024-04-25 06:36:21.000000 nue-0.0.3/setup.py
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:31:36.186159 nue-0.0.4/
+-rw-r--r--   0 juanvera   (501) staff       (20)     1062 2024-04-22 16:56:55.000000 nue-0.0.4/LICENSE
+-rw-r--r--   0 juanvera   (501) staff       (20)     1004 2024-04-26 21:31:36.185818 nue-0.0.4/PKG-INFO
+-rw-r--r--   0 juanvera   (501) staff       (20)     1186 2024-04-26 12:36:27.000000 nue-0.0.4/README.md
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:31:36.184236 nue-0.0.4/models/
+-rw-r--r--   0 juanvera   (501) staff       (20)      924 2024-04-26 15:20:27.000000 nue-0.0.4/models/__init__.py
+-rw-r--r--   0 juanvera   (501) staff       (20)     3538 2024-04-26 12:46:29.000000 nue-0.0.4/models/linreg.py
+-rw-r--r--   0 juanvera   (501) staff       (20)     4000 2024-04-26 02:56:06.000000 nue-0.0.4/models/logreg.py
+-rw-r--r--   0 juanvera   (501) staff       (20)     6694 2024-04-26 12:51:41.000000 nue-0.0.4/models/nn.py
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:31:36.185339 nue-0.0.4/nue.egg-info/
+-rw-r--r--   0 juanvera   (501) staff       (20)     1004 2024-04-26 21:31:36.000000 nue-0.0.4/nue.egg-info/PKG-INFO
+-rw-r--r--   0 juanvera   (501) staff       (20)      226 2024-04-26 21:31:36.000000 nue-0.0.4/nue.egg-info/SOURCES.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)        1 2024-04-26 21:31:36.000000 nue-0.0.4/nue.egg-info/dependency_links.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)       24 2024-04-26 21:31:36.000000 nue-0.0.4/nue.egg-info/requires.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)        7 2024-04-26 21:31:36.000000 nue-0.0.4/nue.egg-info/top_level.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)       38 2024-04-26 21:31:36.186233 nue-0.0.4/setup.cfg
+-rw-r--r--   0 juanvera   (501) staff       (20)     1010 2024-04-26 21:29:31.000000 nue-0.0.4/setup.py
```

### Comparing `nue-0.0.3/LICENSE` & `nue-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nue-0.0.3/README.md` & `nue-0.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-### A Deep Learning Framework for Entry Level Tinkerers
+### Nue
 
-A Python Package for Seamless Usage and Implementation of Deep Learning Models
+A deep learning framework sculpted for seamless implementation of models, geared towards entry level learners.
 
 _Currently in Development, I'll be adding as I learn how to build_
 
 ### **Phase 1**
 
-**MAIN**
-
-- [ ]  Linear Regression Model
+- [X]  Linear Regression Model
     - [x]  Implement
-    - [ ]  Write DocStrings
-- [ ]  Logistic Regression Model
+    - [X]  Write DocStrings
+- [X]  Logistic Regression Model
     - [X]  Implement
-    - [ ]  Write DocStrings
-- [ ]  Vanilla Neural Networks
+    - [X]  Write DocStrings
+- [X]  Vanilla Neural Networks
     - [X]  Implement
-    - [ ]  Write DocStrings
+    - [X]  Write DocStrings
 
 **Organize**
 
 - [ ]  Optimize performance of each model
     - [ ]  Tune the operations and architecture (code)
 - [ ]  Implement scaling / standardization functions
 - [ ]  Ship ‘pip install neo_dl’ functionality once a stable version is released.
```

### Comparing `nue-0.0.3/setup.py` & `nue-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # setup.py
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
-DEFAULTV = '0.0.3'
-DESCRIPTION = 'A Deep Learning Package for Entry Level Tinkerers'
+VERSION = '0.0.4'
+DEFAULTV = '0.0.4'
+DESCRIPTION = 'A deep learning framework sculpted for seamless implementation of models, geared towards entry level learners. '
 
 setup(
     name='nue',
     version= VERSION,
     default_version= DEFAULTV,
-    packages=find_packages(exclude = ['examples']),
+    packages=find_packages(exclude = ['examples', 'docs', 'dist', 'test']),
+    exclude_package_data={'': ['.gitignore', '.gitattributes']},
     author='vxnuaj',
     author_email='jv.100420@gmail.com',
     description= DESCRIPTION,
-    long_description=open('README.md').read(),
+    long_description=open('PYPI.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/vxnuaj/neuo',
+    url='https://vxnuaj.github.io/nue/',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
     ],
```

