# Comparing `tmp/pytest_minio_mock-0.2.11.tar.gz` & `tmp/pytest_minio_mock-0.3.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_minio_mock-0.2.11.tar", last modified: Mon Apr 22 11:11:08 2024, max compression
+gzip compressed data, was "pytest_minio_mock-0.3.13.tar", last modified: Fri Apr 26 08:54:21 2024, max compression
```

## Comparing `pytest_minio_mock-0.2.11.tar` & `pytest_minio_mock-0.3.13.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-22 11:11:08.717315 pytest_minio_mock-0.2.11/
--rw-r--r--   0 ouss       (501) staff       (20)     1086 2024-04-22 11:08:27.000000 pytest_minio_mock-0.2.11/LICENSE
--rw-r--r--   0 ouss       (501) staff       (20)        0 2023-11-28 15:52:51.000000 pytest_minio_mock-0.2.11/MANIFEST.in
--rw-r--r--   0 ouss       (501) staff       (20)     5192 2024-04-22 11:11:08.717090 pytest_minio_mock-0.2.11/PKG-INFO
--rw-r--r--   0 ouss       (501) staff       (20)     3869 2024-04-21 19:28:01.000000 pytest_minio_mock-0.2.11/README.md
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-22 11:11:08.715173 pytest_minio_mock-0.2.11/pytest_minio_mock/
--rw-r--r--   0 ouss       (501) staff       (20)      990 2024-04-22 11:08:27.000000 pytest_minio_mock-0.2.11/pytest_minio_mock/__init__.py
--rw-r--r--   0 ouss       (501) staff       (20)    43658 2024-04-22 11:08:27.000000 pytest_minio_mock-0.2.11/pytest_minio_mock/plugin.py
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-22 11:11:08.716670 pytest_minio_mock-0.2.11/pytest_minio_mock.egg-info/
--rw-r--r--   0 ouss       (501) staff       (20)     5192 2024-04-22 11:11:08.000000 pytest_minio_mock-0.2.11/pytest_minio_mock.egg-info/PKG-INFO
--rw-r--r--   0 ouss       (501) staff       (20)      405 2024-04-22 11:11:08.000000 pytest_minio_mock-0.2.11/pytest_minio_mock.egg-info/SOURCES.txt
--rw-r--r--   0 ouss       (501) staff       (20)        1 2024-04-22 11:11:08.000000 pytest_minio_mock-0.2.11/pytest_minio_mock.egg-info/dependency_links.txt
--rw-r--r--   0 ouss       (501) staff       (20)       56 2024-04-22 11:11:08.000000 pytest_minio_mock-0.2.11/pytest_minio_mock.egg-info/entry_points.txt
--rw-r--r--   0 ouss       (501) staff       (20)       65 2024-04-22 11:11:08.000000 pytest_minio_mock-0.2.11/pytest_minio_mock.egg-info/requires.txt
--rw-r--r--   0 ouss       (501) staff       (20)       18 2024-04-22 11:11:08.000000 pytest_minio_mock-0.2.11/pytest_minio_mock.egg-info/top_level.txt
--rw-r--r--   0 ouss       (501) staff       (20)       38 2024-04-22 11:11:08.717361 pytest_minio_mock-0.2.11/setup.cfg
--rw-r--r--   0 ouss       (501) staff       (20)     1781 2024-04-22 11:08:27.000000 pytest_minio_mock-0.2.11/setup.py
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-22 11:11:08.716429 pytest_minio_mock-0.2.11/tests/
--rw-r--r--   0 ouss       (501) staff       (20)        0 2023-11-28 14:02:59.000000 pytest_minio_mock-0.2.11/tests/__init__.py
--rw-r--r--   0 ouss       (501) staff       (20)      104 2024-04-20 11:16:24.000000 pytest_minio_mock-0.2.11/tests/conftest.py
--rw-r--r--   0 ouss       (501) staff       (20)    16154 2024-04-22 11:08:27.000000 pytest_minio_mock-0.2.11/tests/test_minio_mock.py
+drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-26 08:54:21.072612 pytest_minio_mock-0.3.13/
+-rw-r--r--   0 ouss       (501) staff       (20)     1086 2024-04-22 11:08:27.000000 pytest_minio_mock-0.3.13/LICENSE
+-rw-r--r--   0 ouss       (501) staff       (20)        0 2023-11-28 15:52:51.000000 pytest_minio_mock-0.3.13/MANIFEST.in
+-rw-r--r--   0 ouss       (501) staff       (20)     5192 2024-04-26 08:54:21.072397 pytest_minio_mock-0.3.13/PKG-INFO
+-rw-r--r--   0 ouss       (501) staff       (20)     3869 2024-04-21 19:28:01.000000 pytest_minio_mock-0.3.13/README.md
+drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-26 08:54:21.069864 pytest_minio_mock-0.3.13/pytest_minio_mock/
+-rw-r--r--   0 ouss       (501) staff       (20)     1015 2024-04-26 08:52:30.000000 pytest_minio_mock-0.3.13/pytest_minio_mock/__init__.py
+-rw-r--r--   0 ouss       (501) staff       (20)    44860 2024-04-26 08:24:20.000000 pytest_minio_mock-0.3.13/pytest_minio_mock/plugin.py
+drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-26 08:54:21.072066 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/
+-rw-r--r--   0 ouss       (501) staff       (20)     5192 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/PKG-INFO
+-rw-r--r--   0 ouss       (501) staff       (20)      405 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 ouss       (501) staff       (20)        1 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 ouss       (501) staff       (20)       56 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/entry_points.txt
+-rw-r--r--   0 ouss       (501) staff       (20)       65 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/requires.txt
+-rw-r--r--   0 ouss       (501) staff       (20)       18 2024-04-26 08:54:21.000000 pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/top_level.txt
+-rw-r--r--   0 ouss       (501) staff       (20)       38 2024-04-26 08:54:21.072659 pytest_minio_mock-0.3.13/setup.cfg
+-rw-r--r--   0 ouss       (501) staff       (20)     1781 2024-04-26 08:34:48.000000 pytest_minio_mock-0.3.13/setup.py
+drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-04-26 08:54:21.071687 pytest_minio_mock-0.3.13/tests/
+-rw-r--r--   0 ouss       (501) staff       (20)        0 2024-04-26 08:31:50.000000 pytest_minio_mock-0.3.13/tests/__init__.py
+-rw-r--r--   0 ouss       (501) staff       (20)      104 2024-04-20 11:16:24.000000 pytest_minio_mock-0.3.13/tests/conftest.py
+-rw-r--r--   0 ouss       (501) staff       (20)    16739 2024-04-26 08:24:20.000000 pytest_minio_mock-0.3.13/tests/test_minio_mock.py
```

### Comparing `pytest_minio_mock-0.2.11/LICENSE` & `pytest_minio_mock-0.3.13/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_minio_mock-0.2.11/PKG-INFO` & `pytest_minio_mock-0.3.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-minio-mock
-Version: 0.2.11
+Version: 0.3.13
 Summary: A pytest plugin for mocking Minio S3 interactions
 Home-page: https://github.com/oussjarrousse/pytest-minio-mock
 Author: Oussama Jarrousse
 Author-email: oussama@jarrousse.org
 License: MIT
 Project-URL: Source, https://github.com/oussjarrousse/pytest-minio-mock/
 Project-URL: Tracker, https://github.com/oussjarrousse/pytest-minio-mock/issues
