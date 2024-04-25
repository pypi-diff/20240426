# Comparing `tmp/pf-azuredb-0.0.5.tar.gz` & `tmp/pf_azuredb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pf-azuredb-0.0.5.tar", last modified: Thu Apr  4 05:42:20 2024, max compression
+gzip compressed data, was "pf_azuredb-1.0.0.tar", last modified: Thu Apr 25 23:00:08 2024, max compression
```

## Comparing `pf-azuredb-0.0.5.tar` & `pf_azuredb-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.886023 pf-azuredb-0.0.5/
--rw-rw-rw-   0        0        0       30 2024-02-14 18:46:53.000000 pf-azuredb-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      316 2024-04-04 05:42:20.883041 pf-azuredb-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.881022 pf-azuredb-0.0.5/pf_azuredb.egg-info/
--rw-rw-rw-   0        0        0      316 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.725044 pf-azuredb-0.0.5/pfazuredb/
--rw-rw-rw-   0        0        0       82 2024-02-14 18:46:53.000000 pf-azuredb-0.0.5/pfazuredb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.778414 pf-azuredb-0.0.5/pfazuredb/tools/
--rw-rw-rw-   0        0        0       82 2024-02-14 18:46:53.000000 pf-azuredb-0.0.5/pfazuredb/tools/__init__.py
--rw-rw-rw-   0        0        0     2427 2024-04-04 05:42:11.000000 pf-azuredb-0.0.5/pfazuredb/tools/mongodbvcore.py
--rw-rw-rw-   0        0        0     5241 2024-04-04 05:34:08.000000 pf-azuredb-0.0.5/pfazuredb/tools/postgrespg.py
--rw-rw-rw-   0        0        0      555 2024-02-14 18:46:53.000000 pf-azuredb-0.0.5/pfazuredb/tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.823161 pf-azuredb-0.0.5/pfazuredb/yamls/
--rw-rw-rw-   0        0        0      724 2024-04-04 05:42:11.000000 pf-azuredb-0.0.5/pfazuredb/yamls/mongodbvcore.yaml
--rw-rw-rw-   0        0        0      661 2024-04-04 05:34:08.000000 pf-azuredb-0.0.5/pfazuredb/yamls/postgrespg.yaml
--rw-rw-rw-   0        0        0       42 2024-04-04 05:42:20.886023 pf-azuredb-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      663 2024-04-04 05:42:11.000000 pf-azuredb-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.879017 pf-azuredb-0.0.5/tests/
--rw-rw-rw-   0        0        0        0 2024-02-14 18:46:53.000000 pf-azuredb-0.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0     1966 2024-04-04 05:31:30.000000 pf-azuredb-0.0.5/tests/test_mongovcore.py
--rw-rw-rw-   0        0        0     2075 2024-03-15 21:54:45.000000 pf-azuredb-0.0.5/tests/test_postgres.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:00:08.342271 pf_azuredb-1.0.0/
+-rw-rw-rw-   0        0        0       30 2024-02-14 18:46:53.000000 pf_azuredb-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      316 2024-04-25 23:00:08.339270 pf_azuredb-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 23:00:08.337269 pf_azuredb-1.0.0/pf_azuredb.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-04-25 23:00:08.000000 pf_azuredb-1.0.0/pf_azuredb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2024-04-25 23:00:08.000000 pf_azuredb-1.0.0/pf_azuredb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 23:00:08.000000 pf_azuredb-1.0.0/pf_azuredb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-25 23:00:08.000000 pf_azuredb-1.0.0/pf_azuredb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2024-04-25 23:00:08.000000 pf_azuredb-1.0.0/pf_azuredb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 23:00:08.000000 pf_azuredb-1.0.0/pf_azuredb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 23:00:08.308033 pf_azuredb-1.0.0/pfazuredb/
+-rw-rw-rw-   0        0        0       82 2024-02-14 18:46:53.000000 pf_azuredb-1.0.0/pfazuredb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:00:08.320377 pf_azuredb-1.0.0/pfazuredb/tools/
+-rw-rw-rw-   0        0        0       82 2024-02-14 18:46:53.000000 pf_azuredb-1.0.0/pfazuredb/tools/__init__.py
+-rw-rw-rw-   0        0        0     2427 2024-04-23 23:43:18.000000 pf_azuredb-1.0.0/pfazuredb/tools/mongodbvcore.py
+-rw-rw-rw-   0        0        0     5265 2024-04-24 01:49:40.000000 pf_azuredb-1.0.0/pfazuredb/tools/postgrespg.py
+-rw-rw-rw-   0        0        0      555 2024-02-14 18:46:53.000000 pf_azuredb-1.0.0/pfazuredb/tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:00:08.327509 pf_azuredb-1.0.0/pfazuredb/yamls/
+-rw-rw-rw-   0        0        0      724 2024-04-04 05:42:11.000000 pf_azuredb-1.0.0/pfazuredb/yamls/mongodbvcore.yaml
+-rw-rw-rw-   0        0        0      661 2024-04-04 05:34:08.000000 pf_azuredb-1.0.0/pfazuredb/yamls/postgrespg.yaml
+-rw-rw-rw-   0        0        0       42 2024-04-25 23:00:08.344374 pf_azuredb-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      663 2024-04-24 00:59:17.000000 pf_azuredb-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:00:08.333258 pf_azuredb-1.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-14 18:46:53.000000 pf_azuredb-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1919 2024-04-24 01:38:36.000000 pf_azuredb-1.0.0/tests/test_mongovcore.py
+-rw-rw-rw-   0        0        0     2177 2024-04-24 01:45:09.000000 pf_azuredb-1.0.0/tests/test_postgres.py
```

### Comparing `pf-azuredb-0.0.5/pfazuredb/tools/mongodbvcore.py` & `pf_azuredb-1.0.0/pfazuredb/tools/mongodbvcore.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     embeddings: list,
     filter_query: str = "{}",
     search_type: str = "vector",
     embedding_key: str = "contentVector",
 ) -> str:
     from pymongo import MongoClient
 
