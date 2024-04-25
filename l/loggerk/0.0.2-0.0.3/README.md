# Comparing `tmp/loggerk-0.0.2.tar.gz` & `tmp/loggerk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerk-0.0.2.tar", last modified: Thu Apr 25 14:49:22 2024, max compression
+gzip compressed data, was "loggerk-0.0.3.tar", last modified: Thu Apr 25 15:45:27 2024, max compression
```

## Comparing `loggerk-0.0.2.tar` & `loggerk-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.443180 loggerk-0.0.2/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     7048 2024-04-22 22:17:13.000000 loggerk-0.0.2/LICENSE
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3296 2024-04-25 14:49:22.442988 loggerk-0.0.2/PKG-INFO
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.441047 loggerk-0.0.2/loggerk/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     5043 2024-04-25 14:38:07.000000 loggerk-0.0.2/loggerk/__init__.py
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.441766 loggerk-0.0.2/loggerk/config/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3015 2024-04-25 14:37:20.000000 loggerk-0.0.2/loggerk/config/__init__.py
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.442198 loggerk-0.0.2/loggerk/formatters/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      311 2024-04-23 15:13:03.000000 loggerk-0.0.2/loggerk/formatters/__init__.py
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.442337 loggerk-0.0.2/loggerk/handlers/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     4777 2024-04-25 14:38:13.000000 loggerk-0.0.2/loggerk/handlers/__init__.py
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.442796 loggerk-0.0.2/loggerk.egg-info/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3296 2024-04-25 14:49:22.000000 loggerk-0.0.2/loggerk.egg-info/PKG-INFO
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      277 2024-04-25 14:49:22.000000 loggerk-0.0.2/loggerk.egg-info/SOURCES.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        1 2024-04-25 14:49:22.000000 loggerk-0.0.2/loggerk.egg-info/dependency_links.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        6 2024-04-25 14:49:22.000000 loggerk-0.0.2/loggerk.egg-info/requires.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        8 2024-04-25 14:49:22.000000 loggerk-0.0.2/loggerk.egg-info/top_level.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)       38 2024-04-25 14:49:22.443216 loggerk-0.0.2/setup.cfg
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     1016 2024-04-25 14:47:18.000000 loggerk-0.0.2/setup.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.134089 loggerk-0.0.3/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     7048 2024-04-22 22:17:13.000000 loggerk-0.0.3/LICENSE
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3296 2024-04-25 15:45:27.133890 loggerk-0.0.3/PKG-INFO
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.132545 loggerk-0.0.3/loggerk/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     5620 2024-04-25 15:39:00.000000 loggerk-0.0.3/loggerk/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.133243 loggerk-0.0.3/loggerk/config/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3015 2024-04-25 14:37:20.000000 loggerk-0.0.3/loggerk/config/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.133377 loggerk-0.0.3/loggerk/formatters/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      311 2024-04-23 15:13:03.000000 loggerk-0.0.3/loggerk/formatters/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.133505 loggerk-0.0.3/loggerk/handlers/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     4777 2024-04-25 14:38:13.000000 loggerk-0.0.3/loggerk/handlers/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.133663 loggerk-0.0.3/loggerk.egg-info/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3296 2024-04-25 15:45:27.000000 loggerk-0.0.3/loggerk.egg-info/PKG-INFO
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      277 2024-04-25 15:45:27.000000 loggerk-0.0.3/loggerk.egg-info/SOURCES.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        1 2024-04-25 15:45:27.000000 loggerk-0.0.3/loggerk.egg-info/dependency_links.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        6 2024-04-25 15:45:27.000000 loggerk-0.0.3/loggerk.egg-info/requires.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        8 2024-04-25 15:45:27.000000 loggerk-0.0.3/loggerk.egg-info/top_level.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)       38 2024-04-25 15:45:27.134124 loggerk-0.0.3/setup.cfg
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     1016 2024-04-25 15:45:10.000000 loggerk-0.0.3/setup.py
```

### Comparing `loggerk-0.0.2/LICENSE` & `loggerk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerk-0.0.2/PKG-INFO` & `loggerk-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerk
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a custom logger module for Python
 Author: Kuantik DataJump
 Author-email: master@kuantik.mx
 Maintainer: Angel de Jesús Sanchez Morales
 Maintainer-email: angel.sanchez@kuantik.mx
 Keywords: python,logging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `loggerk-0.0.2/loggerk/config/__init__.py` & `loggerk-0.0.3/loggerk/config/__init__.py`

 * *Files identical despite different names*

### Comparing `loggerk-0.0.2/loggerk/handlers/__init__.py` & `loggerk-0.0.3/loggerk/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `loggerk-0.0.2/loggerk.egg-info/PKG-INFO` & `loggerk-0.0.3/loggerk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerk
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a custom logger module for Python
 Author: Kuantik DataJump
 Author-email: master@kuantik.mx
 Maintainer: Angel de Jesús Sanchez Morales
 Maintainer-email: angel.sanchez@kuantik.mx
 Keywords: python,logging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `loggerk-0.0.2/setup.py` & `loggerk-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 here: pathlib.Path = pathlib.Path(__file__).parent.resolve()
 
 long_description: str = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "This is a custom logger module for Python"
 
 # Setting up
 setup(
     name="loggerk",
     version=VERSION,
     author="Kuantik DataJump",
```

