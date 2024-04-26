# Comparing `tmp/tulona-0.5.4.tar.gz` & `tmp/tulona-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.5.4.tar", last modified: Sun Apr 14 10:09:40 2024, max compression
+gzip compressed data, was "tulona-0.6.3.tar", last modified: Fri Apr 26 15:59:52 2024, max compression
```

## Comparing `tulona-0.5.4.tar` & `tulona-0.6.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:40.310610 tulona-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-14 10:09:29.000000 tulona-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-14 10:09:40.310610 tulona-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-04-14 10:09:29.000000 tulona-0.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:40.302610 tulona-0.5.4/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:40.302610 tulona-0.5.4/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:40.306609 tulona-0.5.4/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:40.306609 tulona-0.5.4/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:40.306609 tulona-0.5.4/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:40.306609 tulona-0.5.4/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:40.306609 tulona-0.5.4/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/task/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:40.310610 tulona-0.5.4/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-14 10:09:29.000000 tulona-0.5.4/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:09:40.310610 tulona-0.5.4/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-14 10:09:40.000000 tulona-0.5.4/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-14 10:09:40.000000 tulona-0.5.4/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 10:09:40.000000 tulona-0.5.4/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-14 10:09:40.000000 tulona-0.5.4/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-14 10:09:40.000000 tulona-0.5.4/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 10:09:40.000000 tulona-0.5.4/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-14 10:09:29.000000 tulona-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 10:09:40.310610 tulona-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.600799 tulona-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:59:48.000000 tulona-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-26 15:59:52.600799 tulona-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-04-26 15:59:48.000000 tulona-0.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.592799 tulona-0.6.3/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.596799 tulona-0.6.3/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.596799 tulona-0.6.3/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.596799 tulona-0.6.3/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.596799 tulona-0.6.3/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.596799 tulona-0.6.3/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.600799 tulona-0.6.3/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22856 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16443 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.600799 tulona-0.6.3/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-26 15:59:48.000000 tulona-0.6.3/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:59:52.600799 tulona-0.6.3/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 15:59:52.000000 tulona-0.6.3/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-26 15:59:48.000000 tulona-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:59:52.600799 tulona-0.6.3/setup.cfg
```

### Comparing `tulona-0.5.4/LICENSE` & `tulona-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/PKG-INFO` & `tulona-0.6.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.5.4
+Version: 0.6.3
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -20,15 +20,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click~=8.1
 Requires-Dist: ruamel.yaml~=0.18
 Requires-Dist: psycopg2-binary~=2.9
 Requires-Dist: pymysql~=1.1
 Requires-Dist: cryptography~=42.0
-Requires-Dist: snowflake-sqlalchemy==1.5
+Requires-Dist: snowflake-sqlalchemy~=1.5
 Requires-Dist: pyodbc~=5.1
 Requires-Dist: pandas~=1.5
 Requires-Dist: openpyxl~=3.1
 Requires-Dist: Jinja2~=3.1
 Requires-Dist: pydantic~=2.7
 
 Tulona
@@ -141,25 +141,49 @@
       table: people_composite_key
       primary_key:
         - ID_1
         - ID_2
       compare_column:
         - ID_1
         - ID_2
+    postgresdb_postgres:
+      connection_profile: pgdb
+      database: postgresdb
+    none_mysql:
+      connection_profile: mydb
+    postgresdb_postgres_schema:
+      connection_profile: pgdb
+      database: postgresdb
+      schema: corporate_copy
+    none_mysql_schema:
+      connection_profile: mydb
+      schema: corporate
+    employee_postgres_query:
+      connection_profile: pgdb
+      query: select * from postgresdb.corporate.employee
+      primary_key: Employee_ID
+      compare_column: Employee_ID
+    employee_mysql_query:
+      connection_profile: mydb
+      query: select * from corporate.employee
+      primary_key: Employee_ID
+      compare_column: Employee_ID
 
   # List of lists
   # The inner lists have datasources that need to be used for tasks like comparison
   # For example employee_postgres vs employee_mysql. So a [employee_postgres, employee_mysql]
   # Outer list is a list of those combinations.
   # So like: [[employee_postgres, employee_mysql], [datasource3, datasource4]]
   source_map:
     - - employee_postgres
       - employee_mysql
     - - person_postgres
       - person_mysql
+    - - employee_postgres_query
+      - employee_mysql_query
 
 
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 All commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
@@ -185,23 +209,27 @@
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
 
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
 
     ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
-* **compare-data**: To compare sample data from two sources/tables. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
+* **compare-row**: To compare sample data from two sources/tables/queries. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
 
   * Command without `--sample-count` parameter:
 
-    ``tulona compare-data --datasources employee_postgres,employee_mysql``
+    ``tulona compare-row --datasources employee_postgres,employee_mysql``
 
   * Command with `--sample-count` parameter:
 
-    ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
+    ``tulona compare-row --sample-count 50 --datasources employee_postgres,employee_mysql``
+
+  * Compare queries instead of tables, useful when you want to compare resutls of two queries:
+
+    ``tulona compare-row --datasources employee_postgres_query,employee_mysql_query``
 
 * **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
 
   * Column[s] to compare is[are] specified in `tulona-project.yml` file as part of datasource configs, with `compare_column` property. Sample command:
 
     ``tulona compare-column --datasources employee_postgres,employee_mysql``
 
@@ -209,14 +237,24 @@
 
     ``tulona compare-column --composite --datasources employee_postgres,employee_mysql``
 
 * **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
   ``tulona compare --datasources employee_postgres,employee_mysql``
 
+* **scan**: To scan and compare databases or schemas in terms of metadata and tables present if you want to compare all tables and don't want to set up datasource config for all of them. Sample commands:
+
+  * Scan without comparing:
+
+    ``tulona scan --datasources postgresdb_postgres_schema,none_mysql_schema``
+
+  * Scan and compare:
+
+    ``tulona scan --compare --datasources postgresdb_postgres_schema,none_mysql_schema``
+
 
 From `tulona v0.4.0` a new project config property has been introduced: `source_map`. If this config is set, in the project config file (tulona-project.yml), then `--datasources` parameter can be skipped with commands.
 For example this command:
 
 ``tulona compare --datasources employee_postgres,employee_mysql``
 
 will become this:
```

### Comparing `tulona-0.5.4/README.rst` & `tulona-0.6.3/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -108,25 +108,49 @@
       table: people_composite_key
       primary_key:
         - ID_1
         - ID_2
       compare_column:
         - ID_1
         - ID_2
+    postgresdb_postgres:
+      connection_profile: pgdb
+      database: postgresdb
+    none_mysql:
+      connection_profile: mydb
+    postgresdb_postgres_schema:
+      connection_profile: pgdb
+      database: postgresdb
+      schema: corporate_copy
+    none_mysql_schema:
+      connection_profile: mydb
+      schema: corporate
+    employee_postgres_query:
+      connection_profile: pgdb
+      query: select * from postgresdb.corporate.employee
+      primary_key: Employee_ID
+      compare_column: Employee_ID
+    employee_mysql_query:
+      connection_profile: mydb
+      query: select * from corporate.employee
+      primary_key: Employee_ID
+      compare_column: Employee_ID
 
   # List of lists
   # The inner lists have datasources that need to be used for tasks like comparison
   # For example employee_postgres vs employee_mysql. So a [employee_postgres, employee_mysql]
   # Outer list is a list of those combinations.
   # So like: [[employee_postgres, employee_mysql], [datasource3, datasource4]]
   source_map:
     - - employee_postgres
       - employee_mysql
     - - person_postgres
       - person_mysql
