# Comparing `tmp/prefect_snowflake-0.27.4.tar.gz` & `tmp/prefect_snowflake-0.27.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_snowflake-0.27.4.tar", last modified: Thu Apr 25 19:14:19 2024, max compression
+gzip compressed data, was "prefect_snowflake-0.27.5.tar", last modified: Fri Apr 26 15:04:01 2024, max compression
```

## Comparing `prefect_snowflake-0.27.4.tar` & `prefect_snowflake-0.27.5.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:14:19.647247 prefect_snowflake-0.27.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-25 19:14:19.647247 prefect_snowflake-0.27.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:14:19.643247 prefect_snowflake-0.27.4/prefect_snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/prefect_snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/prefect_snowflake/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    30139 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/prefect_snowflake/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:14:19.643247 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:14:19.647247 prefect_snowflake-0.27.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:14:19.643247 prefect_snowflake-0.27.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:14:19.643247 prefect_snowflake-0.27.4/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_data/test_cert.p8
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_data/test_cert_malformed_format.p8
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_data/test_cert_no_pass.p8
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:01.621871 prefect_snowflake-0.27.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11231 2024-04-26 15:04:01.617871 prefect_snowflake-0.27.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:01.613871 prefect_snowflake-0.27.5/prefect_snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/prefect_snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-26 15:04:01.000000 prefect_snowflake-0.27.5/prefect_snowflake/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/prefect_snowflake/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30138 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/prefect_snowflake/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:01.617871 prefect_snowflake-0.27.5/prefect_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11231 2024-04-26 15:04:01.000000 prefect_snowflake-0.27.5/prefect_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-26 15:04:01.000000 prefect_snowflake-0.27.5/prefect_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:04:01.000000 prefect_snowflake-0.27.5/prefect_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-26 15:04:01.000000 prefect_snowflake-0.27.5/prefect_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 15:04:01.000000 prefect_snowflake-0.27.5/prefect_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 15:04:01.000000 prefect_snowflake-0.27.5/prefect_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:01.621871 prefect_snowflake-0.27.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:01.617871 prefect_snowflake-0.27.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/tests/test_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:01.617871 prefect_snowflake-0.27.5/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/tests/test_data/test_cert.p8
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/tests/test_data/test_cert_malformed_format.p8
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/tests/test_data/test_cert_no_pass.p8
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-26 15:03:49.000000 prefect_snowflake-0.27.5/tests/test_version.py
```

### Comparing `prefect_snowflake-0.27.4/PKG-INFO` & `prefect_snowflake-0.27.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-snowflake
-Version: 0.27.4
+Version: 0.27.5
 Summary: Prefect integrations for interacting with Snowflake
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-snowflake
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: snowflake-connector-python>=2.7.6
 Requires-Dist: prefect>=2.13.5
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
```

### Comparing `prefect_snowflake-0.27.4/README.md` & `prefect_snowflake-0.27.5/README.md`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.4/prefect_snowflake/credentials.py` & `prefect_snowflake-0.27.5/prefect_snowflake/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.4/prefect_snowflake/database.py` & `prefect_snowflake-0.27.5/prefect_snowflake/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         poll_frequency_s: The number of seconds before checking query.
 
     Examples:
         Load stored Snowflake connector as a context manager:
         ```python
         from prefect_snowflake.database import SnowflakeConnector
 
-        snowflake_connector = SnowflakeConnector.load("BLOCK_NAME"):
+        snowflake_connector = SnowflakeConnector.load("BLOCK_NAME")
         ```
 
         Insert data into database and fetch results.
         ```python
         from prefect_snowflake.database import SnowflakeConnector
 
         with SnowflakeConnector.load("BLOCK_NAME") as conn:
```

### Comparing `prefect_snowflake-0.27.4/prefect_snowflake.egg-info/PKG-INFO` & `prefect_snowflake-0.27.5/prefect_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-snowflake
-Version: 0.27.4
+Version: 0.27.5
 Summary: Prefect integrations for interacting with Snowflake
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-snowflake
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: snowflake-connector-python>=2.7.6
 Requires-Dist: prefect>=2.13.5
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
```

### Comparing `prefect_snowflake-0.27.4/prefect_snowflake.egg-info/SOURCES.txt` & `prefect_snowflake-0.27.5/prefect_snowflake.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 prefect_snowflake/__init__.py
 prefect_snowflake/_version.py
 prefect_snowflake/credentials.py
 prefect_snowflake/database.py
 prefect_snowflake.egg-info/PKG-INFO
```

### Comparing `prefect_snowflake-0.27.4/pyproject.toml` & `prefect_snowflake-0.27.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.4/tests/conftest.py` & `prefect_snowflake-0.27.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.4/tests/test_block_standards.py` & `prefect_snowflake-0.27.5/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.4/tests/test_credentials.py` & `prefect_snowflake-0.27.5/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.4/tests/test_data/test_cert.p8` & `prefect_snowflake-0.27.5/tests/test_data/test_cert.p8`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.4/tests/test_data/test_cert_malformed_format.p8` & `prefect_snowflake-0.27.5/tests/test_data/test_cert_malformed_format.p8`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.4/tests/test_data/test_cert_no_pass.p8` & `prefect_snowflake-0.27.5/tests/test_data/test_cert_no_pass.p8`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.4/tests/test_database.py` & `prefect_snowflake-0.27.5/tests/test_database.py`

 * *Files identical despite different names*

