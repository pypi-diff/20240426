# Comparing `tmp/pyscinloopsr-1.0.2.tar.gz` & `tmp/pyscinloopsr-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscinloopsr-1.0.2.tar", last modified: Thu Apr 25 21:35:33 2024, max compression
+gzip compressed data, was "pyscinloopsr-1.0.3.tar", last modified: Fri Apr 26 04:44:16 2024, max compression
```

## Comparing `pyscinloopsr-1.0.2.tar` & `pyscinloopsr-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 21:35:33.606498 pyscinloopsr-1.0.2/
--rw-rw-rw-   0        0        0       42 2024-04-05 06:04:28.000000 pyscinloopsr-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      815 2024-04-25 21:35:33.606498 pyscinloopsr-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-05 05:31:15.000000 pyscinloopsr-1.0.2/README.md
--rw-rw-rw-   0        0        0     1427 2024-04-25 20:56:55.000000 pyscinloopsr-1.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-25 21:35:33.575248 pyscinloopsr-1.0.2/pyscinloopsr/
--rw-rw-rw-   0        0        0        0 2024-04-05 05:31:53.000000 pyscinloopsr-1.0.2/pyscinloopsr/__init__.py
--rw-rw-rw-   0        0        0      508 2024-04-05 09:45:13.000000 pyscinloopsr-1.0.2/pyscinloopsr/__main__.py
--rw-rw-rw-   0        0        0      946 2024-04-25 20:58:56.000000 pyscinloopsr-1.0.2/pyscinloopsr/before.py
--rw-rw-rw-   0        0        0      211 2024-04-25 20:59:05.000000 pyscinloopsr-1.0.2/pyscinloopsr/test_before.py
-drwxrwxrwx   0        0        0        0 2024-04-25 21:35:33.606498 pyscinloopsr-1.0.2/pyscinloopsr.egg-info/
--rw-rw-rw-   0        0        0      815 2024-04-25 21:35:33.000000 pyscinloopsr-1.0.2/pyscinloopsr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-04-25 21:35:33.000000 pyscinloopsr-1.0.2/pyscinloopsr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 21:35:33.000000 pyscinloopsr-1.0.2/pyscinloopsr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-25 21:35:33.000000 pyscinloopsr-1.0.2/pyscinloopsr.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      106 2024-04-25 21:35:33.000000 pyscinloopsr-1.0.2/pyscinloopsr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 21:35:33.000000 pyscinloopsr-1.0.2/pyscinloopsr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 21:35:33.606498 pyscinloopsr-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      449 2024-04-25 20:57:25.000000 pyscinloopsr-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 04:44:16.693708 pyscinloopsr-1.0.3/
+-rw-rw-rw-   0        0        0       42 2024-04-05 06:04:28.000000 pyscinloopsr-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      815 2024-04-26 04:44:16.693708 pyscinloopsr-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-05 05:31:15.000000 pyscinloopsr-1.0.3/README.md
+-rw-rw-rw-   0        0        0     1427 2024-04-26 04:43:25.000000 pyscinloopsr-1.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-26 04:44:16.662460 pyscinloopsr-1.0.3/pyscinloopsr/
+-rw-rw-rw-   0        0        0        0 2024-04-05 05:31:53.000000 pyscinloopsr-1.0.3/pyscinloopsr/__init__.py
+-rw-rw-rw-   0        0        0      508 2024-04-05 09:45:13.000000 pyscinloopsr-1.0.3/pyscinloopsr/__main__.py
+-rw-rw-rw-   0        0        0    11899 2024-04-26 04:42:58.000000 pyscinloopsr-1.0.3/pyscinloopsr/before.py
+-rw-rw-rw-   0        0        0      211 2024-04-25 20:59:05.000000 pyscinloopsr-1.0.3/pyscinloopsr/test_before.py
+drwxrwxrwx   0        0        0        0 2024-04-26 04:44:16.693708 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/
+-rw-rw-rw-   0        0        0      815 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 04:44:16.693708 pyscinloopsr-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      449 2024-04-26 04:43:45.000000 pyscinloopsr-1.0.3/setup.py
```

### Comparing `pyscinloopsr-1.0.2/PKG-INFO` & `pyscinloopsr-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscinloopsr
-Version: 1.0.2
+Version: 1.0.3
 Summary: Read the latest PyScInLoopSr tutorials
 Author: Djalma Pereira
 Author-email: Djalma Pereira <pereirajunio@gmail.com>
 Project-URL: Homepage, https://github.com/realpython/reader
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyscinloopsr-1.0.2/pyproject.toml` & `pyscinloopsr-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyscinloopsr"
-version = "1.0.2"
+version = "1.0.3"
 description = "Read the latest PyScInLoopSr tutorials"
 readme = "README.md"
 authors = [{ name = "Djalma Pereira", email = "pereirajunio@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyscinloopsr-1.0.2/pyscinloopsr.egg-info/PKG-INFO` & `pyscinloopsr-1.0.3/pyscinloopsr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscinloopsr
-Version: 1.0.2
+Version: 1.0.3
 Summary: Read the latest PyScInLoopSr tutorials
 Author: Djalma Pereira
 Author-email: Djalma Pereira <pereirajunio@gmail.com>
 Project-URL: Homepage, https://github.com/realpython/reader
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