-    uri = connection.configs["AZURE_COSMOSDB_MONGODB_URI"]
+    uri = connection.secrets["AZURE_COSMOSDB_MONGODB_URI"]
     mongo_client = MongoClient(uri)
 
     db = mongo_client[db_name]
     collection = db[collection_name]
 
     if search_type == "vector" and filter_query:
         warnings.warn(
```

### Comparing `pf-azuredb-0.0.5/pfazuredb/tools/postgrespg.py` & `pf_azuredb-1.0.0/pfazuredb/tools/postgrespg.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from pgvector.psycopg2 import register_vector
     from psycopg2 import Error
     import numpy as np
     import psycopg2
     import json
 
     # establish connection
-    pgconnection = psycopg2.connect(connection.configs["conn_string"])
+    pgconnection = psycopg2.connect(connection.secrets["AZURE_COSMOSDB_POSTGRES_CONN_STRING"])
     register_vector(pgconnection)
 
     if vectorsearch_method == "L2":
         distance_operator = "<->"
     elif vectorsearch_method == "Cosine":
         distance_operator = "<=>"
     elif vectorsearch_method == "Inner":
```

### Comparing `pf-azuredb-0.0.5/pfazuredb/tools/utils.py` & `pf_azuredb-1.0.0/pfazuredb/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pf-azuredb-0.0.5/pfazuredb/yamls/mongodbvcore.yaml` & `pf_azuredb-1.0.0/pfazuredb/yamls/mongodbvcore.yaml`

 * *Files identical despite different names*

### Comparing `pf-azuredb-0.0.5/pfazuredb/yamls/postgrespg.yaml` & `pf_azuredb-1.0.0/pfazuredb/yamls/postgrespg.yaml`

 * *Files identical despite different names*

### Comparing `pf-azuredb-0.0.5/setup.py` & `pf_azuredb-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "pf-azuredb"
 
 setup(
     name=PACKAGE_NAME,
     author="Hossein K. Heris and applied ai team@azure data",
-    version="0.0.5",
+    version="1.0.0",
     description="Package for use in promptflow for vector search in azure db",
     packages=find_packages(),
     entry_points={
         "package_tools": ["azuredb = pfazuredb.tools.utils:list_package_tools"],
     },
     include_package_data=True,  # This line tells setuptools to include files from MANIFEST.in
     install_requires=[
```

### Comparing `pf-azuredb-0.0.5/tests/test_mongovcore.py` & `pf_azuredb-1.0.0/tests/test_mongovcore.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,25 +14,24 @@
 config = dotenv_values(os.path.join(root_dir, ".env"))
 
 
 @pytest.fixture
 def test_mongo_connection() -> CustomConnection:
     test_mongo_connection = CustomConnection(
         name="mongovcore_connection",
-        secrets={"my_key": "DUMMY"},  # unsupported
-        configs={
-            "AZURE_COSMOSDB_MONGODB_URI": config["COSMOS_DB_MONGO_URI"],
-        },
+        secrets={
+            "AZURE_COSMOSDB_MONGODB_URI": config["COSMOS_DB_MONGO_URI"]
+        }, 
     )
     return test_mongo_connection
 
 
-@pytest.mark.skip(
-    reason="Need to provide a valid .env file for the Azure CosmosDB MongoDB URI, DB_NAME, and COLLECTION_NAME"
-)
+# @pytest.mark.skip(
+#     reason="Need to provide a valid .env file for the Azure CosmosDB MongoDB URI, DB_NAME, and COLLECTION_NAME"
+# )
 class TestTool:
     def test_vectorsearch(
         self,
         test_mongo_connection,
         db_name=config["DB_NAME"],
         collection_name=config["COLLECTION_NAME"],
         num_results=3,
```

### Comparing `pf-azuredb-0.0.5/tests/test_postgres.py` & `pf_azuredb-1.0.0/tests/test_postgres.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,43 +14,47 @@
 config = dotenv_values(os.path.join(root_dir, ".env"))
 
 
 @pytest.fixture
 def test_postgres_connection() -> CustomConnection:
     test_postgres_connection = CustomConnection(
         name="postgres_connection",
-        secrets={"my_key": "DUMMY"},  # unsupported
-        configs={
-            "conn_string": config["COSMOSDB_POSTGRES_CONN_STRING"],
+        secrets={
+            "AZURE_COSMOSDB_POSTGRES_CONN_STRING": config[
+                "COSMOSDB_POSTGRES_CONN_STRING"
+            ]
         },
     )
     return test_postgres_connection
 
 
-@pytest.mark.skip(
-    reason="Need to provide a valid .env file for the Azure CosmosDB POSTGRES CONNECTION STRING AND TABLE_NAME"
-)
+# @pytest.mark.skip(
+#     reason="Need to provide a valid .env file for the Azure CosmosDB POSTGRES CONNECTION STRING AND TABLE_NAME"
+# )
 class TestTool:
     def test_vectorsearch(
         self,
         test_postgres_connection,
         table_name=config["TABLE_NAME"],
-        num_results=3,
         search_type="vector",
-        vectorsearch_method="L2",
+        num_results=3,
         embeddings=[0.1, 0.2, 0.3] * 512,
+        vectorsearch_method="L2",
+        question="None",
+        filter_text="None",
     ):
         result = vectorsearch(
             connection=test_postgres_connection,
             table_name=table_name,
             search_type=search_type,
             vectorsearch_method=vectorsearch_method,
             num_results=num_results,
             embeddings=embeddings,
-            filter_text=None,
+            filter_text=filter_text,
+            question=question,
         )
         # Assert that the result is a list
         assert isinstance(result, list), "Result is not a list"
         # Assert that the result is not empty
         assert result, "Result is empty"
         # Assert that each element in the result list is a dictionary
         # assert all(isinstance(item, dict) for item in result), "Result contains non-dictionary elements"
```

