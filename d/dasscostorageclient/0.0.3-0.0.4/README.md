# Comparing `tmp/dasscostorageclient-0.0.3.tar.gz` & `tmp/dasscostorageclient-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dasscostorageclient-0.0.3.tar", last modified: Fri Mar 15 11:59:29 2024, max compression
+gzip compressed data, was "dasscostorageclient-0.0.4.tar", last modified: Fri Apr 26 08:54:05 2024, max compression
```

## Comparing `dasscostorageclient-0.0.3.tar` & `dasscostorageclient-0.0.4.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 11:59:29.956043 dasscostorageclient-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-15 11:59:29.956043 dasscostorageclient-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 11:59:29.952043 dasscostorageclient-0.0.3/dasscostorageclient/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/dassco_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 11:59:29.952043 dasscostorageclient-0.0.3/dasscostorageclient/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/exceptions/api_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 11:59:29.952043 dasscostorageclient-0.0.3/dasscostorageclient/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/resources/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/resources/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/resources/fileproxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/resources/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 11:59:29.956043 dasscostorageclient-0.0.3/dasscostorageclient/resources/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/resources/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/resources/models/httpinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/resources/models/specimen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/resources/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/resources/workstations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/dasscostorageclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 11:59:29.956043 dasscostorageclient-0.0.3/dasscostorageclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-15 11:59:29.000000 dasscostorageclient-0.0.3/dasscostorageclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-15 11:59:29.000000 dasscostorageclient-0.0.3/dasscostorageclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 11:59:29.000000 dasscostorageclient-0.0.3/dasscostorageclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-15 11:59:29.000000 dasscostorageclient-0.0.3/dasscostorageclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-15 11:59:29.000000 dasscostorageclient-0.0.3/dasscostorageclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 11:59:29.956043 dasscostorageclient-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 11:59:29.956043 dasscostorageclient-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/tests/dassco_test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/tests/test_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/tests/test_fileproxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/tests/test_institutions.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-15 11:59:21.000000 dasscostorageclient-0.0.3/tests/test_workstations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:54:05.911973 dasscostorageclient-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-26 08:54:05.911973 dasscostorageclient-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:54:05.891973 dasscostorageclient-0.0.4/dasscostorageclient/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:54:05.895973 dasscostorageclient-0.0.4/dasscostorageclient/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/dassco_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:54:05.899973 dasscostorageclient-0.0.4/dasscostorageclient/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/exceptions/api_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:54:05.903973 dasscostorageclient-0.0.4/dasscostorageclient/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/resources/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/resources/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/resources/fileproxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/resources/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:54:05.907973 dasscostorageclient-0.0.4/dasscostorageclient/resources/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/resources/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/resources/models/httpinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/resources/models/specimen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/resources/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/resources/workstations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/dasscostorageclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:54:05.911973 dasscostorageclient-0.0.4/dasscostorageclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-26 08:54:05.000000 dasscostorageclient-0.0.4/dasscostorageclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-26 08:54:05.000000 dasscostorageclient-0.0.4/dasscostorageclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:54:05.000000 dasscostorageclient-0.0.4/dasscostorageclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 08:54:05.000000 dasscostorageclient-0.0.4/dasscostorageclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 08:54:05.000000 dasscostorageclient-0.0.4/dasscostorageclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:54:05.911973 dasscostorageclient-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:54:05.911973 dasscostorageclient-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/tests/dassco_test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/tests/test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/tests/test_fileproxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/tests/test_institutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-26 08:53:56.000000 dasscostorageclient-0.0.4/tests/test_workstations.py
```

### Comparing `dasscostorageclient-0.0.3/PKG-INFO` & `dasscostorageclient-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dasscostorageclient
-Version: 0.0.3
+Version: 0.0.4
 Summary: DaSSCo Storage API SDK
 Author: DaSSCo
 Author-email: dassco@ku.dk
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,11 +35,10 @@
 from dasscostorageclient import DaSSCoStorageClient
 
 client_id = 'CLIENT_ID'
 client_secret = 'CLIENT_SECRET'
 
 client = DaSSCoStorageClient(client_id, client_secret)
 
-res = client.institutions.get_institutions()
+institutions = client.institutions.get()
 
-institutions = res.get('data')
 ```
```

### Comparing `dasscostorageclient-0.0.3/dasscostorageclient/dassco_storage_client.py` & `dasscostorageclient-0.0.4/dasscostorageclient/dassco_storage_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 class DaSSCoStorageClient:
 
     def __init__(self, client_id, client_secret):
         self.client_id = client_id
         self.client_secret = client_secret
         self.token_endpoint = "https://idp.test.dassco.dk/realms/dassco/protocol/openid-connect/token"
