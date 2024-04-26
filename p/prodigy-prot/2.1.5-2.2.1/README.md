# Comparing `tmp/prodigy_prot-2.1.5.tar.gz` & `tmp/prodigy_prot-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodigy_prot-2.1.5.tar", max compression
+gzip compressed data, was "prodigy_prot-2.2.1.tar", max compression
```

## Comparing `prodigy_prot-2.1.5.tar` & `prodigy_prot-2.2.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    10797 2024-04-26 11:36:23.521675 prodigy_prot-2.1.5/LICENSE
--rw-r--r--   0        0        0     6581 2024-04-26 11:36:23.521675 prodigy_prot-2.1.5/README.md
--rw-r--r--   0        0        0     1129 2024-04-26 13:24:22.712905 prodigy_prot-2.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-26 13:07:09.001369 prodigy_prot-2.1.5/src/prodigy_prot/__init__.py
--rw-r--r--   0        0        0      292 2024-04-26 13:07:09.001369 prodigy_prot-2.1.5/src/prodigy_prot/modules/__init__.py
--rw-r--r--   0        0        0     2593 2024-04-26 13:07:09.001369 prodigy_prot-2.1.5/src/prodigy_prot/modules/aa_properties.py
--rw-r--r--   0        0        0     7109 2024-04-26 13:25:53.841527 prodigy_prot-2.1.5/src/prodigy_prot/modules/freesasa_tools.py
--rw-r--r--   0        0        0      947 2024-04-26 13:07:09.001369 prodigy_prot-2.1.5/src/prodigy_prot/modules/models.py
--rw-r--r--   0        0        0        0 2024-04-26 13:07:09.001369 prodigy_prot-2.1.5/src/prodigy_prot/modules/nis_utils.py
--rw-r--r--   0        0        0     4796 2024-04-26 13:07:09.001369 prodigy_prot-2.1.5/src/prodigy_prot/modules/parsers.py
--rw-r--r--   0        0        0      712 2024-04-26 13:07:09.001369 prodigy_prot-2.1.5/src/prodigy_prot/modules/utils.py
--rw-r--r--   0        0        0     2772 2024-04-26 13:07:09.001369 prodigy_prot-2.1.5/src/prodigy_prot/naccess.config
--rw-r--r--   0        0        0    13288 2024-04-26 13:25:33.621720 prodigy_prot-2.1.5/src/prodigy_prot/predict_IC.py
--rw-r--r--   0        0        0     7528 1970-01-01 00:00:00.000000 prodigy_prot-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0    10797 2024-04-26 13:37:04.222817 prodigy_prot-2.2.1/LICENSE
+-rw-r--r--   0        0        0     6581 2024-04-26 13:37:04.222817 prodigy_prot-2.2.1/README.md
+-rw-r--r--   0        0        0     1129 2024-04-26 13:37:04.250816 prodigy_prot-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-26 13:37:04.250816 prodigy_prot-2.2.1/src/prodigy_prot/__init__.py
+-rw-r--r--   0        0        0      292 2024-04-26 13:37:04.250816 prodigy_prot-2.2.1/src/prodigy_prot/modules/__init__.py
+-rw-r--r--   0        0        0     2593 2024-04-26 13:37:04.254817 prodigy_prot-2.2.1/src/prodigy_prot/modules/aa_properties.py
+-rw-r--r--   0        0        0     7109 2024-04-26 13:37:04.254817 prodigy_prot-2.2.1/src/prodigy_prot/modules/freesasa_tools.py
+-rw-r--r--   0        0        0      947 2024-04-26 13:37:04.254817 prodigy_prot-2.2.1/src/prodigy_prot/modules/models.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:37:04.254817 prodigy_prot-2.2.1/src/prodigy_prot/modules/nis_utils.py
+-rw-r--r--   0        0        0     4796 2024-04-26 13:37:04.254817 prodigy_prot-2.2.1/src/prodigy_prot/modules/parsers.py
+-rw-r--r--   0        0        0      712 2024-04-26 13:37:04.254817 prodigy_prot-2.2.1/src/prodigy_prot/modules/utils.py
+-rw-r--r--   0        0        0     2772 2024-04-26 13:37:04.254817 prodigy_prot-2.2.1/src/prodigy_prot/naccess.config
+-rw-r--r--   0        0        0    13288 2024-04-26 13:37:04.254817 prodigy_prot-2.2.1/src/prodigy_prot/predict_IC.py
+-rw-r--r--   0        0        0     7639 1970-01-01 00:00:00.000000 prodigy_prot-2.2.1/setup.py
+-rw-r--r--   0        0        0     7578 1970-01-01 00:00:00.000000 prodigy_prot-2.2.1/PKG-INFO
```

### Comparing `prodigy_prot-2.1.5/LICENSE` & `prodigy_prot-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prodigy_prot-2.1.5/README.md` & `prodigy_prot-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `prodigy_prot-2.1.5/pyproject.toml` & `prodigy_prot-2.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "prodigy-prot"
 license = "Apache-2.0"
-version = "2.1.5"
+version = "2.2.1"
 description = "PROtein binDIng enerGY prediction"
 authors = [
   "Computational Structural Biology Group at Utrecht University <prodigy.bonvinlab@gmail.com>",
 ]
 readme = "README.md"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `prodigy_prot-2.1.5/src/prodigy_prot/modules/aa_properties.py` & `prodigy_prot-2.2.1/src/prodigy_prot/modules/aa_properties.py`

 * *Files identical despite different names*

### Comparing `prodigy_prot-2.1.5/src/prodigy_prot/modules/freesasa_tools.py` & `prodigy_prot-2.2.1/src/prodigy_prot/modules/freesasa_tools.py`

 * *Files identical despite different names*

### Comparing `prodigy_prot-2.1.5/src/prodigy_prot/modules/models.py` & `prodigy_prot-2.2.1/src/prodigy_prot/modules/models.py`

 * *Files identical despite different names*

### Comparing `prodigy_prot-2.1.5/src/prodigy_prot/modules/parsers.py` & `prodigy_prot-2.2.1/src/prodigy_prot/modules/parsers.py`

 * *Files identical despite different names*

### Comparing `prodigy_prot-2.1.5/src/prodigy_prot/modules/utils.py` & `prodigy_prot-2.2.1/src/prodigy_prot/modules/utils.py`

 * *Files identical despite different names*

### Comparing `prodigy_prot-2.1.5/src/prodigy_prot/naccess.config` & `prodigy_prot-2.2.1/src/prodigy_prot/naccess.config`

 * *Files identical despite different names*

### Comparing `prodigy_prot-2.1.5/src/prodigy_prot/predict_IC.py` & `prodigy_prot-2.2.1/src/prodigy_prot/predict_IC.py`

 * *Files identical despite different names*

### Comparing `prodigy_prot-2.1.5/PKG-INFO` & `prodigy_prot-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: prodigy-prot
-Version: 2.1.5
+Version: 2.2.1
 Summary: PROtein binDIng enerGY prediction
 License: Apache-2.0
 Author: Computational Structural Biology Group at Utrecht University
 Author-email: prodigy.bonvinlab@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Dist: biopython (==1.80)
 Requires-Dist: freesasa (==2.2.1)
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
 Description-Content-Type: text/markdown
```

