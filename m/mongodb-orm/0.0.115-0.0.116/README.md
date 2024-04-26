# Comparing `tmp/mongodb_orm-0.0.115.tar.gz` & `tmp/mongodb_orm-0.0.116.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_orm-0.0.115.tar", last modified: Tue Apr 23 15:22:25 2024, max compression
+gzip compressed data, was "mongodb_orm-0.0.116.tar", last modified: Fri Apr 26 09:30:53 2024, max compression
```

## Comparing `mongodb_orm-0.0.115.tar` & `mongodb_orm-0.0.116.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.431671 mongodb_orm-0.0.115/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-23 15:22:25.430765 mongodb_orm-0.0.115/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.115/README.md
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.410009 mongodb_orm-0.0.115/mongodb_orm/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.115/mongodb_orm/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.115/mongodb_orm/apps.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.414426 mongodb_orm-0.0.115/mongodb_orm/custom_urls/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.115/mongodb_orm/custom_urls/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1530 2024-04-23 15:22:07.000000 mongodb_orm-0.0.115/mongodb_orm/custom_urls/bread_urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.415655 mongodb_orm-0.0.115/mongodb_orm/decorators/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.115/mongodb_orm/decorators/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.115/mongodb_orm/decorators/chained.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.416795 mongodb_orm-0.0.115/mongodb_orm/exceptions/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.115/mongodb_orm/exceptions/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.115/mongodb_orm/exceptions/syntax_exceptions.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.418807 mongodb_orm-0.0.115/mongodb_orm/interfaces/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.115/mongodb_orm/interfaces/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2383 2024-04-23 15:18:03.000000 mongodb_orm-0.0.115/mongodb_orm/interfaces/base_mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7213 2024-04-23 15:18:03.000000 mongodb_orm-0.0.115/mongodb_orm/interfaces/mongodb_model.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.419547 mongodb_orm-0.0.115/mongodb_orm/management/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.115/mongodb_orm/management/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.420679 mongodb_orm-0.0.115/mongodb_orm/management/commands/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.115/mongodb_orm/management/commands/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.0.115/mongodb_orm/management/commands/update_schema.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.421336 mongodb_orm-0.0.115/mongodb_orm/models/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.115/mongodb_orm/models/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.422915 mongodb_orm-0.0.115/mongodb_orm/singletons/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.115/mongodb_orm/singletons/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.115/mongodb_orm/singletons/mongodb_singleton_client.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.426778 mongodb_orm-0.0.115/mongodb_orm/types/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.115/mongodb_orm/types/Relation.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.115/mongodb_orm/types/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.115/mongodb_orm/types/index.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.115/mongodb_orm/types/logger_object.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      453 2024-04-04 10:34:44.000000 mongodb_orm-0.0.115/mongodb_orm/types/model_schema.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.0.115/mongodb_orm/types/options.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      148 2024-04-23 14:22:14.000000 mongodb_orm-0.0.115/mongodb_orm/urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.427845 mongodb_orm-0.0.115/mongodb_orm/utils/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.0.115/mongodb_orm/utils/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1159 2024-04-23 15:18:03.000000 mongodb_orm-0.0.115/mongodb_orm/utils/helpers.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.429117 mongodb_orm-0.0.115/mongodb_orm/views/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.115/mongodb_orm/views/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.115/mongodb_orm/views/mongodb_api_model_view.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:22:25.429838 mongodb_orm-0.0.115/mongodb_orm.egg-info/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-23 15:22:25.000000 mongodb_orm-0.0.115/mongodb_orm.egg-info/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1161 2024-04-23 15:22:25.000000 mongodb_orm-0.0.115/mongodb_orm.egg-info/SOURCES.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-04-23 15:22:25.000000 mongodb_orm-0.0.115/mongodb_orm.egg-info/dependency_links.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-04-23 15:22:25.000000 mongodb_orm-0.0.115/mongodb_orm.egg-info/requires.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-04-23 15:22:25.000000 mongodb_orm-0.0.115/mongodb_orm.egg-info/top_level.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-04-23 15:22:25.431898 mongodb_orm-0.0.115/setup.cfg
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-04-23 15:22:18.000000 mongodb_orm-0.0.115/setup.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.121401 mongodb_orm-0.0.116/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-26 09:30:53.120663 mongodb_orm-0.0.116/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.116/README.md
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.082386 mongodb_orm-0.0.116/mongodb_orm/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.116/mongodb_orm/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.116/mongodb_orm/apps.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.103678 mongodb_orm-0.0.116/mongodb_orm/custom_urls/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.116/mongodb_orm/custom_urls/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1530 2024-04-23 15:22:07.000000 mongodb_orm-0.0.116/mongodb_orm/custom_urls/bread_urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.105065 mongodb_orm-0.0.116/mongodb_orm/decorators/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/decorators/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.116/mongodb_orm/decorators/chained.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.106552 mongodb_orm-0.0.116/mongodb_orm/exceptions/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/exceptions/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.116/mongodb_orm/exceptions/syntax_exceptions.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.108761 mongodb_orm-0.0.116/mongodb_orm/interfaces/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.116/mongodb_orm/interfaces/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2335 2024-04-26 09:29:13.000000 mongodb_orm-0.0.116/mongodb_orm/interfaces/base_mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7213 2024-04-23 15:18:03.000000 mongodb_orm-0.0.116/mongodb_orm/interfaces/mongodb_model.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.109609 mongodb_orm-0.0.116/mongodb_orm/management/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.116/mongodb_orm/management/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.110576 mongodb_orm-0.0.116/mongodb_orm/management/commands/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/management/commands/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.0.116/mongodb_orm/management/commands/update_schema.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.111375 mongodb_orm-0.0.116/mongodb_orm/models/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.116/mongodb_orm/models/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.112165 mongodb_orm-0.0.116/mongodb_orm/singletons/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/singletons/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.116/mongodb_orm/singletons/mongodb_singleton_client.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.116250 mongodb_orm-0.0.116/mongodb_orm/types/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.116/mongodb_orm/types/Relation.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/types/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.116/mongodb_orm/types/index.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.116/mongodb_orm/types/logger_object.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      453 2024-04-04 10:34:44.000000 mongodb_orm-0.0.116/mongodb_orm/types/model_schema.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.0.116/mongodb_orm/types/options.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      148 2024-04-23 14:22:14.000000 mongodb_orm-0.0.116/mongodb_orm/urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.117467 mongodb_orm-0.0.116/mongodb_orm/utils/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.0.116/mongodb_orm/utils/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1159 2024-04-23 15:18:03.000000 mongodb_orm-0.0.116/mongodb_orm/utils/helpers.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.118964 mongodb_orm-0.0.116/mongodb_orm/views/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.116/mongodb_orm/views/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.116/mongodb_orm/views/mongodb_api_model_view.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 09:30:53.119905 mongodb_orm-0.0.116/mongodb_orm.egg-info/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-26 09:30:52.000000 mongodb_orm-0.0.116/mongodb_orm.egg-info/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1161 2024-04-26 09:30:53.000000 mongodb_orm-0.0.116/mongodb_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-04-26 09:30:52.000000 mongodb_orm-0.0.116/mongodb_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-04-26 09:30:52.000000 mongodb_orm-0.0.116/mongodb_orm.egg-info/requires.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-04-26 09:30:52.000000 mongodb_orm-0.0.116/mongodb_orm.egg-info/top_level.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-04-26 09:30:53.121555 mongodb_orm-0.0.116/setup.cfg
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-04-26 09:30:44.000000 mongodb_orm-0.0.116/setup.py
```

### Comparing `mongodb_orm-0.0.115/README.md` & `mongodb_orm-0.0.116/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.115/mongodb_orm/custom_urls/bread_urls.py` & `mongodb_orm-0.0.116/mongodb_orm/custom_urls/bread_urls.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.115/mongodb_orm/interfaces/base_mongodb_model.py` & `mongodb_orm-0.0.116/mongodb_orm/interfaces/base_mongodb_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
             schema = {'$jsonSchema': options['schema']}
         collection = client.create_collection(collection,
                                               timeseries={'timeField': 'created_at',
                                                           'metaField': 'consumed'} if
                                               options.get('time_series') else None,
                                               validator=schema if not options.get('time_series') else None,
                                               expireAfterSeconds=30 if options.get('time_series') else None)
