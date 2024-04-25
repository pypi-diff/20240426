# Comparing `tmp/objective_sdk-4.0.2.tar.gz` & `tmp/objective_sdk-4.0.3.tar.gz`

## Comparing `objective_sdk-4.0.2.tar` & `objective_sdk-4.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 objective_sdk-4.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 objective_sdk-4.0.2/src/objective/__init__.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 objective_sdk-4.0.2/src/objective/objective.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 objective_sdk-4.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 objective_sdk-4.0.2/tests/sdk_integration_test.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 objective_sdk-4.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 objective_sdk-4.0.2/LICENSE
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 objective_sdk-4.0.2/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 objective_sdk-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 objective_sdk-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 objective_sdk-4.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 objective_sdk-4.0.3/src/objective/__init__.py
+-rw-r--r--   0        0        0    18352 2020-02-02 00:00:00.000000 objective_sdk-4.0.3/src/objective/objective.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 objective_sdk-4.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 objective_sdk-4.0.3/tests/sdk_integration_test.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 objective_sdk-4.0.3/tests/test_objective.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 objective_sdk-4.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 objective_sdk-4.0.3/LICENSE
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 objective_sdk-4.0.3/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 objective_sdk-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 objective_sdk-4.0.3/PKG-INFO
```

### Comparing `objective_sdk-4.0.2/.github/workflows/python-publish.yml` & `objective_sdk-4.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `objective_sdk-4.0.2/src/objective/objective.py` & `objective_sdk-4.0.3/src/objective/objective.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # TODO(chandler): Use ruff.
 
 from concurrent.futures import ThreadPoolExecutor
 import datetime
+from enum import Enum
 from typing import Dict, Generator, List, Optional, Any, Union
 from dataclasses import dataclass, field
 from more_itertools import chunked
 import requests
 import os, sys
 import time
 
@@ -108,18 +109,20 @@
                     time.sleep(sleep_time)
                     continue
                 else:
                     raise (e)
 
     @property
     def object_store(self) -> "ObjectStore":
+        """Routes for /objects"""
         return ObjectStore(client=self)
 
     @property
     def indexes(self) -> "Indexes":
+        """Routes for /indexes"""
         return Indexes(client=self)
 
     def list_indexes(
         self, limit: Optional[int] = None, cursor: Optional[str] = None
     ) -> List["Index"]:
         return self.indexes.list_indexes(limit=limit, cursor=cursor)
 
@@ -285,20 +288,35 @@
 
             if not cursor:
                 break
 
     def get_all_objects(self) -> Generator[Object, None, None]:
         return self.list_all_objects(include_object=True)
 
-    def get_objects_by_id(self, ids: List[str]) -> List[Object]:
+    def get_objects_by_id(
+        self, ids: List[str], skip_missing_objects: bool = True
+    ) -> List[Object]:
         with ThreadPoolExecutor(max_workers=CPU_COUNT * 12) as executor:
-            return list(executor.map(self.get_object, ids))
-
-    def get_object(self, id: str) -> Object:
-        return Object(**self.client.request("GET", f"objects/{id}"))
+            objects = list(
+                executor.map(
+                    lambda id: self.get_object(id),
+                    ids,
+                )
+            )
+            if skip_missing_objects:
+                objects = [obj for obj in objects if obj]
+            return objects
+
+    def get_object(self, id: str) -> Optional[Object]:
+        try:
+            return Object(**self.client.request("GET", f"objects/{id}"))
+        except requests.exceptions.HTTPError as http_error:
+            if http_error.response.status_code == 404:
+                return None
+            raise
 
     def upsert_objects(self, objects: List[Union[Object, Dict]]) -> BatchOperation:
         def upsert_object(object):
             try:
                 return self._upsert_object(object)
             except Error as e:
                 object._ops_status = {"state": "error", "exception": e}
@@ -402,14 +420,17 @@
         return object
 
 
 @dataclass
 class Index:
     client: Client
     id: str
+    index_type: str
+    version: str
+    fields: Dict[str, Any]
 
     def __str__(self):
         return f"Index(id={self.id})"
 
     def __repr__(self):
         return self.__str__()
 
@@ -477,20 +498,22 @@
         return obj_status
 
     def search(
         self,
         query: str,
         filter_query: Optional[str] = None,
         object_fields: Optional[str] = None,
+        result_fields: Optional[str] = None,
         limit: Optional[int] = None,
     ) -> Dict[str, Any]:
         params = {
             "query": query,
             "filter_query": filter_query,
             "object_fields": object_fields,
+            "result_fields": result_fields,
             "limit": limit,
         }
         return self.client.request("GET", f"indexes/{self.id}/search", data=params)
 
 
 @dataclass
 class Indexes:
@@ -510,39 +533,52 @@
         with ThreadPoolExecutor(max_workers=CPU_COUNT * 12) as executor:
             return list(
                 executor.map(self.get_index, [index["id"] for index in indexes])
             )
 
     def create_index(
         self,
-        index_type,
+        index_type: Union[str, Dict[str, Any]],
         fields: Dict[str, Any],
         version: str = None,
     ) -> "Index":
+        # Support passing the index_type as a string for usability.
+        # In the case it's a string, map it to a dictionary
+        if isinstance(index_type, str):
+            index_type = {"name": index_type}
+
         print("Creating index...", file=sys.stderr)
         index_create = self.client.request(
             "POST",
             "indexes",
             data={
                 "configuration": {
-                    "template": {
-                        **{"name": index_type},
-                        **({"version": version} if version else {}),
-                    },
+                    "index_type": index_type,
                     "fields": _preprocess_fields(fields),
                 }
             },
         )
         if not index_create:
             raise ValueError("Failed to create index!")
         else:
             print(f"Index {index_create['id']} successfully created.", file=sys.stderr)
             return Index(
                 client=self.client,
                 id=index_create["id"],
+                index_type=index_type,
+                version=version,
+                fields=fields,
             )
 
     def get_index(self, id: str) -> "Index":
-        return Index(self.client, id=id)
+        index_response = self.client.request("GET", f"indexes/{id}")
+        index_settings = index_response["settings"]
+        return Index(
+            client=self.client,
+            id=id,
+            index_type=index_settings["template"]["template_name"],
+            version=index_settings["template"]["template_version"],
+            fields=index_settings["fields"],
+        )
 
     def __getitem__(self, id: str) -> "Index":
         return self.get_index(id)
```

