# Comparing `tmp/sru_queryer-1.0.2.tar.gz` & `tmp/sru_queryer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sru_queryer-1.0.2.tar", last modified: Mon Apr 22 14:46:24 2024, max compression
+gzip compressed data, was "sru_queryer-1.0.3.tar", last modified: Fri Apr 26 16:40:53 2024, max compression
```

## Comparing `sru_queryer-1.0.2.tar` & `sru_queryer-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-22 14:46:24.098927 sru_queryer-1.0.2/
--rw-r--r--   0 ejones99   (505) staff       (20)    11354 2024-04-17 20:20:30.000000 sru_queryer-1.0.2/LICENSE
--rw-r--r--   0 ejones99   (505) staff       (20)    39386 2024-04-22 14:46:24.098667 sru_queryer-1.0.2/PKG-INFO
--rw-r--r--   0 ejones99   (505) staff       (20)      512 2024-04-22 14:44:43.000000 sru_queryer-1.0.2/pyproject.toml
--rw-r--r--   0 ejones99   (505) staff       (20)    38890 2024-04-17 17:20:50.000000 sru_queryer-1.0.2/readme.md
--rw-r--r--   0 ejones99   (505) staff       (20)       38 2024-04-22 14:46:24.098978 sru_queryer-1.0.2/setup.cfg
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-22 14:46:24.087633 sru_queryer-1.0.2/src/
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-22 14:46:24.089605 sru_queryer-1.0.2/src/sru_queryer/
--rw-r--r--   0 ejones99   (505) staff       (20)      165 2024-04-17 17:18:26.000000 sru_queryer-1.0.2/src/sru_queryer/__init__.py
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-22 14:46:24.094977 sru_queryer-1.0.2/src/sru_queryer/_base/
--rw-r--r--   0 ejones99   (505) staff       (20)        0 2024-04-17 17:18:54.000000 sru_queryer-1.0.2/src/sru_queryer/_base/__init__.py
--rw-r--r--   0 ejones99   (505) staff       (20)     5619 2024-04-22 13:47:27.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_cql_boolean_operators.py
--rw-r--r--   0 ejones99   (505) staff       (20)      463 2024-04-22 13:47:27.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_cql_literal.py
--rw-r--r--   0 ejones99   (505) staff       (20)     4653 2024-04-22 13:47:27.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_cql_modifiers.py
--rw-r--r--   0 ejones99   (505) staff       (20)     3107 2024-04-17 17:18:54.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_drivers.py
--rw-r--r--   0 ejones99   (505) staff       (20)     3657 2024-04-22 13:47:27.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_query.py
--rw-r--r--   0 ejones99   (505) staff       (20)     3464 2024-04-22 13:47:27.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_search_index_config.py
--rw-r--r--   0 ejones99   (505) staff       (20)     2961 2024-04-22 13:47:27.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_sort_key.py
--rw-r--r--   0 ejones99   (505) staff       (20)     5125 2024-04-22 13:47:27.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_sru_aux_formatter.py
--rw-r--r--   0 ejones99   (505) staff       (20)     1205 2024-04-22 13:47:27.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_sru_configuration.py
--rw-r--r--   0 ejones99   (505) staff       (20)    13516 2024-04-22 13:47:27.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_sru_explain_xml_parser.py
--rw-r--r--   0 ejones99   (505) staff       (20)     6060 2024-04-22 13:47:27.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_sru_util.py
--rw-r--r--   0 ejones99   (505) staff       (20)    11536 2024-04-22 13:47:27.000000 sru_queryer-1.0.2/src/sru_queryer/_base/_sru_validator.py
--rw-r--r--   0 ejones99   (505) staff       (20)      441 2024-04-17 17:18:26.000000 sru_queryer-1.0.2/src/sru_queryer/cql.py
--rw-r--r--   0 ejones99   (505) staff       (20)       67 2024-04-17 17:18:26.000000 sru_queryer-1.0.2/src/sru_queryer/drivers.py
--rw-r--r--   0 ejones99   (505) staff       (20)      223 2024-04-17 17:18:37.000000 sru_queryer-1.0.2/src/sru_queryer/sru.py
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-22 14:46:24.098344 sru_queryer-1.0.2/src/sru_queryer.egg-info/
--rw-r--r--   0 ejones99   (505) staff       (20)    39386 2024-04-22 14:46:24.000000 sru_queryer-1.0.2/src/sru_queryer.egg-info/PKG-INFO
--rw-r--r--   0 ejones99   (505) staff       (20)     1137 2024-04-22 14:46:24.000000 sru_queryer-1.0.2/src/sru_queryer.egg-info/SOURCES.txt
--rw-r--r--   0 ejones99   (505) staff       (20)        1 2024-04-22 14:46:24.000000 sru_queryer-1.0.2/src/sru_queryer.egg-info/dependency_links.txt
--rw-r--r--   0 ejones99   (505) staff       (20)       35 2024-04-22 14:46:24.000000 sru_queryer-1.0.2/src/sru_queryer.egg-info/requires.txt
--rw-r--r--   0 ejones99   (505) staff       (20)       12 2024-04-22 14:46:24.000000 sru_queryer-1.0.2/src/sru_queryer.egg-info/top_level.txt
-drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-22 14:46:24.098028 sru_queryer-1.0.2/tests/
--rw-r--r--   0 ejones99   (505) staff       (20)    10836 2024-04-17 17:20:07.000000 sru_queryer-1.0.2/tests/test_cql_boolean_operators.py
--rw-r--r--   0 ejones99   (505) staff       (20)     1130 2024-04-17 17:20:07.000000 sru_queryer-1.0.2/tests/test_cql_literal.py
--rw-r--r--   0 ejones99   (505) staff       (20)     5583 2024-04-17 17:20:07.000000 sru_queryer-1.0.2/tests/test_cql_modifiers.py
--rw-r--r--   0 ejones99   (505) staff       (20)     4457 2024-04-17 17:20:07.000000 sru_queryer-1.0.2/tests/test_search_index_config.py
--rw-r--r--   0 ejones99   (505) staff       (20)     3439 2024-04-17 17:20:07.000000 sru_queryer-1.0.2/tests/test_sort_key.py
--rw-r--r--   0 ejones99   (505) staff       (20)     8162 2024-04-17 17:20:07.000000 sru_queryer-1.0.2/tests/test_sru_aux_formatter.py
--rw-r--r--   0 ejones99   (505) staff       (20)    20854 2024-04-17 17:20:07.000000 sru_queryer-1.0.2/tests/test_sru_explain_xml_parser.py
--rw-r--r--   0 ejones99   (505) staff       (20)     9898 2024-04-17 17:20:07.000000 sru_queryer-1.0.2/tests/test_sru_query.py
--rw-r--r--   0 ejones99   (505) staff       (20)     7909 2024-04-17 17:20:07.000000 sru_queryer-1.0.2/tests/test_sru_util.py
--rw-r--r--   0 ejones99   (505) staff       (20)    10488 2024-04-17 17:20:07.000000 sru_queryer-1.0.2/tests/test_sru_validator.py
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.463308 sru_queryer-1.0.3/
+-rw-r--r--   0 ejones99   (505) staff       (20)    11354 2024-04-17 20:20:30.000000 sru_queryer-1.0.3/LICENSE
+-rw-r--r--   0 ejones99   (505) staff       (20)    39386 2024-04-26 16:40:53.463013 sru_queryer-1.0.3/PKG-INFO
+-rw-r--r--   0 ejones99   (505) staff       (20)      512 2024-04-26 16:35:01.000000 sru_queryer-1.0.3/pyproject.toml
+-rw-r--r--   0 ejones99   (505) staff       (20)    38890 2024-04-17 17:20:50.000000 sru_queryer-1.0.3/readme.md
+-rw-r--r--   0 ejones99   (505) staff       (20)       38 2024-04-26 16:40:53.463366 sru_queryer-1.0.3/setup.cfg
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.452228 sru_queryer-1.0.3/src/
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.454314 sru_queryer-1.0.3/src/sru_queryer/
+-rw-r--r--   0 ejones99   (505) staff       (20)      165 2024-04-17 17:18:26.000000 sru_queryer-1.0.3/src/sru_queryer/__init__.py
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.458911 sru_queryer-1.0.3/src/sru_queryer/_base/
+-rw-r--r--   0 ejones99   (505) staff       (20)        0 2024-04-17 17:18:54.000000 sru_queryer-1.0.3/src/sru_queryer/_base/__init__.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     5619 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_cql_boolean_operators.py
+-rw-r--r--   0 ejones99   (505) staff       (20)      463 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_cql_literal.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     4653 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_cql_modifiers.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     3107 2024-04-17 17:18:54.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_drivers.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     3657 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_query.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     3464 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_search_index_config.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     2961 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sort_key.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     5125 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sru_aux_formatter.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     1205 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sru_configuration.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    13516 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sru_explain_xml_parser.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     6060 2024-04-22 13:47:27.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sru_util.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    11334 2024-04-26 16:17:40.000000 sru_queryer-1.0.3/src/sru_queryer/_base/_sru_validator.py
+-rw-r--r--   0 ejones99   (505) staff       (20)      441 2024-04-17 17:18:26.000000 sru_queryer-1.0.3/src/sru_queryer/cql.py
+-rw-r--r--   0 ejones99   (505) staff       (20)       67 2024-04-17 17:18:26.000000 sru_queryer-1.0.3/src/sru_queryer/drivers.py
+-rw-r--r--   0 ejones99   (505) staff       (20)      223 2024-04-17 17:18:37.000000 sru_queryer-1.0.3/src/sru_queryer/sru.py
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.462516 sru_queryer-1.0.3/src/sru_queryer.egg-info/
+-rw-r--r--   0 ejones99   (505) staff       (20)    39386 2024-04-26 16:40:53.000000 sru_queryer-1.0.3/src/sru_queryer.egg-info/PKG-INFO
+-rw-r--r--   0 ejones99   (505) staff       (20)     1137 2024-04-26 16:40:53.000000 sru_queryer-1.0.3/src/sru_queryer.egg-info/SOURCES.txt
+-rw-r--r--   0 ejones99   (505) staff       (20)        1 2024-04-26 16:40:53.000000 sru_queryer-1.0.3/src/sru_queryer.egg-info/dependency_links.txt
+-rw-r--r--   0 ejones99   (505) staff       (20)       35 2024-04-26 16:40:53.000000 sru_queryer-1.0.3/src/sru_queryer.egg-info/requires.txt
+-rw-r--r--   0 ejones99   (505) staff       (20)       12 2024-04-26 16:40:53.000000 sru_queryer-1.0.3/src/sru_queryer.egg-info/top_level.txt
+drwxr-xr-x   0 ejones99   (505) staff       (20)        0 2024-04-26 16:40:53.462129 sru_queryer-1.0.3/tests/
+-rw-r--r--   0 ejones99   (505) staff       (20)    10836 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_cql_boolean_operators.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     1130 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_cql_literal.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     5583 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_cql_modifiers.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     4457 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_search_index_config.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     3439 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sort_key.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     8162 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sru_aux_formatter.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    20854 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sru_explain_xml_parser.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     9898 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sru_query.py
+-rw-r--r--   0 ejones99   (505) staff       (20)     7909 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sru_util.py
+-rw-r--r--   0 ejones99   (505) staff       (20)    10488 2024-04-17 17:20:07.000000 sru_queryer-1.0.3/tests/test_sru_validator.py
```

### Comparing `sru_queryer-1.0.2/LICENSE` & `sru_queryer-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/PKG-INFO` & `sru_queryer-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: sru-queryer
-Version: 1.0.2
+Version: 1.0.3
 Summary: A utility for integrating SRU queries into your applications.
 Author-email: Erik Jones <ejones99@umd.edu>
 Maintainer-email: USMAI <libclas@umd.edu>
 Keywords: sru,library,api
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7.17
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.27.1
+Requires-Dist: requests>=2.27.1
 Requires-Dist: xmltodict>=0.13.0
 
 # USMAI SRU Queryer
 
 Welcome to SRU Queryer, a library for working with Search/Retrieval via URL (SRU) created by the USMAI Library Consortium. This package is designed to make working with SRU simple and accurate!
 
 Using this utility has a few big benefits, such as:
