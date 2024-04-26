# Comparing `tmp/kfre-0.1.1a7.tar.gz` & `tmp/kfre-0.1.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfre-0.1.1a7.tar", last modified: Fri Apr 26 06:38:58 2024, max compression
+gzip compressed data, was "kfre-0.1.1a8.tar", last modified: Fri Apr 26 06:56:50 2024, max compression
```

## Comparing `kfre-0.1.1a7.tar` & `kfre-0.1.1a8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 06:38:58.215211 kfre-0.1.1a7/
--rw-rw-rw-   0        0        0     4402 2024-04-26 06:38:58.214211 kfre-0.1.1a7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-26 06:38:58.215211 kfre-0.1.1a7/setup.cfg
--rw-rw-rw-   0        0        0     1149 2024-04-26 06:38:51.000000 kfre-0.1.1a7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:38:58.190694 kfre-0.1.1a7/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 06:38:58.192693 kfre-0.1.1a7/src/kfre/
--rw-rw-rw-   0        0        0       55 2024-04-26 04:56:44.000000 kfre-0.1.1a7/src/kfre/__init__.py
--rw-rw-rw-   0        0        0    12299 2024-04-26 06:08:43.000000 kfre-0.1.1a7/src/kfre/main.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:38:58.213212 kfre-0.1.1a7/src/kfre.egg-info/
--rw-rw-rw-   0        0        0     4402 2024-04-26 06:38:58.000000 kfre-0.1.1a7/src/kfre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-04-26 06:38:58.000000 kfre-0.1.1a7/src/kfre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 06:38:58.000000 kfre-0.1.1a7/src/kfre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-26 06:38:58.000000 kfre-0.1.1a7/src/kfre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-26 06:38:58.000000 kfre-0.1.1a7/src/kfre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 06:56:50.292466 kfre-0.1.1a8/
+-rw-rw-rw-   0        0        0     4520 2024-04-26 06:56:50.291467 kfre-0.1.1a8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-26 06:56:50.292466 kfre-0.1.1a8/setup.cfg
+-rw-rw-rw-   0        0        0     1380 2024-04-26 06:56:10.000000 kfre-0.1.1a8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:56:50.265245 kfre-0.1.1a8/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 06:56:50.268221 kfre-0.1.1a8/src/kfre/
+-rw-rw-rw-   0        0        0       55 2024-04-26 04:56:44.000000 kfre-0.1.1a8/src/kfre/__init__.py
+-rw-rw-rw-   0        0        0    12299 2024-04-26 06:08:43.000000 kfre-0.1.1a8/src/kfre/main.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:56:50.290514 kfre-0.1.1a8/src/kfre.egg-info/
+-rw-rw-rw-   0        0        0     4520 2024-04-26 06:56:50.000000 kfre-0.1.1a8/src/kfre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-04-26 06:56:50.000000 kfre-0.1.1a8/src/kfre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 06:56:50.000000 kfre-0.1.1a8/src/kfre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-26 06:56:50.000000 kfre-0.1.1a8/src/kfre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-26 06:56:50.000000 kfre-0.1.1a8/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.1a7/PKG-INFO` & `kfre-0.1.1a8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.1a7
+Version: 0.1.1a8
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Home-page: https://github.com/lshpaner/kfre
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
+Project-URL: Author Website, https://www.leonshpaner.com
+Project-URL: Source Code, https://github.com/lshpaner/kfre
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.18.5
 Requires-Dist: pandas>=1.0.5
 
-# kfre: Kidney Failure Risk Estimator
+# KFRE: Kidney Failure Risk Estimator
 
 ![PyPI](https://img.shields.io/pypi/v/kfre.svg)
 
 `kfre` is a Python library designed to estimate the risk of chronic kidney disease (CKD) progression over two distinct timelines: 2 years and 5 years. Using Tangri's Kidney Failure Risk Equation (KFRE), the library provides tools for healthcare professionals and researchers to predict CKD risk based on patient data. It supports predictions for both males and females and includes specific adjustments for individuals from North American and non-North American regions.
 
 
 ## Features
```

### Comparing `kfre-0.1.1a7/setup.py` & `kfre-0.1.1a8/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kfre",
-    version="0.1.1-alpha7",
+    version="0.1.1-alpha8",
     author="Leonid Shpaner",
     author_email="Lshpaner@ucla.edu",
     description="A Python library for kidney failure risk estimation using Tangri's KFRE model",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",  # Type of the long description
     url="https://github.com/lshpaner/kfre",  # URL to the repository or documentation
     package_dir={"": "src"},  # Directory where your package files are located
     # Automatically find packages in the specified directory
     packages=find_packages(where="src"),
+    project_urls={  # Optional
+        "Author Website": "https://www.leonshpaner.com",
+        # "Documentation": "https://example.com/project-documentation",
+        "Source Code": "https://github.com/lshpaner/kfre",
+    },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],  # Classifiers for the package
     python_requires=">=3.6",  # Minimum version of Python required
     install_requires=[
```

### Comparing `kfre-0.1.1a7/src/kfre/main.py` & `kfre-0.1.1a8/src/kfre/main.py`

 * *Files identical despite different names*

### Comparing `kfre-0.1.1a7/src/kfre.egg-info/PKG-INFO` & `kfre-0.1.1a8/src/kfre.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.1a7
+Version: 0.1.1a8
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Home-page: https://github.com/lshpaner/kfre
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
+Project-URL: Author Website, https://www.leonshpaner.com
+Project-URL: Source Code, https://github.com/lshpaner/kfre
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.18.5
 Requires-Dist: pandas>=1.0.5
 
-# kfre: Kidney Failure Risk Estimator
+# KFRE: Kidney Failure Risk Estimator
 
 ![PyPI](https://img.shields.io/pypi/v/kfre.svg)
 
 `kfre` is a Python library designed to estimate the risk of chronic kidney disease (CKD) progression over two distinct timelines: 2 years and 5 years. Using Tangri's Kidney Failure Risk Equation (KFRE), the library provides tools for healthcare professionals and researchers to predict CKD risk based on patient data. It supports predictions for both males and females and includes specific adjustments for individuals from North American and non-North American regions.
 
 
 ## Features
```

