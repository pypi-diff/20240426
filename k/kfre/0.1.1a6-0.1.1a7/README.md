# Comparing `tmp/kfre-0.1.1a6.tar.gz` & `tmp/kfre-0.1.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfre-0.1.1a6.tar", last modified: Fri Apr 26 06:36:00 2024, max compression
+gzip compressed data, was "kfre-0.1.1a7.tar", last modified: Fri Apr 26 06:38:58 2024, max compression
```

## Comparing `kfre-0.1.1a6.tar` & `kfre-0.1.1a7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 06:36:00.257875 kfre-0.1.1a6/
--rw-rw-rw-   0        0        0     4402 2024-04-26 06:36:00.256876 kfre-0.1.1a6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-26 06:36:00.257875 kfre-0.1.1a6/setup.cfg
--rw-rw-rw-   0        0        0     1149 2024-04-26 06:35:53.000000 kfre-0.1.1a6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:36:00.184803 kfre-0.1.1a6/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 06:36:00.213790 kfre-0.1.1a6/src/kfre/
--rw-rw-rw-   0        0        0       55 2024-04-26 04:56:44.000000 kfre-0.1.1a6/src/kfre/__init__.py
--rw-rw-rw-   0        0        0    12299 2024-04-26 06:08:43.000000 kfre-0.1.1a6/src/kfre/main.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:36:00.255891 kfre-0.1.1a6/src/kfre.egg-info/
--rw-rw-rw-   0        0        0     4402 2024-04-26 06:36:00.000000 kfre-0.1.1a6/src/kfre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-04-26 06:36:00.000000 kfre-0.1.1a6/src/kfre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 06:36:00.000000 kfre-0.1.1a6/src/kfre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-26 06:36:00.000000 kfre-0.1.1a6/src/kfre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-26 06:36:00.000000 kfre-0.1.1a6/src/kfre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 06:38:58.215211 kfre-0.1.1a7/
+-rw-rw-rw-   0        0        0     4402 2024-04-26 06:38:58.214211 kfre-0.1.1a7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-26 06:38:58.215211 kfre-0.1.1a7/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2024-04-26 06:38:51.000000 kfre-0.1.1a7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:38:58.190694 kfre-0.1.1a7/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 06:38:58.192693 kfre-0.1.1a7/src/kfre/
+-rw-rw-rw-   0        0        0       55 2024-04-26 04:56:44.000000 kfre-0.1.1a7/src/kfre/__init__.py
+-rw-rw-rw-   0        0        0    12299 2024-04-26 06:08:43.000000 kfre-0.1.1a7/src/kfre/main.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:38:58.213212 kfre-0.1.1a7/src/kfre.egg-info/
+-rw-rw-rw-   0        0        0     4402 2024-04-26 06:38:58.000000 kfre-0.1.1a7/src/kfre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-04-26 06:38:58.000000 kfre-0.1.1a7/src/kfre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 06:38:58.000000 kfre-0.1.1a7/src/kfre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-26 06:38:58.000000 kfre-0.1.1a7/src/kfre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-26 06:38:58.000000 kfre-0.1.1a7/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.1a6/PKG-INFO` & `kfre-0.1.1a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.1a6
+Version: 0.1.1a7
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Home-page: https://github.com/lshpaner/kfre
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kfre-0.1.1a6/setup.py` & `kfre-0.1.1a7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kfre",
-    version="0.1.1-alpha6",
+    version="0.1.1-alpha7",
     author="Leonid Shpaner",
     author_email="Lshpaner@ucla.edu",
     description="A Python library for kidney failure risk estimation using Tangri's KFRE model",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",  # Type of the long description
     url="https://github.com/lshpaner/kfre",  # URL to the repository or documentation
     package_dir={"": "src"},  # Directory where your package files are located
```

### Comparing `kfre-0.1.1a6/src/kfre/main.py` & `kfre-0.1.1a7/src/kfre/main.py`

 * *Files identical despite different names*

### Comparing `kfre-0.1.1a6/src/kfre.egg-info/PKG-INFO` & `kfre-0.1.1a7/src/kfre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.1a6
+Version: 0.1.1a7
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Home-page: https://github.com/lshpaner/kfre
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

