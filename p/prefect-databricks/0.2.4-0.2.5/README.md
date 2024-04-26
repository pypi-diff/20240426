# Comparing `tmp/prefect_databricks-0.2.4.tar.gz` & `tmp/prefect_databricks-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_databricks-0.2.4.tar", last modified: Thu Apr 25 19:20:20 2024, max compression
+gzip compressed data, was "prefect_databricks-0.2.5.tar", last modified: Fri Apr 26 15:03:56 2024, max compression
```

## Comparing `prefect_databricks-0.2.4.tar` & `prefect_databricks-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.327712 prefect_databricks-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-25 19:20:20.327712 prefect_databricks-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.319712 prefect_databricks-0.2.4/prefect_databricks/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:19.000000 prefect_databricks-0.2.4/prefect_databricks/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    81198 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.323712 prefect_databricks-0.2.4/prefect_databricks/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   168341 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.323712 prefect_databricks-0.2.4/prefect_databricks/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   178999 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/schemas/jobs-2.1-aws.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.323712 prefect_databricks-0.2.4/prefect_databricks/schemas/original/
--rw-r--r--   0 runner    (1001) docker     (127)   178843 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/prefect_databricks/schemas/original/jobs-2.1-aws.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.327712 prefect_databricks-0.2.4/prefect_databricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 19:20:20.000000 prefect_databricks-0.2.4/prefect_databricks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:20.327712 prefect_databricks-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:20.323712 prefect_databricks-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/mock_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-25 19:20:01.000000 prefect_databricks-0.2.4/tests/test_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.199693 prefect_databricks-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-04-26 15:03:56.199693 prefect_databricks-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.195693 prefect_databricks-0.2.5/prefect_databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81198 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.195693 prefect_databricks-0.2.5/prefect_databricks/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   168341 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.195693 prefect_databricks-0.2.5/prefect_databricks/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   178999 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/schemas/jobs-2.1-aws.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.195693 prefect_databricks-0.2.5/prefect_databricks/schemas/original/
+-rw-r--r--   0 runner    (1001) docker     (127)   178843 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/prefect_databricks/schemas/original/jobs-2.1-aws.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.199693 prefect_databricks-0.2.5/prefect_databricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-26 15:03:56.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 15:03:55.000000 prefect_databricks-0.2.5/prefect_databricks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:03:56.199693 prefect_databricks-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.199693 prefect_databricks-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/mock_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-26 15:03:43.000000 prefect_databricks-0.2.5/tests/test_version.py
```

### Comparing `prefect_databricks-0.2.4/PKG-INFO` & `prefect_databricks-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-databricks
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations with Databricks
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-databricks
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
 Requires-Dist: prefect>=2.14.10
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
```

### Comparing `prefect_databricks-0.2.4/README.md` & `prefect_databricks-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/prefect_databricks/credentials.py` & `prefect_databricks-0.2.5/prefect_databricks/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/prefect_databricks/flows.py` & `prefect_databricks-0.2.5/prefect_databricks/flows.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/prefect_databricks/jobs.py` & `prefect_databricks-0.2.5/prefect_databricks/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/prefect_databricks/models/jobs.py` & `prefect_databricks-0.2.5/prefect_databricks/models/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/prefect_databricks/rest.py` & `prefect_databricks-0.2.5/prefect_databricks/rest.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/prefect_databricks/schemas/jobs-2.1-aws.yaml` & `prefect_databricks-0.2.5/prefect_databricks/schemas/jobs-2.1-aws.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/prefect_databricks/schemas/original/jobs-2.1-aws.yaml` & `prefect_databricks-0.2.5/prefect_databricks/schemas/original/jobs-2.1-aws.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/prefect_databricks.egg-info/PKG-INFO` & `prefect_databricks-0.2.5/prefect_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-databricks
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations with Databricks
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-databricks
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
 Requires-Dist: prefect>=2.14.10
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
```

### Comparing `prefect_databricks-0.2.4/prefect_databricks.egg-info/SOURCES.txt` & `prefect_databricks-0.2.5/prefect_databricks.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 prefect_databricks/__init__.py
 prefect_databricks/_version.py
 prefect_databricks/credentials.py
 prefect_databricks/flows.py
 prefect_databricks/jobs.py
@@ -19,8 +21,9 @@
 tests/conftest.py
 tests/mock_schema.yaml
 tests/test_block_standards.py
 tests/test_credentials.py
 tests/test_flows.py
 tests/test_generate.py
 tests/test_jobs.py
-tests/test_rest.py
+tests/test_rest.py
+tests/test_version.py
```

### Comparing `prefect_databricks-0.2.4/pyproject.toml` & `prefect_databricks-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/tests/mock_schema.yaml` & `prefect_databricks-0.2.5/tests/mock_schema.yaml`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/tests/test_block_standards.py` & `prefect_databricks-0.2.5/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/tests/test_flows.py` & `prefect_databricks-0.2.5/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/tests/test_generate.py` & `prefect_databricks-0.2.5/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/tests/test_jobs.py` & `prefect_databricks-0.2.5/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_databricks-0.2.4/tests/test_rest.py` & `prefect_databricks-0.2.5/tests/test_rest.py`

 * *Files identical despite different names*

