# Comparing `tmp/uyghur-tili-quralliri-0.1.3.tar.gz` & `tmp/uyghur-tili-quralliri-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uyghur-tili-quralliri-0.1.3.tar", last modified: Thu Apr 25 12:24:35 2024, max compression
+gzip compressed data, was "uyghur-tili-quralliri-0.1.4.tar", last modified: Thu Apr 25 12:32:05 2024, max compression
```

## Comparing `uyghur-tili-quralliri-0.1.3.tar` & `uyghur-tili-quralliri-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 12:24:35.471386 uyghur-tili-quralliri-0.1.3/
--rw-rw-rw-   0        0        0      973 2024-04-25 12:24:35.471386 uyghur-tili-quralliri-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-04-25 12:24:06.000000 uyghur-tili-quralliri-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 12:24:35.472390 uyghur-tili-quralliri-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      889 2024-04-25 12:23:43.000000 uyghur-tili-quralliri-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:24:35.464405 uyghur-tili-quralliri-0.1.3/uyghur_language_tools/
--rw-rw-rw-   0        0        0   104707 2024-04-25 12:24:35.000000 uyghur-tili-quralliri-0.1.3/uyghur_language_tools/UyghurLanguageTools.py
--rw-rw-rw-   0        0        0       92 2024-04-25 12:19:03.000000 uyghur-tili-quralliri-0.1.3/uyghur_language_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:24:35.470407 uyghur-tili-quralliri-0.1.3/uyghur_tili_quralliri.egg-info/
--rw-rw-rw-   0        0        0      973 2024-04-25 12:24:35.000000 uyghur-tili-quralliri-0.1.3/uyghur_tili_quralliri.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-25 12:24:35.000000 uyghur-tili-quralliri-0.1.3/uyghur_tili_quralliri.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 12:24:35.000000 uyghur-tili-quralliri-0.1.3/uyghur_tili_quralliri.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-25 12:24:35.000000 uyghur-tili-quralliri-0.1.3/uyghur_tili_quralliri.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 12:32:05.435607 uyghur-tili-quralliri-0.1.4/
+-rw-rw-rw-   0        0        0      970 2024-04-25 12:32:05.434610 uyghur-tili-quralliri-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2024-04-25 12:29:42.000000 uyghur-tili-quralliri-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 12:32:05.435607 uyghur-tili-quralliri-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      889 2024-04-25 12:30:54.000000 uyghur-tili-quralliri-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:32:05.426632 uyghur-tili-quralliri-0.1.4/uyghur_language_tools/
+-rw-rw-rw-   0        0        0   104707 2024-04-25 12:32:05.000000 uyghur-tili-quralliri-0.1.4/uyghur_language_tools/UyghurLanguageTools.py
+-rw-rw-rw-   0        0        0       92 2024-04-25 12:19:03.000000 uyghur-tili-quralliri-0.1.4/uyghur_language_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:32:05.432614 uyghur-tili-quralliri-0.1.4/uyghur_tili_quralliri.egg-info/
+-rw-rw-rw-   0        0        0      970 2024-04-25 12:32:05.000000 uyghur-tili-quralliri-0.1.4/uyghur_tili_quralliri.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-25 12:32:05.000000 uyghur-tili-quralliri-0.1.4/uyghur_tili_quralliri.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 12:32:05.000000 uyghur-tili-quralliri-0.1.4/uyghur_tili_quralliri.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-25 12:32:05.000000 uyghur-tili-quralliri-0.1.4/uyghur_tili_quralliri.egg-info/top_level.txt
```

### Comparing `uyghur-tili-quralliri-0.1.3/PKG-INFO` & `uyghur-tili-quralliri-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uyghur-tili-quralliri
-Version: 0.1.3
+Version: 0.1.4
 Summary: uyghur language writing and processing tool box ...
 Home-page: https://github.com/kompasim/uyghur-tili-quralliri
 Author: kompasim
 Author-email: kompasim@163.com
 License: MIT Licence
 Keywords: uyghur,uighur,til,yeziq,qural,language,tools
 Platform: any
@@ -18,15 +18,15 @@
 ## 0. Description
 
 > a tool box including some useful functions to handle with uyghur writing ...
 
 ## 1. Installing
 
 ```cmd
-pip install -g uyghur-tili-quralliri
+pip install uyghur-tili-quralliri
 ```
 
 ## 2. Usage
 
 ```python
 from uyghur_language_tools.UyghurLanguageTools import UyghurLanguageTools as Tools
 Tools.main()
```

### Comparing `uyghur-tili-quralliri-0.1.3/setup.py` & `uyghur-tili-quralliri-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "uyghur-tili-quralliri",
-    version = "0.1.3",
+    version = "0.1.4",
     keywords = ("uyghur", "uighur","til", "yeziq", "qural", "language", "tools"),
     description = "uyghur language writing and processing tool box ...",
     long_description = long_description,
     long_description_content_type="text/markdown",
     license = "MIT Licence",
 
     url = "https://github.com/kompasim/uyghur-tili-quralliri",
```

### Comparing `uyghur-tili-quralliri-0.1.3/uyghur_language_tools/UyghurLanguageTools.py` & `uyghur-tili-quralliri-0.1.4/uyghur_language_tools/UyghurLanguageTools.py`

 * *Files identical despite different names*

### Comparing `uyghur-tili-quralliri-0.1.3/uyghur_tili_quralliri.egg-info/PKG-INFO` & `uyghur-tili-quralliri-0.1.4/uyghur_tili_quralliri.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uyghur-tili-quralliri
-Version: 0.1.3
+Version: 0.1.4
 Summary: uyghur language writing and processing tool box ...
 Home-page: https://github.com/kompasim/uyghur-tili-quralliri
 Author: kompasim
 Author-email: kompasim@163.com
 License: MIT Licence
 Keywords: uyghur,uighur,til,yeziq,qural,language,tools
 Platform: any
@@ -18,15 +18,15 @@
 ## 0. Description
 
 > a tool box including some useful functions to handle with uyghur writing ...
 
 ## 1. Installing
 
 ```cmd
-pip install -g uyghur-tili-quralliri
+pip install uyghur-tili-quralliri
 ```
 
 ## 2. Usage
 
 ```python
 from uyghur_language_tools.UyghurLanguageTools import UyghurLanguageTools as Tools
 Tools.main()
```

