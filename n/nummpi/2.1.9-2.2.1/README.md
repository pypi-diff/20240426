# Comparing `tmp/nummpi-2.1.9.tar.gz` & `tmp/nummpi-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nummpi-2.1.9.tar", last modified: Wed Apr 24 17:47:50 2024, max compression
+gzip compressed data, was "nummpi-2.2.1.tar", last modified: Fri Apr 26 02:48:27 2024, max compression
```

## Comparing `nummpi-2.1.9.tar` & `nummpi-2.2.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 17:47:50.327103 nummpi-2.1.9/
--rw-rw-rw-   0        0        0     1088 2024-04-22 12:14:20.000000 nummpi-2.1.9/LICENSE
--rw-rw-rw-   0        0        0      976 2024-04-24 17:47:50.326103 nummpi-2.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 17:47:50.306376 nummpi-2.1.9/nummpi/
--rw-rw-rw-   0        0        0        0 2024-04-22 12:21:04.000000 nummpi-2.1.9/nummpi/__init__.py
--rw-rw-rw-   0        0        0     1602 2024-04-24 17:39:27.000000 nummpi-2.1.9/nummpi/brand.py
--rw-rw-rw-   0        0        0     2322 2024-04-24 17:39:27.000000 nummpi-2.1.9/nummpi/competitor.py
--rw-rw-rw-   0        0        0     2516 2024-04-24 17:39:27.000000 nummpi-2.1.9/nummpi/content.py
--rw-rw-rw-   0        0        0     2199 2024-04-24 17:39:27.000000 nummpi-2.1.9/nummpi/eda.py
--rw-rw-rw-   0        0        0     2387 2024-04-24 17:39:27.000000 nummpi-2.1.9/nummpi/engagement.py
--rw-rw-rw-   0        0        0     3176 2024-04-24 17:39:27.000000 nummpi-2.1.9/nummpi/hashtag.py
--rw-rw-rw-   0        0        0     1933 2024-04-24 17:39:27.000000 nummpi-2.1.9/nummpi/location.py
--rw-rw-rw-   0        0        0     1877 2024-04-24 17:39:27.000000 nummpi-2.1.9/nummpi/network.py
--rw-rw-rw-   0        0        0     2195 2024-04-24 17:39:27.000000 nummpi-2.1.9/nummpi/sentiment.py
--rw-rw-rw-   0        0        0     2052 2024-04-24 17:39:27.000000 nummpi-2.1.9/nummpi/trend.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:47:50.325091 nummpi-2.1.9/nummpi.egg-info/
--rw-rw-rw-   0        0        0      976 2024-04-24 17:47:50.000000 nummpi-2.1.9/nummpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2024-04-24 17:47:50.000000 nummpi-2.1.9/nummpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 17:47:50.000000 nummpi-2.1.9/nummpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 17:47:50.000000 nummpi-2.1.9/nummpi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 17:47:50.328107 nummpi-2.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1227 2024-04-24 17:47:47.000000 nummpi-2.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:48:27.332944 nummpi-2.2.1/
+-rw-rw-rw-   0        0        0     1088 2024-04-22 12:14:20.000000 nummpi-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0      976 2024-04-26 02:48:27.332944 nummpi-2.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 02:48:27.304940 nummpi-2.2.1/nummpi/
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:21:04.000000 nummpi-2.2.1/nummpi/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-04-24 17:59:56.000000 nummpi-2.2.1/nummpi/brand.py
+-rw-rw-rw-   0        0        0     2324 2024-04-25 15:49:04.000000 nummpi-2.2.1/nummpi/competitor.py
+-rw-rw-rw-   0        0        0     2516 2024-04-24 17:39:27.000000 nummpi-2.2.1/nummpi/content.py
+-rw-rw-rw-   0        0        0     2199 2024-04-24 17:39:27.000000 nummpi-2.2.1/nummpi/eda.py
+-rw-rw-rw-   0        0        0     2387 2024-04-24 17:39:27.000000 nummpi-2.2.1/nummpi/engagement.py
+-rw-rw-rw-   0        0        0     3176 2024-04-24 17:39:27.000000 nummpi-2.2.1/nummpi/hashtag.py
+-rw-rw-rw-   0        0        0     1933 2024-04-24 17:39:27.000000 nummpi-2.2.1/nummpi/location.py
+-rw-rw-rw-   0        0        0     1877 2024-04-24 17:39:27.000000 nummpi-2.2.1/nummpi/network.py
+-rw-rw-rw-   0        0        0     2728 2024-04-25 17:53:40.000000 nummpi-2.2.1/nummpi/preprocessing.py
+-rw-rw-rw-   0        0        0     2195 2024-04-24 17:39:27.000000 nummpi-2.2.1/nummpi/sentiment.py
+-rw-rw-rw-   0        0        0     2052 2024-04-24 17:39:27.000000 nummpi-2.2.1/nummpi/trend.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:48:27.332944 nummpi-2.2.1/nummpi.egg-info/
+-rw-rw-rw-   0        0        0      976 2024-04-26 02:48:26.000000 nummpi-2.2.1/nummpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-04-26 02:48:27.000000 nummpi-2.2.1/nummpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 02:48:26.000000 nummpi-2.2.1/nummpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 02:48:26.000000 nummpi-2.2.1/nummpi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 02:48:27.332944 nummpi-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1227 2024-04-26 02:48:17.000000 nummpi-2.2.1/setup.py
```

### Comparing `nummpi-2.1.9/LICENSE` & `nummpi-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nummpi-2.1.9/PKG-INFO` & `nummpi-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nummpi
-Version: 2.1.9
+Version: 2.2.1
 Summary: A package that facilitates efficient coding and development
 Author: Tom Hanks
 Author-email: <tomhanks02@gmail.com>
 Keywords: python,development,productivity,utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nummpi-2.1.9/nummpi/brand.py` & `nummpi-2.2.1/nummpi/brand.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-# -*- coding: utf-8 -*-
