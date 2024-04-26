# Comparing `tmp/mknn-0.0.1.tar.gz` & `tmp/mknn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mknn-0.0.1.tar", last modified: Fri Apr 26 18:56:45 2024, max compression
+gzip compressed data, was "mknn-0.0.2.tar", last modified: Fri Apr 26 19:02:54 2024, max compression
```

## Comparing `mknn-0.0.1.tar` & `mknn-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:56:45.919836 mknn-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-26 18:56:45.919836 mknn-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-26 18:56:41.000000 mknn-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:56:45.919836 mknn-0.0.1/mknn/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 18:56:41.000000 mknn-0.0.1/mknn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-26 18:56:41.000000 mknn-0.0.1/mknn/mknn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:56:45.919836 mknn-0.0.1/mknn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-26 18:56:45.000000 mknn-0.0.1/mknn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-26 18:56:45.000000 mknn-0.0.1/mknn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:56:45.000000 mknn-0.0.1/mknn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 18:56:45.000000 mknn-0.0.1/mknn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 18:56:45.000000 mknn-0.0.1/mknn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:56:45.919836 mknn-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 18:56:41.000000 mknn-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:02:54.085847 mknn-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-26 19:02:54.085847 mknn-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-26 19:02:49.000000 mknn-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:02:54.085847 mknn-0.0.2/mknn/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 19:02:49.000000 mknn-0.0.2/mknn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-26 19:02:49.000000 mknn-0.0.2/mknn/mknn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:02:54.085847 mknn-0.0.2/mknn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-26 19:02:54.000000 mknn-0.0.2/mknn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-26 19:02:54.000000 mknn-0.0.2/mknn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:02:54.000000 mknn-0.0.2/mknn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 19:02:54.000000 mknn-0.0.2/mknn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 19:02:54.000000 mknn-0.0.2/mknn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:02:54.085847 mknn-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-26 19:02:49.000000 mknn-0.0.2/setup.py
```

### Comparing `mknn-0.0.1/PKG-INFO` & `mknn-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mknn
-Version: 0.0.1
+Version: 0.0.2
 Summary: Modified K-Nearest Neighbor
 Home-page: https://github.com/nsandarma/Modified-K-Nearest-Neighbor
 Author: nsandarma
 Author-email: nsandarma@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `mknn-0.0.1/README.md` & `mknn-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mknn-0.0.1/mknn/mknn.py` & `mknn-0.0.2/mknn/mknn.py`

 * *Files identical despite different names*

### Comparing `mknn-0.0.1/mknn.egg-info/PKG-INFO` & `mknn-0.0.2/mknn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mknn
-Version: 0.0.1
+Version: 0.0.2
 Summary: Modified K-Nearest Neighbor
 Home-page: https://github.com/nsandarma/Modified-K-Nearest-Neighbor
 Author: nsandarma
 Author-email: nsandarma@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `mknn-0.0.1/setup.py` & `mknn-0.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
-with open("requirements.txt", "r") as req_file:
-    requirements = req_file.read().splitlines()
-
 DESCRIPTION = "Modified K-Nearest Neighbor"
 
 NAME = "mknn"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nsandarma/Modified-K-Nearest-Neighbor",
@@ -21,9 +18,9 @@
     author_email="nsandarma@gmail.com",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.10",
-    install_requires=requirements,
+    install_requires=['scikit-learn','numpy'],
 )
```

