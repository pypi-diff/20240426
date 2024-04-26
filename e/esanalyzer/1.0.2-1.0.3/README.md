# Comparing `tmp/esanalyzer-1.0.2.tar.gz` & `tmp/esanalyzer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esanalyzer-1.0.2.tar", last modified: Thu Apr 25 15:19:47 2024, max compression
+gzip compressed data, was "esanalyzer-1.0.3.tar", last modified: Thu Apr 25 15:25:06 2024, max compression
```

## Comparing `esanalyzer-1.0.2.tar` & `esanalyzer-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 15:19:47.310021 esanalyzer-1.0.2/
--rw-rw-rw-   0        0        0     1074 2024-04-25 11:23:48.000000 esanalyzer-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1071 2024-04-25 15:19:47.308247 esanalyzer-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      494 2024-04-25 14:16:26.000000 esanalyzer-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 15:19:47.283762 esanalyzer-1.0.2/esanalyzer/
-drwxrwxrwx   0        0        0        0 2024-04-25 15:19:47.301264 esanalyzer-1.0.2/esanalyzer/src/
-drwxrwxrwx   0        0        0        0 2024-04-25 15:19:47.306250 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/
--rw-rw-rw-   0        0        0     1071 2024-04-25 15:19:47.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-04-25 15:19:47.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 15:19:47.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2024-04-25 15:19:47.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-25 15:19:47.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    23767 2024-04-25 13:08:05.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.py
--rw-rw-rw-   0        0        0       42 2024-04-25 15:19:47.310021 esanalyzer-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1316 2024-04-25 15:18:54.000000 esanalyzer-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:25:06.479287 esanalyzer-1.0.3/
+-rw-rw-rw-   0        0        0     1074 2024-04-25 11:23:48.000000 esanalyzer-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1289 2024-04-25 15:25:06.477293 esanalyzer-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2024-04-25 14:16:26.000000 esanalyzer-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 15:25:06.452656 esanalyzer-1.0.3/esanalyzer/
+drwxrwxrwx   0        0        0        0 2024-04-25 15:25:06.470240 esanalyzer-1.0.3/esanalyzer/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 15:25:06.474235 esanalyzer-1.0.3/esanalyzer/src/esanalyzer.egg-info/
+-rw-rw-rw-   0        0        0     1289 2024-04-25 15:25:06.000000 esanalyzer-1.0.3/esanalyzer/src/esanalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-04-25 15:25:06.000000 esanalyzer-1.0.3/esanalyzer/src/esanalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 15:25:06.000000 esanalyzer-1.0.3/esanalyzer/src/esanalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-04-25 15:25:06.000000 esanalyzer-1.0.3/esanalyzer/src/esanalyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 15:25:06.000000 esanalyzer-1.0.3/esanalyzer/src/esanalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    23767 2024-04-25 13:08:05.000000 esanalyzer-1.0.3/esanalyzer/src/esanalyzer.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 15:25:06.479287 esanalyzer-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1534 2024-04-25 15:24:49.000000 esanalyzer-1.0.3/setup.py
```

### Comparing `esanalyzer-1.0.2/LICENSE` & `esanalyzer-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `esanalyzer-1.0.2/PKG-INFO` & `esanalyzer-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esanalyzer
-Version: 1.0.2
+Version: 1.0.3
 Summary: Emotion and Sentiment Analysis
 Home-page: https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer
 Author: Ajay Singh Rajput
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nrclex
@@ -30,13 +30,17 @@
     ```python
     from esanalyzer.emotion_analyzer import EmotionAnalyzer
 
     # Create an instance of EmotionAnalyzer
     analyzer = EmotionAnalyzer()
 
     # Call the analyze method with the text
-    text = "This is a test text."
+    text = "Wow, I am so happy"
     result = analyzer.analyze(text)
 
     # Use the result as needed
     print(result)
     
+    
+    {'library': 'default', 'result': {'surprise': 80}, 'max_prediction': {'label': 'surprise', 'percentage': 80}, 'sentiment': 'Positive', 'sentiment_score': 0.999592125415802, 'threshold_value': 0.8}
+    
+
```

### Comparing `esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/PKG-INFO` & `esanalyzer-1.0.3/esanalyzer/src/esanalyzer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esanalyzer
-Version: 1.0.2
+Version: 1.0.3
 Summary: Emotion and Sentiment Analysis
 Home-page: https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer
 Author: Ajay Singh Rajput
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nrclex
@@ -30,13 +30,17 @@
     ```python
     from esanalyzer.emotion_analyzer import EmotionAnalyzer
 
     # Create an instance of EmotionAnalyzer
     analyzer = EmotionAnalyzer()
 
     # Call the analyze method with the text
-    text = "This is a test text."
+    text = "Wow, I am so happy"
     result = analyzer.analyze(text)
 
     # Use the result as needed
     print(result)
     
+    
+    {'library': 'default', 'result': {'surprise': 80}, 'max_prediction': {'label': 'surprise', 'percentage': 80}, 'sentiment': 'Positive', 'sentiment_score': 0.999592125415802, 'threshold_value': 0.8}
+    
+
```

### Comparing `esanalyzer-1.0.2/esanalyzer/src/esanalyzer.py` & `esanalyzer-1.0.3/esanalyzer/src/esanalyzer.py`

 * *Files identical despite different names*

### Comparing `esanalyzer-1.0.2/setup.py` & `esanalyzer-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='esanalyzer',
-    version='1.0.2',
+    version='1.0.3',
     author='Ajay Singh Rajput',
     description='Emotion and Sentiment Analysis',
     url='https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer',
     long_description="""# esanalyzer
 
     The Python Emotion and Sentiment Analysis library you've been looking for.
 
@@ -20,19 +20,23 @@
     ```python
     from esanalyzer.emotion_analyzer import EmotionAnalyzer
 
     # Create an instance of EmotionAnalyzer
     analyzer = EmotionAnalyzer()
 
     # Call the analyze method with the text
-    text = "This is a test text."
+    text = "Wow, I am so happy"
     result = analyzer.analyze(text)
 
     # Use the result as needed
     print(result)
+    
+    
+    {'library': 'default', 'result': {'surprise': 80}, 'max_prediction': {'label': 'surprise', 'percentage': 80}, 'sentiment': 'Positive', 'sentiment_score': 0.999592125415802, 'threshold_value': 0.8}
+    
     """,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
     py_modules=["esanalyzer"],
     packages=find_packages(),
     install_requires=[
         'nrclex',
```