-"""sma_8_brand_prac_exam.ipynb
-
-Automatically generated by Colab.
-
-Original file is located at
-    https://colab.research.google.com/drive/1e9WKG65l70a-AaMlcf-m_uK2-FPfuHJf
-"""
-
-#Brand Analysis
+# Brand Analysis
 
 import pandas as pd
 import matplotlib.pyplot as plt
 import nltk
 from wordcloud import WordCloud
 from nltk.tokenize import word_tokenize
 from nltk.corpus import stopwords
@@ -19,15 +10,15 @@
 
 nltk.download('stopwords')
 nltk.download('wordnet')
 nltk.download('punkt')
 nltk.download('vader_lexicon')
 
 # Read data from CSV file
-df = pd.read_csv('/content/drive/MyDrive/SMA_datasets_prac_exam/tweets.csv')  # Replace 'your_dataset.csv' with your CSV file path
+df = pd.read_csv('tweets.csv')  # Replace 'your_dataset.csv' with your CSV file path
 
 # Text preprocessing
 stop_words = set(stopwords.words('english'))
 sia = SentimentIntensityAnalyzer()
 
 def preprocess_text(text):
     tokens = word_tokenize(text.lower())
```

### Comparing `nummpi-2.1.9/nummpi/competitor.py` & `nummpi-2.2.1/nummpi/competitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Automatically generated by Colab.
 
 Original file is located at
     https://colab.research.google.com/drive/1GUb9yHFwhxNCV2EzLhfEexNBzluhHJWj
 """
 
-!pip install rake_nltk
+# !pip install rake_nltk
 
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 from collections import Counter
 from nltk.tokenize import word_tokenize
 from nltk.corpus import stopwords
```

### Comparing `nummpi-2.1.9/nummpi/content.py` & `nummpi-2.2.1/nummpi/content.py`

 * *Files identical despite different names*

### Comparing `nummpi-2.1.9/nummpi/eda.py` & `nummpi-2.2.1/nummpi/eda.py`

 * *Files identical despite different names*

### Comparing `nummpi-2.1.9/nummpi/engagement.py` & `nummpi-2.2.1/nummpi/engagement.py`

 * *Files identical despite different names*

### Comparing `nummpi-2.1.9/nummpi/hashtag.py` & `nummpi-2.2.1/nummpi/hashtag.py`

 * *Files identical despite different names*

### Comparing `nummpi-2.1.9/nummpi/location.py` & `nummpi-2.2.1/nummpi/location.py`

 * *Files identical despite different names*

### Comparing `nummpi-2.1.9/nummpi/network.py` & `nummpi-2.2.1/nummpi/network.py`

 * *Files identical despite different names*

### Comparing `nummpi-2.1.9/nummpi/sentiment.py` & `nummpi-2.2.1/nummpi/sentiment.py`

 * *Files identical despite different names*

### Comparing `nummpi-2.1.9/nummpi/trend.py` & `nummpi-2.2.1/nummpi/trend.py`

 * *Files identical despite different names*

### Comparing `nummpi-2.1.9/nummpi.egg-info/PKG-INFO` & `nummpi-2.2.1/nummpi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nummpi
-Version: 2.1.9
+Version: 2.2.1
 Summary: A package that facilitates efficient coding and development
 Author: Tom Hanks
 Author-email: <tomhanks02@gmail.com>
 Keywords: python,development,productivity,utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nummpi-2.1.9/setup.py` & `nummpi-2.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.1.9'
+VERSION = '2.2.1'
 DESCRIPTION = 'A package that facilitates efficient coding and development'
 LONG_DESCRIPTION = '''
 Pandaz is a Python package designed to enhance coding productivity and streamline development workflows. 
 It provides utilities and tools that simplify common programming tasks, allowing users to write cleaner, 
 more concise code with fewer lines. Pandaz aims to empower developers to focus more on problem-solving 
 and less on boilerplate code.
 '''
```

