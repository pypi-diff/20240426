# Comparing `tmp/mongodb_orm-0.0.116.tar.gz` & `tmp/mongodb_orm-0.0.117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_orm-0.0.116.tar", last modified: Fri Apr 26 09:30:53 2024, max compression
+gzip compressed data, was "mongodb_orm-0.0.117.tar", last modified: Fri Apr 26 10:17:10 2024, max compression
```

## Comparing `mongodb_orm-0.0.116.tar` & `mongodb_orm-0.0.117.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.121401 mongodb_orm-0.0.116/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-26 09:30:53.120663 mongodb_orm-0.0.116/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.116/README.md
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.082386 mongodb_orm-0.0.116/mongodb_orm/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.116/mongodb_orm/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.116/mongodb_orm/apps.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.103678 mongodb_orm-0.0.116/mongodb_orm/custom_urls/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.116/mongodb_orm/custom_urls/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1530 2024-04-23 15:22:07.000000 mongodb_orm-0.0.116/mongodb_orm/custom_urls/bread_urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.105065 mongodb_orm-0.0.116/mongodb_orm/decorators/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/decorators/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.116/mongodb_orm/decorators/chained.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.106552 mongodb_orm-0.0.116/mongodb_orm/exceptions/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/exceptions/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.116/mongodb_orm/exceptions/syntax_exceptions.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.108761 mongodb_orm-0.0.116/mongodb_orm/interfaces/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.116/mongodb_orm/interfaces/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2335 2024-04-26 09:29:13.000000 mongodb_orm-0.0.116/mongodb_orm/interfaces/base_mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7213 2024-04-23 15:18:03.000000 mongodb_orm-0.0.116/mongodb_orm/interfaces/mongodb_model.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.109609 mongodb_orm-0.0.116/mongodb_orm/management/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.116/mongodb_orm/management/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.110576 mongodb_orm-0.0.116/mongodb_orm/management/commands/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/management/commands/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.0.116/mongodb_orm/management/commands/update_schema.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.111375 mongodb_orm-0.0.116/mongodb_orm/models/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.116/mongodb_orm/models/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.112165 mongodb_orm-0.0.116/mongodb_orm/singletons/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/singletons/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.116/mongodb_orm/singletons/mongodb_singleton_client.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.116250 mongodb_orm-0.0.116/mongodb_orm/types/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.116/mongodb_orm/types/Relation.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/types/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.116/mongodb_orm/types/index.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.116/mongodb_orm/types/logger_object.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      453 2024-04-04 10:34:44.000000 mongodb_orm-0.0.116/mongodb_orm/types/model_schema.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.0.116/mongodb_orm/types/options.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      148 2024-04-23 14:22:14.000000 mongodb_orm-0.0.116/mongodb_orm/urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.117467 mongodb_orm-0.0.116/mongodb_orm/utils/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.0.116/mongodb_orm/utils/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1159 2024-04-23 15:18:03.000000 mongodb_orm-0.0.116/mongodb_orm/utils/helpers.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.118964 mongodb_orm-0.0.116/mongodb_orm/views/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/views/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.116/mongodb_orm/views/mongodb_api_model_view.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.119905 mongodb_orm-0.0.116/mongodb_orm.egg-info/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-26 09:30:52.000000 mongodb_orm-0.0.116/mongodb_orm.egg-info/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1161 2024-04-26 09:30:53.000000 mongodb_orm-0.0.116/mongodb_orm.egg-info/SOURCES.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-04-26 09:30:52.000000 mongodb_orm-0.0.116/mongodb_orm.egg-info/dependency_links.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-04-26 09:30:52.000000 mongodb_orm-0.0.116/mongodb_orm.egg-info/requires.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-04-26 09:30:52.000000 mongodb_orm-0.0.116/mongodb_orm.egg-info/top_level.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-04-26 09:30:53.121555 mongodb_orm-0.0.116/setup.cfg
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-04-26 09:30:44.000000 mongodb_orm-0.0.116/setup.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:10.012413 mongodb_orm-0.0.117/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-26 10:17:10.011633 mongodb_orm-0.0.117/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.117/README.md
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:09.984174 mongodb_orm-0.0.117/mongodb_orm/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.117/mongodb_orm/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.117/mongodb_orm/apps.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:09.987059 mongodb_orm-0.0.117/mongodb_orm/custom_urls/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.117/mongodb_orm/custom_urls/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1530 2024-04-23 15:22:07.000000 mongodb_orm-0.0.117/mongodb_orm/custom_urls/bread_urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:09.992117 mongodb_orm-0.0.117/mongodb_orm/decorators/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.117/mongodb_orm/decorators/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.117/mongodb_orm/decorators/chained.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:09.993456 mongodb_orm-0.0.117/mongodb_orm/exceptions/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.117/mongodb_orm/exceptions/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.117/mongodb_orm/exceptions/syntax_exceptions.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:09.996509 mongodb_orm-0.0.117/mongodb_orm/interfaces/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.117/mongodb_orm/interfaces/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2331 2024-04-26 10:05:08.000000 mongodb_orm-0.0.117/mongodb_orm/interfaces/base_mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7637 2024-04-26 10:15:42.000000 mongodb_orm-0.0.117/mongodb_orm/interfaces/mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      801 2024-04-26 10:15:42.000000 mongodb_orm-0.0.117/mongodb_orm/interfaces/mongodb_model_events.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:09.997106 mongodb_orm-0.0.117/mongodb_orm/management/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.117/mongodb_orm/management/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:09.998098 mongodb_orm-0.0.117/mongodb_orm/management/commands/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.117/mongodb_orm/management/commands/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.0.117/mongodb_orm/management/commands/update_schema.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:09.998987 mongodb_orm-0.0.117/mongodb_orm/models/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.117/mongodb_orm/models/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:09.999903 mongodb_orm-0.0.117/mongodb_orm/singletons/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.117/mongodb_orm/singletons/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.117/mongodb_orm/singletons/mongodb_singleton_client.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:10.007040 mongodb_orm-0.0.117/mongodb_orm/types/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.117/mongodb_orm/types/Relation.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.117/mongodb_orm/types/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.117/mongodb_orm/types/index.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.117/mongodb_orm/types/logger_object.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      453 2024-04-04 10:34:44.000000 mongodb_orm-0.0.117/mongodb_orm/types/model_schema.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.0.117/mongodb_orm/types/options.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      148 2024-04-23 14:22:14.000000 mongodb_orm-0.0.117/mongodb_orm/urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:10.008371 mongodb_orm-0.0.117/mongodb_orm/utils/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.0.117/mongodb_orm/utils/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1159 2024-04-23 15:18:03.000000 mongodb_orm-0.0.117/mongodb_orm/utils/helpers.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:10.009796 mongodb_orm-0.0.117/mongodb_orm/views/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.117/mongodb_orm/views/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.117/mongodb_orm/views/mongodb_api_model_view.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:17:10.010745 mongodb_orm-0.0.117/mongodb_orm.egg-info/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-26 10:17:09.000000 mongodb_orm-0.0.117/mongodb_orm.egg-info/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-04-26 10:17:09.000000 mongodb_orm-0.0.117/mongodb_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-04-26 10:17:09.000000 mongodb_orm-0.0.117/mongodb_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-04-26 10:17:09.000000 mongodb_orm-0.0.117/mongodb_orm.egg-info/requires.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-04-26 10:17:09.000000 mongodb_orm-0.0.117/mongodb_orm.egg-info/top_level.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-04-26 10:17:10.012608 mongodb_orm-0.0.117/setup.cfg
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-04-26 10:16:04.000000 mongodb_orm-0.0.117/setup.py
```

### Comparing `mongodb_orm-0.0.116/README.md` & `mongodb_orm-0.0.117/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.116/mongodb_orm/custom_urls/bread_urls.py` & `mongodb_orm-0.0.117/mongodb_orm/custom_urls/bread_urls.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.116/mongodb_orm/interfaces/base_mongodb_model.py` & `mongodb_orm-0.0.117/mongodb_orm/interfaces/base_mongodb_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from mongodb_orm.types.options import Options
 from mongodb_orm.types.Relation import Relation
 from mongodb_orm.singletons.mongodb_singleton_client import MongoDBClient
 
 
 class BaseMongoDBModel:
     """
-            Preventing direct Instantiation of this class
+        Preventing direct Instantiation of this class
     """
 
     def __new__(cls, *args, **kwargs):
         if cls is BaseMongoDBModel:
             raise TypeError(f"only children of '{cls.__name__}' may be instantiated")
         return object.__new__(cls)