+    - - employee_postgres_query
+      - employee_mysql_query
 
 
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 All commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
@@ -152,23 +176,27 @@
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
 
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
 
     ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
-* **compare-data**: To compare sample data from two sources/tables. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
+* **compare-row**: To compare sample data from two sources/tables/queries. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
 
   * Command without `--sample-count` parameter:
 
-    ``tulona compare-data --datasources employee_postgres,employee_mysql``
+    ``tulona compare-row --datasources employee_postgres,employee_mysql``
 
   * Command with `--sample-count` parameter:
 
-    ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
+    ``tulona compare-row --sample-count 50 --datasources employee_postgres,employee_mysql``
+
+  * Compare queries instead of tables, useful when you want to compare resutls of two queries:
+
+    ``tulona compare-row --datasources employee_postgres_query,employee_mysql_query``
 
 * **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
 
   * Column[s] to compare is[are] specified in `tulona-project.yml` file as part of datasource configs, with `compare_column` property. Sample command:
 
     ``tulona compare-column --datasources employee_postgres,employee_mysql``
 
@@ -176,14 +204,24 @@
 
     ``tulona compare-column --composite --datasources employee_postgres,employee_mysql``
 
 * **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
   ``tulona compare --datasources employee_postgres,employee_mysql``
 
+* **scan**: To scan and compare databases or schemas in terms of metadata and tables present if you want to compare all tables and don't want to set up datasource config for all of them. Sample commands:
+
+  * Scan without comparing:
+
+    ``tulona scan --datasources postgresdb_postgres_schema,none_mysql_schema``
+
+  * Scan and compare:
+
+    ``tulona scan --compare --datasources postgresdb_postgres_schema,none_mysql_schema``
+
 
 From `tulona v0.4.0` a new project config property has been introduced: `source_map`. If this config is set, in the project config file (tulona-project.yml), then `--datasources` parameter can be skipped with commands.
 For example this command:
 
 ``tulona compare --datasources employee_postgres,employee_mysql``
 
 will become this:
```

### Comparing `tulona-0.5.4/core/tulona/adapter/connection.py` & `tulona-0.6.3/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/core/tulona/adapter/mssql.py` & `tulona-0.6.3/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/core/tulona/adapter/mysql.py` & `tulona-0.6.3/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/core/tulona/adapter/postgres.py` & `tulona-0.6.3/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/core/tulona/adapter/snowflake.py` & `tulona-0.6.3/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/core/tulona/cli/base.py` & `tulona-0.6.3/core/tulona/cli/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import logging
+from pathlib import Path
 
 import click
 
 from tulona.cli import params as p
 from tulona.config.profile import Profile
 from tulona.config.project import Project
 from tulona.config.runtime import RunConfig
 from tulona.exceptions import TulonaMissingArgumentError
-from tulona.task.compare import CompareColumnTask, CompareDataTask, CompareTask
-
-# from tulona.task.scan import ScanTask
+from tulona.task.compare import CompareColumnTask, CompareRowTask, CompareTask
 from tulona.task.ping import PingTask
 from tulona.task.profile import ProfileTask
-from tulona.util.filesystem import get_outfile_fqn
+from tulona.task.scan import ScanTask
+from tulona.util.filesystem import get_final_outdir
 
 log = logging.getLogger(__name__)
 logging.basicConfig(
     level=logging.INFO,
     format="[%(asctime)s] {%(filename)s:%(lineno)d} %(levelname)s - %(message)s",
 )
 
-# TODO: Make use of command line arguments like exec_engine, outdir etc.
-# to override project config values.
-
 
 # command: tulona
 @click.group(
     context_settings={"help_option_names": ["-h", "--help"]},
     no_args_is_help=True,
     epilog="Execute: tulona <command> -h/--help for more help with specific commands",
 )
@@ -64,14 +61,84 @@
         profile=ctx.obj["profile"],
         project=ctx.obj["project"],
         datasources=datasource_list,
     )
     task.execute()
 
 
+# command: tulona scan
+@cli.command("scan")
+@click.pass_context
+# @p.exec_engine
+@p.outdir
+@p.verbose
+@p.datasources
+@p.compare
+@p.sample_count
+@p.composite
+def scan(ctx, **kwargs):
+    """Scan data sources to collect metadata"""
+
+    if kwargs["verbose"]:
+        logging.getLogger("tulona").setLevel(logging.DEBUG)
+
+    prof = Profile()
+    proj = Project()
+
+    ctx.obj = ctx.obj or {}
+    ctx.obj["project"] = proj.load_project_config()
+    ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
+    ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
+
+    # Override config outdir if provided in command line
+    if kwargs["outdir"]:
+        ctx.obj["project"]["outdir"] = kwargs["outdir"]
+
+    source_maps = []
+    if kwargs["compare"]:
+        if kwargs["datasources"]:
+            source_maps.append(kwargs["datasources"].split(","))
+        elif "source_map" in ctx.obj["project"]:
+            source_maps = ctx.obj["project"]["source_map"]
+        else:
+            raise TulonaMissingArgumentError(
+                "Either --datasources command line argument or source_map (tulona-project.yml)"
+                " must be provided for comparison with command: scan"
+                " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file#project-config-file"
+                " for more information on source_map"
+            )
+    else:
+        if kwargs["datasources"]:
+            source_maps.append(kwargs["datasources"].split(","))
+        else:
+            raise TulonaMissingArgumentError(
+                "--datasources command line argument must be provided with command: scan"
+                " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file"
+                " for more information"
+            )
+
+    for datasource_list in source_maps:
+        final_outdir = get_final_outdir(
+            basedir=ctx.obj["project"]["outdir"],
+            ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
+        )
+
+        task = ScanTask(
+            profile=ctx.obj["profile"],
+            project=ctx.obj["project"],
+            runtime=ctx.obj["runtime"],
+            datasources=datasource_list,
+            final_outdir=final_outdir,
+            compare=kwargs["compare"],
+            sample_count=kwargs["sample_count"],
+            composite=kwargs["composite"],
+        )
+        task.execute()
+
+
 # command: tulona profile
 @cli.command("profile")
 @click.pass_context
 # @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
@@ -91,54 +158,64 @@
     ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
 
     # Override config outdir if provided in command line
     if kwargs["outdir"]:
         ctx.obj["project"]["outdir"] = kwargs["outdir"]
 
     source_maps = []
-    if kwargs["datasources"]:
-        source_maps.append(kwargs["datasources"].split(","))
-    elif "source_map" in ctx.obj["project"]:
-        source_maps = ctx.obj["project"]["source_map"]
+    if kwargs["compare"]:
+        if kwargs["datasources"]:
+            source_maps.append(kwargs["datasources"].split(","))
+        elif "source_map" in ctx.obj["project"]:
+            source_maps = ctx.obj["project"]["source_map"]
+        else:
+            raise TulonaMissingArgumentError(
+                "Either --datasources command line argument or source_map (tulona-project.yml)"
+                " must be provided for comparison with command: profile"
+                " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file#project-config-file"
+                " for more information on source_map"
+            )
     else:
