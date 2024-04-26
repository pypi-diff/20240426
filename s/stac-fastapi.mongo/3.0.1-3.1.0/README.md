# Comparing `tmp/stac_fastapi_mongo-3.0.1.tar.gz` & `tmp/stac_fastapi_mongo-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_mongo-3.0.1.tar", last modified: Mon Apr 15 06:55:54 2024, max compression
+gzip compressed data, was "stac_fastapi_mongo-3.1.0.tar", last modified: Fri Apr 26 04:56:31 2024, max compression
```

## Comparing `stac_fastapi_mongo-3.0.1.tar` & `stac_fastapi_mongo-3.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-15 06:55:54.546510 stac_fastapi_mongo-3.0.1/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1071 2024-03-03 16:18:26.000000 stac_fastapi_mongo-3.0.1/LICENSE
--rw-r--r--   0 primeradiant   (501) staff       (20)       42 2024-03-10 17:01:51.000000 stac_fastapi_mongo-3.0.1/MANIFEST.in
--rw-r--r--   0 primeradiant   (501) staff       (20)     3194 2024-04-15 06:55:54.545365 stac_fastapi_mongo-3.0.1/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)     1843 2024-04-15 06:40:35.000000 stac_fastapi_mongo-3.0.1/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)       38 2024-04-15 06:55:54.546884 stac_fastapi_mongo-3.0.1/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1495 2024-04-15 06:46:05.000000 stac_fastapi_mongo-3.0.1/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-15 06:55:54.464399 stac_fastapi_mongo-3.0.1/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-15 06:55:54.527717 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/
--rw-r--r--   0 primeradiant   (501) staff       (20)       25 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2995 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/app.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2477 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/config.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    39873 2024-04-15 06:40:35.000000 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     1072 2024-03-10 17:01:51.000000 stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/utilities.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-15 06:55:54.529154 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     3194 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      488 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       66 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/entry_points.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      219 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       59 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.0.1/stac_fastapi.mongo.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-26 04:56:30.960650 stac_fastapi_mongo-3.1.0/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1071 2024-03-03 16:18:26.000000 stac_fastapi_mongo-3.1.0/LICENSE
+-rw-r--r--   0 primeradiant   (501) staff       (20)       42 2024-03-10 17:01:51.000000 stac_fastapi_mongo-3.1.0/MANIFEST.in
+-rw-r--r--   0 primeradiant   (501) staff       (20)     6330 2024-04-26 04:56:30.949797 stac_fastapi_mongo-3.1.0/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)     4938 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.1.0/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)       38 2024-04-26 04:56:30.961627 stac_fastapi_mongo-3.1.0/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1527 2024-04-26 04:45:17.000000 stac_fastapi_mongo-3.1.0/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-26 04:56:30.813793 stac_fastapi_mongo-3.1.0/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-26 04:56:30.931146 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       25 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3077 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/app.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3741 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/basic_auth.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2477 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/config.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    40317 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2911 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/utilities.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-26 04:56:30.933967 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     6330 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      521 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       66 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/entry_points.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      244 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       59 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/top_level.txt
```

### Comparing `stac_fastapi_mongo-3.0.1/LICENSE` & `stac_fastapi_mongo-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_fastapi_mongo-3.0.1/setup.py` & `stac_fastapi_mongo-3.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "stac-fastapi.core==2.1.0",
+    "stac-fastapi.core==2.3.0",
     "motor==3.3.2",
     "pymongo==4.6.2",
     "uvicorn",
     "starlette",
+    "typing_extensions==4.4.0",
 ]
 
 extra_reqs = {
     "dev": [
         "pytest",
         "pytest-cov",
         "pytest-asyncio",
@@ -25,15 +26,15 @@
     ],
     "docs": ["mkdocs", "mkdocs-material", "pdocs"],
     "server": ["uvicorn[standard]==0.19.0"],
 }
 
 setup(
     name="stac-fastapi.mongo",
-    version="3.0.1",
+    version="3.1.0",
     description="Mongodb stac-fastapi backend.",
     long_description=desc,
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
```

### Comparing `stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/app.py` & `stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     ContextExtension,
     FieldsExtension,
     FilterExtension,
     SortExtension,
     TokenPaginationExtension,
     TransactionExtension,
 )
