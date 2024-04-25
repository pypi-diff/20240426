# Comparing `tmp/tmnt-0.7.52b20240423.tar.gz` & `tmp/tmnt-0.7.52b20240424.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmnt-0.7.52b20240423.tar", last modified: Tue Apr 23 23:05:17 2024, max compression
+gzip compressed data, was "tmnt-0.7.52b20240424.tar", last modified: Wed Apr 24 23:04:59 2024, max compression
```

## Comparing `tmnt-0.7.52b20240423.tar` & `tmnt-0.7.52b20240424.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:05:17.806827 tmnt-0.7.52b20240423/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-23 23:05:17.806827 tmnt-0.7.52b20240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 23:05:17.806827 tmnt-0.7.52b20240423/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:05:17.802827 tmnt-0.7.52b20240423/tmnt/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18736 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/data_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    77217 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/eval_npmi.py
--rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    34549 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:05:17.802827 tmnt-0.7.52b20240423/tmnt/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/preprocess/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/preprocess/vectorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:05:17.806827 tmnt-0.7.52b20240423/tmnt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/utils/csv2json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/utils/mat_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/utils/ngram_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/utils/pubmed_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-23 23:05:00.000000 tmnt-0.7.52b20240423/tmnt/utils/recalibrate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:05:17.806827 tmnt-0.7.52b20240423/tmnt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-23 23:05:17.000000 tmnt-0.7.52b20240423/tmnt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-23 23:05:17.000000 tmnt-0.7.52b20240423/tmnt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:05:17.000000 tmnt-0.7.52b20240423/tmnt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-23 23:05:17.000000 tmnt-0.7.52b20240423/tmnt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 23:05:17.000000 tmnt-0.7.52b20240423/tmnt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:04:59.819561 tmnt-0.7.52b20240424/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-24 23:04:59.819561 tmnt-0.7.52b20240424/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 23:04:59.819561 tmnt-0.7.52b20240424/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:04:59.815561 tmnt-0.7.52b20240424/tmnt/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18736 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77217 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/eval_npmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34549 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:04:59.815561 tmnt-0.7.52b20240424/tmnt/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/preprocess/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/preprocess/vectorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:04:59.819561 tmnt-0.7.52b20240424/tmnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/utils/csv2json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/utils/mat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/utils/ngram_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/utils/pubmed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-24 23:04:49.000000 tmnt-0.7.52b20240424/tmnt/utils/recalibrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:04:59.819561 tmnt-0.7.52b20240424/tmnt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-24 23:04:59.000000 tmnt-0.7.52b20240424/tmnt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 23:04:59.000000 tmnt-0.7.52b20240424/tmnt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:04:59.000000 tmnt-0.7.52b20240424/tmnt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-24 23:04:59.000000 tmnt-0.7.52b20240424/tmnt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 23:04:59.000000 tmnt-0.7.52b20240424/tmnt.egg-info/top_level.txt
```

### Comparing `tmnt-0.7.52b20240423/LICENSE` & `tmnt-0.7.52b20240424/LICENSE`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/PKG-INFO` & `tmnt-0.7.52b20240424/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmnt
-Version: 0.7.52b20240423
+Version: 0.7.52b20240424
 Summary: Topic modeling neural toolkit
 Home-page: https://github.com/mitre/tmnt.git
 Author: The MITRE Corporation
 Author-email: wellner@mitre.org
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tmnt-0.7.52b20240423/setup.py` & `tmnt-0.7.52b20240424/setup.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/configuration.py` & `tmnt-0.7.52b20240424/tmnt/configuration.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/data_loading.py` & `tmnt-0.7.52b20240424/tmnt/data_loading.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/distribution.py` & `tmnt-0.7.52b20240424/tmnt/distribution.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/estimator.py` & `tmnt-0.7.52b20240424/tmnt/estimator.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/eval_npmi.py` & `tmnt-0.7.52b20240424/tmnt/eval_npmi.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/inference.py` & `tmnt-0.7.52b20240424/tmnt/inference.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/modeling.py` & `tmnt-0.7.52b20240424/tmnt/modeling.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/preprocess/tokenizer.py` & `tmnt-0.7.52b20240424/tmnt/preprocess/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/preprocess/vectorizer.py` & `tmnt-0.7.52b20240424/tmnt/preprocess/vectorizer.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/utils/csv2json.py` & `tmnt-0.7.52b20240424/tmnt/utils/csv2json.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/utils/log_utils.py` & `tmnt-0.7.52b20240424/tmnt/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/utils/mat_utils.py` & `tmnt-0.7.52b20240424/tmnt/utils/mat_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/utils/ngram_helpers.py` & `tmnt-0.7.52b20240424/tmnt/utils/ngram_helpers.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/utils/pubmed_utils.py` & `tmnt-0.7.52b20240424/tmnt/utils/pubmed_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt/utils/recalibrate.py` & `tmnt-0.7.52b20240424/tmnt/utils/recalibrate.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.52b20240423/tmnt.egg-info/PKG-INFO` & `tmnt-0.7.52b20240424/tmnt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmnt
-Version: 0.7.52b20240423
+Version: 0.7.52b20240424
 Summary: Topic modeling neural toolkit
 Home-page: https://github.com/mitre/tmnt.git
 Author: The MITRE Corporation
 Author-email: wellner@mitre.org
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tmnt-0.7.52b20240423/tmnt.egg-info/SOURCES.txt` & `tmnt-0.7.52b20240424/tmnt.egg-info/SOURCES.txt`

 * *Files identical despite different names*