-        raise TulonaMissingArgumentError(
-            "Either --datasources command line argument or source_map (tulona-project.yml)"
-            " must be provided with command: profile"
-            " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file#project-config-file"
-            " for more information on source_map"
-        )
+        if kwargs["datasources"]:
+            source_maps.append(kwargs["datasources"].split(","))
+        else:
+            raise TulonaMissingArgumentError(
+                "--datasources command line argument must be provided with command: profile"
+                " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file"
+                " for more information"
+            )
 
     for datasource_list in source_maps:
-        outfile_fqn = get_outfile_fqn(
-            outdir=ctx.obj["project"]["outdir"],
+        final_outdir = get_final_outdir(
+            basedir=ctx.obj["project"]["outdir"],
             ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
-            infix="profiling",
         )
+        outfile_fqn = Path(final_outdir, "profile_metadata.xlsx")
 
         task = ProfileTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             runtime=ctx.obj["runtime"],
             datasources=datasource_list,
             outfile_fqn=outfile_fqn,
             compare=kwargs["compare"],
         )
         task.execute()
 
 
-# command: tulona compare-data
-@cli.command("compare-data")
+# command: tulona compare-row
+@cli.command("compare-row")
 @click.pass_context
 # @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
 @p.sample_count
-def compare_data(ctx, **kwargs):
-    """Compares two data entities"""
+def compare_row(ctx, **kwargs):
+    """Compares rows from two data entities"""
 
     if kwargs["verbose"]:
         logging.getLogger("tulona").setLevel(logging.DEBUG)
 
     prof = Profile()
     proj = Project()
 
@@ -155,27 +232,27 @@
     if kwargs["datasources"]:
         source_maps.append(kwargs["datasources"].split(","))
     elif "source_map" in ctx.obj["project"]:
         source_maps = ctx.obj["project"]["source_map"]
     else:
         raise TulonaMissingArgumentError(
             "Either --datasources command line argument or source_map (tulona-project.yml)"
-            " must be provided with command: compare-data"
+            " must be provided with command: compare-row"
             " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file#project-config-file"
             " for more information on source_map"
         )
 
     for datasource_list in source_maps:
-        outfile_fqn = get_outfile_fqn(
-            outdir=ctx.obj["project"]["outdir"],
+        final_outdir = get_final_outdir(
+            basedir=ctx.obj["project"]["outdir"],
             ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
-            infix="data_comparison",
         )
+        outfile_fqn = Path(final_outdir, "row_comparison.xlsx")
 
-        task = CompareDataTask(
+        task = CompareRowTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             runtime=ctx.obj["runtime"],
             datasources=datasource_list,
             outfile_fqn=outfile_fqn,
             sample_count=kwargs["sample_count"],
         )
@@ -223,19 +300,19 @@
             "Either --datasources command line argument or source_map (tulona-project.yml)"
             " must be provided with command: compare-column"
             " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file#project-config-file"
             " for more information on source_map"
         )
 
     for datasource_list in source_maps:
-        outfile_fqn = get_outfile_fqn(
-            outdir=ctx.obj["project"]["outdir"],
+        final_outdir = get_final_outdir(
+            basedir=ctx.obj["project"]["outdir"],
             ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
-            infix="column_comparison",
         )
+        outfile_fqn = Path(final_outdir, "column_comparison.xlsx")
 
         task = CompareColumnTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             runtime=ctx.obj["runtime"],
             datasources=datasource_list,
             outfile_fqn=outfile_fqn,
@@ -283,19 +360,19 @@
             "Either --datasources command line argument or source_map (tulona-project.yml)"
             " must be provided with command: compare"
             " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file#project-config-file"
             " for more information on source_map"
         )
 
     for datasource_list in source_maps:
