# Comparing `tmp/aett_dynamodb-0.9.0.tar.gz` & `tmp/aett_dynamodb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_dynamodb-0.9.0.tar", last modified: Mon Apr 22 13:59:25 2024, max compression
+gzip compressed data, was "aett_dynamodb-1.0.0.tar", last modified: Fri Apr 26 16:18:54 2024, max compression
```

## Comparing `aett_dynamodb-0.9.0.tar` & `aett_dynamodb-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:25.276361 aett_dynamodb-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 13:59:16.000000 aett_dynamodb-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 13:59:16.000000 aett_dynamodb-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-22 13:59:25.276361 aett_dynamodb-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-22 13:59:16.000000 aett_dynamodb-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-22 13:59:16.000000 aett_dynamodb-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:59:25.276361 aett_dynamodb-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:25.272361 aett_dynamodb-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:25.272361 aett_dynamodb-0.9.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:25.272361 aett_dynamodb-0.9.0/src/aett/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-22 13:59:16.000000 aett_dynamodb-0.9.0/src/aett/dynamodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:25.272361 aett_dynamodb-0.9.0/src/aett_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-22 13:59:25.000000 aett_dynamodb-0.9.0/src/aett_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-22 13:59:25.000000 aett_dynamodb-0.9.0/src/aett_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:59:25.000000 aett_dynamodb-0.9.0/src/aett_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 13:59:25.000000 aett_dynamodb-0.9.0/src/aett_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 13:59:25.000000 aett_dynamodb-0.9.0/src/aett_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:54.491484 aett_dynamodb-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:46.000000 aett_dynamodb-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:46.000000 aett_dynamodb-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-26 16:18:54.491484 aett_dynamodb-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-26 16:18:46.000000 aett_dynamodb-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-26 16:18:46.000000 aett_dynamodb-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:54.491484 aett_dynamodb-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:54.487485 aett_dynamodb-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:54.487485 aett_dynamodb-1.0.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:54.487485 aett_dynamodb-1.0.0/src/aett/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-26 16:18:46.000000 aett_dynamodb-1.0.0/src/aett/dynamodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:54.487485 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-26 16:18:54.000000 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-26 16:18:54.000000 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:54.000000 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 16:18:54.000000 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:54.000000 aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/top_level.txt
```

### Comparing `aett_dynamodb-0.9.0/LICENSE` & `aett_dynamodb-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_dynamodb-0.9.0/PKG-INFO` & `aett_dynamodb-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-dynamodb
-Version: 0.9.0
+Version: 1.0.0
 Summary: DynamoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: events,event store,dynamodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.9.0
+Requires-Dist: aett-domain>=1.0.0
 Requires-Dist: boto3[crt]~=1.34.88
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_dynamodb-0.9.0/README.md` & `aett_dynamodb-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_dynamodb-0.9.0/pyproject.toml` & `aett_dynamodb-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-# pyproject.toml
-
 [build-system]
-requires = ["setuptools>=69.1.1", "wheel"]
+requires = ["setuptools>=69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.dynamodb"]
 
 [project]
 name = "aett-dynamodb"
-version = "0.9.0"
+version = "1.0.0"
 description = "DynamoDB connector for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "dynamodb"]
 dependencies = [
-    'aett-domain >= 0.9.0',
+    'aett-domain >= 1.0.0',
     'boto3[crt]~=1.34.88'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
```

### Comparing `aett_dynamodb-0.9.0/src/aett/dynamodb/__init__.py` & `aett_dynamodb-1.0.0/src/aett/dynamodb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 import boto3
 import jsonpickle
 from boto3.dynamodb.conditions import Key, Attr
 
 from aett.domain import ConflictDetector, ConflictingCommitException, NonConflictingCommitException, \
     DuplicateCommitException
 from aett.eventstore import ICommitEvents, IAccessSnapshots, Snapshot, Commit, MAX_INT, EventMessage, \
-    TopicMap
+    TopicMap, COMMITS, SNAPSHOTS
 
 
-def _get_resource(region: str):
-    return boto3.resource('dynamodb',
-                          region_name=region,
-                          endpoint_url='http://localhost:8000' if region == 'localhost' else None)
+def _get_resource(profile_name: str, region: str):
+    session = boto3.Session(profile_name=profile_name)
+    return session.resource('dynamodb',
+                            region_name=region,
+                            endpoint_url='http://localhost:8000' if region == 'localhost' else None)
 
 
 class CommitStore(ICommitEvents):
-    def __init__(self, topic_map: TopicMap, conflict_detector: ConflictDetector = None, table_name: str = 'commits',
-                 region: str = 'eu-central-1'):
+    def __init__(self, topic_map: TopicMap, conflict_detector: ConflictDetector = None, table_name: str = COMMITS,
+                 region: str = 'eu-central-1', profile_name: str = 'default'):
         self._topic_map = topic_map
         self._table_name = table_name
         self._region = region
-        self._dynamodb = _get_resource(region)
+        self._dynamodb = _get_resource(profile_name=profile_name, region=region)
         self.table = self._dynamodb.Table(table_name)
         self._conflict_detector: ConflictDetector = conflict_detector if conflict_detector is not None \
             else ConflictDetector()
 
     def get(self, tenant_id: str, stream_id: str, min_revision: int = 0,
             max_revision: int = MAX_INT) -> typing.Iterable[Commit]:
         max_revision = MAX_INT if max_revision >= MAX_INT else max_revision + 1
@@ -151,16 +152,16 @@
 
     @staticmethod
     def _get_body(em: EventMessage):
         return em.body
 
 
 class SnapshotStore(IAccessSnapshots):
-    def __init__(self, table_name: str = 'snapshots', region: str = 'eu-central-1'):
-        self.dynamodb = _get_resource(region)
+    def __init__(self, table_name: str = SNAPSHOTS, region: str = 'eu-central-1', profile_name: str = 'default'):
+        self.dynamodb = _get_resource(profile_name=profile_name, region=region)
         self.table = self.dynamodb.Table(table_name)
         self.table_name = table_name
 
     def get(self, tenant_id: str, stream_id: str, max_revision: int = MAX_INT) -> Snapshot | None:
         try:
             query_response = self.table.query(
                 TableName=self.table_name,
@@ -204,18 +205,19 @@
         except Exception as e:
             raise Exception(
                 f"Failed to add snapshot for stream {snapshot.stream_id} with status code {e.response['ResponseMetadata']['HTTPStatusCode']}")
 
 
 class PersistenceManagement:
     def __init__(self,
-                 commits_table_name: str = 'commits',
-                 snapshots_table_name: str = 'snapshots',
-                 region: str = 'eu-central-1'):
-        self.dynamodb = _get_resource(region)
+                 commits_table_name: str = COMMITS,
+                 snapshots_table_name: str = SNAPSHOTS,
+                 region: str = 'eu-central-1',
+                 profile_name='default'):
+        self.dynamodb = _get_resource(profile_name, region)
         self.commits_table_name = commits_table_name
         self.snapshots_table_name = snapshots_table_name
 
     def initialize(self):
         tables = self.dynamodb.tables.all()
         table_names = [table.name for table in tables]
         if self.commits_table_name not in table_names:
```

### Comparing `aett_dynamodb-0.9.0/src/aett_dynamodb.egg-info/PKG-INFO` & `aett_dynamodb-1.0.0/src/aett_dynamodb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-dynamodb
-Version: 0.9.0
+Version: 1.0.0
 Summary: DynamoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: events,event store,dynamodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.9.0
+Requires-Dist: aett-domain>=1.0.0
 Requires-Dist: boto3[crt]~=1.34.88
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