-        self.api_url = "https://storage.test.dassco.dk/api"
         self.access_token = self.__get_access_token()
         self.institutions = Institutions(self.access_token)
         self.assets = Assets(self.access_token)
         self.workstations = Workstations(self.access_token)
         self.pipelines = Pipelines(self.access_token)
         self.collections = Collections(self.access_token)
         self.file_proxy = FileProxy(self.access_token)
```

### Comparing `dasscostorageclient-0.0.3/dasscostorageclient/resources/assets.py` & `dasscostorageclient-0.0.4/dasscostorageclient/resources/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,18 @@
     file_formats: list[str]
     asset_locked: bool
     restricted_access: list[str]
     institution: str
     collection: str
     pipeline: str
     digitiser: str | None
+    parent_guid: str | None
+    audited: bool
+    internal_status: str
+    tags: dict | None
     http_info: HTTPInfoModel | None = Field(alias='httpInfo')
 
 
 class EventModel(BaseModel):
     user: str | None
     timestamp: datetime = Field(alias="timeStamp")
     event: str
```

### Comparing `dasscostorageclient-0.0.3/dasscostorageclient/resources/fileproxy.py` & `dasscostorageclient-0.0.4/dasscostorageclient/resources/fileproxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ..utils import *
 import zlib
+import os
 
 
 class FileProxy:
 
     def __init__(self, access_token):
         self.access_token = access_token
 
@@ -20,18 +21,20 @@
         file_data = file.read()
 
         file.close()
 
         # Calculate checksum
         crc = zlib.crc32(file_data)
 
