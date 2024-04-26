# Comparing `tmp/pyscinloopsr-1.0.3.tar.gz` & `tmp/pyscinloopsr-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscinloopsr-1.0.3.tar", last modified: Fri Apr 26 04:44:16 2024, max compression
+gzip compressed data, was "pyscinloopsr-1.0.4.tar", last modified: Fri Apr 26 04:55:24 2024, max compression
```

## Comparing `pyscinloopsr-1.0.3.tar` & `pyscinloopsr-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 04:44:16.693708 pyscinloopsr-1.0.3/
--rw-rw-rw-   0        0        0       42 2024-04-05 06:04:28.000000 pyscinloopsr-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      815 2024-04-26 04:44:16.693708 pyscinloopsr-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-05 05:31:15.000000 pyscinloopsr-1.0.3/README.md
--rw-rw-rw-   0        0        0     1427 2024-04-26 04:43:25.000000 pyscinloopsr-1.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-26 04:44:16.662460 pyscinloopsr-1.0.3/pyscinloopsr/
--rw-rw-rw-   0        0        0        0 2024-04-05 05:31:53.000000 pyscinloopsr-1.0.3/pyscinloopsr/__init__.py
--rw-rw-rw-   0        0        0      508 2024-04-05 09:45:13.000000 pyscinloopsr-1.0.3/pyscinloopsr/__main__.py
--rw-rw-rw-   0        0        0    11899 2024-04-26 04:42:58.000000 pyscinloopsr-1.0.3/pyscinloopsr/before.py
--rw-rw-rw-   0        0        0      211 2024-04-25 20:59:05.000000 pyscinloopsr-1.0.3/pyscinloopsr/test_before.py
-drwxrwxrwx   0        0        0        0 2024-04-26 04:44:16.693708 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/
--rw-rw-rw-   0        0        0      815 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      106 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-26 04:44:16.000000 pyscinloopsr-1.0.3/pyscinloopsr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 04:44:16.693708 pyscinloopsr-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      449 2024-04-26 04:43:45.000000 pyscinloopsr-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 04:55:24.626652 pyscinloopsr-1.0.4/
+-rw-rw-rw-   0        0        0       42 2024-04-05 06:04:28.000000 pyscinloopsr-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      815 2024-04-26 04:55:24.611026 pyscinloopsr-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-05 05:31:15.000000 pyscinloopsr-1.0.4/README.md
+-rw-rw-rw-   0        0        0     1427 2024-04-26 04:55:03.000000 pyscinloopsr-1.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-26 04:55:24.595402 pyscinloopsr-1.0.4/pyscinloopsr/
+-rw-rw-rw-   0        0        0        0 2024-04-05 05:31:53.000000 pyscinloopsr-1.0.4/pyscinloopsr/__init__.py
+-rw-rw-rw-   0        0        0      508 2024-04-05 09:45:13.000000 pyscinloopsr-1.0.4/pyscinloopsr/__main__.py
+-rw-rw-rw-   0        0        0    11907 2024-04-26 04:54:48.000000 pyscinloopsr-1.0.4/pyscinloopsr/before.py
+-rw-rw-rw-   0        0        0      211 2024-04-25 20:59:05.000000 pyscinloopsr-1.0.4/pyscinloopsr/test_before.py
+drwxrwxrwx   0        0        0        0 2024-04-26 04:55:24.611026 pyscinloopsr-1.0.4/pyscinloopsr.egg-info/
+-rw-rw-rw-   0        0        0      815 2024-04-26 04:55:24.000000 pyscinloopsr-1.0.4/pyscinloopsr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:55:24.000000 pyscinloopsr-1.0.4/pyscinloopsr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 04:55:24.000000 pyscinloopsr-1.0.4/pyscinloopsr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-26 04:55:24.000000 pyscinloopsr-1.0.4/pyscinloopsr.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2024-04-26 04:55:24.000000 pyscinloopsr-1.0.4/pyscinloopsr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-26 04:55:24.000000 pyscinloopsr-1.0.4/pyscinloopsr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 04:55:24.626652 pyscinloopsr-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      449 2024-04-26 04:55:08.000000 pyscinloopsr-1.0.4/setup.py
```

### Comparing `pyscinloopsr-1.0.3/PKG-INFO` & `pyscinloopsr-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscinloopsr
-Version: 1.0.3
+Version: 1.0.4
 Summary: Read the latest PyScInLoopSr tutorials
 Author: Djalma Pereira
 Author-email: Djalma Pereira <pereirajunio@gmail.com>
 Project-URL: Homepage, https://github.com/realpython/reader
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyscinloopsr-1.0.3/pyproject.toml` & `pyscinloopsr-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyscinloopsr"
-version = "1.0.3"
+version = "1.0.4"
 description = "Read the latest PyScInLoopSr tutorials"
 readme = "README.md"
 authors = [{ name = "Djalma Pereira", email = "pereirajunio@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyscinloopsr-1.0.3/pyscinloopsr/before.py` & `pyscinloopsr-1.0.4/pyscinloopsr/before.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 
 
   from sklearn.model_selection import train_test_split
 
   # X and y already set
 
   # split the data into training and testing sets
-  X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
+  X_train, X_test, y_train, y_test = train_test_split(dfxbr, dfybr, test_size=0.2, random_state=42)
 
 
 
   class ConsoleColor:
       # Color
       BLACK = '\033[90m'
       RED = '\033[91m'
```

### Comparing `pyscinloopsr-1.0.3/pyscinloopsr.egg-info/PKG-INFO` & `pyscinloopsr-1.0.4/pyscinloopsr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscinloopsr
-Version: 1.0.3
+Version: 1.0.4
 Summary: Read the latest PyScInLoopSr tutorials
 Author: Djalma Pereira
 Author-email: Djalma Pereira <pereirajunio@gmail.com>
 Project-URL: Homepage, https://github.com/realpython/reader
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

