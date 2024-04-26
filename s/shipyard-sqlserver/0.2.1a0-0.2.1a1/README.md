# Comparing `tmp/shipyard_sqlserver-0.2.1a0.tar.gz` & `tmp/shipyard_sqlserver-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_sqlserver-0.2.1a0.tar", max compression
+gzip compressed data, was "shipyard_sqlserver-0.2.1a1.tar", max compression
```

## Comparing `shipyard_sqlserver-0.2.1a0.tar` & `shipyard_sqlserver-0.2.1a1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-08-14 16:50:02.446349 shipyard_sqlserver-0.2.1a0/README.md
--rw-r--r--   0        0        0      679 2024-04-24 20:36:40.925511 shipyard_sqlserver-0.2.1a0/pyproject.toml
--rw-r--r--   0        0        0       39 2023-08-14 16:50:02.447093 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 19:26:39.005282 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/__init__.py
--rw-r--r--   0        0        0      947 2024-04-23 20:50:28.200126 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/authtest.py
--rw-r--r--   0        0        0     2059 2024-04-18 03:07:13.754478 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/execute_sql.py
--rw-r--r--   0        0        0     2991 2024-04-18 03:07:13.754853 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/store_query_results.py
--rw-r--r--   0        0        0     4149 2024-04-18 03:07:13.755269 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/upload_file.py
--rw-r--r--   0        0        0      342 2024-04-18 03:07:13.755839 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/exceptions.py
--rw-r--r--   0        0        0     4652 2024-04-23 20:22:26.196919 shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/sqlserver.py
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 shipyard_sqlserver-0.2.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-14 16:50:02.446349 shipyard_sqlserver-0.2.1a1/README.md
+-rw-r--r--   0        0        0      679 2024-04-25 21:26:32.699057 shipyard_sqlserver-0.2.1a1/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-08-14 16:50:02.447093 shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 19:26:39.005282 shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/cli/__init__.py
+-rw-r--r--   0        0        0      770 2024-04-25 21:21:56.495164 shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/cli/authtest.py
+-rw-r--r--   0        0        0     2059 2024-04-18 03:07:13.754478 shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/cli/execute_sql.py
+-rw-r--r--   0        0        0     2991 2024-04-18 03:07:13.754853 shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/cli/store_query_results.py
+-rw-r--r--   0        0        0     4149 2024-04-18 03:07:13.755269 shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/cli/upload_file.py
+-rw-r--r--   0        0        0      342 2024-04-18 03:07:13.755839 shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/exceptions.py
+-rw-r--r--   0        0        0     4652 2024-04-25 03:06:02.600469 shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/sqlserver.py
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 shipyard_sqlserver-0.2.1a1/PKG-INFO
```

### Comparing `shipyard_sqlserver-0.2.1a0/pyproject.toml` & `shipyard_sqlserver-0.2.1a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-sqlserver"
-version = "0.2.1a0"
+version = "0.2.1a1"
 description = "A local client for connecting and working with Sql Server Databases"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_sqlserver"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/authtest.py` & `shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/cli/authtest.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,22 +13,18 @@
             pwd=os.getenv("MSSQL_PASSWORD"),
             host=os.getenv("MSSQL_HOST"),
             database=os.getenv("MSSQL_DATABASE"),
             port=os.getenv("MSSQL_PORT"),
         )
         client.connect()
     except Exception as e:
-        logger.error(
-            f"Error in connecting to SQL Server. Message from the server reads: {e}"
-        )
         logger.authtest(
             f"Error in connecting to SQL Server. Message from the server reads: {e}"
         )
         sys.exit(1)
     else:
-        logger.info("Successfully connected to SQL Server")
         logger.authtest("Successfully connected to SQL Server")
         sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/execute_sql.py` & `shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/cli/execute_sql.py`

 * *Files identical despite different names*

### Comparing `shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/store_query_results.py` & `shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/cli/store_query_results.py`

 * *Files identical despite different names*

### Comparing `shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/cli/upload_file.py` & `shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/cli/upload_file.py`

 * *Files identical despite different names*

### Comparing `shipyard_sqlserver-0.2.1a0/shipyard_sqlserver/sqlserver.py` & `shipyard_sqlserver-0.2.1a1/shipyard_sqlserver/sqlserver.py`

 * *Files identical despite different names*

### Comparing `shipyard_sqlserver-0.2.1a0/PKG-INFO` & `shipyard_sqlserver-0.2.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-sqlserver
-Version: 0.2.1a0
+Version: 0.2.1a1
 Summary: A local client for connecting and working with Sql Server Databases
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

