# Comparing `tmp/epate-1.0.1.tar.gz` & `tmp/epate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epate-1.0.1.tar", last modified: Fri Apr 26 17:25:45 2024, max compression
+gzip compressed data, was "epate-1.0.2.tar", last modified: Fri Apr 26 17:42:13 2024, max compression
```

## Comparing `epate-1.0.1.tar` & `epate-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 17:25:45.380529 epate-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-26 17:25:45.341313 epate-1.0.1/Epate/
--rw-rw-rw-   0        0        0        0 2024-04-26 16:39:01.000000 epate-1.0.1/Epate/__init__.py
--rw-rw-rw-   0        0        0     5589 2024-04-26 16:35:52.000000 epate-1.0.1/Epate/epate.py
-drwxrwxrwx   0        0        0        0 2024-04-26 17:25:45.376438 epate-1.0.1/Epate.egg-info/
--rw-rw-rw-   0        0        0      562 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      562 2024-04-26 17:25:45.377441 epate-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       66 2024-04-26 15:22:07.000000 epate-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 17:25:45.380529 epate-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      901 2024-04-26 17:25:43.000000 epate-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:42:13.306277 epate-1.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-26 17:42:13.258966 epate-1.0.2/Epate/
+-rw-rw-rw-   0        0        0       21 2024-04-26 17:40:18.000000 epate-1.0.2/Epate/__init__.py
+-rw-rw-rw-   0        0        0     5589 2024-04-26 16:35:52.000000 epate-1.0.2/Epate/epate.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:42:13.300935 epate-1.0.2/Epate.egg-info/
+-rw-rw-rw-   0        0        0      562 2024-04-26 17:42:13.000000 epate-1.0.2/Epate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-26 17:42:13.000000 epate-1.0.2/Epate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 17:42:13.000000 epate-1.0.2/Epate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-26 17:42:13.000000 epate-1.0.2/Epate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-26 17:42:13.000000 epate-1.0.2/Epate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 17:42:13.000000 epate-1.0.2/Epate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      562 2024-04-26 17:42:13.302936 epate-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2024-04-26 15:22:07.000000 epate-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 17:42:13.307278 epate-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      901 2024-04-26 17:40:41.000000 epate-1.0.2/setup.py
```

### Comparing `epate-1.0.1/Epate/epate.py` & `epate-1.0.2/Epate/epate.py`

 * *Files identical despite different names*

### Comparing `epate-1.0.1/Epate.egg-info/PKG-INFO` & `epate-1.0.2/Epate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.1/LICENSE` & `epate-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epate-1.0.1/PKG-INFO` & `epate-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.1/setup.py` & `epate-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  
 from pkg_resources import parse_requirements
 
 install_requires = ['requests==2.31.0']
  
 setup(
     name="Epate",
-    version="1.0.1",
+    version="1.0.2",
     author="xiaoxlh",
     author_email="xiaoxiaogzs@outlook.com",
     description="A python library for many API of the codemao's website.",
     long_description="eds sdk for python",
     license="Apache License, Version 2.0",
     url="https://xiao.asia",
```

