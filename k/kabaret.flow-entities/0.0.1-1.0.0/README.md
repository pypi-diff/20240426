# Comparing `tmp/kabaret.flow_entities-0.0.1.tar.gz` & `tmp/kabaret_flow_entities-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kabaret.flow_entities-0.0.1.tar", last modified: Tue Mar 30 13:19:21 2021, max compression
+gzip compressed data, was "kabaret_flow_entities-1.0.0.tar", last modified: Fri Apr 26 09:16:32 2024, max compression
```

## Comparing `kabaret.flow_entities-0.0.1.tar` & `kabaret_flow_entities-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/
--rw-rw-rw-   0 root         (0) root         (0)       68 2021-03-30 13:19:11.000000 kabaret.flow_entities-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6768 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4727 2021-03-30 13:19:11.000000 kabaret.flow_entities-0.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      224 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1930 2021-03-30 13:19:11.000000 kabaret.flow_entities-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/src/kabaret/
--rw-rw-rw-   0 root         (0) root         (0)       65 2021-03-30 13:19:11.000000 kabaret.flow_entities-0.0.1/src/kabaret/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/src/kabaret/flow_entities/
--rw-rw-rw-   0 root         (0) root         (0)       93 2021-03-30 13:19:11.000000 kabaret.flow_entities-0.0.1/src/kabaret/flow_entities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/src/kabaret/flow_entities/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4217 2021-03-30 13:19:11.000000 kabaret.flow_entities-0.0.1/src/kabaret/flow_entities/demo.py
--rw-rw-rw-   0 root         (0) root         (0)     8782 2021-03-30 13:19:11.000000 kabaret.flow_entities-0.0.1/src/kabaret/flow_entities/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2484 2021-03-30 13:19:11.000000 kabaret.flow_entities-0.0.1/src/kabaret/flow_entities/store.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2021-03-30 13:19:11.000000 kabaret.flow_entities-0.0.1/src/kabaret/flow_entities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/src/kabaret.flow_entities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6768 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/src/kabaret.flow_entities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      540 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/src/kabaret.flow_entities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/src/kabaret.flow_entities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/src/kabaret.flow_entities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-03-30 13:19:21.000000 kabaret.flow_entities-0.0.1/src/kabaret.flow_entities.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    70144 2021-03-30 13:19:11.000000 kabaret.flow_entities-0.0.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:16:32.749845 kabaret_flow_entities-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      362 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5896 2024-04-26 09:16:32.749845 kabaret_flow_entities-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-04-26 09:16:32.749845 kabaret_flow_entities-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:16:32.744845 kabaret_flow_entities-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:16:32.746845 kabaret_flow_entities-1.0.0/src/kabaret/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/src/kabaret/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:16:32.750845 kabaret_flow_entities-1.0.0/src/kabaret/flow_entities/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/src/kabaret/flow_entities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-26 09:16:32.750845 kabaret_flow_entities-1.0.0/src/kabaret/flow_entities/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4217 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/src/kabaret/flow_entities/demo.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/src/kabaret/flow_entities/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2484 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/src/kabaret/flow_entities/store.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/src/kabaret/flow_entities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:16:32.749845 kabaret_flow_entities-1.0.0/src/kabaret.flow_entities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5896 2024-04-26 09:16:32.000000 kabaret_flow_entities-1.0.0/src/kabaret.flow_entities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      561 2024-04-26 09:16:32.000000 kabaret_flow_entities-1.0.0/src/kabaret.flow_entities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 09:16:32.000000 kabaret_flow_entities-1.0.0/src/kabaret.flow_entities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-26 09:16:32.000000 kabaret_flow_entities-1.0.0/src/kabaret.flow_entities.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-26 09:16:32.000000 kabaret_flow_entities-1.0.0/src/kabaret.flow_entities.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70144 2024-04-26 09:16:22.000000 kabaret_flow_entities-1.0.0/versioneer.py
```

### Comparing `kabaret.flow_entities-0.0.1/PKG-INFO` & `kabaret_flow_entities-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,196 @@
 Metadata-Version: 2.1
 Name: kabaret.flow_entities
