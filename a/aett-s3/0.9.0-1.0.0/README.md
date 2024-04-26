# Comparing `tmp/aett_s3-0.9.0.tar.gz` & `tmp/aett_s3-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_s3-0.9.0.tar", last modified: Mon Apr 22 13:59:25 2024, max compression
+gzip compressed data, was "aett_s3-1.0.0.tar", last modified: Fri Apr 26 16:18:50 2024, max compression
```

## Comparing `aett_s3-0.9.0.tar` & `aett_s3-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:25.556922 aett_s3-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 13:59:19.000000 aett_s3-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 13:59:19.000000 aett_s3-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-22 13:59:25.556922 aett_s3-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-22 13:59:19.000000 aett_s3-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-22 13:59:19.000000 aett_s3-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:59:25.556922 aett_s3-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:25.552922 aett_s3-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:25.552922 aett_s3-0.9.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:25.552922 aett_s3-0.9.0/src/aett/s3/
--rw-r--r--   0 runner    (1001) docker     (127)     9259 2024-04-22 13:59:19.000000 aett_s3-0.9.0/src/aett/s3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:25.552922 aett_s3-0.9.0/src/aett_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-22 13:59:25.000000 aett_s3-0.9.0/src/aett_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-22 13:59:25.000000 aett_s3-0.9.0/src/aett_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:59:25.000000 aett_s3-0.9.0/src/aett_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 13:59:25.000000 aett_s3-0.9.0/src/aett_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 13:59:25.000000 aett_s3-0.9.0/src/aett_s3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.171749 aett_s3-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:44.000000 aett_s3-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:44.000000 aett_s3-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-26 16:18:50.171749 aett_s3-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-26 16:18:44.000000 aett_s3-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-26 16:18:44.000000 aett_s3-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:50.171749 aett_s3-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.167749 aett_s3-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.167749 aett_s3-1.0.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.171749 aett_s3-1.0.0/src/aett/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-26 16:18:44.000000 aett_s3-1.0.0/src/aett/s3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:50.171749 aett_s3-1.0.0/src/aett_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-26 16:18:50.000000 aett_s3-1.0.0/src/aett_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-26 16:18:50.000000 aett_s3-1.0.0/src/aett_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:50.000000 aett_s3-1.0.0/src/aett_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 16:18:50.000000 aett_s3-1.0.0/src/aett_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:50.000000 aett_s3-1.0.0/src/aett_s3.egg-info/top_level.txt
```

### Comparing `aett_s3-0.9.0/LICENSE` & `aett_s3-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_s3-0.9.0/PKG-INFO` & `aett_s3-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-s3
-Version: 0.9.0
+Version: 1.0.0
 Summary: S3 connector for aett event store
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
 Requires-Dist: boto3[crt]~=1.34.79
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_s3-0.9.0/README.md` & `aett_s3-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_s3-0.9.0/pyproject.toml` & `aett_s3-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-# pyproject.toml
-
 [build-system]
 requires = ["setuptools>=69.1.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.s3"]
 
 [project]
 name = "aett-s3"
-version = "0.9.0"
+version = "1.0.0"
 description = "S3 connector for aett event store"
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
-    'aett-domain >= 0.9.0',
+    'aett-domain >= 1.0.0',
     'boto3[crt]~=1.34.79'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
```

### Comparing `aett_s3-0.9.0/src/aett/s3/__init__.py` & `aett_s3-1.0.0/src/aett/s3/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,36 +4,57 @@
 from aett.domain import *
 from aett.eventstore import *
 
 
 class S3Config:
     def __init__(self, bucket: str, aws_access_key_id: str = None, aws_secret_access_key: str = None,
                  aws_session_token: str = None,
-                 region: str = 'us-east-1', endpoint_url: str = None, use_tls: bool = True):
-        self.aws_session_token = aws_session_token
-        self.aws_secret_access_key = aws_secret_access_key
-        self.aws_access_key_id: str = aws_access_key_id
-        self.use_tls = use_tls
+                 region: str = 'us-east-1', endpoint_url: str = None, use_tls: bool = True,
+                 profile_name: str = 'default'):
+        """
+        Defines the configuration for the S3 client.
+        If a profile name is provided, the access key id and secret access are disregarded and the profile credentials are used.
+
+        :param bucket: The name of the bucket
+        :param aws_access_key_id: The AWS access key id
+        :param aws_secret_access_key: The AWS secret access key
+        :param aws_session_token: The AWS session token
+        :param region: The AWS region
+        :param endpoint_url: The endpoint URL
+        :param use_tls: Whether to use TLS
+        :param profile_name: The profile name
+        """
+        self._aws_session_token = aws_session_token
+        self._aws_secret_access_key = aws_secret_access_key
+        self._aws_access_key_id: str = aws_access_key_id
+        self._use_tls = use_tls
         self.bucket = bucket
-        self.region = region
-        self.endpoint_url = endpoint_url
+        self._region = region
+        self._endpoint_url = endpoint_url
+        self._profile_name = profile_name
 
     def to_client(self):
+        if self._profile_name != '':
+            session = boto3.Session(profile_name=self._profile_name)
+            return session.client(service_name='s3',
+                                  region_name=self._region,
+                                  endpoint_url=self._endpoint_url,
+                                  verify=self._use_tls)
         return boto3.client('s3',
-                            aws_access_key_id=self.aws_access_key_id,
-                            aws_secret_access_key=self.aws_secret_access_key,
-                            aws_session_token=self.aws_session_token,
-                            region_name=self.region,
-                            endpoint_url=self.endpoint_url,
-                            verify=self.use_tls)
+                            aws_access_key_id=self._aws_access_key_id,
+                            aws_secret_access_key=self._aws_secret_access_key,
+                            aws_session_token=self._aws_session_token,
+                            region_name=self._region,
+                            endpoint_url=self._endpoint_url,
+                            verify=self._use_tls)
 
 
 class CommitStore(ICommitEvents):
     def __init__(self, s3_config: S3Config, topic_map: TopicMap, conflict_detector: ConflictDetector = None,
-                 folder_name='commits'):
+                 folder_name=COMMITS):
         self._s3_bucket = s3_config.bucket
         self._topic_map = topic_map
         self._resource: client = s3_config.to_client()
         self._conflict_detector = conflict_detector
         self._folder_name = folder_name
 
     def get(self, tenant_id: str, stream_id: str, min_revision: int = 0,
@@ -135,15 +156,15 @@
 
     @staticmethod
     def _get_body(em: EventMessage):
         return em.body
 
 
 class SnapshotStore(IAccessSnapshots):
-    def __init__(self, s3_config: S3Config, folder_name: str = 'snapshots'):
+    def __init__(self, s3_config: S3Config, folder_name: str = SNAPSHOTS):
         self._s3_bucket = s3_config.bucket
         self._folder_name = folder_name
         self._resource: client = s3_config.to_client()
 
     def get(self, tenant_id: str, stream_id: str, max_revision: int = MAX_INT) -> Snapshot | None:
         files = self._resource.list_objects(Bucket=self._s3_bucket,
                                             Delimiter='/',
```

### Comparing `aett_s3-0.9.0/src/aett_s3.egg-info/PKG-INFO` & `aett_s3-1.0.0/src/aett_s3.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-s3
-Version: 0.9.0
+Version: 1.0.0
 Summary: S3 connector for aett event store
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
 Requires-Dist: boto3[crt]~=1.34.79
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

