# Comparing `tmp/kfre-0.1.1a4.tar.gz` & `tmp/kfre-0.1.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfre-0.1.1a4.tar", last modified: Fri Apr 26 06:10:45 2024, max compression
+gzip compressed data, was "kfre-0.1.1a5.tar", last modified: Fri Apr 26 06:31:25 2024, max compression
```

## Comparing `kfre-0.1.1a4.tar` & `kfre-0.1.1a5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 06:10:45.501523 kfre-0.1.1a4/
--rw-rw-rw-   0        0        0     4402 2024-04-26 06:10:45.499525 kfre-0.1.1a4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-26 06:10:45.502523 kfre-0.1.1a4/setup.cfg
--rw-rw-rw-   0        0        0     1149 2024-04-26 06:09:07.000000 kfre-0.1.1a4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:10:45.464933 kfre-0.1.1a4/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 06:10:45.497525 kfre-0.1.1a4/src/kfre.egg-info/
--rw-rw-rw-   0        0        0     4402 2024-04-26 06:10:45.000000 kfre-0.1.1a4/src/kfre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-04-26 06:10:45.000000 kfre-0.1.1a4/src/kfre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 06:10:45.000000 kfre-0.1.1a4/src/kfre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-26 06:10:45.000000 kfre-0.1.1a4/src/kfre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 06:10:45.000000 kfre-0.1.1a4/src/kfre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 06:31:25.008922 kfre-0.1.1a5/
+-rw-rw-rw-   0        0        0     4402 2024-04-26 06:31:25.007919 kfre-0.1.1a5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-26 06:31:25.008922 kfre-0.1.1a5/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2024-04-26 06:31:19.000000 kfre-0.1.1a5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:31:24.993994 kfre-0.1.1a5/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 06:31:25.006922 kfre-0.1.1a5/src/kfre.egg-info/
+-rw-rw-rw-   0        0        0     4402 2024-04-26 06:31:24.000000 kfre-0.1.1a5/src/kfre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-04-26 06:31:24.000000 kfre-0.1.1a5/src/kfre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 06:31:24.000000 kfre-0.1.1a5/src/kfre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-26 06:31:24.000000 kfre-0.1.1a5/src/kfre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 06:31:24.000000 kfre-0.1.1a5/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.1a4/PKG-INFO` & `kfre-0.1.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.1a4
+Version: 0.1.1a5
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Home-page: https://github.com/lshpaner/kfre
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kfre-0.1.1a4/setup.py` & `kfre-0.1.1a5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kfre",
-    version="0.1.1-alpha4",
+    version="0.1.1-alpha5",
     author="Leonid Shpaner",
     author_email="Lshpaner@ucla.edu",
     description="A Python library for kidney failure risk estimation using Tangri's KFRE model",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",  # Type of the long description
     url="https://github.com/lshpaner/kfre",  # URL to the repository or documentation
     package_dir={"": "src"},  # Directory where your package files are located
```

### Comparing `kfre-0.1.1a4/src/kfre.egg-info/PKG-INFO` & `kfre-0.1.1a5/src/kfre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.1a4
+Version: 0.1.1a5
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Home-page: https://github.com/lshpaner/kfre
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```