### Comparing `objective_sdk-4.0.2/tests/sdk_integration_test.py` & `objective_sdk-4.0.3/tests/sdk_integration_test.py`

 * *Files identical despite different names*

### Comparing `objective_sdk-4.0.2/.gitignore` & `objective_sdk-4.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `objective_sdk-4.0.2/LICENSE` & `objective_sdk-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `objective_sdk-4.0.2/README.md` & `objective_sdk-4.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Documentation
 
 Our documentation can be found at [docs.objective.inc](https://docs.objective.inc).
 
 ## Install and configure API key
 
-To get an API key, create an account at [app.objective.inc](https://app.objective.inc).
+To get an API key today join the [waitlist](https://www.objective.inc/contact).
 
 ```bash
 pip install objective-sdk
 ```
 
 ## Quickstart
```

### Comparing `objective_sdk-4.0.2/pyproject.toml` & `objective_sdk-4.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "objective-sdk"
-version = "4.0.2"
+version = "4.0.3"
 description = "Official Python SDK for Objective, Inc. APIs"
 authors = [
     { name = "Objective, Inc.", email = "support@objective.inc" }
 ]
 dependencies = [
     "requests>=2.26.0",
-    "more-itertools==8.10.0"
+    "more-itertools>=8.10.0"
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 
 [project.urls]
 Homepage = "https://github.com/objective-inc/objective-py"
 Repository = "https://github.com/objective-inc/objective-py"
```

### Comparing `objective_sdk-4.0.2/PKG-INFO` & `objective_sdk-4.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: objective-sdk
-Version: 4.0.2
+Version: 4.0.3
 Summary: Official Python SDK for Objective, Inc. APIs
 Project-URL: Homepage, https://github.com/objective-inc/objective-py
 Project-URL: Repository, https://github.com/objective-inc/objective-py
 Author-email: "Objective, Inc." <support@objective.inc>
 License-File: LICENSE
 Requires-Python: >=3.8
-Requires-Dist: more-itertools==8.10.0
+Requires-Dist: more-itertools>=8.10.0
 Requires-Dist: requests>=2.26.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # Objective, Inc. Python Library
 
@@ -19,15 +19,15 @@
 
 ## Documentation
 
 Our documentation can be found at [docs.objective.inc](https://docs.objective.inc).
 
 ## Install and configure API key
 
-To get an API key, create an account at [app.objective.inc](https://app.objective.inc).
+To get an API key today join the [waitlist](https://www.objective.inc/contact).
 
 ```bash
 pip install objective-sdk
 ```
 
 ## Quickstart
```

