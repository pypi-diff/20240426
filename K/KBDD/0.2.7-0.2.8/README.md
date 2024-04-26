# Comparing `tmp/KBDD-0.2.7.tar.gz` & `tmp/KBDD-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KBDD-0.2.7.tar", last modified: Thu Apr 25 19:10:52 2024, max compression
+gzip compressed data, was "KBDD-0.2.8.tar", last modified: Thu Apr 25 20:00:53 2024, max compression
```

## Comparing `KBDD-0.2.7.tar` & `KBDD-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:10:52.442810 KBDD-0.2.7/
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:10:52.441270 KBDD-0.2.7/KBDD/
--rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:37:55.000000 KBDD-0.2.7/KBDD/KGML_to_Matrix.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     5906 2024-04-25 19:10:30.000000 KBDD-0.2.7/KBDD/Network_score_with_cor.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      241 2024-04-25 19:03:43.000000 KBDD-0.2.7/KBDD/__init__.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1275 2024-04-25 18:12:10.000000 KBDD-0.2.7/KBDD/alpha_estimation.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      964 2024-04-25 18:57:13.000000 KBDD-0.2.7/KBDD/deviation_calculation.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1492 2024-04-25 17:58:42.000000 KBDD-0.2.7/KBDD/import_references.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)    11230 2024-04-25 19:01:26.000000 KBDD-0.2.7/KBDD/pns_construction.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.2.7/KBDD/show_graph_with_labels.py
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:10:52.442243 KBDD-0.2.7/KBDD.egg-info/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 19:10:52.000000 KBDD-0.2.7/KBDD.egg-info/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      350 2024-04-25 19:10:52.000000 KBDD-0.2.7/KBDD.egg-info/SOURCES.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 19:10:52.000000 KBDD-0.2.7/KBDD.egg-info/dependency_links.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 19:10:52.000000 KBDD-0.2.7/KBDD.egg-info/top_level.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.2.7/LICENSE.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 19:10:52.442522 KBDD-0.2.7/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.2.7/README.md
--rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 19:10:52.442881 KBDD-0.2.7/setup.cfg
--rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 19:10:46.000000 KBDD-0.2.7/setup.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 20:00:53.000284 KBDD-0.2.8/
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 20:00:52.998785 KBDD-0.2.8/KBDD/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:37:55.000000 KBDD-0.2.8/KBDD/KGML_to_Matrix.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     5906 2024-04-25 19:10:30.000000 KBDD-0.2.8/KBDD/Network_score_with_cor.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      281 2024-04-25 19:59:49.000000 KBDD-0.2.8/KBDD/__init__.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1275 2024-04-25 18:12:10.000000 KBDD-0.2.8/KBDD/alpha_estimation.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      964 2024-04-25 18:57:13.000000 KBDD-0.2.8/KBDD/deviation_calculation.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     2680 2024-04-25 19:59:45.000000 KBDD-0.2.8/KBDD/generate_ensemble_network.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1492 2024-04-25 17:58:42.000000 KBDD-0.2.8/KBDD/import_references.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)    11230 2024-04-25 19:01:26.000000 KBDD-0.2.8/KBDD/pns_construction.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.2.8/KBDD/show_graph_with_labels.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 20:00:52.999725 KBDD-0.2.8/KBDD.egg-info/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 20:00:52.000000 KBDD-0.2.8/KBDD.egg-info/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      384 2024-04-25 20:00:52.000000 KBDD-0.2.8/KBDD.egg-info/SOURCES.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 20:00:52.000000 KBDD-0.2.8/KBDD.egg-info/dependency_links.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 20:00:52.000000 KBDD-0.2.8/KBDD.egg-info/top_level.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.2.8/LICENSE.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 20:00:53.000013 KBDD-0.2.8/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.2.8/README.md
+-rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 20:00:53.000345 KBDD-0.2.8/setup.cfg
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 20:00:49.000000 KBDD-0.2.8/setup.py
```

### Comparing `KBDD-0.2.7/KBDD/KGML_to_Matrix.py` & `KBDD-0.2.8/KBDD/KGML_to_Matrix.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.7/KBDD/Network_score_with_cor.py` & `KBDD-0.2.8/KBDD/Network_score_with_cor.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.7/KBDD/alpha_estimation.py` & `KBDD-0.2.8/KBDD/alpha_estimation.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.7/KBDD/deviation_calculation.py` & `KBDD-0.2.8/KBDD/deviation_calculation.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.7/KBDD/import_references.py` & `KBDD-0.2.8/KBDD/import_references.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.7/KBDD/pns_construction.py` & `KBDD-0.2.8/KBDD/pns_construction.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.7/KBDD/show_graph_with_labels.py` & `KBDD-0.2.8/KBDD/show_graph_with_labels.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.7/KBDD.egg-info/PKG-INFO` & `KBDD-0.2.8/KBDD.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.2.7
+Version: 0.2.8
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.2.7/LICENSE.txt` & `KBDD-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.7/PKG-INFO` & `KBDD-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.2.7
+Version: 0.2.8
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.2.7/setup.py` & `KBDD-0.2.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='KBDD',
-    version='0.2.7',
+    version='0.2.8',
     packages=setuptools.find_packages(),
     description='A package for KBDD: a knowledge-based and data-driven method for genetic network construction',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chen-Po Liao',
     author_email='liaochenpo@gmail.com',
     license='MIT',
```