```

### Comparing `mongodb_orm-0.0.116/mongodb_orm/interfaces/mongodb_model.py` & `mongodb_orm-0.0.117/mongodb_orm/interfaces/mongodb_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 import pymongo
 from bson import ObjectId
 from datetime import datetime
 from typing import List, Union, Sequence
 from pymongo.cursor import Cursor
 from pymongo.collection import Collection
 from pymongo.results import InsertOneResult
+
+from mongodb_orm.interfaces.mongodb_model_events import MongoDBModelEvents
 from mongodb_orm.types.index import Index
 from mongodb_orm.utils.helpers import Helper
 from mongodb_orm.types.options import Options
 from mongodb_orm.types.Relation import Relation
 from mongodb_orm.decorators.chained import chained
 from mongodb_orm.exceptions.syntax_exceptions import ChainingError
 from mongodb_orm.interfaces.base_mongodb_model import BaseMongoDBModel
 
 
-class MongoDBModel(BaseMongoDBModel):
+class MongoDBModel(BaseMongoDBModel, MongoDBModelEvents):
     """
         Public class variables to be overridden by the model
     """
     collection_name: str = ''
     # Check the following link to check what are the possible valid options for collection creation
     # https://www.mongodb.com/docs/manual/reference/method/db.createCollection/
     options: Options = None