-        outfile_fqn = get_outfile_fqn(
-            outdir=ctx.obj["project"]["outdir"],
+        final_outdir = get_final_outdir(
+            basedir=ctx.obj["project"]["outdir"],
             ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
-            infix="comparison",
         )
+        outfile_fqn = Path(final_outdir, "comparison.xlsx")
 
         task = CompareTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             runtime=ctx.obj["runtime"],
             datasources=datasource_list,
             outfile_fqn=outfile_fqn,
```

### Comparing `tulona-0.5.4/core/tulona/cli/params.py` & `tulona-0.6.3/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/core/tulona/config/profile.py` & `tulona-0.6.3/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/core/tulona/config/project.py` & `tulona-0.6.3/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/core/tulona/exceptions.py` & `tulona-0.6.3/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/core/tulona/task/base.py` & `tulona-0.6.3/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/core/tulona/task/compare.py` & `tulona-0.6.3/core/tulona/task/compare.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import logging
 import os
+import re
 import time
+import traceback
+from copy import deepcopy
 from dataclasses import _MISSING_TYPE, dataclass, fields
 from pathlib import Path
 from typing import Dict, List, Union
 
 import pandas as pd
 
 from tulona.config.runtime import RunConfig
 from tulona.exceptions import TulonaMissingPrimaryKeyError, TulonaMissingPropertyError
 from tulona.task.base import BaseTask
 from tulona.task.helper import perform_comparison
 from tulona.task.profile import ProfileTask
+from tulona.util.database import get_table_primary_keys
 from tulona.util.dataframe import apply_column_exclusion
 from tulona.util.excel import highlight_mismatch_cells
 from tulona.util.filesystem import create_dir_if_not_exist
 from tulona.util.profiles import extract_profile_name, get_connection_profile
 from tulona.util.sql import (
     build_filter_query_expression,
     get_column_query,
@@ -29,15 +33,15 @@
 DEFAULT_VALUES = {
     "sample_count": 20,
     "compare_column_composite": False,
 }
 
 
 @dataclass
-class CompareDataTask(BaseTask):
+class CompareRowTask(BaseTask):
     profile: Dict
     project: Dict
     runtime: RunConfig
     datasources: List[str]
     outfile_fqn: Union[Path, str]
     sample_count: int = DEFAULT_VALUES["sample_count"]
 
@@ -47,149 +51,227 @@
             # If there is a default and the value of the field is none we can assign a value
             if (
                 not isinstance(field.default, _MISSING_TYPE)
                 and getattr(self, field.name) is None
             ):
                 setattr(self, field.name, field.default)
 
-    def execute(self):
-        log.info("------------------------ Starting task: compare-data")
-        start_time = time.time()
-
-        if len(self.datasources) != 2:
-            raise ValueError("Data comparison needs two data sources.")
-
-        log.info(f"Comparing {self.datasources}")
-
+    def extract_confs(self):
         # TODO: Add support for different names of primary keys in different tables
         # Check if primary key[s] is[are] specified for row comparison
-        primary_keys = set()
-        ds_names = []
-        ds_name_compressed_list = []
-        ds_configs = []
-        dbtypes = []
-        table_fqns = []
-        connection_managers = []
-        exclude_columns_lol = []
+        econf_dict = {}
+        primary_keys = []
+        econf_dict["ds_names"] = []
+        econf_dict["ds_name_compressed_list"] = []
+        econf_dict["ds_configs"] = []
+        econf_dict["dbtypes"] = []
+        econf_dict["table_fqns"] = []
+        econf_dict["queries"] = []
+        econf_dict["connection_managers"] = []
+        econf_dict["exclude_columns_lol"] = []
         for ds_name in self.datasources:
             log.debug(f"Extracting configs for: {ds_name}")
             # Extract data source name from datasource:column combination
             ds_name = ds_name.split(":")[0]
-            ds_names.append(ds_name)
-            ds_name_compressed_list.append(ds_name.replace("_", ""))
+            econf_dict["ds_names"].append(ds_name)
+            econf_dict["ds_name_compressed_list"].append(ds_name.replace("_", ""))
 
             ds_config = self.project["datasources"][ds_name]
-            ds_configs.append(ds_config)
+            econf_dict["ds_configs"].append(ds_config)
             dbtype = self.profile["profiles"][
                 extract_profile_name(self.project, ds_name)
             ]["type"]
-            dbtypes.append(dbtype)
+            econf_dict["dbtypes"].append(dbtype)
 
-            # MySQL doesn't have logical database
-            if "database" in ds_config and dbtype.lower() != "mysql":
-                database = ds_config["database"]
+            if "query" in ds_config and "table" in ds_config:
+                raise AttributeError(
+                    "Both 'query' and 'table' cannot be specified in datasource config"
+                )
+
+            if "query" in ds_config:
+                econf_dict["queries"].append(ds_config["query"])
+                if "exclude_columns" in ds_config:
+                    log.warning(
+                        "Attribute 'exclude_columns' doesn't have any effect"
+                        " with attribute 'query'"
+                    )
+                econf_dict["exclude_columns_lol"].append([])
+                if "schema" in ds_config:
+                    log.warning(
+                        "Attribute 'schema' doesn't have any effect"
+                        " with attribute 'query'"
+                    )
+                if "table_fqns" in econf_dict:
+                    if len(econf_dict["table_fqns"]) > 0:
+                        raise AttributeError(
+                            "Same attribute from 'query' and 'table' has to be"
+                            " specified in all candidate datasource confgis"
+                        )
+                    else:
+                        econf_dict.pop("table_fqns")
+
+            elif "table" in ds_config:
+                # MySQL doesn't have logical database
+                if "database" in ds_config and dbtype.lower() != "mysql":
+                    database = ds_config["database"]
+                else:
+                    database = None
+                schema = ds_config["schema"]
+                table = ds_config["table"]
+
+                table_fqn = get_table_fqn(
+                    database,
+                    schema,
+                    table,
+                )
+
+                exclude_columns = (
+                    ds_config["exclude_columns"] if "exclude_columns" in ds_config else []
+                )
+                if isinstance(exclude_columns, str):
+                    exclude_columns = [exclude_columns]
+                econf_dict["exclude_columns_lol"].append(exclude_columns)
+
+                econf_dict["table_fqns"].append(table_fqn)
+                if "queries" in econf_dict:
+                    if len(econf_dict["queries"]) > 0:
+                        raise AttributeError(
+                            "Same attribute from 'query' and 'table' has to be"
+                            " specified in all candidate datasource confgis"
+                        )
+                    else:
+                        econf_dict.pop("queries")
             else:
-                database = None
-            schema = ds_config["schema"]
-            table = ds_config["table"]
-
-            table_fqn = get_table_fqn(
-                database,
-                schema,
-                table,
-            )
-            table_fqns.append(table_fqn)
+                raise TulonaMissingPropertyError(
+                    "Either 'table' for 'query' must be specified"
+                    "in datasource config for row comparison."
+                )
 
             log.debug(f"Acquiring connection to the database of: {ds_name}")
-            connection_profile = get_connection_profile(
-                self.profile, self.project, ds_name
-            )
-            connection_managers.append(
-                self.get_connection_manager(conn_profile=connection_profile)
-            )
-
-            exclude_columns = (
-                ds_config["exclude_columns"] if "exclude_columns" in ds_config else []
-            )
-            if isinstance(exclude_columns, str):
-                exclude_columns = [exclude_columns]
-            exclude_columns_lol.append(exclude_columns)
+            connection_profile = get_connection_profile(self.profile, ds_config)
+            conman = self.get_connection_manager(conn_profile=connection_profile)
+            econf_dict["connection_managers"].append(conman)
 
             if "primary_key" in ds_config:
-                primary_keys.add(
+                ds_pk = (
                     (ds_config["primary_key"],)
                     if isinstance(ds_config["primary_key"], str)
                     else tuple(sorted(ds_config["primary_key"]))
                 )
+                log.debug(f"Provided primary key for datasource {ds_name}: {ds_pk}")
+            else:
+                log.debug(
+                    f"Primary key not provided for datasource {ds_name}"
+                    " Tulona will try to extract it from table metadata"
+                )
+                ds_pk = tuple(get_table_primary_keys(conman.engine, schema, table))
+                log.debug(f"Extracted primary key for datasource {ds_name}: {ds_pk}")
+
+            if len(ds_pk) > 0:
+                primary_keys.append(ds_pk)
+
+        pk_ci_set = {tuple(map(lambda x: x.lower(), k)) for k in primary_keys}
 
         if len(primary_keys) == 0:
             raise TulonaMissingPrimaryKeyError(
-                "Primary key must be provided for comparison"
+                "Primary key[s] is[are] not available. Abort!"
             )
+        elif len(primary_keys) > 0:
+            if len(primary_keys) != len(primary_keys):
+                raise TulonaMissingPrimaryKeyError(
+                    "If primary key is provided, it must be provided for all datasources"
+                )
 
-        if len(primary_keys) > 1:
-            raise ValueError(
-                "Primary key must be same in all candidate tables for comparison"
+            if len(pk_ci_set) > 1:
+                raise ValueError(
+                    "Primary key must be same in all candidate tables for comparison"
+                )
+            econf_dict["primary_key"] = primary_keys[0]
+            log.debug(f"Final primary key: {econf_dict['primary_key']}")
+        else:
+            raise TulonaMissingPrimaryKeyError(
+                f"Primary key for {table_fqn}[{ds_name}] could not be found."
+                " Row comparison without primary key has not been implemented yet."
+                " Abort!"
             )
-        primary_key = primary_keys.pop()
+
+        return econf_dict
+
+    def execute(self):
+        log.info("------------------------ Starting task: compare-row")
+        start_time = time.time()
+
+        if len(self.datasources) != 2:
+            raise ValueError("Data comparison needs two data sources.")
 
         # Config extraction
-        dbtype1, dbtype2 = dbtypes
-        table_fqn1, table_fqn2 = table_fqns
-        conman1, conman2 = connection_managers
-        exclude_columns1, exclude_columns2 = exclude_columns_lol
+        econf_dict = self.extract_confs()
+        dbtype1, dbtype2 = econf_dict["dbtypes"]
+        if "table_fqns" in econf_dict:
+            table_fqn1, table_fqn2 = econf_dict["table_fqns"]
+        else:
+            query1, query2 = econf_dict["queries"]
+        exclude_columns1, exclude_columns2 = econf_dict["exclude_columns_lol"]
+        conman1, conman2 = econf_dict["connection_managers"]
 
         # TODO: push column exclusion down to the database/query
-        primary_key = tuple([k.lower() for k in primary_key])
+        # TODO: We probably don't need to create pk tuple out of pk
+        # lists as that is already happening while extracting pks
+        primary_key = tuple([k.lower() for k in econf_dict["primary_key"]])
         query_expr = None
 
+        log.info(f"Comparing {self.datasources}")
+        num_try = 1 if "queries" in econf_dict else 5
         i = 0
-        while i < 5:
-            log.debug(f"Extraction iteration: {i + 1}/5")
+        while i < num_try:
+            log.debug(f"Extraction iteration: {i + 1}/{num_try}")
 
-            query1 = get_table_data_query(
-                dbtype1, table_fqn1, self.sample_count, query_expr
-            )
+            if "table_fqns" in econf_dict:
+                query1 = get_table_data_query(
+                    dbtype1, table_fqn1, self.sample_count, query_expr
+                )
             if self.sample_count < 51:
-                log.debug(f"Executing query: {query1}")
+                sanitized_query1 = re.sub(r"\(.*\)", "(...)", query1)
+                log.debug(f"Executing query: {sanitized_query1}")
             df1 = get_query_output_as_df(connection_manager=conman1, query_text=query1)
             if df1.shape[0] == 0:
                 raise ValueError(f"Table {table_fqn1} doesn't have any data")
 
             df1 = df1.rename(columns={c: c.lower() for c in df1.columns})
             for k in primary_key:
                 if k not in df1.columns.tolist():
                     raise ValueError(f"Primary key {k} not present in {table_fqn1}")
 
             # Exclude columns
-            log.debug(f"Excluding columns from {table_fqn1}")
-            if len(exclude_columns1):
+            if len(exclude_columns1) > 0:
+                log.debug(f"Excluding columns from {table_fqn1}: {exclude_columns1}")
                 df1 = apply_column_exclusion(
                     df1, primary_key, exclude_columns1, table_fqn1
                 )
-
-            query2 = get_table_data_query(
-                dbtype2,
-                table_fqn2,
-                self.sample_count,
-                query_expr=build_filter_query_expression(df1, primary_key),
-            )
+            if "table_fqns" in econf_dict:
+                query2 = get_table_data_query(
+                    dbtype2,
+                    table_fqn2,
+                    self.sample_count,
+                    query_expr=build_filter_query_expression(df1, primary_key),
+                )
             if self.sample_count < 51:
-                log.debug(f"Executing query: {query2}")
+                sanitized_query2 = re.sub(r"\(.*\)", "(...)", query2)
+                log.debug(f"Executing query: {sanitized_query2}")
 
             df2 = get_query_output_as_df(connection_manager=conman2, query_text=query2)
             df2 = df2.rename(columns={c: c.lower() for c in df2.columns})
 
             for k in primary_key:
                 if k not in df2.columns.tolist():
                     raise ValueError(f"Primary key {k} not present in {table_fqn2}")
 
             # Exclude columns
-            log.debug(f"Excluding columns from {table_fqn2}")
-            if len(exclude_columns2):
+            if len(exclude_columns2) > 0:
+                log.debug(f"Excluding columns from {table_fqn2}: {exclude_columns2}")
                 df2 = apply_column_exclusion(
                     df2, primary_key, exclude_columns2, table_fqn2
                 )
 
             if df2.shape[0] > 0:
                 for k in primary_key:
                     df1 = df1[df1[k].isin(df2[k].tolist())]
@@ -200,49 +282,51 @@
                     df1, primary_key, positive=False
                 )
 
             i += 1
 
         if df2.shape[0] == 0:
             raise ValueError(
-                f"Could not find common data between {table_fqn1} and {table_fqn2}"
+                f"Could not find common rows between {table_fqn1} and {table_fqn2}"
             )
 
-        log.debug("Preparing row comparison")
+        log.debug(
+            f"Preparing row comparison for: {econf_dict['ds_name_compressed_list']}"
+        )
         df_row_comp = perform_comparison(
-            ds_compressed_names=ds_name_compressed_list,
+            ds_compressed_names=econf_dict["ds_name_compressed_list"],
             dataframes=row_data_list,
             on=primary_key,
         )
         log.debug(f"Prepared comparison for {df_row_comp.shape[0]} rows")
 
         log.debug(f"Writing comparison result into: {self.outfile_fqn}")
+        # TODO: Remove it as it is already happening in perform_comparison
         # Moving key columns to the beginning
         new_columns = list(primary_key) + [
             col for col in df_row_comp if col not in primary_key
         ]
         df_row_comp = df_row_comp[new_columns]
 
-        _ = create_dir_if_not_exist(self.project["outdir"])
+        _ = create_dir_if_not_exist(self.outfile_fqn.parent)
         with pd.ExcelWriter(
             self.outfile_fqn, mode="a" if os.path.exists(self.outfile_fqn) else "w"
         ) as writer:
             df_row_comp.to_excel(writer, sheet_name="Row Comparison", index=False)
 
         log.debug("Highlighting mismtach cells")
         highlight_mismatch_cells(
             excel_file=self.outfile_fqn,
             sheet="Row Comparison",
             num_ds=len(self.datasources),
             skip_columns=primary_key,
         )
 
-        end_time = time.time()
-        log.info("------------------------ Finished task: compare-data")
-        log.info(f"Total time taken: {(end_time - start_time):.2f} seconds")
+        exec_time = time.time() - start_time
+        log.info(f"Finished task: compare-row in {exec_time:.2f} seconds")
 
 
 @dataclass
 class CompareColumnTask(BaseTask):
     profile: Dict
     project: Dict
     runtime: RunConfig
@@ -265,71 +349,88 @@
             ds_compressed_names.append(ds_name.replace("_", ""))
             ds_config = self.project["datasources"][ds_name]
 
             if "compare_column" in ds_config:
                 columns = ds_config["compare_column"]
                 columns = [columns] if isinstance(columns, str) else columns
                 compare_columns.append(columns)
+                log.debug(f"Column[s] to compare: {columns}")
             else:
                 raise TulonaMissingPropertyError(
                     "Property 'compare_column' must be specified"
-                    "in tulona-project.yml for column comparison"
+                    " in project config for column comparison"
                 )
 
             dbtype = self.profile["profiles"][
                 extract_profile_name(self.project, ds_name)
             ]["type"]
             log.debug(f"Database type: {dbtype}")
 
-            # MySQL doesn't have logical database
-            if "database" in ds_config and dbtype.lower() != "mysql":
-                database = ds_config["database"]
-            else:
-                database = None
-            schema = ds_config["schema"]
-            table = ds_config["table"]
-            table_fqn = get_table_fqn(database, schema, table)
-            log.debug(f"Table FQN: {table_fqn}")
-
-            log.debug(f"Extracting data for column {columns}")
             log.debug(f"Acquiring connection to the database of: {ds_name}")
-            connection_profile = get_connection_profile(
-                self.profile, self.project, ds_name
-            )
+            connection_profile = get_connection_profile(self.profile, ds_config)
             conman = self.get_connection_manager(conn_profile=connection_profile)
 
-            query = get_column_query(table_fqn, columns)
-            try:
-                log.debug(f"Trying unquoted column names: {columns}")
-                log.debug(f"Executing query: {query}")
-                df = get_query_output_as_df(connection_manager=conman, query_text=query)
-            except Exception as exp:
-                log.warning(f"Failed with error: {exp}")
-                log.debug(f'Trying quoted column names: "{columns}"')
-                query = get_column_query(table_fqn, columns, quoted=True)
+            if "query" in ds_config and "table" in ds_config:
+                raise AttributeError(
+                    "Both 'query' and 'table' cannot be specified in datasource config"
+                )
+            if "query" in ds_config:
+                query = ds_config["query"]
                 log.debug(f"Executing query: {query}")
                 df = get_query_output_as_df(connection_manager=conman, query_text=query)
+            elif "table" in ds_config:
+                # MySQL doesn't have logical database
+                if "database" in ds_config and dbtype.lower() != "mysql":
+                    database = ds_config["database"]
+                else:
+                    database = None
+                if "schema" in ds_config:
+                    schema = ds_config["schema"]
+
+                table = ds_config["table"]
+                table_fqn = get_table_fqn(database, schema, table)
+                log.debug(f"Table FQN: {table_fqn}")
+                query = get_column_query(table_fqn, columns)
+                try:
+                    log.debug(f"Trying unquoted column names: {columns}")
+                    log.debug(f"Executing query: {query}")
+                    df = get_query_output_as_df(
+                        connection_manager=conman, query_text=query
+                    )
+                except Exception as exc:
+                    log.warning(f"Failed with error: {exc}")
+                    log.debug(f'Trying quoted column names: "{columns}"')
+                    query = get_column_query(table_fqn, columns, quoted=True)
+                    log.debug(f"Executing query: {query}")
+                    df = get_query_output_as_df(
+                        connection_manager=conman, query_text=query
+                    )
+            else:
+                raise TulonaMissingPropertyError(
+                    "Either 'table' for 'query' must be specified"
+                    "in datasource config for row comparison."
+                )
 
             if df.shape[0] == 0:
-                raise ValueError(f"Table {table_fqn} doesn't have any data")
+                raise ValueError("Query didn't result into any data")
 
-            log.debug(f"Found {df.shape[0]} records in {table_fqn}")
+            log.debug(f"Extracted {df.shape[0]} records as query result")
 
             df = df.rename(columns={c: c.lower() for c in df.columns})
             column_df_list.append(df)
 
         compare_columns = {
             tuple(map(lambda c: c.lower(), clist)) for clist in compare_columns
         }
         if len(compare_columns) > 1:
             raise ValueError(
                 "Column comparison works only when the column name is same for all data sources"
-                "(not case sensitive)"
-                "and they have to be specified in the same order"
-                "in the config file for all data sources"
+                " (not case sensitive)"
+                " and they have to be specified in the same order"
+                " in the config file for all data sources"
             )
         compare_columns = compare_columns.pop()
         log.debug(f"Final list of columns for comparison: {compare_columns}")
 
         output_dataframes = dict()
         if self.composite:
             log.debug(f"Performing composite comparison for: {compare_columns}")
@@ -371,26 +472,25 @@
                         "right_only": ds_compressed_names[1],
                     }
                 )
                 log.debug(f"Found {df_comp.shape[0]} mismatches all sides combined")
                 output_dataframes[c] = df_comp
 
         log.debug(f"Writing output into: {self.outfile_fqn}")
-        _ = create_dir_if_not_exist(self.project["outdir"])
+        _ = create_dir_if_not_exist(self.outfile_fqn.parent)
         for sheet, df in output_dataframes.items():
             with pd.ExcelWriter(
                 self.outfile_fqn, mode="a" if os.path.exists(self.outfile_fqn) else "w"
             ) as writer:
                 df.to_excel(
                     writer, sheet_name=f"Column Comparison-> {sheet}", index=False
                 )
 
-        end_time = time.time()
-        log.info("------------------------ Finished task: compare-column")
-        log.info(f"Total time taken: {(end_time - start_time):.2f} seconds")
+        exec_time = time.time() - start_time
+        log.info(f"Finished task: compare-column in {exec_time:.2f} seconds")
 
 
 @dataclass
 class CompareTask(BaseTask):
     profile: Dict
     project: Dict
     runtime: RunConfig
@@ -419,41 +519,48 @@
                 profile=self.profile,
                 project=self.project,
                 runtime=self.runtime,
                 datasources=self.datasources,
                 outfile_fqn=self.outfile_fqn,
                 compare=True,
             ).execute()