```

### Comparing `pytest_minio_mock-0.2.11/README.md` & `pytest_minio_mock-0.3.13/README.md`

 * *Files identical despite different names*

### Comparing `pytest_minio_mock-0.2.11/pytest_minio_mock/__init__.py` & `pytest_minio_mock-0.3.13/pytest_minio_mock/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 
 For more information and usage examples, please refer to the project's README.md.
 
 """
 
 __title__ = "pytest-minio-mock"
 __description__ = "A pytest plugin for mocking Minio S3 interactions"
-__version__ = "0.2.11"
+__version__ = "0.3.13"
 __status__ = "Production"
 __license__ = "MIT"
 __author__ = "Oussama Jarrousse"
 __maintainer__ = "Oussama Jarrousse"
 __email__ = "oussama@jarrousse.org"
-__credits__ = ["Gustavo Satheler", "@cottephi"]
+__credits__ = ["Gustavo Satheler", "@cottephi", "Wouter van Atteveldt"]
```

### Comparing `pytest_minio_mock-0.2.11/pytest_minio_mock/plugin.py` & `pytest_minio_mock-0.3.13/pytest_minio_mock/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,27 @@
     minio_mock: A pytest fixture to patch the Minio client with a mock for testing.
 
 This module allows you to test file uploads, downloads, bucket creations, and other Minio operations
 by simulating the Minio environment. It's useful in scenarios where you want to ensure your
 application interacts correctly with Minio, without the overhead of connecting to an actual Minio
 server.
 """
