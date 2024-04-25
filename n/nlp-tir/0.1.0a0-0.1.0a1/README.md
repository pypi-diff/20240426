# Comparing `tmp/nlp_tir-0.1.0a0.tar.gz` & `tmp/nlp_tir-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp_tir-0.1.0a0.tar", last modified: Sun Apr 21 16:33:32 2024, max compression
+gzip compressed data, was "nlp_tir-0.1.0a1.tar", last modified: Thu Apr 25 23:23:49 2024, max compression
```

## Comparing `nlp_tir-0.1.0a0.tar` & `nlp_tir-0.1.0a1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      421 2024-03-22 23:51:41.026334 nlp_tir-0.1.0a0/README.md
--rw-r--r--   0        0        0     2360 2024-03-26 21:58:41.004444 nlp_tir-0.1.0a0/nlp_tir/.ipynb_checkpoints/datasets-checkpoint.py
--rwxr-xr-x   0        0        0      512 2024-04-21 04:03:45.185747 nlp_tir-0.1.0a0/nlp_tir/.ipynb_checkpoints/setup-checkpoint.py
--rw-r--r--   0        0        0        0 2024-03-15 19:20:42.079548 nlp_tir-0.1.0a0/nlp_tir/__init__.py
--rw-r--r--   0        0        0     2360 2024-03-26 21:58:41.004444 nlp_tir-0.1.0a0/nlp_tir/datasets.py
--rwxr-xr-x   0        0        0      512 2024-04-21 04:03:45.185747 nlp_tir-0.1.0a0/nlp_tir/setup.py
--rw-r--r--   0        0        0     1578 2024-04-21 16:33:32.537135 nlp_tir-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-24 03:08:47.331367 nlp_tir-0.1.0a0/tests/__init__.py
--rw-r--r--   0        0        0     2940 2024-03-26 22:03:08.262977 nlp_tir-0.1.0a0/tests/coverage.xml
--rw-r--r--   0        0        0      389 2024-03-25 15:38:51.482489 nlp_tir-0.1.0a0/tests/test_datasets.py
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 nlp_tir-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0      421 2024-03-22 23:51:41.026334 nlp_tir-0.1.0a1/README.md
+-rw-r--r--   0        0        0     2360 2024-03-26 21:58:41.004444 nlp_tir-0.1.0a1/nlp_tir/.ipynb_checkpoints/datasets-checkpoint.py
+-rwxr-xr-x   0        0        0      512 2024-04-21 04:03:45.185747 nlp_tir-0.1.0a1/nlp_tir/.ipynb_checkpoints/setup-checkpoint.py
+-rw-r--r--   0        0        0        0 2024-03-15 19:20:42.079548 nlp_tir-0.1.0a1/nlp_tir/__init__.py
+-rw-r--r--   0        0        0     2360 2024-03-26 21:58:41.004444 nlp_tir-0.1.0a1/nlp_tir/datasets.py
+-rwxr-xr-x   0        0        0      512 2024-04-25 23:23:10.219048 nlp_tir-0.1.0a1/nlp_tir/setup.py
+-rw-r--r--   0        0        0     1578 2024-04-25 23:23:49.583917 nlp_tir-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-24 03:08:47.331367 nlp_tir-0.1.0a1/tests/__init__.py
+-rw-r--r--   0        0        0     2940 2024-03-26 22:03:08.262977 nlp_tir-0.1.0a1/tests/coverage.xml
+-rw-r--r--   0        0        0      389 2024-03-25 15:38:51.482489 nlp_tir-0.1.0a1/tests/test_datasets.py
+-rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 nlp_tir-0.1.0a1/PKG-INFO
```

### Comparing `nlp_tir-0.1.0a0/nlp_tir/.ipynb_checkpoints/datasets-checkpoint.py` & `nlp_tir-0.1.0a1/nlp_tir/.ipynb_checkpoints/datasets-checkpoint.py`

 * *Files identical despite different names*

### Comparing `nlp_tir-0.1.0a0/nlp_tir/.ipynb_checkpoints/setup-checkpoint.py` & `nlp_tir-0.1.0a1/nlp_tir/.ipynb_checkpoints/setup-checkpoint.py`

 * *Files identical despite different names*

### Comparing `nlp_tir-0.1.0a0/nlp_tir/datasets.py` & `nlp_tir-0.1.0a1/nlp_tir/datasets.py`

 * *Files identical despite different names*

### Comparing `nlp_tir-0.1.0a0/nlp_tir/setup.py` & `nlp_tir-0.1.0a1/nlp_tir/setup.py`

 * *Files identical despite different names*

### Comparing `nlp_tir-0.1.0a0/pyproject.toml` & `nlp_tir-0.1.0a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nlp-tir"
-version = "0.1.0a0"
+version = "0.1.0a1"
 description = "Tir is the god of written language, schooling, rhetoric, wisdom, and the arts in Armenian mythology."
 authors = [
     { name = "Manoel Vilela", email = "manoel_vilela@engineer.com" },
 ]
 dependencies = [
     "nltk>=3.8.1",
     "pyenchant>=3.2.2",
```

### Comparing `nlp_tir-0.1.0a0/tests/coverage.xml` & `nlp_tir-0.1.0a1/tests/coverage.xml`

 * *Files identical despite different names*

### Comparing `nlp_tir-0.1.0a0/PKG-INFO` & `nlp_tir-0.1.0a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-tir
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Tir is the god of written language, schooling, rhetoric, wisdom, and the arts in Armenian mythology.
 Author-Email: Manoel Vilela <manoel_vilela@engineer.com>
 License: MIT
 Requires-Python: <3.12,>=3.10
 Requires-Dist: nltk>=3.8.1
 Requires-Dist: pyenchant>=3.2.2
 Requires-Dist: scikit-learn>=1.4.0
```

