# Comparing `tmp/asciicards-0.0.8.0.tar.gz` & `tmp/asciicards-0.0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciicards-0.0.8.0.tar", last modified: Wed Apr 17 01:26:47 2024, max compression
+gzip compressed data, was "asciicards-0.0.8.1.tar", last modified: Fri Apr 26 19:00:33 2024, max compression
```

## Comparing `asciicards-0.0.8.0.tar` & `asciicards-0.0.8.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 01:26:47.293310 asciicards-0.0.8.0/
--rw-rw-rw-   0        0        0    35149 2023-05-06 18:11:30.000000 asciicards-0.0.8.0/LICENSE
--rw-rw-rw-   0        0        0    41777 2024-04-17 01:26:47.292310 asciicards-0.0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-05-06 18:11:30.000000 asciicards-0.0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 01:26:47.290311 asciicards-0.0.8.0/asciicards.egg-info/
--rw-rw-rw-   0        0        0    41777 2024-04-17 01:26:47.000000 asciicards-0.0.8.0/asciicards.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-04-17 01:26:47.000000 asciicards-0.0.8.0/asciicards.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 01:26:47.000000 asciicards-0.0.8.0/asciicards.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 01:26:47.000000 asciicards-0.0.8.0/asciicards.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1696 2024-04-17 00:49:07.000000 asciicards-0.0.8.0/asciicards.py
--rw-rw-rw-   0        0        0      538 2024-04-17 01:26:41.000000 asciicards-0.0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 01:26:47.293310 asciicards-0.0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 19:00:33.763349 asciicards-0.0.8.1/
+-rw-rw-rw-   0        0        0    35149 2023-05-06 18:11:30.000000 asciicards-0.0.8.1/LICENSE
+-rw-rw-rw-   0        0        0    41777 2024-04-26 19:00:33.760343 asciicards-0.0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-05-06 18:11:30.000000 asciicards-0.0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 19:00:33.757342 asciicards-0.0.8.1/asciicards.egg-info/
+-rw-rw-rw-   0        0        0    41777 2024-04-26 19:00:33.000000 asciicards-0.0.8.1/asciicards.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-04-26 19:00:33.000000 asciicards-0.0.8.1/asciicards.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 19:00:33.000000 asciicards-0.0.8.1/asciicards.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 19:00:33.000000 asciicards-0.0.8.1/asciicards.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1696 2024-04-17 00:49:07.000000 asciicards-0.0.8.1/asciicards.py
+-rw-rw-rw-   0        0        0      538 2024-04-26 19:00:24.000000 asciicards-0.0.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 19:00:33.763349 asciicards-0.0.8.1/setup.cfg
```

### Comparing `asciicards-0.0.8.0/LICENSE` & `asciicards-0.0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asciicards-0.0.8.0/PKG-INFO` & `asciicards-0.0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asciicards
-Version: 0.0.8.0
+Version: 0.0.8.1
 Summary: Ascii Card Library
 Author-email: Paper <none@none.com>
 Maintainer-email: Paper <none@none.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `asciicards-0.0.8.0/asciicards.egg-info/PKG-INFO` & `asciicards-0.0.8.1/asciicards.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asciicards
-Version: 0.0.8.0
+Version: 0.0.8.1
 Summary: Ascii Card Library
 Author-email: Paper <none@none.com>
 Maintainer-email: Paper <none@none.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `asciicards-0.0.8.0/asciicards.py` & `asciicards-0.0.8.1/asciicards.py`

 * *Files identical despite different names*

### Comparing `asciicards-0.0.8.0/pyproject.toml` & `asciicards-0.0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asciicards"
-version = "0.0.8.0"
+version = "0.0.8.1"
 dependencies = []
 requires-python = ">=3.8"
 authors = [
   {name = "Paper", email = "none@none.com"}
 ]
 maintainers = [
   {name = "Paper", email = "none@none.com"}
```

