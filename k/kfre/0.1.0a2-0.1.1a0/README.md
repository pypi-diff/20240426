# Comparing `tmp/kfre-0.1.0a2.tar.gz` & `tmp/kfre-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfre-0.1.0a2.tar", last modified: Fri Apr 26 04:53:00 2024, max compression
+gzip compressed data, was "kfre-0.1.1a0.tar", last modified: Fri Apr 26 05:00:34 2024, max compression
```

## Comparing `kfre-0.1.0a2.tar` & `kfre-0.1.1a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 04:53:00.229230 kfre-0.1.0a2/
--rw-rw-rw-   0        0        0     4409 2024-04-26 04:53:00.227318 kfre-0.1.0a2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-26 04:53:00.229230 kfre-0.1.0a2/setup.cfg
--rw-rw-rw-   0        0        0     1149 2024-04-26 04:52:56.000000 kfre-0.1.0a2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 04:53:00.209175 kfre-0.1.0a2/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 04:53:00.226234 kfre-0.1.0a2/src/kfre.egg-info/
--rw-rw-rw-   0        0        0     4409 2024-04-26 04:53:00.000000 kfre-0.1.0a2/src/kfre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-04-26 04:53:00.000000 kfre-0.1.0a2/src/kfre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 04:53:00.000000 kfre-0.1.0a2/src/kfre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-26 04:53:00.000000 kfre-0.1.0a2/src/kfre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 04:53:00.000000 kfre-0.1.0a2/src/kfre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 05:00:34.896618 kfre-0.1.1a0/
+-rw-rw-rw-   0        0        0     4402 2024-04-26 05:00:34.895624 kfre-0.1.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-26 05:00:34.896618 kfre-0.1.1a0/setup.cfg
+-rw-rw-rw-   0        0        0     1148 2024-04-26 05:00:24.000000 kfre-0.1.1a0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:00:34.881457 kfre-0.1.1a0/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 05:00:34.894605 kfre-0.1.1a0/src/kfre.egg-info/
+-rw-rw-rw-   0        0        0     4402 2024-04-26 05:00:34.000000 kfre-0.1.1a0/src/kfre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-04-26 05:00:34.000000 kfre-0.1.1a0/src/kfre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 05:00:34.000000 kfre-0.1.1a0/src/kfre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-26 05:00:34.000000 kfre-0.1.1a0/src/kfre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 05:00:34.000000 kfre-0.1.1a0/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.0a2/PKG-INFO` & `kfre-0.1.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.0a2
+Version: 0.1.1a0
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Home-page: https://github.com/lshpaner/kfre
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 ![PyPI](https://img.shields.io/pypi/v/kfre.svg)
 
 `kfre` is a Python library designed to estimate the risk of chronic kidney disease (CKD) progression over two distinct timelines: 2 years and 5 years. Using Tangri's Kidney Failure Risk Equation (KFRE), the library provides tools for healthcare professionals and researchers to predict CKD risk based on patient data. It supports predictions for both males and females and includes specific adjustments for individuals from North American and non-North American regions.
 
 
 ## Features
 
-- **Risk Prediction**: Utilize Tangriâ€™s validated risk prediction model to estimate kidney failure risk using
+- **Risk Prediction**: Utilize Tangri's validated risk prediction model to estimate kidney failure risk using
     - 4 variables: sex, age, eGFR, uACR (log-normalized)
     - 6 variables: sex, age, eGFR, uACR (log-normalized), diabetes mellitus, hypertension
     - 8 variables: sex, age, eGFR, uACR (log-normalized), serum albumin, serum phosphorous, serum calcium, and serum bicarbonate.
 - **Data Flexibility**: Handles various input data formats and maps them to required model parameters.
 - **Conversion Utilities**: Includes functions to convert common laboratory results to the required units for risk prediction.
 
 ## Important Note on Data Units
```

### Comparing `kfre-0.1.0a2/setup.py` & `kfre-0.1.1a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kfre",
-    version="0.1.0-alpha2",
+    version="0.1.1-alpha",
     author="Leonid Shpaner",
     author_email="Lshpaner@ucla.edu",
     description="A Python library for kidney failure risk estimation using Tangri's KFRE model",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",  # Type of the long description
     url="https://github.com/lshpaner/kfre",  # URL to the repository or documentation
     package_dir={"": "src"},  # Directory where your package files are located
```

### Comparing `kfre-0.1.0a2/src/kfre.egg-info/PKG-INFO` & `kfre-0.1.1a0/src/kfre.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.0a2
+Version: 0.1.1a0
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Home-page: https://github.com/lshpaner/kfre
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 ![PyPI](https://img.shields.io/pypi/v/kfre.svg)
 
 `kfre` is a Python library designed to estimate the risk of chronic kidney disease (CKD) progression over two distinct timelines: 2 years and 5 years. Using Tangri's Kidney Failure Risk Equation (KFRE), the library provides tools for healthcare professionals and researchers to predict CKD risk based on patient data. It supports predictions for both males and females and includes specific adjustments for individuals from North American and non-North American regions.
 
 
 ## Features
 
-- **Risk Prediction**: Utilize Tangriâ€™s validated risk prediction model to estimate kidney failure risk using
+- **Risk Prediction**: Utilize Tangri's validated risk prediction model to estimate kidney failure risk using
     - 4 variables: sex, age, eGFR, uACR (log-normalized)
     - 6 variables: sex, age, eGFR, uACR (log-normalized), diabetes mellitus, hypertension
     - 8 variables: sex, age, eGFR, uACR (log-normalized), serum albumin, serum phosphorous, serum calcium, and serum bicarbonate.
 - **Data Flexibility**: Handles various input data formats and maps them to required model parameters.
 - **Conversion Utilities**: Includes functions to convert common laboratory results to the required units for risk prediction.
 
 ## Important Note on Data Units
```

