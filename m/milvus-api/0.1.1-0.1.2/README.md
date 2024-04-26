# Comparing `tmp/milvus_api-0.1.1.tar.gz` & `tmp/milvus_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milvus_api-0.1.1.tar", last modified: Thu Apr 25 15:57:10 2024, max compression
+gzip compressed data, was "milvus_api-0.1.2.tar", last modified: Fri Apr 26 01:32:28 2024, max compression
```

## Comparing `milvus_api-0.1.1.tar` & `milvus_api-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 15:57:10.154861 milvus_api-0.1.1/
--rw-rw-rw-   0        0        0     2482 2024-04-25 15:57:10.154861 milvus_api-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2023 2024-04-25 15:39:25.000000 milvus_api-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 15:57:10.106657 milvus_api-0.1.1/milvus_api/
--rw-rw-rw-   0        0        0        0 2024-04-25 15:55:58.000000 milvus_api-0.1.1/milvus_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:57:10.138795 milvus_api-0.1.1/milvus_api/db_model/
--rw-rw-rw-   0        0        0        0 2024-04-25 13:02:02.000000 milvus_api-0.1.1/milvus_api/db_model/__init__.py
--rw-rw-rw-   0        0        0     5824 2024-04-25 15:07:24.000000 milvus_api-0.1.1/milvus_api/db_model/milvus_db.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:57:10.138795 milvus_api-0.1.1/milvus_api/embed_model/
--rw-rw-rw-   0        0        0        0 2024-04-25 15:06:57.000000 milvus_api-0.1.1/milvus_api/embed_model/__init__.py
--rw-rw-rw-   0        0        0     1257 2024-04-25 15:29:44.000000 milvus_api-0.1.1/milvus_api/embed_model/bgem3.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:57:10.122163 milvus_api-0.1.1/milvus_api.egg-info/
--rw-rw-rw-   0        0        0     2482 2024-04-25 15:57:09.000000 milvus_api-0.1.1/milvus_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-25 15:57:09.000000 milvus_api-0.1.1/milvus_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 15:57:09.000000 milvus_api-0.1.1/milvus_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2024-04-25 15:57:09.000000 milvus_api-0.1.1/milvus_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-25 15:57:09.000000 milvus_api-0.1.1/milvus_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 15:57:10.154861 milvus_api-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      616 2024-04-25 15:56:50.000000 milvus_api-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:32:28.579153 milvus_api-0.1.2/
+-rw-rw-rw-   0        0        0     2526 2024-04-26 01:32:28.579153 milvus_api-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2067 2024-04-26 01:19:55.000000 milvus_api-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 01:32:28.547388 milvus_api-0.1.2/milvus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-25 15:55:58.000000 milvus_api-0.1.2/milvus_api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:32:28.563648 milvus_api-0.1.2/milvus_api/db_model/
+-rw-rw-rw-   0        0        0        0 2024-04-25 13:02:02.000000 milvus_api-0.1.2/milvus_api/db_model/__init__.py
+-rw-rw-rw-   0        0        0     5826 2024-04-26 01:09:46.000000 milvus_api-0.1.2/milvus_api/db_model/milvus_db.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:32:28.579153 milvus_api-0.1.2/milvus_api/embed_model/
+-rw-rw-rw-   0        0        0        0 2024-04-25 15:06:57.000000 milvus_api-0.1.2/milvus_api/embed_model/__init__.py
+-rw-rw-rw-   0        0        0     1257 2024-04-25 15:29:44.000000 milvus_api-0.1.2/milvus_api/embed_model/bgem3.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:32:28.563648 milvus_api-0.1.2/milvus_api.egg-info/
+-rw-rw-rw-   0        0        0     2526 2024-04-26 01:32:28.000000 milvus_api-0.1.2/milvus_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-26 01:32:28.000000 milvus_api-0.1.2/milvus_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 01:32:28.000000 milvus_api-0.1.2/milvus_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2024-04-26 01:32:28.000000 milvus_api-0.1.2/milvus_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 01:32:28.000000 milvus_api-0.1.2/milvus_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 01:32:28.579153 milvus_api-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      616 2024-04-26 01:28:34.000000 milvus_api-0.1.2/setup.py
```

### Comparing `milvus_api-0.1.1/PKG-INFO` & `milvus_api-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milvus_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Milvus API used for quickly setting up a Milvus vector database
 Author: ShengWen
 Author-email: shengwen8785@example.com
 Description-Content-Type: text/markdown
 Requires-Dist: pymilvus==2.4.0
 Requires-Dist: milvus-model==0.2.0
 Requires-Dist: pydantic==2.7.0