@@ -109,41 +111,46 @@
 
     @chained
     def find_one(self, filters: dict, sort_criteria: List[tuple] = None) -> Union[dict, 'MongoDBModel']:
         return self._collection.find_one(filters, sort=sort_criteria, projection=self._projection)
 
     @chained
     def put(self, pk: str, record: dict) -> Union[dict, 'MongoDBModel']:
-        return self._collection.find_one_and_update({'_id': ObjectId(pk)},
-                                                    {'$set': {**record, **({
-                                                                               'updated_at': datetime.utcnow()
-                                                                           } if self.timestamp else {})}},
-                                                    projection=self._projection)
+        query = self._collection.find_one_and_update({'_id': ObjectId(pk)},
+                                                     {'$set': {**record, **({
+                                                                                'updated_at': datetime.utcnow()
+                                                                            } if self.timestamp else {})}},
+                                                     projection=self._projection)
+        MongoDBModelEvents.on_partial_update(self, self.get(pk).json(), record)
+        return query
 
     @chained
     def patch(self, pk: str, record: dict) -> Union[dict, 'MongoDBModel']:
-        return self._collection.find_one_and_update({'_id': ObjectId(pk)},
-                                                    {'$push': record,
-                                                     '$set':
-                                                         {**({
-                                                                 'updated_at': datetime.utcnow()
-                                                             } if self.timestamp else {})}
-                                                     },
-                                                    projection=self._projection)
+        query = self._collection.find_one_and_update({'_id': ObjectId(pk)},
+                                                     {'$push': record,
+                                                      '$set':
+                                                          {**({
+                                                                  'updated_at': datetime.utcnow()
+                                                              } if self.timestamp else {})}
+                                                      },
+                                                     projection=self._projection)
+        MongoDBModelEvents.on_partial_update(self, record, self.get(pk).json())
+        return query
 
     @chained
     def put_patch(self, pk: str, put_record: dict, patch_record: dict) -> Union[dict, 'MongoDBModel']:
         return self._collection.find_one_and_update({'_id': ObjectId(pk)},
                                                     {'$set': {**put_record, **({
                                                                                    'updated_at': datetime.utcnow()
                                                                                } if self.timestamp else {})},
                                                      '$push': patch_record},
                                                     projection=self._projection)
 
     def post(self, record: dict) -> Union[InsertOneResult, 'MongoDBModel']:
+        MongoDBModelEvents.on_save(self, record)
         return self._collection.insert_one({**record, **({
                                                              'created_at': datetime.utcnow(),
                                                              'updated_at': datetime.utcnow()
                                                          } if self.timestamp else {})})
 
     # def mass_patch(self):
     #     return self._collection.update_many(
@@ -155,11 +162,12 @@
     #                     'updated_at': datetime.utcnow()
     #                 }
     #             }
     #         ]
     #     )
 
     def delete(self, pk: str) -> bool:
+        MongoDBModelEvents.on_delete(self, self.get(pk).json())
         return bool(self._collection.find_one_and_delete({'_id': ObjectId(pk)}, projection=self._projection))
 
     def count(self, filters: dict = None) -> int:
         return self._collection.count_documents(filters if filters else {})
```

### Comparing `mongodb_orm-0.0.116/mongodb_orm/management/commands/update_schema.py` & `mongodb_orm-0.0.117/mongodb_orm/management/commands/update_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.116/mongodb_orm/utils/helpers.py` & `mongodb_orm-0.0.117/mongodb_orm/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.116/mongodb_orm/views/mongodb_api_model_view.py` & `mongodb_orm-0.0.117/mongodb_orm/views/mongodb_api_model_view.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.116/mongodb_orm.egg-info/SOURCES.txt` & `mongodb_orm-0.0.117/mongodb_orm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 mongodb_orm/decorators/__init__.py
 mongodb_orm/decorators/chained.py
 mongodb_orm/exceptions/__init__.py
 mongodb_orm/exceptions/syntax_exceptions.py
 mongodb_orm/interfaces/__init__.py
 mongodb_orm/interfaces/base_mongodb_model.py
 mongodb_orm/interfaces/mongodb_model.py
+mongodb_orm/interfaces/mongodb_model_events.py
 mongodb_orm/management/__init__.py
 mongodb_orm/management/commands/__init__.py
 mongodb_orm/management/commands/update_schema.py
 mongodb_orm/models/__init__.py
 mongodb_orm/singletons/__init__.py
 mongodb_orm/singletons/mongodb_singleton_client.py
 mongodb_orm/types/Relation.py
```

### Comparing `mongodb_orm-0.0.116/setup.py` & `mongodb_orm-0.0.117/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 # Fix and optimise the library installation
 setup(
     name="mongodb_orm",
-    version="0.0.116",
+    version="0.0.117",
     author="Khai",
     author_email="sarraj.khaireddine@gmail.com",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     description="mongodb ORM for django framework",
     long_description="mongodb ORM for django framework",
```

