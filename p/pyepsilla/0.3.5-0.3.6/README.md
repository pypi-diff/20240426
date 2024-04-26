# Comparing `tmp/pyepsilla-0.3.5.tar.gz` & `tmp/pyepsilla-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepsilla-0.3.5.tar", last modified: Thu Mar 21 14:10:14 2024, max compression
+gzip compressed data, was "pyepsilla-0.3.6.tar", last modified: Fri Apr 26 16:01:43 2024, max compression
```

## Comparing `pyepsilla-0.3.5.tar` & `pyepsilla-0.3.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:14.990947 pyepsilla-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-21 14:10:14.990947 pyepsilla-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:14.986947 pyepsilla-0.3.5/pyepsilla/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:14.986947 pyepsilla-0.3.5/pyepsilla/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/cloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/cloud/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:14.986947 pyepsilla-0.3.5/pyepsilla/enterprise/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/enterprise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/enterprise/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/enterprise/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:14.986947 pyepsilla-0.3.5/pyepsilla/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10342 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/utils/search_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:14.986947 pyepsilla-0.3.5/pyepsilla/vectordb/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13172 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/vectordb/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/vectordb/field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:14.986947 pyepsilla-0.3.5/pyepsilla/vectordb/machineid/
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/vectordb/machineid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/vectordb/machineid/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/vectordb/sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/vectordb/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:14.986947 pyepsilla-0.3.5/pyepsilla/vectordb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/vectordb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/vectordb/utils/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/pyepsilla/vectordb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:10:14.990947 pyepsilla-0.3.5/pyepsilla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-21 14:10:14.000000 pyepsilla-0.3.5/pyepsilla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-21 14:10:14.000000 pyepsilla-0.3.5/pyepsilla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 14:10:14.000000 pyepsilla-0.3.5/pyepsilla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-21 14:10:14.000000 pyepsilla-0.3.5/pyepsilla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-21 14:10:14.000000 pyepsilla-0.3.5/pyepsilla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 14:10:14.990947 pyepsilla-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-21 14:10:03.000000 pyepsilla-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.688896 pyepsilla-0.3.6/pyepsilla/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.688896 pyepsilla-0.3.6/pyepsilla/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/cloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/cloud/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.688896 pyepsilla-0.3.6/pyepsilla/enterprise/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/enterprise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/enterprise/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/enterprise/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.688896 pyepsilla-0.3.6/pyepsilla/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10361 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/utils/search_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/pyepsilla/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13172 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/pyepsilla/vectordb/machineid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/machineid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/machineid/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/pyepsilla/vectordb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/utils/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/pyepsilla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-26 16:01:43.000000 pyepsilla-0.3.6/pyepsilla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-26 16:01:43.000000 pyepsilla-0.3.6/pyepsilla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:01:43.000000 pyepsilla-0.3.6/pyepsilla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 16:01:43.000000 pyepsilla-0.3.6/pyepsilla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 16:01:43.000000 pyepsilla-0.3.6/pyepsilla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/setup.py
```

### Comparing `pyepsilla-0.3.5/LICENSE.txt` & `pyepsilla-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/README.md` & `pyepsilla-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/pyepsilla/cloud/client.py` & `pyepsilla-0.3.6/pyepsilla/cloud/client.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/pyepsilla/cloud/sentry.py` & `pyepsilla-0.3.6/pyepsilla/cloud/sentry.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/pyepsilla/enterprise/client.py` & `pyepsilla-0.3.6/pyepsilla/enterprise/client.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/pyepsilla/enterprise/sentry.py` & `pyepsilla-0.3.6/pyepsilla/enterprise/sentry.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/pyepsilla/utils/search_engine.py` & `pyepsilla-0.3.6/pyepsilla/utils/search_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             # Raise exception if the primary_key_field is not found in the record
             if self._primary_key_field not in record:
                 raise Exception(f"Primary key field {self._primary_key_field} not found in the response from table {self._table_name}")
             record["@id"] = record[self._primary_key_field]
         return response["result"]
 
 class Reranker:
-    def rerank(self, candidates: list[list[any]]) -> list[any]:
+    def rerank(self, candidates: list[list[any]], query: str = None) -> list[any]:
         pass
 
 class RRFReRanker(Reranker):
     def __init__(self, weights: list[float] = None, k = 50, limit = None):
         self._weights = weights
         self._k = k
         self._limit = limit
```

### Comparing `pyepsilla-0.3.5/pyepsilla/vectordb/client.py` & `pyepsilla-0.3.6/pyepsilla/vectordb/client.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/pyepsilla/vectordb/field.py` & `pyepsilla-0.3.6/pyepsilla/vectordb/field.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/pyepsilla/vectordb/machineid/__init__.py` & `pyepsilla-0.3.6/pyepsilla/vectordb/machineid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/pyepsilla/vectordb/sentry.py` & `pyepsilla-0.3.6/pyepsilla/vectordb/sentry.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/pyepsilla/vectordb/telemetry.py` & `pyepsilla-0.3.6/pyepsilla/vectordb/telemetry.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/pyepsilla/vectordb/utils/embedding_functions.py` & `pyepsilla-0.3.6/pyepsilla/vectordb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/pyepsilla.egg-info/SOURCES.txt` & `pyepsilla-0.3.6/pyepsilla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.5/setup.py` & `pyepsilla-0.3.6/setup.py`

 * *Files identical despite different names*