+
 import copy
 import datetime
 import io
 import logging
 import os
 from uuid import uuid4
 
 import pytest
 import validators
 from minio import Minio
 from minio.commonconfig import ENABLED
-from minio.datatypes import Object
+from minio.datatypes import Object, Bucket
 from minio.error import S3Error
 from minio.versioningconfig import OFF
 from minio.versioningconfig import SUSPENDED
 from minio.versioningconfig import VersioningConfig
 from urllib3.connection import HTTPConnection
 from urllib3.response import HTTPResponse
 
@@ -381,14 +382,15 @@
         object_lock=False,
     ):
         self._bucket_name = bucket_name
         self._versioning = versioning
         self._objects = {}
         self._location = location
         self._object_lock = object_lock
+        self._creation_date = datetime.datetime.now()
 
     @property
     def bucket_name(self):
         """Gets the name of the bucket stored at initialization."""
         return self._bucket_name
 
     @property
@@ -491,30 +493,33 @@
                 bucket_name=self.bucket_name,
                 object_name=object_name,
             )
         return the_object_version
 
     def list_objects(
         self,
-        prefix="",
+        prefix=None,
         recursive=False,
-        start_after="",
+        start_after=None,
         include_version=False,
     ):
         """
         Returns
             Iterator of MockMinioObjectVersions of the current bucket
         """
         # Initialization
         # bucket_objects = []
         seen_prefixes = set()
+        if prefix is None:
+            prefix = ""
 
-        for object_name, obj in self.objects.items():
+        # Note: Wrapped items() in list(.) to allow modification during iteration
+        for object_name, obj in list(self.objects.items()):
             if object_name.startswith(prefix) and (
-                start_after == "" or object_name > start_after
+                not start_after or object_name > start_after
             ):
                 # Handle non-recursive listing by identifying and adding unique directory names
                 if not recursive:
                     sub_path = object_name[len(prefix) :].strip("/")
                     dir_end_idx = sub_path.find("/")
                     if dir_end_idx != -1:
                         dir_name = prefix + sub_path[: dir_end_idx + 1]
@@ -1066,18 +1071,15 @@
         Simulates listing all the buckets available to the user in the Minio server.
 
         Returns:
             list: A list of bucket names.
         """
         try:
             self._health_check()
-            buckets_list = []
-            for bucket_name in self.buckets.keys():
-                buckets_list.append(bucket_name)
-            return buckets_list
+            return [Bucket(name, bucket._creation_date) for (name, bucket) in list(self.buckets.items())]
         except Exception as e:
             logging.error(e)
             raise e
 
     def bucket_exists(self, bucket_name):
         """
         Checks if a bucket exists in the mock Minio server.
@@ -1119,14 +1121,46 @@
             bucket_name=bucket_name,
             versioning=VersioningConfig(),
             location=location,
             object_lock=object_lock,
         )
         return True
 