```

### Comparing `sru_queryer-1.0.2/pyproject.toml` & `sru_queryer-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sru-queryer"
-version = "1.0.2"
+version = "1.0.3"
 description = "A utility for integrating SRU queries into your applications."
 readme = "readme.md"
 requires-python = ">=3.7.17"
 keywords = ["sru", "library", "api"]
 
 authors = [
     {name = "Erik Jones", email = "ejones99@umd.edu"},
@@ -12,8 +12,8 @@
 
 maintainers = [
     {name = "USMAI", email = "libclas@umd.edu"},
 ]
 
 classifiers = ["Programming Language :: Python :: 3", "Development Status :: 5 - Production/Stable"]
 
-dependencies = ["requests==2.27.1", "xmltodict>=0.13.0"]
+dependencies = ["requests>=2.27.1", "xmltodict>=0.13.0"]
```

### Comparing `sru_queryer-1.0.2/readme.md` & `sru_queryer-1.0.3/readme.md`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/src/sru_queryer/_base/_cql_boolean_operators.py` & `sru_queryer-1.0.3/src/sru_queryer/_base/_cql_boolean_operators.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/src/sru_queryer/_base/_cql_modifiers.py` & `sru_queryer-1.0.3/src/sru_queryer/_base/_cql_modifiers.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/src/sru_queryer/_base/_drivers.py` & `sru_queryer-1.0.3/src/sru_queryer/_base/_drivers.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/src/sru_queryer/_base/_query.py` & `sru_queryer-1.0.3/src/sru_queryer/_base/_query.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/src/sru_queryer/_base/_search_index_config.py` & `sru_queryer-1.0.3/src/sru_queryer/_base/_search_index_config.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/src/sru_queryer/_base/_sort_key.py` & `sru_queryer-1.0.3/src/sru_queryer/_base/_sort_key.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/src/sru_queryer/_base/_sru_aux_formatter.py` & `sru_queryer-1.0.3/src/sru_queryer/_base/_sru_aux_formatter.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/src/sru_queryer/_base/_sru_configuration.py` & `sru_queryer-1.0.3/src/sru_queryer/_base/_sru_configuration.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/src/sru_queryer/_base/_sru_explain_xml_parser.py` & `sru_queryer-1.0.3/src/sru_queryer/_base/_sru_explain_xml_parser.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/src/sru_queryer/_base/_sru_util.py` & `sru_queryer-1.0.3/src/sru_queryer/_base/_sru_util.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/src/sru_queryer/_base/_sru_validator.py` & `sru_queryer-1.0.3/src/sru_queryer/_base/_sru_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,22 +120,17 @@
                 
             
     @staticmethod
     def validate_base_query(sru_configuration: SRUConfiguration, start_record: str | None, maximum_record: str | None, record_schema: str | None, record_packing: str | None) -> None:
         if start_record and start_record < 1:
             raise ValueError("Start record must be greater than 0.")
 
-        if maximum_record:
-            if start_record:
-                if maximum_record < start_record:
-                    raise ValueError("Maximum record must be greater than start record.")
-            
-            if sru_configuration.max_records_supported:
-                if maximum_record > sru_configuration.max_records_supported:
-                    raise ValueError(f"Maximum records returned must be less than {str(sru_configuration.max_records_supported)}.") 
+        if maximum_record and sru_configuration.max_records_supported:
+            if maximum_record > sru_configuration.max_records_supported:
+                raise ValueError(f"Maximum records returned must be less than {str(sru_configuration.max_records_supported)}.") 
         
         if record_schema:
             if record_schema not in sru_configuration.available_record_schemas:
                 raise ValueError(f"Record schema '{record_schema}' is not available.")
             
         if record_packing:
             if record_packing not in sru_configuration.available_record_packing_values:
```

### Comparing `sru_queryer-1.0.2/src/sru_queryer.egg-info/PKG-INFO` & `sru_queryer-1.0.3/src/sru_queryer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: sru-queryer
-Version: 1.0.2
+Version: 1.0.3
 Summary: A utility for integrating SRU queries into your applications.
 Author-email: Erik Jones <ejones99@umd.edu>
 Maintainer-email: USMAI <libclas@umd.edu>
 Keywords: sru,library,api
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7.17
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.27.1
+Requires-Dist: requests>=2.27.1
 Requires-Dist: xmltodict>=0.13.0
 
 # USMAI SRU Queryer
 
 Welcome to SRU Queryer, a library for working with Search/Retrieval via URL (SRU) created by the USMAI Library Consortium. This package is designed to make working with SRU simple and accurate!
 
 Using this utility has a few big benefits, such as:
```

### Comparing `sru_queryer-1.0.2/src/sru_queryer.egg-info/SOURCES.txt` & `sru_queryer-1.0.3/src/sru_queryer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/tests/test_cql_boolean_operators.py` & `sru_queryer-1.0.3/tests/test_cql_boolean_operators.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/tests/test_cql_literal.py` & `sru_queryer-1.0.3/tests/test_cql_literal.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/tests/test_cql_modifiers.py` & `sru_queryer-1.0.3/tests/test_cql_modifiers.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/tests/test_search_index_config.py` & `sru_queryer-1.0.3/tests/test_search_index_config.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/tests/test_sort_key.py` & `sru_queryer-1.0.3/tests/test_sort_key.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/tests/test_sru_aux_formatter.py` & `sru_queryer-1.0.3/tests/test_sru_aux_formatter.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/tests/test_sru_explain_xml_parser.py` & `sru_queryer-1.0.3/tests/test_sru_explain_xml_parser.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/tests/test_sru_query.py` & `sru_queryer-1.0.3/tests/test_sru_query.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/tests/test_sru_util.py` & `sru_queryer-1.0.3/tests/test_sru_util.py`

 * *Files identical despite different names*

### Comparing `sru_queryer-1.0.2/tests/test_sru_validator.py` & `sru_queryer-1.0.3/tests/test_sru_validator.py`

 * *Files identical despite different names*

