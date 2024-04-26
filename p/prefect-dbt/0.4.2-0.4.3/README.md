# Comparing `tmp/prefect_dbt-0.4.2.tar.gz` & `tmp/prefect_dbt-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_dbt-0.4.2.tar", last modified: Thu Apr 25 19:20:12 2024, max compression
+gzip compressed data, was "prefect_dbt-0.4.3.tar", last modified: Fri Apr 26 15:03:58 2024, max compression
```

## Comparing `prefect_dbt-0.4.2.tar` & `prefect_dbt-0.4.3.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.740582 prefect_dbt-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-04-25 19:20:12.740582 prefect_dbt-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.728582 prefect_dbt-0.4.2/prefect_dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.732582 prefect_dbt-0.4.2/prefect_dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15255 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.732582 prefect_dbt-0.4.2/prefect_dbt/cli/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/configs/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/configs/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/configs/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cli/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.732582 prefect_dbt-0.4.2/prefect_dbt/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    43316 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/prefect_dbt/cloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.736582 prefect_dbt-0.4.2/prefect_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 19:20:12.000000 prefect_dbt-0.4.2/prefect_dbt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:12.740582 prefect_dbt-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.732582 prefect_dbt-0.4.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.732582 prefect_dbt-0.4.2/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.736582 prefect_dbt-0.4.2/tests/cli/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/configs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/configs/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/configs/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/configs/test_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cli/test_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:12.736582 prefect_dbt-0.4.2/tests/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cloud/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cloud/test_cloud_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cloud/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cloud/test_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/cloud/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 19:20:00.000000 prefect_dbt-0.4.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.745123 prefect_dbt-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-04-26 15:03:58.745123 prefect_dbt-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.733123 prefect_dbt-0.4.3/prefect_dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.733123 prefect_dbt-0.4.3/prefect_dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15255 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.733123 prefect_dbt-0.4.3/prefect_dbt/cli/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/configs/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/configs/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/configs/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.737123 prefect_dbt-0.4.3/prefect_dbt/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43316 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.741123 prefect_dbt-0.4.3/prefect_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:03:58.745123 prefect_dbt-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.737123 prefect_dbt-0.4.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.737123 prefect_dbt-0.4.3/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.737123 prefect_dbt-0.4.3/tests/cli/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/configs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/configs/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/configs/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/configs/test_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/test_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.741123 prefect_dbt-0.4.3/tests/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cloud/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cloud/test_cloud_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cloud/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cloud/test_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cloud/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/test_version.py
```

### Comparing `prefect_dbt-0.4.2/PKG-INFO` & `prefect_dbt-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-dbt
-Version: 0.4.2
+Version: 0.4.3
 Summary: Prefect integrations for working with dbt
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dbt
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
 Requires-Dist: prefect>=2.16.6
 Requires-Dist: dbt_core>=1.1.1
 Requires-Dist: prefect_shell>=0.1.4
 Requires-Dist: sgqlc>=16.0.0
 Provides-Extra: snowflake
 Requires-Dist: prefect-snowflake>=0.2.4; extra == "snowflake"
 Requires-Dist: dbt-snowflake; extra == "snowflake"
```

### Comparing `prefect_dbt-0.4.2/README.md` & `prefect_dbt-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/__init__.py` & `prefect_dbt-0.4.3/prefect_dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cli/__init__.py` & `prefect_dbt-0.4.3/prefect_dbt/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cli/commands.py` & `prefect_dbt-0.4.3/prefect_dbt/cli/commands.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cli/configs/base.py` & `prefect_dbt-0.4.3/prefect_dbt/cli/configs/base.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cli/configs/bigquery.py` & `prefect_dbt-0.4.3/prefect_dbt/cli/configs/bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cli/configs/postgres.py` & `prefect_dbt-0.4.3/prefect_dbt/cli/configs/postgres.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cli/configs/snowflake.py` & `prefect_dbt-0.4.3/prefect_dbt/cli/configs/snowflake.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cli/credentials.py` & `prefect_dbt-0.4.3/prefect_dbt/cli/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cli/tasks.py` & `prefect_dbt-0.4.3/prefect_dbt/cli/tasks.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cloud/clients.py` & `prefect_dbt-0.4.3/prefect_dbt/cloud/clients.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cloud/credentials.py` & `prefect_dbt-0.4.3/prefect_dbt/cloud/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cloud/exceptions.py` & `prefect_dbt-0.4.3/prefect_dbt/cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cloud/jobs.py` & `prefect_dbt-0.4.3/prefect_dbt/cloud/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cloud/models.py` & `prefect_dbt-0.4.3/prefect_dbt/cloud/models.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cloud/runs.py` & `prefect_dbt-0.4.3/prefect_dbt/cloud/runs.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt/cloud/utils.py` & `prefect_dbt-0.4.3/prefect_dbt/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/prefect_dbt.egg-info/PKG-INFO` & `prefect_dbt-0.4.3/prefect_dbt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-dbt
-Version: 0.4.2
+Version: 0.4.3
 Summary: Prefect integrations for working with dbt
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dbt
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
 Requires-Dist: prefect>=2.16.6
 Requires-Dist: dbt_core>=1.1.1
 Requires-Dist: prefect_shell>=0.1.4
 Requires-Dist: sgqlc>=16.0.0
 Provides-Extra: snowflake
 Requires-Dist: prefect-snowflake>=0.2.4; extra == "snowflake"
 Requires-Dist: dbt-snowflake; extra == "snowflake"
```

### Comparing `prefect_dbt-0.4.2/prefect_dbt.egg-info/SOURCES.txt` & `prefect_dbt-0.4.3/prefect_dbt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 prefect_dbt/__init__.py
 prefect_dbt/_version.py
 prefect_dbt.egg-info/PKG-INFO
 prefect_dbt.egg-info/SOURCES.txt
 prefect_dbt.egg-info/dependency_links.txt
```

### Comparing `prefect_dbt-0.4.2/prefect_dbt.egg-info/requires.txt` & `prefect_dbt-0.4.3/prefect_dbt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/pyproject.toml` & `prefect_dbt-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cli/configs/test_base.py` & `prefect_dbt-0.4.3/tests/cli/configs/test_base.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cli/configs/test_bigquery.py` & `prefect_dbt-0.4.3/tests/cli/configs/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cli/configs/test_postgres.py` & `prefect_dbt-0.4.3/tests/cli/configs/test_postgres.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cli/configs/test_snowflake.py` & `prefect_dbt-0.4.3/tests/cli/configs/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cli/test_commands.py` & `prefect_dbt-0.4.3/tests/cli/test_commands.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cli/test_credentials.py` & `prefect_dbt-0.4.3/tests/cli/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cli/test_tasks.py` & `prefect_dbt-0.4.3/tests/cli/test_tasks.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cloud/test_clients.py` & `prefect_dbt-0.4.3/tests/cloud/test_clients.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cloud/test_cloud_credentials.py` & `prefect_dbt-0.4.3/tests/cloud/test_cloud_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cloud/test_jobs.py` & `prefect_dbt-0.4.3/tests/cloud/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cloud/test_runs.py` & `prefect_dbt-0.4.3/tests/cloud/test_runs.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/cloud/test_utils.py` & `prefect_dbt-0.4.3/tests/cloud/test_utils.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/conftest.py` & `prefect_dbt-0.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.2/tests/test_block_standards.py` & `prefect_dbt-0.4.3/tests/test_block_standards.py`

 * *Files identical despite different names*