-        if indexes:
-            for index in indexes:
-                collection.create_index([
-                    (index['name'], 1 if index['asc'] else -1)
-                ],
-                    unique=index['unique'] if not options['time_series'] else None,
-                    expireAfterSeconds=index['expireAfterSeconds'] if index['expireAfterSeconds'] else None
-                )
+        for index in indexes:
+            collection.create_index([
+                (index['name'], 1 if index['asc'] else -1)
+            ],
+                unique=index['unique'] if not options['time_series'] else None,
+                expireAfterSeconds=index['expireAfterSeconds'] if index['expireAfterSeconds'] else None
+            )
```

### Comparing `mongodb_orm-0.0.115/mongodb_orm/interfaces/mongodb_model.py` & `mongodb_orm-0.0.116/mongodb_orm/interfaces/mongodb_model.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.115/mongodb_orm/management/commands/update_schema.py` & `mongodb_orm-0.0.116/mongodb_orm/management/commands/update_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.115/mongodb_orm/utils/helpers.py` & `mongodb_orm-0.0.116/mongodb_orm/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.115/mongodb_orm/views/mongodb_api_model_view.py` & `mongodb_orm-0.0.116/mongodb_orm/views/mongodb_api_model_view.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.115/mongodb_orm.egg-info/SOURCES.txt` & `mongodb_orm-0.0.116/mongodb_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.115/setup.py` & `mongodb_orm-0.0.116/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 # Fix and optimise the library installation
 setup(
     name="mongodb_orm",
-    version="0.0.115",
+    version="0.0.116",
     author="Khai",
     author_email="sarraj.khaireddine@gmail.com",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     description="mongodb ORM for django framework",
     long_description="mongodb ORM for django framework",
```