+from stac_fastapi.mongo.basic_auth import apply_basic_auth
 
 # from stac_fastapi.extensions.third_party import BulkTransactionExtension
 from stac_fastapi.mongo.config import AsyncMongoDBSettings
 from stac_fastapi.mongo.database_logic import (
     DatabaseLogic,
     create_collection_index,
     create_item_index,
@@ -67,14 +68,16 @@
         database=database_logic, session=session, post_request_model=post_request_model
     ),
     search_get_request_model=create_get_request_model(extensions),
     search_post_request_model=post_request_model,
 )
 app = api.app
 
+apply_basic_auth(api)
+
 
 @app.on_event("startup")
 async def _startup_event() -> None:
     await create_collection_index()
     await create_item_index()
```

### Comparing `stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/config.py` & `stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_mongo-3.0.1/stac_fastapi/mongo/database_logic.py` & `stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/database_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,21 @@
 
 from stac_fastapi.core import serializers
 from stac_fastapi.core.extensions import filter
 from stac_fastapi.core.utilities import bbox2polygon
 from stac_fastapi.extensions.core import SortExtension
 from stac_fastapi.mongo.config import AsyncMongoDBSettings as AsyncSearchSettings
 from stac_fastapi.mongo.config import MongoDBSettings as SyncSearchSettings
-from stac_fastapi.mongo.utilities import decode_token, encode_token, serialize_doc
+from stac_fastapi.mongo.utilities import (
+    convert_obj_datetimes,
+    decode_token,
+    encode_token,
+    parse_datestring,
+    serialize_doc,
+)
 from stac_fastapi.types.errors import ConflictError, NotFoundError
 from stac_fastapi.types.stac import Collection, Item
 
 logger = logging.getLogger(__name__)
 
 NumType = Union[float, int]
 
@@ -247,23 +253,33 @@
             search (Search): The search object to filter.
             datetime_search (dict): The datetime filter criteria.
 
         Returns:
             Search: The filtered search object.
         """
         if "eq" in datetime_search:
-            search.add_filter({"properties.datetime": datetime_search["eq"]})
+            search.add_filter(
+                {"properties.datetime": parse_datestring(datetime_search["eq"])}
+            )
         else:
-            if "gte" in datetime_search:
+            if "gte" in datetime_search and datetime_search["gte"]:
                 search.add_filter(
-                    {"properties.datetime": {"$gte": datetime_search["gte"]}}
+                    {
+                        "properties.datetime": {
+                            "$gte": parse_datestring(datetime_search["gte"])
+                        }
+                    }
                 )
-            if "lte" in datetime_search:
+            if "lte" in datetime_search and datetime_search["lte"]:
                 search.add_filter(
-                    {"properties.datetime": {"$lte": datetime_search["lte"]}}
+                    {
+                        "properties.datetime": {
+                            "$lte": parse_datestring(datetime_search["lte"])
+                        }
+                    }
                 )
         return search
 
     @staticmethod
     def apply_bbox_filter(search: MongoSearchAdapter, bbox: List):
         """Filter search results based on bounding box.
 
@@ -634,14 +650,15 @@
             {"id": item["collection"]}, limit=1
         )
         if not collection_exists:
             raise NotFoundError(f"Collection {item['collection']} does not exist")
 
         new_item = item.copy()
         new_item["_id"] = item.get("_id", ObjectId())
+        convert_obj_datetimes(new_item)
 
         existing_item = await items_collection.find_one({"_id": new_item["_id"]})
         if existing_item:
             raise ConflictError(f"Item with _id {item['_id']} already exists")
 
         await items_collection.insert_one(new_item)
```

