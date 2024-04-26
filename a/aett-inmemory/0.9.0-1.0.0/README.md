# Comparing `tmp/aett_inmemory-0.9.0.tar.gz` & `tmp/aett_inmemory-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_inmemory-0.9.0.tar", last modified: Mon Apr 22 13:59:24 2024, max compression
+gzip compressed data, was "aett_inmemory-1.0.0.tar", last modified: Fri Apr 26 16:18:50 2024, max compression
```

## Comparing `aett_inmemory-0.9.0.tar` & `aett_inmemory-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:24.276818 aett_inmemory-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 13:59:18.000000 aett_inmemory-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 13:59:18.000000 aett_inmemory-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-22 13:59:24.276818 aett_inmemory-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-22 13:59:18.000000 aett_inmemory-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-22 13:59:18.000000 aett_inmemory-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:59:24.276818 aett_inmemory-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:24.272817 aett_inmemory-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:24.272817 aett_inmemory-0.9.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:24.276818 aett_inmemory-0.9.0/src/aett/inmemory/
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-22 13:59:18.000000 aett_inmemory-0.9.0/src/aett/inmemory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:24.276818 aett_inmemory-0.9.0/src/aett_inmemory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-22 13:59:24.000000 aett_inmemory-0.9.0/src/aett_inmemory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-22 13:59:24.000000 aett_inmemory-0.9.0/src/aett_inmemory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:59:24.000000 aett_inmemory-0.9.0/src/aett_inmemory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 13:59:24.000000 aett_inmemory-0.9.0/src/aett_inmemory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 13:59:24.000000 aett_inmemory-0.9.0/src/aett_inmemory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.274976 aett_inmemory-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:44.000000 aett_inmemory-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:44.000000 aett_inmemory-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-26 16:18:50.274976 aett_inmemory-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-26 16:18:44.000000 aett_inmemory-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-26 16:18:44.000000 aett_inmemory-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:50.274976 aett_inmemory-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.270976 aett_inmemory-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.270976 aett_inmemory-1.0.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.274976 aett_inmemory-1.0.0/src/aett/inmemory/
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-26 16:18:44.000000 aett_inmemory-1.0.0/src/aett/inmemory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.274976 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-26 16:18:50.000000 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-26 16:18:50.000000 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:50.000000 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 16:18:50.000000 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:50.000000 aett_inmemory-1.0.0/src/aett_inmemory.egg-info/top_level.txt
```

### Comparing `aett_inmemory-0.9.0/LICENSE` & `aett_inmemory-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_inmemory-0.9.0/PKG-INFO` & `aett_inmemory-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-inmemory
-Version: 0.9.0
+Version: 1.0.0
 Summary: In-Memory persistence for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: events,event store,s3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.9.0
+Requires-Dist: aett-domain>=1.0.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_inmemory-0.9.0/README.md` & `aett_inmemory-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_inmemory-0.9.0/pyproject.toml` & `aett_inmemory-1.0.0/pyproject.toml`

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
 include = ["aett.inmemory"]
 
 [project]
 name = "aett-inmemory"
-version = "0.9.0"
+version = "1.0.0"
 description = "In-Memory persistence for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "s3"]
 dependencies = [
-    'aett-domain >= 0.9.0'
+    'aett-domain >= 1.0.0'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
```

### Comparing `aett_inmemory-0.9.0/src/aett/inmemory/__init__.py` & `aett_inmemory-1.0.0/src/aett/inmemory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     ConflictDetector
 from aett.eventstore import ICommitEvents, IAccessSnapshots, Snapshot, Commit, MAX_INT, EventMessage
 
 
 class CommitStore(ICommitEvents):
     def __init__(self, conflict_detector: ConflictDetector = None):
         self._buckets: typing.Dict[str, typing.Dict[str, typing.List[Commit]]] = {}
-        self._conflict_detector: ConflictDetector = conflict_detector if conflict_detector is not None else ConflictDetector()
+        self._conflict_detector: ConflictDetector = \
+            conflict_detector if conflict_detector is not None else ConflictDetector()
 
     def get(self, tenant_id: str, stream_id: str, min_revision: int = 0,
             max_revision: int = MAX_INT) -> typing.Iterable[Commit]:
         if not self._ensure_stream(tenant_id=tenant_id, stream_id=stream_id):
             return []
         max_revision = MAX_INT if max_revision >= MAX_INT else max_revision
         min_revision = 0 if min_revision < 0 else min_revision
```

### Comparing `aett_inmemory-0.9.0/src/aett_inmemory.egg-info/PKG-INFO` & `aett_inmemory-1.0.0/src/aett_inmemory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-inmemory
-Version: 0.9.0
+Version: 1.0.0
 Summary: In-Memory persistence for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: events,event store,s3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.9.0
+Requires-Dist: aett-domain>=1.0.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

