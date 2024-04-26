# Comparing `tmp/kfre-0.1.1a2.tar.gz` & `tmp/kfre-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfre-0.1.1a2.tar", last modified: Fri Apr 26 05:18:23 2024, max compression
+gzip compressed data, was "kfre-0.1.1a3.tar", last modified: Fri Apr 26 05:44:02 2024, max compression
```

## Comparing `kfre-0.1.1a2.tar` & `kfre-0.1.1a3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 05:18:23.534733 kfre-0.1.1a2/
--rw-rw-rw-   0        0        0     4402 2024-04-26 05:18:23.531621 kfre-0.1.1a2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-26 05:18:23.535627 kfre-0.1.1a2/setup.cfg
--rw-rw-rw-   0        0        0     1149 2024-04-26 05:17:48.000000 kfre-0.1.1a2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:18:23.492976 kfre-0.1.1a2/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 05:18:23.530739 kfre-0.1.1a2/src/kfre.egg-info/
--rw-rw-rw-   0        0        0     4402 2024-04-26 05:18:23.000000 kfre-0.1.1a2/src/kfre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-04-26 05:18:23.000000 kfre-0.1.1a2/src/kfre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 05:18:23.000000 kfre-0.1.1a2/src/kfre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-26 05:18:23.000000 kfre-0.1.1a2/src/kfre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 05:18:23.000000 kfre-0.1.1a2/src/kfre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 05:44:02.557559 kfre-0.1.1a3/
+-rw-rw-rw-   0        0        0     4402 2024-04-26 05:44:02.556578 kfre-0.1.1a3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-26 05:44:02.557559 kfre-0.1.1a3/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2024-04-26 05:42:28.000000 kfre-0.1.1a3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:44:02.524467 kfre-0.1.1a3/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 05:44:02.555554 kfre-0.1.1a3/src/kfre.egg-info/
+-rw-rw-rw-   0        0        0     4402 2024-04-26 05:44:02.000000 kfre-0.1.1a3/src/kfre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-04-26 05:44:02.000000 kfre-0.1.1a3/src/kfre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 05:44:02.000000 kfre-0.1.1a3/src/kfre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-26 05:44:02.000000 kfre-0.1.1a3/src/kfre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 05:44:02.000000 kfre-0.1.1a3/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.1a2/PKG-INFO` & `kfre-0.1.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Home-page: https://github.com/lshpaner/kfre
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kfre-0.1.1a2/setup.py` & `kfre-0.1.1a3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from setuptools import setup, find_packages
+from setuptools import setup, find_packages  # type: ignore
 
 setup(
     name="kfre",
-    version="0.1.1-alpha2",
+    version="0.1.1-alpha3",
     author="Leonid Shpaner",
     author_email="Lshpaner@ucla.edu",
     description="A Python library for kidney failure risk estimation using Tangri's KFRE model",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",  # Type of the long description
     url="https://github.com/lshpaner/kfre",  # URL to the repository or documentation
     package_dir={"": "src"},  # Directory where your package files are located
```

### Comparing `kfre-0.1.1a2/src/kfre.egg-info/PKG-INFO` & `kfre-0.1.1a3/src/kfre.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Home-page: https://github.com/lshpaner/kfre
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

