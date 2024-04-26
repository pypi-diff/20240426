# Comparing `tmp/nue-0.0.4.tar.gz` & `tmp/nue-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nue-0.0.4.tar", last modified: Fri Apr 26 21:31:36 2024, max compression
+gzip compressed data, was "nue-0.0.5.tar", last modified: Fri Apr 26 21:53:42 2024, max compression
```

## Comparing `nue-0.0.4.tar` & `nue-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:31:36.186159 nue-0.0.4/
--rw-r--r--   0 juanvera   (501) staff       (20)     1062 2024-04-22 16:56:55.000000 nue-0.0.4/LICENSE
--rw-r--r--   0 juanvera   (501) staff       (20)     1004 2024-04-26 21:31:36.185818 nue-0.0.4/PKG-INFO
--rw-r--r--   0 juanvera   (501) staff       (20)     1186 2024-04-26 12:36:27.000000 nue-0.0.4/README.md
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:31:36.184236 nue-0.0.4/models/
--rw-r--r--   0 juanvera   (501) staff       (20)      924 2024-04-26 15:20:27.000000 nue-0.0.4/models/__init__.py
--rw-r--r--   0 juanvera   (501) staff       (20)     3538 2024-04-26 12:46:29.000000 nue-0.0.4/models/linreg.py
--rw-r--r--   0 juanvera   (501) staff       (20)     4000 2024-04-26 02:56:06.000000 nue-0.0.4/models/logreg.py
--rw-r--r--   0 juanvera   (501) staff       (20)     6694 2024-04-26 12:51:41.000000 nue-0.0.4/models/nn.py
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:31:36.185339 nue-0.0.4/nue.egg-info/
--rw-r--r--   0 juanvera   (501) staff       (20)     1004 2024-04-26 21:31:36.000000 nue-0.0.4/nue.egg-info/PKG-INFO
--rw-r--r--   0 juanvera   (501) staff       (20)      226 2024-04-26 21:31:36.000000 nue-0.0.4/nue.egg-info/SOURCES.txt
--rw-r--r--   0 juanvera   (501) staff       (20)        1 2024-04-26 21:31:36.000000 nue-0.0.4/nue.egg-info/dependency_links.txt
--rw-r--r--   0 juanvera   (501) staff       (20)       24 2024-04-26 21:31:36.000000 nue-0.0.4/nue.egg-info/requires.txt
--rw-r--r--   0 juanvera   (501) staff       (20)        7 2024-04-26 21:31:36.000000 nue-0.0.4/nue.egg-info/top_level.txt
--rw-r--r--   0 juanvera   (501) staff       (20)       38 2024-04-26 21:31:36.186233 nue-0.0.4/setup.cfg
--rw-r--r--   0 juanvera   (501) staff       (20)     1010 2024-04-26 21:29:31.000000 nue-0.0.4/setup.py
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:53:42.583076 nue-0.0.5/
+-rw-r--r--   0 juanvera   (501) staff       (20)     1062 2024-04-22 16:56:55.000000 nue-0.0.5/LICENSE
+-rw-r--r--   0 juanvera   (501) staff       (20)     1004 2024-04-26 21:53:42.582684 nue-0.0.5/PKG-INFO
+-rw-r--r--   0 juanvera   (501) staff       (20)     1572 2024-04-26 21:49:31.000000 nue-0.0.5/README.md
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:53:42.580885 nue-0.0.5/models/
+-rw-r--r--   0 juanvera   (501) staff       (20)      924 2024-04-26 15:20:27.000000 nue-0.0.5/models/__init__.py
+-rw-r--r--   0 juanvera   (501) staff       (20)     3538 2024-04-26 12:46:29.000000 nue-0.0.5/models/linreg.py
+-rw-r--r--   0 juanvera   (501) staff       (20)     4000 2024-04-26 02:56:06.000000 nue-0.0.5/models/logreg.py
+-rw-r--r--   0 juanvera   (501) staff       (20)     6694 2024-04-26 12:51:41.000000 nue-0.0.5/models/nn.py
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:53:42.582034 nue-0.0.5/nue.egg-info/
+-rw-r--r--   0 juanvera   (501) staff       (20)     1004 2024-04-26 21:53:42.000000 nue-0.0.5/nue.egg-info/PKG-INFO
+-rw-r--r--   0 juanvera   (501) staff       (20)      226 2024-04-26 21:53:42.000000 nue-0.0.5/nue.egg-info/SOURCES.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)        1 2024-04-26 21:53:42.000000 nue-0.0.5/nue.egg-info/dependency_links.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)       24 2024-04-26 21:53:42.000000 nue-0.0.5/nue.egg-info/requires.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)        7 2024-04-26 21:53:42.000000 nue-0.0.5/nue.egg-info/top_level.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)       38 2024-04-26 21:53:42.583156 nue-0.0.5/setup.cfg
+-rw-r--r--   0 juanvera   (501) staff       (20)     1010 2024-04-26 21:53:39.000000 nue-0.0.5/setup.py
```

### Comparing `nue-0.0.4/LICENSE` & `nue-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nue-0.0.4/PKG-INFO` & `nue-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nue
-Version: 0.0.4
+Version: 0.0.5
 Summary: A deep learning framework sculpted for seamless implementation of models, geared towards entry level learners. 
 Home-page: https://vxnuaj.github.io/nue/
 Author: vxnuaj
 Author-email: jv.100420@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nue-0.0.4/models/__init__.py` & `nue-0.0.5/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nue-0.0.4/models/linreg.py` & `nue-0.0.5/models/linreg.py`

 * *Files identical despite different names*

### Comparing `nue-0.0.4/models/logreg.py` & `nue-0.0.5/models/logreg.py`

 * *Files identical despite different names*

### Comparing `nue-0.0.4/models/nn.py` & `nue-0.0.5/models/nn.py`

 * *Files identical despite different names*

### Comparing `nue-0.0.4/nue.egg-info/PKG-INFO` & `nue-0.0.5/nue.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nue
-Version: 0.0.4
+Version: 0.0.5
 Summary: A deep learning framework sculpted for seamless implementation of models, geared towards entry level learners. 
 Home-page: https://vxnuaj.github.io/nue/
 Author: vxnuaj
 Author-email: jv.100420@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nue-0.0.4/setup.py` & `nue-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
-DEFAULTV = '0.0.4'
+VERSION = '0.0.5'
+DEFAULTV = '0.0.5'
 DESCRIPTION = 'A deep learning framework sculpted for seamless implementation of models, geared towards entry level learners. '
 
 setup(
     name='nue',
     version= VERSION,
     default_version= DEFAULTV,
     packages=find_packages(exclude = ['examples', 'docs', 'dist', 'test']),
```