-        except Exception as exc:
-            log.error(f"Profiling failed with error: {exc}")
+        except Exception:
+            log.error(f"Profiling failed with error: {traceback.format_exc()}")
 
         # Row comparison
+        primary_key = None
+        cdt = CompareRowTask(
+            profile=self.profile,
+            project=self.project,
+            runtime=self.runtime,
+            datasources=self.datasources,
+            outfile_fqn=self.outfile_fqn,
+            sample_count=self.sample_count,
+        )
         try:
-            CompareDataTask(
-                profile=self.profile,
-                project=self.project,
-                runtime=self.runtime,
-                datasources=self.datasources,
-                outfile_fqn=self.outfile_fqn,
-                sample_count=self.sample_count,
-            ).execute()
-        except Exception as exc:
-            log.error(f"Row comparison failed with error: {exc}")
+            primary_key = cdt.extract_confs()["primary_key"]
+            cdt.execute()
+        except Exception:
+            log.error(f"Row comparison failed with error: {traceback.format_exc()}")
 
         # Column comparison
+        project_copy = deepcopy(self.project)
+        for ds in project_copy["datasources"]:
+            if "compare_column" not in ds and primary_key:
+                project_copy["datasources"][ds]["compare_column"] = primary_key
         try:
             CompareColumnTask(
                 profile=self.profile,
-                project=self.project,
+                project=project_copy,
                 runtime=self.runtime,
                 datasources=self.datasources,
                 outfile_fqn=self.outfile_fqn,
                 composite=self.composite,
             ).execute()