-Version: 0.0.1
+Version: 1.0.0
 Summary: A kabaret.flow extension providing searchable large collections of entities.
 Home-page: https://gitlab.com/kabaretstudio/kabaret.flow_entities
 Author: Damien "dee" Coureau
 Author-email: kabaret-dev@googlegroups.com
 License: LGPLv3+
-Description: # kabaret.flow_entities
-        
-        A `kabaret.flow` extension providing searchable large collections of entities, stored in a mongodb.
-        
-        Create your Entities
-        ====================
-        
-        Entities are a queryable collection of objects. 
-        
-        In order to define an entity, you must inherit
-        the `Entity` class and add some `Property` in it:
-        
-        ```python
-        from kabaret.flow_entities.entities import Entity, Property
-        
-        class Asset(Entity):
-        
-            asset_type = Property()
-            asset_family = Property()
-            
-            status = Property()
-        
-        ```
-        
-        You can also add classic relations like `Param` and `Child` and build a whole branch
-        inside your entity. But keep in mind that the `Propery` relations will be the only ones
-        usable in your queries.
-        
-        Once you have an Entity defined, you must use it in an `EntityCollection`:
-        
-        ```python
-        from kabaret.flow_entities.entities import EntityCollection, CreateEntitiesAction, DeleteEntitiesAction
-        
-        class Assets(EntityCollection):
-        
-            # Those actions are provided for convenience,
-            # you will probably want to define your owns:
-            create_assets = flow.Child(CreateEntitiesAction)
-            delete_assets = flow.Child(DeleteEntitiesAction)
-        
-            @classmethod
-            def mapped_type(cls):
-                # This tells which entity is show in 
-                # this collection:
-                return Asset
-        ```
-        
-        When using the `Assets` collection in your flow, the users will see a
-        table with "Asset Type", "Asset Family" and "Status" columns.
-        
-        This table is more efficient than a `kabaret.flow.Map` and can retrieve thousands of items
-        in a fraction of seconds.
-        
-        Still, the `EntityCollection` class inherits `kabaret.flow.DynamicMap` so you can use all the classic
-        customization points (`columns()`, `_fill_row_style()`, etc...).
-        
-        
-        Filter your Entities
-        ====================
-        
-        The `EntityCollection.query_filter()` method can be overidden to return a mongodb filter and
-        restrict the list of displayed entities. You can for example decide to show only the Assets
-        with a "WIP" status:
-        
-        ```python
-        class Assets(EntityCollection):
-        
-            create_assets = flow.Child(CreateEntitiesAction)
-            delete_assets = flow.Child(DeleteEntitiesAction)
-        
-            @classmethod
-            def mapped_type(cls):
-                return Asset
-        
-            def query_filter(self):
-                """
-                Listing only assets with a WIP status
-                """ 
-                return {"status": "WIP"}
-        ```
-        
-        Now you can add some `Action` and `Param` on your collection to control 
-        the returned value of `query_filter()`.
-        
-        Note that only the `Property` relations of your entity can be used 
-        in the filter !
-        
-        The query filter must be a valid argument for a mongodb `collection.find()` call. Here is some documentation about it: https://docs.mongodb.com/manual/tutorial/query-documents/
-        
-        
-        Multiple Entity Views
-        =====================
-        
-        The `EntityCollection.collection_name()` method can be overidden to point
-        to another entity collection. This is usefull if you want to display some
-        entities with a different query filter in different place of your flow.
-        
-        Here is an example of showing only unfinished tasks assigned to the
-        current user from a collection of tasks managed in an `admin` section of the
-        project:
-        
-        ```python
-        
-        class MyTodo(EntityCollection):
-        
-            @classmethod
-            def mapped_type(cls):
-                # be sure to match the source
-                # collection here:
-                return AwesomeTask
-        
-            def collection_name(self):
-                return self.root().project().admin.all_tasks.collection_name()
-            
-            def query_filter(self):
-                return {
-                    "assignee": getpass.getuser(), 
-                    "status": {"$in": ["NYS", "WIP"]},
-                }
-        ```
-        
-        MongoDB Connection
-        ==================
-        
-        The entities are stored as documents in collections of a `mongodb`.
-        
-        In order for your `EntityCollection` to connect to the database, you
-        must add an `EntityStore` somewhere in your project and implement a `get_entity_store()` method on your project's root.
-        
-        A classic aproach is to use an `admin` group in your project:
-        ```python
-        
-        from kabaret.flow_entities.store import EntityStore
-        
-        class Admin(flow.Object):
-        
-            entity_store = flow.Child(EntityStore)
-            
-        class AwesomePipeline(flow.Object):
-        
-            admin = flow.Child(Admin)
-        
-            def get_entity_store(self):
-                return self.admin.entity_store
-        
-        
-        ```
-        
-        The `EntityStore` has an `uri` param that you will need to 
-        set before showing or creating entity. The default value connects to a local mongodb database using the default port and options. Contact your beloved IT support team and ask them the value to use for production.
-        
-        Here is a detailed documentation of the URI syntaxe: https://docs.mongodb.com/manual/reference/connection-string/
-        
-        Demo
-        ====
-        
-        See `kabaret.flow_entities.demo` for more demo code.
-        
-        Create a project with the type `kabaret.flow_entities.demo.EntitiesDemo` to see it in action.
-        
-        
 Keywords: kabaret pipeline dataflow workflow mongodb
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: kabaret>=2.1.5
+Requires-Dist: pymongo
+
+# kabaret.flow_entities
+
+A `kabaret.flow` extension providing searchable large collections of entities, stored in a mongodb.
+
+Create your Entities
+====================
+
+Entities are a queryable collection of objects. 
+
+In order to define an entity, you must inherit
+the `Entity` class and add some `Property` in it:
+
+```python
+from kabaret.flow_entities.entities import Entity, Property
+
+class Asset(Entity):
+
+    asset_type = Property()
+    asset_family = Property()
+    
+    status = Property()
+
+```
+
+You can also add classic relations like `Param` and `Child` and build a whole branch
+inside your entity. But keep in mind that the `Propery` relations will be the only ones
+usable in your queries.
+
+Once you have an Entity defined, you must use it in an `EntityCollection`:
+
+```python
+from kabaret.flow_entities.entities import EntityCollection, CreateEntitiesAction, DeleteEntitiesAction
+
+class Assets(EntityCollection):
+
+    # Those actions are provided for convenience,
+    # you will probably want to define your owns:
+    create_assets = flow.Child(CreateEntitiesAction)
+    delete_assets = flow.Child(DeleteEntitiesAction)
+
+    @classmethod
+    def mapped_type(cls):
+        # This tells which entity is show in 
+        # this collection:
+        return Asset
+```
+
+When using the `Assets` collection in your flow, the users will see a
+table with "Asset Type", "Asset Family" and "Status" columns.
+
+This table is more efficient than a `kabaret.flow.Map` and can retrieve thousands of items
+in a fraction of seconds.
+
+Still, the `EntityCollection` class inherits `kabaret.flow.DynamicMap` so you can use all the classic
+customization points (`columns()`, `_fill_row_style()`, etc...).
+
+
+Filter your Entities
+====================
+
+The `EntityCollection.query_filter()` method can be overidden to return a mongodb filter and
+restrict the list of displayed entities. You can for example decide to show only the Assets
+with a "WIP" status:
+
+```python
+class Assets(EntityCollection):
+
+    create_assets = flow.Child(CreateEntitiesAction)
+    delete_assets = flow.Child(DeleteEntitiesAction)
+
+    @classmethod
+    def mapped_type(cls):
+        return Asset
+
+    def query_filter(self):
+        """
+        Listing only assets with a WIP status
+        """ 
+        return {"status": "WIP"}
+```
+
+Now you can add some `Action` and `Param` on your collection to control 
+the returned value of `query_filter()`.
+
+Note that only the `Property` relations of your entity can be used 
+in the filter !
+
+The query filter must be a valid argument for a mongodb `collection.find()` call. Here is some documentation about it: https://docs.mongodb.com/manual/tutorial/query-documents/
+
+
+Multiple Entity Views
+=====================
+
+The `EntityCollection.collection_name()` method can be overidden to point
+to another entity collection. This is usefull if you want to display some
+entities with a different query filter in different place of your flow.
+
+Here is an example of showing only unfinished tasks assigned to the
+current user from a collection of tasks managed in an `admin` section of the
+project:
+
+```python
+
+class MyTodo(EntityCollection):
+
+    @classmethod
+    def mapped_type(cls):
+        # be sure to match the source
+        # collection here:
+        return AwesomeTask
+
+    def collection_name(self):
+        return self.root().project().admin.all_tasks.collection_name()
+    
+    def query_filter(self):
+        return {
+            "assignee": getpass.getuser(), 
+            "status": {"$in": ["NYS", "WIP"]},
+        }
+```
+
+MongoDB Connection
+==================
+
+The entities are stored as documents in collections of a `mongodb`.
+
+In order for your `EntityCollection` to connect to the database, you
+must add an `EntityStore` somewhere in your project and implement a `get_entity_store()` method on your project's root.
+
+A classic aproach is to use an `admin` group in your project:
+```python
+
+from kabaret.flow_entities.store import EntityStore
+
+class Admin(flow.Object):
+
+    entity_store = flow.Child(EntityStore)
+    
+class AwesomePipeline(flow.Object):
+
+    admin = flow.Child(Admin)
+
+    def get_entity_store(self):
+        return self.admin.entity_store
+
+
+```
+
+The `EntityStore` has an `uri` param that you will need to 
+set before showing or creating entity. The default value connects to a local mongodb database using the default port and options. Contact your beloved IT support team and ask them the value to use for production.
+
+Here is a detailed documentation of the URI syntaxe: https://docs.mongodb.com/manual/reference/connection-string/
+
+Demo
+====
+
+See `kabaret.flow_entities.demo` for more demo code.
+
+Create a project with the type `kabaret.flow_entities.demo.EntitiesDemo` to see it in action.
+
+
+
+# Changelog
+
+## [1.0.0] - 2024-04-26
+
+After 3 years of beta testing of version 0.0.1, this is the long awaited release of version 1.0.0 stable for production.
+
+### Changed
+
+issue #4: Verbose property print : removed annoying print and change it to logger
+
+## [0.0.1] - 2021-03-30
+
+Initial release by Damien Dee Coureau allowing to expand flow entities to Mongo
+
```

### Comparing `kabaret.flow_entities-0.0.1/README.md` & `kabaret_flow_entities-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `kabaret.flow_entities-0.0.1/setup.py` & `kabaret_flow_entities-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from setuptools import setup, find_packages
 import versioneer
 
 readme = os.path.normpath(os.path.join(__file__, "..", "README.md"))
 with open(readme, "r") as fh:
     long_description = fh.read()
 
-# long_description += '\n\n'
-# changelog = os.path.normpath(os.path.join(__file__, '..', 'CHANGELOG.md'))
-# with open(changelog, 'r') as fh:
-#     long_description += fh.read()
+long_description += '\n\n'
+changelog = os.path.normpath(os.path.join(__file__, '..', 'CHANGELOG.md'))
+with open(changelog, 'r') as fh:
+    long_description += fh.read()
 
 
 setup(
     cmdclass=versioneer.get_cmdclass(),
     name="kabaret.flow_entities",
     version=versioneer.get_version(),
     description=(
```

