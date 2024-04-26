# Comparing `tmp/airbyte-source-pokeapi-0.2.0.dev202404081051.tar.gz` & `tmp/airbyte_source_pokeapi-0.2.0.dev202404262155.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-pokeapi-0.2.0.dev202404081051.tar", last modified: Mon Apr  8 10:52:14 2024, max compression
+gzip compressed data, was "airbyte_source_pokeapi-0.2.0.dev202404262155.tar", last modified: Fri Apr 26 21:56:12 2024, max compression
```

## Comparing `airbyte-source-pokeapi-0.2.0.dev202404081051.tar` & `airbyte_source_pokeapi-0.2.0.dev202404262155.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 10:52:14.268828 airbyte-source-pokeapi-0.2.0.dev202404081051/
--rw-r--r--   0 root         (0) root         (0)     4199 2024-04-08 10:52:14.268828 airbyte-source-pokeapi-0.2.0.dev202404081051/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4011 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 10:52:14.268828 airbyte-source-pokeapi-0.2.0.dev202404081051/airbyte_source_pokeapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4199 2024-04-08 10:52:14.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/airbyte_source_pokeapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      723 2024-04-08 10:52:14.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/airbyte_source_pokeapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 10:52:14.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/airbyte_source_pokeapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-08 10:52:14.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/airbyte_source_pokeapi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-08 10:52:14.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/airbyte_source_pokeapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-08 10:52:14.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/airbyte_source_pokeapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 10:52:14.268828 airbyte-source-pokeapi-0.2.0.dev202404081051/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      243 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4067 2024-04-08 10:52:14.272828 airbyte-source-pokeapi-0.2.0.dev202404081051/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      919 2024-04-08 10:52:12.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 10:52:14.268828 airbyte-source-pokeapi-0.2.0.dev202404081051/source_pokeapi/
--rw-r--r--   0 root         (0) root         (0)      126 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/source_pokeapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)      828 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/source_pokeapi/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      232 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/source_pokeapi/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 10:52:14.268828 airbyte-source-pokeapi-0.2.0.dev202404081051/source_pokeapi/schemas/
--rw-r--r--   0 root         (0) root         (0)     8544 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/source_pokeapi/schemas/pokemon.json
--rw-r--r--   0 root         (0) root         (0)      476 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/source_pokeapi/source.py
--rw-r--r--   0 root         (0) root         (0)    17094 2024-04-08 10:48:55.000000 airbyte-source-pokeapi-0.2.0.dev202404081051/source_pokeapi/spec.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 21:56:12.681567 airbyte_source_pokeapi-0.2.0.dev202404262155/
+-rw-r--r--   0 root         (0) root         (0)     4199 2024-04-26 21:56:12.681567 airbyte_source_pokeapi-0.2.0.dev202404262155/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4011 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 21:56:12.681567 airbyte_source_pokeapi-0.2.0.dev202404262155/airbyte_source_pokeapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4199 2024-04-26 21:56:12.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/airbyte_source_pokeapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      723 2024-04-26 21:56:12.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/airbyte_source_pokeapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 21:56:12.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/airbyte_source_pokeapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-26 21:56:12.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/airbyte_source_pokeapi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 21:56:12.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/airbyte_source_pokeapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-26 21:56:12.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/airbyte_source_pokeapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 21:56:12.677567 airbyte_source_pokeapi-0.2.0.dev202404262155/integration_tests/
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/integration_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/integration_tests/abnormal_state.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/integration_tests/acceptance.py
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/integration_tests/configured_catalog.json
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/integration_tests/invalid_config.json
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/integration_tests/sample_config.json
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/integration_tests/sample_state.json
+-rw-r--r--   0 root         (0) root         (0)     4067 2024-04-26 21:56:12.681567 airbyte_source_pokeapi-0.2.0.dev202404262155/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      919 2024-04-26 21:56:10.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 21:56:12.681567 airbyte_source_pokeapi-0.2.0.dev202404262155/source_pokeapi/
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/source_pokeapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      828 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/source_pokeapi/manifest.yaml
+-rw-r--r--   0 root         (0) root         (0)      232 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/source_pokeapi/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 21:56:12.681567 airbyte_source_pokeapi-0.2.0.dev202404262155/source_pokeapi/schemas/
+-rw-r--r--   0 root         (0) root         (0)     8544 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/source_pokeapi/schemas/pokemon.json
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/source_pokeapi/source.py
+-rw-r--r--   0 root         (0) root         (0)    17094 2024-04-26 21:52:46.000000 airbyte_source_pokeapi-0.2.0.dev202404262155/source_pokeapi/spec.yaml
```

### Comparing `airbyte-source-pokeapi-0.2.0.dev202404081051/PKG-INFO` & `airbyte_source_pokeapi-0.2.0.dev202404262155/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-pokeapi
-Version: 0.2.0.dev202404081051
+Version: 0.2.0.dev202404262155
 Summary: Source implementation for Pokeapi.
 Author: Airbyte
 Author-email: contact@airbyte.io
 Description-Content-Type: text/markdown
 Requires-Dist: airbyte-cdk
 Provides-Extra: tests
 Requires-Dist: requests-mock~=1.9.3; extra == "tests"
```

### Comparing `airbyte-source-pokeapi-0.2.0.dev202404081051/README.md` & `airbyte_source_pokeapi-0.2.0.dev202404262155/README.md`

 * *Files identical despite different names*

### Comparing `airbyte-source-pokeapi-0.2.0.dev202404081051/airbyte_source_pokeapi.egg-info/PKG-INFO` & `airbyte_source_pokeapi-0.2.0.dev202404262155/airbyte_source_pokeapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-pokeapi
-Version: 0.2.0.dev202404081051
+Version: 0.2.0.dev202404262155
 Summary: Source implementation for Pokeapi.
 Author: Airbyte
 Author-email: contact@airbyte.io
 Description-Content-Type: text/markdown
 Requires-Dist: airbyte-cdk
 Provides-Extra: tests
 Requires-Dist: requests-mock~=1.9.3; extra == "tests"
```

### Comparing `airbyte-source-pokeapi-0.2.0.dev202404081051/airbyte_source_pokeapi.egg-info/SOURCES.txt` & `airbyte_source_pokeapi-0.2.0.dev202404262155/airbyte_source_pokeapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airbyte-source-pokeapi-0.2.0.dev202404081051/setup.cfg` & `airbyte_source_pokeapi-0.2.0.dev202404262155/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = airbyte-source-pokeapi
-version = 0.2.0.dev202404081051
+version = 0.2.0.dev202404262155
 author = Airbyte
 author_email = contact@airbyte.io
 long_description = # Pokeapi Source
 	
 	This is the repository for the Pokeapi configuration based source connector.
 	For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pokeapi).
```

### Comparing `airbyte-source-pokeapi-0.2.0.dev202404081051/setup.py` & `airbyte_source_pokeapi-0.2.0.dev202404262155/setup.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-pokeapi-0.2.0.dev202404081051/source_pokeapi/manifest.yaml` & `airbyte_source_pokeapi-0.2.0.dev202404262155/source_pokeapi/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-pokeapi-0.2.0.dev202404081051/source_pokeapi/schemas/pokemon.json` & `airbyte_source_pokeapi-0.2.0.dev202404262155/source_pokeapi/schemas/pokemon.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pokeapi-0.2.0.dev202404081051/source_pokeapi/spec.yaml` & `airbyte_source_pokeapi-0.2.0.dev202404262155/source_pokeapi/spec.yaml`

 * *Files identical despite different names*