-        except Exception as exc:
-            log.error(f"Column comparison failed with error: {exc}")
+        except Exception:
+            log.error(f"Column comparison failed with error: {traceback.format_exc()}")
 
-        end_time = time.time()
-        log.info("------------------------ Finished task: compare")
+        exec_time = time.time() - start_time
         log.info(
-            f"Total time taken [profile, compare-data, compare-column]: {(end_time - start_time):.2f} seconds"
+            "Finished task: compare[profile, compare-row, compare-column]"
+            f" in {exec_time:.2f} seconds"
         )
```

### Comparing `tulona-0.5.4/core/tulona/task/helper.py` & `tulona-0.6.3/core/tulona/task/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,29 +37,28 @@
     try:
         log.debug("Trying query with unquoted column names")
         metric_query = get_metric_query(table_fqn, columns_dtype, metrics)
         log.debug(f"Executing query: {metric_query}")
         df_metric = get_query_output_as_df(
             connection_manager=conman, query_text=metric_query
         )
-    except Exception as exp:
-        log.warning(f"Previous query failed with error: {exp}")
+    except Exception as exc:
+        log.warning(f"Previous query failed with error: {exc}")
         log.debug("Trying query with quoted column names")
         metric_query = get_metric_query(
             table_fqn,
             columns_dtype,
             metrics,
             quoted=True,
         )
         log.debug(f"Executing query: {metric_query}")
         df_metric = get_query_output_as_df(
             connection_manager=conman, query_text=metric_query
         )
 
-    log.debug("Converting metric data into presentable format")
     metric_dict = {m: [] for m in ["column_name"] + metrics}
     for col in df_meta["column_name"]:
         metric_dict["column_name"].append(col)
         for m in metrics:
             try:
                 metric_value = df_metric.iloc[0][f"{col}_{m}"]
             except Exception:
@@ -87,20 +86,21 @@
     primary_key = [k.lower() for k in on]
     common_columns = {c.lower() for c in dataframes[0].columns.tolist()}
 
     dataframes_final = []
     for df in dataframes[1:]:
         colset = {c.lower() for c in df.columns.tolist()}
         common_columns = common_columns.intersection(colset)
+    log.debug(f"Common columns: {common_columns}")
 
     for ds_name, df in zip(ds_compressed_names, dataframes):
         df = df[list(common_columns)]
         df = df.rename(
             columns={
-                c: f"{c}_{ds_name}" if c.lower() not in primary_key else c
+                c: f"{c}-{ds_name}" if c.lower() not in primary_key else c
                 for c in df.columns
             }
         )
         for k in primary_key:
             if pd.api.types.is_string_dtype(df[k]):
                 df[k] = df[k].str.lower()
         dataframes_final.append(df)