@@ -27,14 +27,15 @@
 
 ## Usage Examples
 ### Creating a Database Collection
 
 Here's how to create a new database collection using `milvus_api`:
 ```
 from milvus_api.db_model.milvus_db import MilvusDB
+from pymilvus import FiledSchema, DataType
 
 host = 'localhost'
 port = '19530'
 db = MilvusDB(host, port)
 
 fields = [  
     FieldSchema(name="id", dtype=DataType.INT64, auto_id=True, is_primary=True),
```

### Comparing `milvus_api-0.1.1/README.md` & `milvus_api-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 ## Usage Examples
 ### Creating a Database Collection
 
 Here's how to create a new database collection using `milvus_api`:
 ```
 from milvus_api.db_model.milvus_db import MilvusDB
+from pymilvus import FiledSchema, DataType
 
 host = 'localhost'
 port = '19530'
 db = MilvusDB(host, port)
 
 fields = [  
     FieldSchema(name="id", dtype=DataType.INT64, auto_id=True, is_primary=True),
```

### Comparing `milvus_api-0.1.1/milvus_api/db_model/milvus_db.py` & `milvus_api-0.1.2/milvus_api/db_model/milvus_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         ]
 
     def info(self):
         """
         Display connection information of Milvus.
         """
         print(f"Milvus | Host Server : {self.__host} | Port: {self.__port}")
-        print(f"All collections: {reduce(lambda e1,e2: e1+','+e2, utility.list_collections())}")
+        # print(f"All collections: {reduce(lambda e1,e2: e1+','+e2, utility.list_collections())}")
 
     @staticmethod
     def insert_data(collection_name: str, data: List[dict], chunk_size: int = 1000) -> None:
         """
         Batch insert data into the database.
         This function takes a list of data and inserts it into the database in a batch manner,
         improving efficiency for large datasets.
```

### Comparing `milvus_api-0.1.1/milvus_api/embed_model/bgem3.py` & `milvus_api-0.1.2/milvus_api/embed_model/bgem3.py`

 * *Files identical despite different names*

### Comparing `milvus_api-0.1.1/milvus_api.egg-info/PKG-INFO` & `milvus_api-0.1.2/milvus_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milvus-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Milvus API used for quickly setting up a Milvus vector database
 Author: ShengWen
 Author-email: shengwen8785@example.com
 Description-Content-Type: text/markdown
 Requires-Dist: pymilvus==2.4.0
 Requires-Dist: milvus-model==0.2.0
 Requires-Dist: pydantic==2.7.0
@@ -27,14 +27,15 @@
 
 ## Usage Examples
 ### Creating a Database Collection
 
 Here's how to create a new database collection using `milvus_api`:
 ```
 from milvus_api.db_model.milvus_db import MilvusDB
+from pymilvus import FiledSchema, DataType
 
 host = 'localhost'
 port = '19530'
 db = MilvusDB(host, port)
 
 fields = [  
     FieldSchema(name="id", dtype=DataType.INT64, auto_id=True, is_primary=True),
```

### Comparing `milvus_api-0.1.1/setup.py` & `milvus_api-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='milvus_api',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         "pymilvus==2.4.0",
         "milvus-model==0.2.0",
         "pydantic==2.7.0",
         "tqdm==4.66.2",
         "FlagEmbedding==1.2.9",
```