+        filename = os.path.basename(file_path)
+
         res = send_request_to_file_proxy(
             RequestMethod.PUT,
             self.access_token,
-            f"/assetfiles/{institution}/{collection}/{asset_guid}/{file.name}?crc={crc}&file_size_mb={file_size_mb}",
+            f"/assetfiles/{institution}/{collection}/{asset_guid}/{filename}?crc={crc}&file_size_mb={file_size_mb}",
             data=file_data)
         return res
 
     def list_available_files(self, asset_guid):
         res = send_request_to_file_proxy(
             RequestMethod.GET,
             self.access_token,
```

### Comparing `dasscostorageclient-0.0.3/dasscostorageclient/resources/pipelines.py` & `dasscostorageclient-0.0.4/dasscostorageclient/resources/pipelines.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from typing import List
+
+from ..core.models import Pipeline
+from ..core.utils import json_to_model
 from ..utils import *
 
 
 class Pipelines:
 
     def __init__(self, access_token):
         self.access_token = access_token
@@ -10,26 +14,28 @@
         """
         Gets a list of all pipelines in a given institution
 
         Args:
             institution_name (str): The name of the given institution
 
         Returns:
-            A dictionary containing the pipelines
+            A list pipelines
         """
-        return send_request(RequestMethod.GET, self.access_token, f"/v1/institutions/{institution_name}/pipelines")
+        res = send_request(RequestMethod.GET, self.access_token, f"/v1/institutions/{institution_name}/pipelines")
+        return json_to_model(List[Pipeline], res.json())
 
     def create(self, institution_name: str, pipeline_name: str):
         """
           Creates a pipeline in a given institution
 
           Args:
               institution_name (str): The name of the institution to create the pipeline in
               pipeline_name (str): The name of the pipeline to be created
 
          Returns:
-            A dictionary containing the created pipeline
+            The created pipeline
         """
         body = {
             'name': pipeline_name,
         }
-        return send_request(RequestMethod.POST, self.access_token, f"/v1/institutions/{institution_name}/pipelines", body)
+        res = send_request(RequestMethod.POST, self.access_token, f"/v1/institutions/{institution_name}/pipelines", body)
+        return json_to_model(Pipeline, res.json())
```

### Comparing `dasscostorageclient-0.0.3/dasscostorageclient/resources/workstations.py` & `dasscostorageclient-0.0.4/dasscostorageclient/resources/workstations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,13 @@
 from typing import List
-from ..utils import *
-from pydantic import BaseModel, TypeAdapter
-from enum import Enum
-
-
-class WorkstationModel(BaseModel):
-    name: str
-    status: str
-    institution_name: str
-
 
-class WorkstationStatus(Enum):
-    IN_SERVICE = 'IN_SERVICE'
-    OUT_OF_SERVICE = 'OUT_OF_SERVICE'
+from ..core.enums import WorkstationStatus
+from ..core.models import Workstation
+from ..core.utils import json_to_model
+from ..utils import *
 
 
 class Workstations:
 
     def __init__(self, access_token):
         self.access_token = access_token
 
@@ -27,21 +18,15 @@
         Args:
             institution_name (str): The name of the given institution
 
         Returns:
             A list of Workstation objects
         """
         res = send_request(RequestMethod.GET, self.access_token, f"/v1/institutions/{institution_name}/workstations")
-
-        ta = TypeAdapter(List[WorkstationModel])
-
-        return {
-            'data': ta.validate_python(res.json()),
-            'status_code': res.status_code
-        }
+        return json_to_model(List[Workstation], res.json())
 
     def create(self, institution_name: str, workstation_name: str, status: WorkstationStatus = WorkstationStatus.IN_SERVICE):
         """
            Creates a workstation in a given institution
 
            Args:
                institution_name (str): The name of the given institution
@@ -49,25 +34,26 @@
                status (WorkstationStatus): The status of the workstation to be created. The options are: IN_SERVICE or OUT_OF_SERVICE
 
            Returns:
                The created Workstation object
         """
         body = {
             'name': workstation_name,
-            'status': status
+            'status': status.value
         }
         res = send_request(RequestMethod.POST, self.access_token, f"/v1/institutions/{institution_name}/workstations", body)
-        return WorkstationModel.model_validate(res.get('data'))
+        return json_to_model(Workstation, res.json())
 
     def update(self, institution_name: str, workstation_name: str, body: dict):
         """
         Updates a workstation in a given institution
 
         Args:
             institution_name (str): The name of the given institution
             workstation_name (str): The name of the workstation to be updated
             body (dict): The fields to be updated in the given workstation
 
         Returns:
             Currently returns empty data as a 204 (No Content) status code is returned by the API
         """
-        return send_request(RequestMethod.PUT, self.access_token, f"/v1/institutions/{institution_name}/workstations/{workstation_name}", body)
+        return send_request(RequestMethod.PUT, self.access_token,
+                            f"/v1/institutions/{institution_name}/workstations/{workstation_name}", body)
```

### Comparing `dasscostorageclient-0.0.3/dasscostorageclient/utils.py` & `dasscostorageclient-0.0.4/dasscostorageclient/utils.py`

 * *Files identical despite different names*

### Comparing `dasscostorageclient-0.0.3/dasscostorageclient.egg-info/PKG-INFO` & `dasscostorageclient-0.0.4/dasscostorageclient.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dasscostorageclient
-Version: 0.0.3
+Version: 0.0.4
 Summary: DaSSCo Storage API SDK
 Author: DaSSCo
 Author-email: dassco@ku.dk
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,11 +35,10 @@
 from dasscostorageclient import DaSSCoStorageClient
 
 client_id = 'CLIENT_ID'
 client_secret = 'CLIENT_SECRET'
 
 client = DaSSCoStorageClient(client_id, client_secret)
 
-res = client.institutions.get_institutions()
+institutions = client.institutions.get()
 
-institutions = res.get('data')
 ```
```

### Comparing `dasscostorageclient-0.0.3/dasscostorageclient.egg-info/SOURCES.txt` & `dasscostorageclient-0.0.4/dasscostorageclient.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 dasscostorageclient/dassco_storage_client.py
 dasscostorageclient/utils.py
 dasscostorageclient.egg-info/PKG-INFO
 dasscostorageclient.egg-info/SOURCES.txt
 dasscostorageclient.egg-info/dependency_links.txt
 dasscostorageclient.egg-info/requires.txt
 dasscostorageclient.egg-info/top_level.txt
+dasscostorageclient/core/__init__.py
+dasscostorageclient/core/enums.py
+dasscostorageclient/core/models.py
+dasscostorageclient/core/utils.py
 dasscostorageclient/exceptions/__init__.py
 dasscostorageclient/exceptions/api_error.py
 dasscostorageclient/resources/__init__.py
 dasscostorageclient/resources/assets.py
 dasscostorageclient/resources/collections.py
 dasscostorageclient/resources/fileproxy.py
 dasscostorageclient/resources/institutions.py
```

### Comparing `dasscostorageclient-0.0.3/setup.py` & `dasscostorageclient-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `dasscostorageclient-0.0.3/tests/test_assets.py` & `dasscostorageclient-0.0.4/tests/test_assets.py`

 * *Files identical despite different names*

### Comparing `dasscostorageclient-0.0.3/tests/test_fileproxy.py` & `dasscostorageclient-0.0.4/tests/test_fileproxy.py`

 * *Files identical despite different names*