### Comparing `kabaret.flow_entities-0.0.1/src/kabaret/flow_entities/demo.py` & `kabaret_flow_entities-1.0.0/src/kabaret/flow_entities/demo.py`

 * *Files identical despite different names*

### Comparing `kabaret.flow_entities-0.0.1/src/kabaret/flow_entities/entities.py` & `kabaret_flow_entities-1.0.0/src/kabaret/flow_entities/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     def set_property(self, entity_name, property_name, value):
         self.get_entity_store().get_collection(self.collection_name()).update_one(
             {"name": entity_name},
             {"$set": {property_name: value}},
         )
 
     def get_property(self, entity_name, property_name):
-        print("===========>", entity_name, property_name)
+        self.root().session().log_debug(f"===========> {entity_name} {property_name}")
         value = (
             self.get_entity_store()
             .get_collection(self.collection_name())
             .find_one(
                 {"name": entity_name},
                 {property_name: 1},
             )
```

### Comparing `kabaret.flow_entities-0.0.1/src/kabaret/flow_entities/store.py` & `kabaret_flow_entities-1.0.0/src/kabaret/flow_entities/store.py`

 * *Files identical despite different names*

### Comparing `kabaret.flow_entities-0.0.1/src/kabaret/flow_entities/utils.py` & `kabaret_flow_entities-1.0.0/src/kabaret/flow_entities/utils.py`

 * *Files identical despite different names*

### Comparing `kabaret.flow_entities-0.0.1/src/kabaret.flow_entities.egg-info/PKG-INFO` & `kabaret_flow_entities-1.0.0/src/kabaret.flow_entities.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,196 @@
 Metadata-Version: 2.1
-Name: kabaret.flow-entities
-Version: 0.0.1
+Name: kabaret.flow_entities
+Version: 1.0.0
 Summary: A kabaret.flow extension providing searchable large collections of entities.
 Home-page: https://gitlab.com/kabaretstudio/kabaret.flow_entities
 Author: Damien "dee" Coureau
 Author-email: kabaret-dev@googlegroups.com
 License: LGPLv3+
-Description: # kabaret.flow_entities
-        
-        A `kabaret.flow` extension providing searchable large collections of entities, stored in a mongodb.
-        
-        Create your Entities
-        ====================
-        
-        Entities are a queryable collection of objects. 
-        
-        In order to define an entity, you must inherit
-        the `Entity` class and add some `Property` in it:
-        
-        ```python
-        from kabaret.flow_entities.entities import Entity, Property
-        
-        class Asset(Entity):
-        
-            asset_type = Property()
-            asset_family = Property()
-            
-            status = Property()
-        
-        ```
-        
-        You can also add classic relations like `Param` and `Child` and build a whole branch
-        inside your entity. But keep in mind that the `Propery` relations will be the only ones
-        usable in your queries.
-        
-        Once you have an Entity defined, you must use it in an `EntityCollection`:
-        
-        ```python
-        from kabaret.flow_entities.entities import EntityCollection, CreateEntitiesAction, DeleteEntitiesAction
-        
-        class Assets(EntityCollection):
-        
-            # Those actions are provided for convenience,
-            # you will probably want to define your owns:
-            create_assets = flow.Child(CreateEntitiesAction)
-            delete_assets = flow.Child(DeleteEntitiesAction)
-        
-            @classmethod
-            def mapped_type(cls):
-                # This tells which entity is show in 
-                # this collection:
-                return Asset
-        ```
-        
-        When using the `Assets` collection in your flow, the users will see a
-        table with "Asset Type", "Asset Family" and "Status" columns.
-        
-        This table is more efficient than a `kabaret.flow.Map` and can retrieve thousands of items
-        in a fraction of seconds.
-        
-        Still, the `EntityCollection` class inherits `kabaret.flow.DynamicMap` so you can use all the classic
-        customization points (`columns()`, `_fill_row_style()`, etc...).
-        
-        
-        Filter your Entities
-        ====================
-        
-        The `EntityCollection.query_filter()` method can be overidden to return a mongodb filter and
-        restrict the list of displayed entities. You can for example decide to show only the Assets
-        with a "WIP" status:
-        
-        ```python
-        class Assets(EntityCollection):
-        
-            create_assets = flow.Child(CreateEntitiesAction)
-            delete_assets = flow.Child(DeleteEntitiesAction)
-        
-            @classmethod
-            def mapped_type(cls):
-                return Asset
-        
-            def query_filter(self):
-                """
-                Listing only assets with a WIP status
-                """ 
-                return {"status": "WIP"}
-        ```
-        
-        Now you can add some `Action` and `Param` on your collection to control 
-        the returned value of `query_filter()`.
-        
-        Note that only the `Property` relations of your entity can be used 
-        in the filter !
-        
-        The query filter must be a valid argument for a mongodb `collection.find()` call. Here is some documentation about it: https://docs.mongodb.com/manual/tutorial/query-documents/
-        
-        
-        Multiple Entity Views
-        =====================
-        
-        The `EntityCollection.collection_name()` method can be overidden to point
-        to another entity collection. This is usefull if you want to display some
-        entities with a different query filter in different place of your flow.
-        
-        Here is an example of showing only unfinished tasks assigned to the
-        current user from a collection of tasks managed in an `admin` section of the
-        project:
-        
-        ```python
-        
-        class MyTodo(EntityCollection):
-        
-            @classmethod
-            def mapped_type(cls):
-                # be sure to match the source
-                # collection here:
-                return AwesomeTask
-        
-            def collection_name(self):
-                return self.root().project().admin.all_tasks.collection_name()
-            
-            def query_filter(self):
-                return {
-                    "assignee": getpass.getuser(), 
-                    "status": {"$in": ["NYS", "WIP"]},
-                }
-        ```
-        
-        MongoDB Connection
-        ==================
-        
-        The entities are stored as documents in collections of a `mongodb`.
-        
-        In order for your `EntityCollection` to connect to the database, you
-        must add an `EntityStore` somewhere in your project and implement a `get_entity_store()` method on your project's root.
-        
-        A classic aproach is to use an `admin` group in your project:
-        ```python
-        
-        from kabaret.flow_entities.store import EntityStore
-        
-        class Admin(flow.Object):
-        
-            entity_store = flow.Child(EntityStore)
-            
-        class AwesomePipeline(flow.Object):
-        
-            admin = flow.Child(Admin)
-        
-            def get_entity_store(self):
-                return self.admin.entity_store
-        
-        
-        ```
-        
-        The `EntityStore` has an `uri` param that you will need to 
-        set before showing or creating entity. The default value connects to a local mongodb database using the default port and options. Contact your beloved IT support team and ask them the value to use for production.
-        
-        Here is a detailed documentation of the URI syntaxe: https://docs.mongodb.com/manual/reference/connection-string/
-        
-        Demo
-        ====
-        
-        See `kabaret.flow_entities.demo` for more demo code.
-        
-        Create a project with the type `kabaret.flow_entities.demo.EntitiesDemo` to see it in action.
-        
-        
 Keywords: kabaret pipeline dataflow workflow mongodb
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: kabaret>=2.1.5
+Requires-Dist: pymongo
+
+# kabaret.flow_entities
+
+A `kabaret.flow` extension providing searchable large collections of entities, stored in a mongodb.
+
+Create your Entities
+====================
+
+Entities are a queryable collection of objects. 
+
+In order to define an entity, you must inherit
+the `Entity` class and add some `Property` in it:
+
+```python
+from kabaret.flow_entities.entities import Entity, Property
+
+class Asset(Entity):
+
+    asset_type = Property()
+    asset_family = Property()
+    
+    status = Property()
+
+```
+
+You can also add classic relations like `Param` and `Child` and build a whole branch
+inside your entity. But keep in mind that the `Propery` relations will be the only ones
+usable in your queries.
+
+Once you have an Entity defined, you must use it in an `EntityCollection`:
+
+```python
+from kabaret.flow_entities.entities import EntityCollection, CreateEntitiesAction, DeleteEntitiesAction
+
+class Assets(EntityCollection):
+
+    # Those actions are provided for convenience,
+    # you will probably want to define your owns:
+    create_assets = flow.Child(CreateEntitiesAction)
+    delete_assets = flow.Child(DeleteEntitiesAction)
+
+    @classmethod
+    def mapped_type(cls):
+        # This tells which entity is show in 
+        # this collection:
+        return Asset
+```
+
+When using the `Assets` collection in your flow, the users will see a
+table with "Asset Type", "Asset Family" and "Status" columns.
+
+This table is more efficient than a `kabaret.flow.Map` and can retrieve thousands of items
+in a fraction of seconds.
+
+Still, the `EntityCollection` class inherits `kabaret.flow.DynamicMap` so you can use all the classic
+customization points (`columns()`, `_fill_row_style()`, etc...).
+
+
+Filter your Entities
+====================
+
+The `EntityCollection.query_filter()` method can be overidden to return a mongodb filter and
+restrict the list of displayed entities. You can for example decide to show only the Assets
+with a "WIP" status:
+
+```python
+class Assets(EntityCollection):
+
+    create_assets = flow.Child(CreateEntitiesAction)
+    delete_assets = flow.Child(DeleteEntitiesAction)
+
+    @classmethod
+    def mapped_type(cls):
+        return Asset
+
+    def query_filter(self):
+        """
+        Listing only assets with a WIP status
+        """ 
+        return {"status": "WIP"}
+```
+
+Now you can add some `Action` and `Param` on your collection to control 
+the returned value of `query_filter()`.
+
+Note that only the `Property` relations of your entity can be used 
+in the filter !
+
+The query filter must be a valid argument for a mongodb `collection.find()` call. Here is some documentation about it: https://docs.mongodb.com/manual/tutorial/query-documents/
+
+
+Multiple Entity Views
+=====================
+
+The `EntityCollection.collection_name()` method can be overidden to point
+to another entity collection. This is usefull if you want to display some
+entities with a different query filter in different place of your flow.
+
+Here is an example of showing only unfinished tasks assigned to the
+current user from a collection of tasks managed in an `admin` section of the
+project:
+
+```python
+
+class MyTodo(EntityCollection):
+
+    @classmethod
+    def mapped_type(cls):
+        # be sure to match the source
+        # collection here:
+        return AwesomeTask
+
+    def collection_name(self):
+        return self.root().project().admin.all_tasks.collection_name()
+    
+    def query_filter(self):
+        return {
+            "assignee": getpass.getuser(), 
+            "status": {"$in": ["NYS", "WIP"]},
+        }
+```
+
+MongoDB Connection
+==================
+
+The entities are stored as documents in collections of a `mongodb`.
+
+In order for your `EntityCollection` to connect to the database, you
+must add an `EntityStore` somewhere in your project and implement a `get_entity_store()` method on your project's root.
+
+A classic aproach is to use an `admin` group in your project:
+```python
+
+from kabaret.flow_entities.store import EntityStore
+
+class Admin(flow.Object):
+
+    entity_store = flow.Child(EntityStore)
+    
+class AwesomePipeline(flow.Object):
+
+    admin = flow.Child(Admin)
+
+    def get_entity_store(self):
+        return self.admin.entity_store
+
+
+```
+
+The `EntityStore` has an `uri` param that you will need to 
+set before showing or creating entity. The default value connects to a local mongodb database using the default port and options. Contact your beloved IT support team and ask them the value to use for production.
+
+Here is a detailed documentation of the URI syntaxe: https://docs.mongodb.com/manual/reference/connection-string/
+
+Demo
+====
+
+See `kabaret.flow_entities.demo` for more demo code.
+
+Create a project with the type `kabaret.flow_entities.demo.EntitiesDemo` to see it in action.
+
+
+
+# Changelog
+
+## [1.0.0] - 2024-04-26
+
+After 3 years of beta testing of version 0.0.1, this is the long awaited release of version 1.0.0 stable for production.
+
+### Changed
+
+issue #4: Verbose property print : removed annoying print and change it to logger
+
+## [0.0.1] - 2021-03-30
+
+Initial release by Damien Dee Coureau allowing to expand flow entities to Mongo
+
```

### Comparing `kabaret.flow_entities-0.0.1/src/kabaret.flow_entities.egg-info/SOURCES.txt` & `kabaret_flow_entities-1.0.0/src/kabaret.flow_entities.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+CHANGELOG.md
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 src/kabaret/__init__.py
 src/kabaret.flow_entities.egg-info/PKG-INFO
```

### Comparing `kabaret.flow_entities-0.0.1/versioneer.py` & `kabaret_flow_entities-1.0.0/versioneer.py`

 * *Files identical despite different names*

