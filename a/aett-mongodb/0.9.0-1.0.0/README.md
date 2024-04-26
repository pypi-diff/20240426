# Comparing `tmp/aett_mongodb-0.9.0.tar.gz` & `tmp/aett_mongodb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_mongodb-0.9.0.tar", last modified: Mon Apr 22 13:59:32 2024, max compression
+gzip compressed data, was "aett_mongodb-1.0.0.tar", last modified: Fri Apr 26 16:18:53 2024, max compression
```

## Comparing `aett_mongodb-0.9.0.tar` & `aett_mongodb-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:32.645732 aett_mongodb-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 13:59:23.000000 aett_mongodb-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 13:59:23.000000 aett_mongodb-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-22 13:59:32.645732 aett_mongodb-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 13:59:23.000000 aett_mongodb-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-22 13:59:23.000000 aett_mongodb-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:59:32.645732 aett_mongodb-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:32.641733 aett_mongodb-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:32.641733 aett_mongodb-0.9.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:32.641733 aett_mongodb-0.9.0/src/aett/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-22 13:59:23.000000 aett_mongodb-0.9.0/src/aett/mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:32.645732 aett_mongodb-0.9.0/src/aett_mongodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-22 13:59:32.000000 aett_mongodb-0.9.0/src/aett_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 13:59:32.000000 aett_mongodb-0.9.0/src/aett_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:59:32.000000 aett_mongodb-0.9.0/src/aett_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 13:59:32.000000 aett_mongodb-0.9.0/src/aett_mongodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 13:59:32.000000 aett_mongodb-0.9.0/src/aett_mongodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:47.000000 aett_mongodb-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:47.000000 aett_mongodb-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 16:18:47.000000 aett_mongodb-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-26 16:18:47.000000 aett_mongodb-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/src/aett/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-04-26 16:18:47.000000 aett_mongodb-1.0.0/src/aett/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.108583 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-26 16:18:53.000000 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-26 16:18:53.000000 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:53.000000 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 16:18:53.000000 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:53.000000 aett_mongodb-1.0.0/src/aett_mongodb.egg-info/top_level.txt
```

### Comparing `aett_mongodb-0.9.0/LICENSE` & `aett_mongodb-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_mongodb-0.9.0/PKG-INFO` & `aett_mongodb-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-mongodb
-Version: 0.9.0
+Version: 1.0.0
 Summary: MongoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,16 @@
 Keywords: events,event store,mongo,mongodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.9.0
-Requires-Dist: pymongo~=4.6.2
+Requires-Dist: aett-domain>=1.0.0
+Requires-Dist: pymongo~=4.6.3
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_mongodb-0.9.0/README.md` & `aett_mongodb-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_mongodb-0.9.0/pyproject.toml` & `aett_mongodb-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-# pyproject.toml
-
 [build-system]
-requires = ["setuptools>=69.1.1", "wheel"]
+requires = ["setuptools>=69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.mongodb"]
 
 [project]
 name = "aett-mongodb"
-version = "0.9.0"
+version = "1.0.0"
 description = "MongoDB connector for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "mongo", "mongodb"]
 dependencies = [
-    'aett-domain >= 0.9.0',
-    'pymongo~=4.6.2'
+    'aett-domain >= 1.0.0',
+    'pymongo~=4.6.3'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
```

### Comparing `aett_mongodb-0.9.0/src/aett/mongodb/__init__.py` & `aett_mongodb-1.0.0/src/aett/mongodb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 import jsonpickle
 import pymongo
 from pymongo import database, results, errors
 
 from aett.domain import ConflictingCommitException, NonConflictingCommitException, ConflictDetector
 from aett.eventstore import ICommitEvents, IAccessSnapshots, Snapshot, Commit, MAX_INT, EventMessage, \
-    TopicMap
+    TopicMap, COMMITS, SNAPSHOTS
 
 
 # noinspection DuplicatedCode
 class CommitStore(ICommitEvents):
     def __init__(self, db: database.Database, topic_map: TopicMap, conflict_detector: ConflictDetector = None,
-                 table_name='commits'):
+                 table_name=COMMITS):
         self._topic_map = topic_map
         self._collection: database.Collection = db.get_collection(table_name)
         self._counters_collection: database.Collection = db.get_collection('counters')
         self._conflict_detector = conflict_detector if conflict_detector is not None else ConflictDetector()
 
     def get(self, tenant_id: str, stream_id: str, min_revision: int = 0,
             max_revision: int = MAX_INT) -> typing.Iterable[Commit]:
@@ -123,15 +123,15 @@
 
     @staticmethod
     def _get_body(e):
         return e.body
 
 
 class SnapshotStore(IAccessSnapshots):
-    def __init__(self, db: database.Database, table_name: str = 'snapshots'):
+    def __init__(self, db: database.Database, table_name: str = SNAPSHOTS):
         self.collection: database.Collection = db.get_collection(table_name)
 
     def get(self, tenant_id: str, stream_id: str, max_revision: int = MAX_INT) -> Snapshot | None:
         try:
             item = self.collection.find_one(
                 {'TenantId': tenant_id, 'StreamId': stream_id, 'StreamRevision': max_revision})
             if item is None:
@@ -162,16 +162,16 @@
             raise Exception(
                 f"Failed to add snapshot for stream {snapshot.stream_id} with status code {e.response['ResponseMetadata']['HTTPStatusCode']}")
 
 
 class PersistenceManagement:
     def __init__(self,
                  db: database.Database,
-                 commits_table_name: str = 'commits',
-                 snapshots_table_name: str = 'snapshots'):
+                 commits_table_name: str = COMMITS,
+                 snapshots_table_name: str = SNAPSHOTS):
         self.db: database.Database = db
         self.commits_table_name = commits_table_name
         self.snapshots_table_name = snapshots_table_name
 
     def initialize(self):
         try:
             counters_collection: database.Collection = self.db.create_collection('counters', check_exists=True)
```

### Comparing `aett_mongodb-0.9.0/src/aett_mongodb.egg-info/PKG-INFO` & `aett_mongodb-1.0.0/src/aett_mongodb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-mongodb
-Version: 0.9.0
+Version: 1.0.0
 Summary: MongoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,16 @@
 Keywords: events,event store,mongo,mongodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.9.0
-Requires-Dist: pymongo~=4.6.2
+Requires-Dist: aett-domain>=1.0.0
+Requires-Dist: pymongo~=4.6.3
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

