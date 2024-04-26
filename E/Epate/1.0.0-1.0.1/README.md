# Comparing `tmp/epate-1.0.0.tar.gz` & `tmp/epate-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epate-1.0.0.tar", last modified: Fri Apr 26 17:14:41 2024, max compression
+gzip compressed data, was "epate-1.0.1.tar", last modified: Fri Apr 26 17:25:45 2024, max compression
```

## Comparing `epate-1.0.0.tar` & `epate-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 17:14:41.439499 epate-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-04-26 17:14:41.346495 epate-1.0.0/Epate/
--rw-rw-rw-   0        0        0        0 2024-04-26 16:39:01.000000 epate-1.0.0/Epate/__init__.py
--rw-rw-rw-   0        0        0     5589 2024-04-26 16:35:52.000000 epate-1.0.0/Epate/epate.py
-drwxrwxrwx   0        0        0        0 2024-04-26 17:14:41.427495 epate-1.0.0/Epate.egg-info/
--rw-rw-rw-   0        0        0      562 2024-04-26 17:14:41.000000 epate-1.0.0/Epate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-26 17:14:41.000000 epate-1.0.0/Epate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 17:14:41.000000 epate-1.0.0/Epate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-26 17:14:41.000000 epate-1.0.0/Epate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-26 17:14:41.000000 epate-1.0.0/Epate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 17:14:41.000000 epate-1.0.0/Epate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      562 2024-04-26 17:14:41.429496 epate-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       66 2024-04-26 15:22:07.000000 epate-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 17:14:41.439499 epate-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      999 2024-04-26 17:07:38.000000 epate-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:25:45.380529 epate-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-04-26 17:25:45.341313 epate-1.0.1/Epate/
+-rw-rw-rw-   0        0        0        0 2024-04-26 16:39:01.000000 epate-1.0.1/Epate/__init__.py
+-rw-rw-rw-   0        0        0     5589 2024-04-26 16:35:52.000000 epate-1.0.1/Epate/epate.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:25:45.376438 epate-1.0.1/Epate.egg-info/
+-rw-rw-rw-   0        0        0      562 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 17:25:45.000000 epate-1.0.1/Epate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      562 2024-04-26 17:25:45.377441 epate-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2024-04-26 15:22:07.000000 epate-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 17:25:45.380529 epate-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      901 2024-04-26 17:25:43.000000 epate-1.0.1/setup.py
```

### Comparing `epate-1.0.0/Epate/epate.py` & `epate-1.0.1/Epate/epate.py`

 * *Files identical despite different names*

### Comparing `epate-1.0.0/Epate.egg-info/PKG-INFO` & `epate-1.0.1/Epate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.0/LICENSE` & `epate-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epate-1.0.0/PKG-INFO` & `epate-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.0/setup.py` & `epate-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
  
 from pkg_resources import parse_requirements
-with open("requirements.txt", encoding="utf-8") as fp:
-    install_requires = [str(requirement) for requirement in parse_requirements(fp)]
+
+install_requires = ['requests==2.31.0']
  
 setup(
     name="Epate",
-    version="1.0.0",
+    version="1.0.1",
     author="xiaoxlh",
     author_email="xiaoxiaogzs@outlook.com",
     description="A python library for many API of the codemao's website.",
     long_description="eds sdk for python",
     license="Apache License, Version 2.0",
     url="https://xiao.asia",
```