+    def remove_bucket(self, bucket_name: str):
+        """
+        Remove an empty bucket.
+
+        :param bucket_name: Name of the bucket.
+
+        Example::
+            client.remove_bucket("my-bucket")
+        """
+        self._health_check()
+        if bucket_name not in self.buckets:
+            raise S3Error(
+                code="NoSuchBucket",
+                message="The specified bucket does not exist",
+                resource=f"/{bucket_name}",
+                request_id=None,
+                host_id=None,
+                response="mocked_response",
+                bucket_name=bucket_name,
+            )
+        if self.buckets[bucket_name].objects:
+            raise S3Error(
+                code="BucketNotEmpty",
+                message="The bucket you tried to delete is not empty",
+                resource=f"/{bucket_name}",
+                request_id=None,
+                host_id=None,
+                response="mocked_response",
+                bucket_name=bucket_name,
+            )
+        del self.buckets[bucket_name]
+
     def set_bucket_versioning(self, bucket_name: str, config: VersioningConfig):
         """Bucket versioning can be set to ENABLED or SUSPENDED, but not to
         OFF (filtered out by VersioningConfig itself)
         """
         self._health_check()
         if not self.bucket_exists(bucket_name):
             raise S3Error(
@@ -1160,17 +1194,17 @@
                 object_name=None,
             )
         return self.buckets[bucket_name].versioning
 
     def list_objects(
         self,
         bucket_name,
-        prefix="",
+        prefix=None,
         recursive=False,
-        start_after="",
+        start_after=None,
         include_version=False,
     ):
         """
         Lists objects in a bucket with the specified prefix and conditions.
 
         Simulates listing objects in a bucket in the mock Minio server.
```

### Comparing `pytest_minio_mock-0.2.11/pytest_minio_mock.egg-info/PKG-INFO` & `pytest_minio_mock-0.3.13/pytest_minio_mock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-minio-mock
-Version: 0.2.11
+Version: 0.3.13
 Summary: A pytest plugin for mocking Minio S3 interactions
 Home-page: https://github.com/oussjarrousse/pytest-minio-mock
 Author: Oussama Jarrousse
 Author-email: oussama@jarrousse.org
 License: MIT
 Project-URL: Source, https://github.com/oussjarrousse/pytest-minio-mock/
 Project-URL: Tracker, https://github.com/oussjarrousse/pytest-minio-mock/issues
```

### Comparing `pytest_minio_mock-0.2.11/setup.py` & `pytest_minio_mock-0.3.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     license="MIT",
     author="Oussama Jarrousse",
     author_email="oussama@jarrousse.org",
     description="A pytest plugin for mocking Minio S3 interactions",
     long_description=open("README.md").read(),
     keywords="pytest minio mock",
     extras_require={"dev": ["pre-commit", "tox"]},
-    version="0.2.11",
+    version="0.3.13",
     long_description_content_type="text/markdown",
     classifiers=[
         "Framework :: Pytest",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
```

### Comparing `pytest_minio_mock-0.2.11/tests/test_minio_mock.py` & `pytest_minio_mock-0.3.13/tests/test_minio_mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import validators
 from minio import Minio
 from minio.commonconfig import ENABLED
 from minio.error import S3Error
 from minio.versioningconfig import OFF
 from minio.versioningconfig import SUSPENDED
 from minio.versioningconfig import VersioningConfig
+from minio.datatypes import Bucket
 
 from pytest_minio_mock.plugin import MockMinioBucket
 from pytest_minio_mock.plugin import MockMinioObject
 
 
 @pytest.mark.UNIT
 class TestsMockMinioObject:
@@ -59,14 +60,29 @@
 def test_make_bucket(minio_mock):
     bucket_name = "test-bucket"
     client = Minio("http://local.host:9000")
     client.make_bucket(bucket_name)
     assert client.bucket_exists(bucket_name), "Bucket should exist after creation"
 
 
+@pytest.mark.UNIT
+@pytest.mark.API
+def test_remove_bucket(minio_mock):
+    client = Minio("http://local.host:9000")
+    original_buckets = client.list_buckets()
+    n = len(original_buckets)
+    bucket_name = "new-bucket"
+    client.make_bucket(bucket_name)
+    buckets = client.list_buckets()
+    assert len(buckets) == n + 1
+    client.remove_bucket(bucket_name)
+    buckets = client.list_buckets()
+    assert buckets == original_buckets
+
+
 @pytest.mark.API
 @pytest.mark.FUNC
 def test_putting_and_removing_objects_no_versionning(minio_mock):
     # simple thing
     bucket_name = "test-bucket"
     object_name = "test-object"
     file_path = "tests/fixtures/maya.jpeg"
@@ -365,14 +381,16 @@
     client = Minio("http://local.host:9000")
     buckets = client.list_buckets()
     n = len(buckets)
     bucket_name = "new-bucket"
     client.make_bucket(bucket_name)
     buckets = client.list_buckets()
     assert len(buckets) == n + 1
+    assert "new-bucket" in {b.name for b in buckets}
+    assert all(isinstance(b, Bucket) for b in buckets)
 
 
 @pytest.mark.REGRESSION
 @pytest.mark.UNIT
 @pytest.mark.API
 def test_list_objects(minio_mock):
     client = Minio("http://local.host:9000")
```