@@ -112,10 +112,13 @@
             right=df,
             on=primary_key,
             how=how,
             suffixes=suffixes,
             indicator=indicator,
             validate=validate,
         )
+
     df_merge = df_merge[sorted(df_merge.columns.tolist())]
+    new_columns = primary_key + [col for col in df_merge if col not in primary_key]
+    df_merge = df_merge[new_columns]
 
     return df_merge
```

### Comparing `tulona-0.5.4/core/tulona/task/profile.py` & `tulona-0.6.3/core/tulona/task/profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,27 @@
 from tulona.task.helper import create_profile, perform_comparison
 from tulona.util.excel import highlight_mismatch_cells
 from tulona.util.filesystem import create_dir_if_not_exist
 from tulona.util.profiles import extract_profile_name, get_connection_profile
 
 log = logging.getLogger(__name__)
 
+DEFAULT_VALUES = {
+    "compare_profiles": False,
+}
+
 
 @dataclass
 class ProfileTask(BaseTask):
     profile: Dict
     project: Dict
     runtime: RunConfig
     datasources: List[str]
     outfile_fqn: Union[Path, str]
-    compare: bool = False
+    compare: bool = DEFAULT_VALUES["compare_profiles"]
 
     # Support for default values
     def __post_init__(self):
         for field in fields(self):
             # If there is a default and the value of the field is none we can assign a value
             if (
                 not isinstance(field.default, _MISSING_TYPE)
@@ -47,44 +51,49 @@
             log.debug(f"Extracting configs for: {ds_name}")
             # Extract data source name from datasource:column combination
             ds_name = ds_name.split(":")[0]
             ds_name_compressed = ds_name.replace("_", "")
             ds_name_compressed_list.append(ds_name_compressed)
 
             ds_config = self.project["datasources"][ds_name]
+
+            if "query" in ds_config:
+                raise AttributeError(
+                    "Profiling only works with tables, not with queries"
+                    f" Check your datasource config for: {ds_name}"
+                )
+
             dbtype = self.profile["profiles"][
                 extract_profile_name(self.project, ds_name)
             ]["type"]
 
             # MySQL doesn't have logical database
             if "database" in ds_config and dbtype.lower() != "mysql":
                 database = ds_config["database"]
             else:
                 database = None
             schema = ds_config["schema"]
             table = ds_config["table"]
 
             log.debug(f"Acquiring connection to the database of: {ds_name}")
-            connection_profile = get_connection_profile(
-                self.profile, self.project, ds_name
-            )
+            connection_profile = get_connection_profile(self.profile, ds_config)
             conman = self.get_connection_manager(conn_profile=connection_profile)
 
             log.info(f"Profiling {ds_name}")
             metrics = [
                 "min",
                 "max",
                 "avg",
                 "count",
                 "distinct_count",
             ]
             df = create_profile(database, schema, table, metrics, conman)
             df_collection.append(df)
 
-        _ = create_dir_if_not_exist(self.project["outdir"])
+        _ = create_dir_if_not_exist(self.outfile_fqn.parent)
         if self.compare:
             log.debug("Preparing metadata comparison")
             df_merge = perform_comparison(
                 ds_name_compressed_list, df_collection, "column_name"
             )
             log.debug(f"Calculated comparison for {df_merge.shape[0]} columns")
```

### Comparing `tulona-0.5.4/core/tulona/task/scan.py` & `tulona-0.6.3/core/tulona/task/ping.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import logging
 import time
+import traceback
 from dataclasses import dataclass
 from typing import Dict, List
 
-from tulona.config.runtime import RunConfig
 from tulona.task.base import BaseTask
-
-# from tulona.util.profiles import get_connection_profile
+from tulona.util.profiles import get_connection_profile
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
-class ScanTask(BaseTask):
+class PingTask(BaseTask):
     profile: Dict
     project: Dict
-    runtime: RunConfig
     datasources: List[str]
 
     def execute(self):
 
-        log.info("Starting task: Scan")
+        log.info("Starting task: ping")
         start_time = time.time()
 
-        # # TODO: Change the implementation
-        # for ds in self.datasources:
-        #     log.debug(f"Testing connection to data source: {ds}")
-
-        #     connection_profile = get_connection_profile(self.profile, self.project, ds)
-        #     try:
-        #         conman = self.get_connection_manager(conn_profile=connection_profile)
-        #         with conman.engine.open() as connection:
-        #             results = connection.execute(
-        #                 "select * from information_schema"
-        #             ).fetchone()
-        #     except Exception as exp:
-        #         log.error(f"Connection to data source {ds} failed because of: {exp}")
+        log.debug(f"Data sources to ping: {self.datasources}")
+
+        for ds in self.datasources:
+            connection_profile = get_connection_profile(
+                self.profile, self.project["datasources"][ds]
+            )
+            log.info(
+                f"Testing connection to data source: {ds}[{connection_profile['type']}]"
+            )
+            try:
+                conman = self.get_connection_manager(conn_profile=connection_profile)
+                with conman.engine.connect() as connection:
+                    results = connection.execute(
+                        "select * from information_schema.tables"
+                    ).fetchone()
+                    _ = results[0]
+                    log.info("Connection successful")
+            except Exception:
+                log.error(f"Connection failed with error: {traceback.format_exc()}")
 
         end_time = time.time()
-        log.info("Finished task: Scan")
+        log.info("Finished task: ping")
         log.info(f"Total time taken: {(end_time - start_time):.2f} seconds")
```

### Comparing `tulona-0.5.4/core/tulona/util/database.py` & `tulona-0.6.3/core/tulona/util/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 
 
 def get_tables_from_schema(engine, schema):
     inspector = inspect(engine)
     return sorted(inspector.get_table_names(schema=schema))
 
 
-def get_table_primary_keys(engine, table):
-    tabmeta = Table(table, MetaData(), autoload_with=engine)
-    return tabmeta.primary_key.columns.values()
+def get_table_primary_keys(engine, schema, table):
+    tabmeta = Table(table, MetaData(), schema=schema, autoload_with=engine)
+    return [c.name for c in tabmeta.primary_key.columns.values()]
```

### Comparing `tulona-0.5.4/core/tulona/util/dataframe.py` & `tulona-0.6.3/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/core/tulona/util/excel.py` & `tulona-0.6.3/core/tulona/util/excel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from typing import List, Tuple, Union
+from pathlib import Path
+from typing import Dict, List, Tuple, Union
 
+import pandas as pd
 from openpyxl import load_workbook, styles
 from openpyxl.styles import Border, Side
 from openpyxl.worksheet.worksheet import Worksheet
 
 
 def get_column_index(sheet: Worksheet, column: str):
     for row in sheet.iter_rows(min_row=1, max_row=1, values_only=True):
@@ -76,7 +78,15 @@
                         row[col_idx].border = left_border
                     elif i == num_ds - 1:
                         row[col_idx + i].border = right_border
                     else:
                         row[col_idx + i].border = middle_border
 
     wb.save(excel_file)
+
+
+def dataframes_into_excel(
+    sheet_df_map: Dict, outfile_fqn: Union[Path, str], mode: str
+) -> None:
+    with pd.ExcelWriter(outfile_fqn, mode=mode) as writer:
+        for sheet, df in sheet_df_map.items():
+            df.to_excel(writer, sheet_name=sheet, index=False)
```

### Comparing `tulona-0.5.4/core/tulona/util/filesystem.py` & `tulona-0.6.3/core/tulona/util/filesystem.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,12 +37,11 @@
 
 def get_result_dir(dir_dict: dict, base: Union[str, Path], key: str) -> Path:
     p = Path(get_output_base_dir(base), dir_dict[key])
     return create_or_replace_dir(p)
 
 
 # TODO: Testable - pull current timestamp from caller
-def get_outfile_fqn(outdir: str, ds_list: List[str], infix: str):
+def get_final_outdir(basedir: str, ds_list: List[str]):
     out_timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
-    outfile = f"{'_'.join(ds_list)}_{infix}_{out_timestamp}.xlsx"
-    outfile_fqn = Path(outdir, outfile)
-    return outfile_fqn
+    final_outdir = Path(basedir, f"{'_'.join(ds_list)}_{out_timestamp}")
+    return final_outdir
```

### Comparing `tulona-0.5.4/core/tulona/util/profiles.py` & `tulona-0.6.3/core/tulona/util/profiles.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 
 
 def extract_profile_name(project: Dict, datasource: str):
     ds_profile_name = project["datasources"][datasource]["connection_profile"]
     return ds_profile_name
 
 
-def get_connection_profile(profile: Dict, project: Dict, datasource: str):
-    ds_profile_name = extract_profile_name(project, datasource)
+def get_connection_profile(profile: Dict, config: Dict):
+    ds_profile_name = config["connection_profile"]
     connection_profile = profile["profiles"][ds_profile_name]
     return connection_profile
```

### Comparing `tulona-0.5.4/core/tulona/util/sql.py` & `tulona-0.6.3/core/tulona/util/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         # TODO: system_rows method not implemented, tablesample works for percentage selection
         # query = f"select * from {table_name} tablesample system_rows({sample_count})"
         query = f"select * from {table_name} limit {sample_count}"
     elif dbtype == "mysql":
         query = f"select * from {table_name} limit {sample_count}"
     else:
         raise TulonaNotImplementedError(
-            f"Extracting sample rows from source type {dbtype} is not implemented."
+            f"Extracting sample rows from adapter type {dbtype} is not implemented."
         )
 
     return query
 
 
 def get_column_query(table_fqn: str, columns: List[str], quoted=False):
     column_expr = ", ".join([f'"{c}"' if quoted else c for c in columns])
```

### Comparing `tulona-0.5.4/core/tulona.egg-info/PKG-INFO` & `tulona-0.6.3/core/tulona.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.5.4
+Version: 0.6.3
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -20,15 +20,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click~=8.1
 Requires-Dist: ruamel.yaml~=0.18
 Requires-Dist: psycopg2-binary~=2.9
 Requires-Dist: pymysql~=1.1
 Requires-Dist: cryptography~=42.0
-Requires-Dist: snowflake-sqlalchemy==1.5
+Requires-Dist: snowflake-sqlalchemy~=1.5
 Requires-Dist: pyodbc~=5.1
 Requires-Dist: pandas~=1.5
 Requires-Dist: openpyxl~=3.1
 Requires-Dist: Jinja2~=3.1
 Requires-Dist: pydantic~=2.7
 
 Tulona
@@ -141,25 +141,49 @@
       table: people_composite_key
       primary_key:
         - ID_1
         - ID_2
       compare_column:
         - ID_1
         - ID_2
+    postgresdb_postgres:
+      connection_profile: pgdb
+      database: postgresdb
+    none_mysql:
+      connection_profile: mydb
+    postgresdb_postgres_schema:
+      connection_profile: pgdb
+      database: postgresdb
+      schema: corporate_copy
+    none_mysql_schema:
+      connection_profile: mydb
+      schema: corporate
+    employee_postgres_query:
+      connection_profile: pgdb
+      query: select * from postgresdb.corporate.employee
+      primary_key: Employee_ID
+      compare_column: Employee_ID
+    employee_mysql_query:
+      connection_profile: mydb
+      query: select * from corporate.employee
+      primary_key: Employee_ID
+      compare_column: Employee_ID
 
   # List of lists
   # The inner lists have datasources that need to be used for tasks like comparison
   # For example employee_postgres vs employee_mysql. So a [employee_postgres, employee_mysql]
   # Outer list is a list of those combinations.
   # So like: [[employee_postgres, employee_mysql], [datasource3, datasource4]]
   source_map:
     - - employee_postgres
       - employee_mysql
     - - person_postgres
       - person_mysql
+    - - employee_postgres_query
+      - employee_mysql_query
 
 
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 All commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
@@ -185,23 +209,27 @@
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
 
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
 
     ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
-* **compare-data**: To compare sample data from two sources/tables. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
+* **compare-row**: To compare sample data from two sources/tables/queries. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
 
   * Command without `--sample-count` parameter:
 
-    ``tulona compare-data --datasources employee_postgres,employee_mysql``
+    ``tulona compare-row --datasources employee_postgres,employee_mysql``
 
   * Command with `--sample-count` parameter:
 
-    ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
+    ``tulona compare-row --sample-count 50 --datasources employee_postgres,employee_mysql``
+
+  * Compare queries instead of tables, useful when you want to compare resutls of two queries:
+
+    ``tulona compare-row --datasources employee_postgres_query,employee_mysql_query``
 
 * **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
 
   * Column[s] to compare is[are] specified in `tulona-project.yml` file as part of datasource configs, with `compare_column` property. Sample command:
 
     ``tulona compare-column --datasources employee_postgres,employee_mysql``
 
@@ -209,14 +237,24 @@
 
     ``tulona compare-column --composite --datasources employee_postgres,employee_mysql``
 
 * **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
   ``tulona compare --datasources employee_postgres,employee_mysql``
 
+* **scan**: To scan and compare databases or schemas in terms of metadata and tables present if you want to compare all tables and don't want to set up datasource config for all of them. Sample commands:
+
+  * Scan without comparing:
+
+    ``tulona scan --datasources postgresdb_postgres_schema,none_mysql_schema``
+
+  * Scan and compare:
+
+    ``tulona scan --compare --datasources postgresdb_postgres_schema,none_mysql_schema``
+
 
 From `tulona v0.4.0` a new project config property has been introduced: `source_map`. If this config is set, in the project config file (tulona-project.yml), then `--datasources` parameter can be skipped with commands.
 For example this command:
 
 ``tulona compare --datasources employee_postgres,employee_mysql``
 
 will become this:
```

### Comparing `tulona-0.5.4/core/tulona.egg-info/SOURCES.txt` & `tulona-0.6.3/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.5.4/pyproject.toml` & `tulona-0.6.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "tulona"
-version = "0.5.4"
+version = "0.6.3"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
-  "snowflake-sqlalchemy==1.5", # can't upgrade or set to ~= until https://github.com/snowflakedb/snowflake-sqlalchemy/issues/485 is resolved
+  "snowflake-sqlalchemy~=1.5",
   "pyodbc~=5.1",
   "pandas~=1.5", # can't upgrade until https://github.com/pandas-dev/pandas/issues/57053 is resolved
   "openpyxl~=3.1",
   "Jinja2~=3.1",
   "pydantic~=2.7",
 ]
 requires-python = ">= 3.8"
@@ -111,15 +111,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.5.4"
+current_version = "0.6.3"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = false
```

