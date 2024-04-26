# Comparing `tmp/aett_postgres-0.9.0.tar.gz` & `tmp/aett_postgres-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_postgres-0.9.0.tar", last modified: Mon Apr 22 13:59:26 2024, max compression
+gzip compressed data, was "aett_postgres-1.0.0.tar", last modified: Fri Apr 26 16:18:55 2024, max compression
```

## Comparing `aett_postgres-0.9.0.tar` & `aett_postgres-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:26.837373 aett_postgres-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 13:59:20.000000 aett_postgres-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 13:59:20.000000 aett_postgres-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-22 13:59:26.837373 aett_postgres-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-22 13:59:20.000000 aett_postgres-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-22 13:59:20.000000 aett_postgres-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:59:26.837373 aett_postgres-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:26.833373 aett_postgres-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:26.833373 aett_postgres-0.9.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:26.833373 aett_postgres-0.9.0/src/aett/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-04-22 13:59:20.000000 aett_postgres-0.9.0/src/aett/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:26.833373 aett_postgres-0.9.0/src/aett_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-22 13:59:26.000000 aett_postgres-0.9.0/src/aett_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-22 13:59:26.000000 aett_postgres-0.9.0/src/aett_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:59:26.000000 aett_postgres-0.9.0/src/aett_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 13:59:26.000000 aett_postgres-0.9.0/src/aett_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 13:59:26.000000 aett_postgres-0.9.0/src/aett_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:55.184433 aett_postgres-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:48.000000 aett_postgres-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:48.000000 aett_postgres-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-26 16:18:55.184433 aett_postgres-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-26 16:18:48.000000 aett_postgres-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-26 16:18:48.000000 aett_postgres-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:55.184433 aett_postgres-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:55.180433 aett_postgres-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:55.180433 aett_postgres-1.0.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:55.180433 aett_postgres-1.0.0/src/aett/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-04-26 16:18:48.000000 aett_postgres-1.0.0/src/aett/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:55.184433 aett_postgres-1.0.0/src/aett_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-26 16:18:55.000000 aett_postgres-1.0.0/src/aett_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-26 16:18:55.000000 aett_postgres-1.0.0/src/aett_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:55.000000 aett_postgres-1.0.0/src/aett_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-26 16:18:55.000000 aett_postgres-1.0.0/src/aett_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:55.000000 aett_postgres-1.0.0/src/aett_postgres.egg-info/top_level.txt
```

### Comparing `aett_postgres-0.9.0/LICENSE` & `aett_postgres-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_postgres-0.9.0/PKG-INFO` & `aett_postgres-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-postgres
-Version: 0.9.0
+Version: 1.0.0
 Summary: Postgres connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: events,event store,postgres
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.9.0
+Requires-Dist: aett-domain>=1.0.0
 Requires-Dist: psycopg-binary~=3.1.18
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_postgres-0.9.0/README.md` & `aett_postgres-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_postgres-0.9.0/pyproject.toml` & `aett_postgres-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-# pyproject.toml
-
 [build-system]
 requires = ["setuptools>=69.1.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.postgres"]
 
 [project]
 name = "aett-postgres"
-version = "0.9.0"
+version = "1.0.0"
 description = "Postgres connector for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "postgres"]
 dependencies = [
-    'aett-domain >= 0.9.0',
+    'aett-domain >= 1.0.0',
     'psycopg-binary~=3.1.18'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
```

### Comparing `aett_postgres-0.9.0/src/aett/postgres/__init__.py` & `aett_postgres-1.0.0/src/aett/postgres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 import jsonpickle
 import psycopg
 
 from aett.domain import ConflictDetector, ConflictingCommitException, NonConflictingCommitException, \
     DuplicateCommitException
 from aett.eventstore import ICommitEvents, IAccessSnapshots, Snapshot, Commit, MAX_INT, TopicMap, \
-    EventMessage
+    EventMessage, COMMITS, SNAPSHOTS
 
 
 # noinspection DuplicatedCode
 class CommitStore(ICommitEvents):
     def __init__(self, db: psycopg.connect, topic_map: TopicMap, conflict_detector: ConflictDetector = None,
-                 table_name='commits'):
+                 table_name=COMMITS):
         self._topic_map = topic_map
         self._connection: psycopg.connect = db
         self._conflict_detector = conflict_detector if conflict_detector is not None else ConflictDetector()
         self._table_name = table_name
 
     def get(self, tenant_id: str, stream_id: str, min_revision: int = 0,
             max_revision: int = MAX_INT) -> typing.Iterable[Commit]:
@@ -149,15 +149,15 @@
 
     @staticmethod
     def _get_body(e):
         return e.body
 
 
 class SnapshotStore(IAccessSnapshots):
-    def __init__(self, db: psycopg.connect, table_name: str = 'snapshots'):
+    def __init__(self, db: psycopg.connect, table_name: str = SNAPSHOTS):
         self.connection: psycopg.connect = db
         self._table_name = table_name
 
     def get(self, tenant_id: str, stream_id: str, max_revision: int = MAX_INT) -> Snapshot | None:
         try:
             cur = self.connection.cursor()
             cur.execute(f"""SELECT *
@@ -198,16 +198,16 @@
             raise Exception(
                 f"Failed to add snapshot for stream {snapshot.stream_id} with error {e}")
 
 
 class PersistenceManagement:
     def __init__(self,
                  db: psycopg.connect,
-                 commits_table_name: str = 'commits',
-                 snapshots_table_name: str = 'snapshots'):
+                 commits_table_name: str = COMMITS,
+                 snapshots_table_name: str = SNAPSHOTS):
         self.db: psycopg.connect = db
         self.commits_table_name = commits_table_name
         self.snapshots_table_name = snapshots_table_name
 
     def initialize(self):
         try:
             c = self.db.cursor()
@@ -237,12 +237,12 @@
     StreamId char(40) NOT NULL,
     StreamRevision int NOT NULL CHECK (StreamRevision > 0),
     Payload bytea NOT NULL,
     Headers bytea NOT NULL,
     CONSTRAINT PK_Snapshots PRIMARY KEY (TenantId, StreamId, StreamRevision)
 );""")
             c.commit()
-        except Exception as e:
+        except Exception:
             pass
 
     def drop(self):
         self.db.cursor().execute(f"""DROP TABLE {self.snapshots_table_name};DROP TABLE {self.commits_table_name};""")
```

### Comparing `aett_postgres-0.9.0/src/aett_postgres.egg-info/PKG-INFO` & `aett_postgres-1.0.0/src/aett_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-postgres
-Version: 0.9.0
+Version: 1.0.0
 Summary: Postgres connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: events,event store,postgres
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.9.0
+Requires-Dist: aett-domain>=1.0.0
 Requires-Dist: psycopg-binary~=3.1.18
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

