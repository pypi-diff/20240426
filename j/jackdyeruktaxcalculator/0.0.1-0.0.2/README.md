# Comparing `tmp/jackdyeruktaxcalculator-0.0.1.tar.gz` & `tmp/jackdyeruktaxcalculator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jackdyeruktaxcalculator-0.0.1.tar", last modified: Fri Apr 26 17:08:49 2024, max compression
+gzip compressed data, was "jackdyeruktaxcalculator-0.0.2.tar", last modified: Fri Apr 26 17:22:05 2024, max compression
```

## Comparing `jackdyeruktaxcalculator-0.0.1.tar` & `jackdyeruktaxcalculator-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 17:08:49.202873 jackdyeruktaxcalculator-0.0.1/
--rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      512 2024-04-26 17:08:49.200878 jackdyeruktaxcalculator-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 17:08:49.199881 jackdyeruktaxcalculator-0.0.1/jackdyeruktaxcalculator.egg-info/
--rw-rw-rw-   0        0        0      512 2024-04-26 17:08:49.000000 jackdyeruktaxcalculator-0.0.1/jackdyeruktaxcalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-04-26 17:08:49.000000 jackdyeruktaxcalculator-0.0.1/jackdyeruktaxcalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 17:08:49.000000 jackdyeruktaxcalculator-0.0.1/jackdyeruktaxcalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-26 17:08:49.000000 jackdyeruktaxcalculator-0.0.1/jackdyeruktaxcalculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 17:08:49.202873 jackdyeruktaxcalculator-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      645 2024-04-26 17:08:38.000000 jackdyeruktaxcalculator-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 17:08:49.195892 jackdyeruktaxcalculator-0.0.1/source/
--rw-rw-rw-   0        0        0        0 2024-04-26 13:27:18.000000 jackdyeruktaxcalculator-0.0.1/source/__init__.py
--rw-rw-rw-   0        0        0     4605 2024-03-18 10:56:49.000000 jackdyeruktaxcalculator-0.0.1/source/income_calculator.py
-drwxrwxrwx   0        0        0        0 2024-04-26 17:08:49.198884 jackdyeruktaxcalculator-0.0.1/test/
--rw-rw-rw-   0        0        0        0 2024-04-26 13:35:04.000000 jackdyeruktaxcalculator-0.0.1/test/__init__.py
--rw-rw-rw-   0        0        0     9566 2024-04-26 13:34:45.000000 jackdyeruktaxcalculator-0.0.1/test/test_income_calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:22:05.189237 jackdyeruktaxcalculator-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      512 2024-04-26 17:22:05.188238 jackdyeruktaxcalculator-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 17:22:05.188238 jackdyeruktaxcalculator-0.0.2/jackdyeruktaxcalculator.egg-info/
+-rw-rw-rw-   0        0        0      512 2024-04-26 17:22:05.000000 jackdyeruktaxcalculator-0.0.2/jackdyeruktaxcalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-04-26 17:22:05.000000 jackdyeruktaxcalculator-0.0.2/jackdyeruktaxcalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 17:22:05.000000 jackdyeruktaxcalculator-0.0.2/jackdyeruktaxcalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-26 17:22:05.000000 jackdyeruktaxcalculator-0.0.2/jackdyeruktaxcalculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 17:22:05.189237 jackdyeruktaxcalculator-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      645 2024-04-26 17:21:55.000000 jackdyeruktaxcalculator-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:22:05.185247 jackdyeruktaxcalculator-0.0.2/source/
+-rw-rw-rw-   0        0        0        0 2024-04-26 13:27:18.000000 jackdyeruktaxcalculator-0.0.2/source/__init__.py
+-rw-rw-rw-   0        0        0     4605 2024-03-18 10:56:49.000000 jackdyeruktaxcalculator-0.0.2/source/income_calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:22:05.187241 jackdyeruktaxcalculator-0.0.2/test/
+-rw-rw-rw-   0        0        0        0 2024-04-26 13:35:04.000000 jackdyeruktaxcalculator-0.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0     9566 2024-04-26 13:34:45.000000 jackdyeruktaxcalculator-0.0.2/test/test_income_calculator.py
```

### Comparing `jackdyeruktaxcalculator-0.0.1/LICENSE` & `jackdyeruktaxcalculator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jackdyeruktaxcalculator-0.0.1/PKG-INFO` & `jackdyeruktaxcalculator-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jackdyeruktaxcalculator
-Version: 0.0.1
+Version: 0.0.2
 Summary: UK Tax Calculator
 Home-page: https://github.com/jackLDyer/uk-tax-calculator
 Author: Jack Dyer
 Author-email: jack.dyer387@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jackdyeruktaxcalculator-0.0.1/jackdyeruktaxcalculator.egg-info/PKG-INFO` & `jackdyeruktaxcalculator-0.0.2/jackdyeruktaxcalculator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jackdyeruktaxcalculator
-Version: 0.0.1
+Version: 0.0.2
 Summary: UK Tax Calculator
 Home-page: https://github.com/jackLDyer/uk-tax-calculator
 Author: Jack Dyer
 Author-email: jack.dyer387@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jackdyeruktaxcalculator-0.0.1/setup.py` & `jackdyeruktaxcalculator-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jackdyeruktaxcalculator",
-    version="0.0.1",
+    version="0.0.2",
     author="Jack Dyer",
     author_email="jack.dyer387@gmail.com",
     description="UK Tax Calculator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jackLDyer/uk-tax-calculator",
     packages=setuptools.find_packages(),
```

### Comparing `jackdyeruktaxcalculator-0.0.1/source/income_calculator.py` & `jackdyeruktaxcalculator-0.0.2/source/income_calculator.py`

 * *Files identical despite different names*

### Comparing `jackdyeruktaxcalculator-0.0.1/test/test_income_calculator.py` & `jackdyeruktaxcalculator-0.0.2/test/test_income_calculator.py`

 * *Files identical despite different names*

