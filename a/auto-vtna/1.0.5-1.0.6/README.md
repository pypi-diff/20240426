# Comparing `tmp/auto_vtna-1.0.5.tar.gz` & `tmp/auto_vtna-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_vtna-1.0.5.tar", last modified: Fri Apr 26 14:30:32 2024, max compression
+gzip compressed data, was "auto_vtna-1.0.6.tar", last modified: Fri Apr 26 15:34:01 2024, max compression
```

## Comparing `auto_vtna-1.0.5.tar` & `auto_vtna-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 14:30:32.044778 auto_vtna-1.0.5/
--rw-rw-rw-   0        0        0      539 2024-04-26 14:30:32.043773 auto_vtna-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-04-18 14:11:13.000000 auto_vtna-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 14:30:31.993865 auto_vtna-1.0.5/auto_vtna/
--rw-rw-rw-   0        0        0   203326 2024-04-26 14:26:47.000000 auto_vtna-1.0.5/auto_vtna/Auto_VTNA_GUI.py
--rw-rw-rw-   0        0        0    22230 2024-04-21 08:40:37.000000 auto_vtna-1.0.5/auto_vtna/Automatic_VTNA.py
--rw-rw-rw-   0        0        0    23125 2024-04-18 20:28:15.000000 auto_vtna-1.0.5/auto_vtna/Normal_VTNA.py
--rw-rw-rw-   0        0        0    45282 2024-04-20 15:02:10.000000 auto_vtna-1.0.5/auto_vtna/VTNA_functions.py
--rw-rw-rw-   0        0        0    51883 2024-04-22 20:40:40.000000 auto_vtna-1.0.5/auto_vtna/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:30:32.040773 auto_vtna-1.0.5/auto_vtna.egg-info/
--rw-rw-rw-   0        0        0      539 2024-04-26 14:30:30.000000 auto_vtna-1.0.5/auto_vtna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-04-26 14:30:31.000000 auto_vtna-1.0.5/auto_vtna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 14:30:30.000000 auto_vtna-1.0.5/auto_vtna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-26 14:30:30.000000 auto_vtna-1.0.5/auto_vtna.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-26 14:30:30.000000 auto_vtna-1.0.5/auto_vtna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 14:30:32.044778 auto_vtna-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      963 2024-04-26 14:28:05.000000 auto_vtna-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:34:01.510263 auto_vtna-1.0.6/
+-rw-rw-rw-   0        0        0      539 2024-04-26 15:34:01.509013 auto_vtna-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-04-18 14:11:13.000000 auto_vtna-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 15:34:01.482999 auto_vtna-1.0.6/auto_vtna/
+-rw-rw-rw-   0        0        0   203326 2024-04-26 15:26:42.000000 auto_vtna-1.0.6/auto_vtna/Auto_VTNA_GUI.py
+-rw-rw-rw-   0        0        0    22230 2024-04-21 08:40:37.000000 auto_vtna-1.0.6/auto_vtna/Automatic_VTNA.py
+-rw-rw-rw-   0        0        0    23125 2024-04-26 15:32:15.000000 auto_vtna-1.0.6/auto_vtna/Normal_VTNA.py
+-rw-rw-rw-   0        0        0    45282 2024-04-26 15:26:38.000000 auto_vtna-1.0.6/auto_vtna/VTNA_functions.py
+-rw-rw-rw-   0        0        0    51883 2024-04-22 20:40:40.000000 auto_vtna-1.0.6/auto_vtna/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:34:01.505015 auto_vtna-1.0.6/auto_vtna.egg-info/
+-rw-rw-rw-   0        0        0      539 2024-04-26 15:34:00.000000 auto_vtna-1.0.6/auto_vtna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-26 15:34:01.000000 auto_vtna-1.0.6/auto_vtna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 15:34:00.000000 auto_vtna-1.0.6/auto_vtna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-26 15:34:00.000000 auto_vtna-1.0.6/auto_vtna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-26 15:34:00.000000 auto_vtna-1.0.6/auto_vtna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 15:34:01.510263 auto_vtna-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      963 2024-04-26 15:33:49.000000 auto_vtna-1.0.6/setup.py
```

### Comparing `auto_vtna-1.0.5/PKG-INFO` & `auto_vtna-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_vtna
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python package for efficient and automatic VTNA analysis
 Author: Daniel Dalland
 Author-email: dd4518@ic.ac.uk
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `auto_vtna-1.0.5/auto_vtna/Auto_VTNA_GUI.py` & `auto_vtna-1.0.6/auto_vtna/Auto_VTNA_GUI.py`

 * *Files identical despite different names*

### Comparing `auto_vtna-1.0.5/auto_vtna/Automatic_VTNA.py` & `auto_vtna-1.0.6/auto_vtna/Automatic_VTNA.py`

 * *Files identical despite different names*

### Comparing `auto_vtna-1.0.5/auto_vtna/Normal_VTNA.py` & `auto_vtna-1.0.6/auto_vtna/Normal_VTNA.py`

 * *Files identical despite different names*

### Comparing `auto_vtna-1.0.5/auto_vtna/VTNA_functions.py` & `auto_vtna-1.0.6/auto_vtna/VTNA_functions.py`

 * *Files identical despite different names*

### Comparing `auto_vtna-1.0.5/auto_vtna/__init__.py` & `auto_vtna-1.0.6/auto_vtna/__init__.py`

 * *Files identical despite different names*

### Comparing `auto_vtna-1.0.5/auto_vtna.egg-info/PKG-INFO` & `auto_vtna-1.0.6/auto_vtna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-vtna
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python package for efficient and automatic VTNA analysis
 Author: Daniel Dalland
 Author-email: dd4518@ic.ac.uk
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `auto_vtna-1.0.5/setup.py` & `auto_vtna-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from os import path
 
 # Meta-data of the package.
 NAME = 'auto_vtna'
 DESCRIPTION = 'A Python package for efficient and automatic VTNA analysis'
 EMAIL = 'dd4518@ic.ac.uk'
 AUTHOR = 'Daniel Dalland'
-VERSION = "1.0.5"
+VERSION = "1.0.6"
 REQUIRED=[
     'pandas',
     'numpy',
     'matplotlib',
     'num2words',
     'mplcursors',
     'scipy',
```

