# Comparing `tmp/tehzor-0.0.4.tar.gz` & `tmp/tehzor-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tehzor-0.0.4.tar", last modified: Wed Apr 17 16:03:26 2024, max compression
+gzip compressed data, was "tehzor-0.0.5.tar", last modified: Fri Apr 26 15:46:41 2024, max compression
```

## Comparing `tehzor-0.0.4.tar` & `tehzor-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 16:03:26.709702 tehzor-0.0.4/
--rw-rw-rw-   0        0        0     1082 2024-04-12 09:32:26.000000 tehzor-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1955 2024-04-17 16:03:26.709702 tehzor-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1180 2024-04-17 06:48:00.000000 tehzor-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 16:03:26.709702 tehzor-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1028 2024-04-17 16:01:35.000000 tehzor-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 16:03:26.698820 tehzor-0.0.4/tehzor/
--rw-rw-rw-   0        0        0       77 2024-04-17 06:33:50.000000 tehzor-0.0.4/tehzor/__init__.py
--rw-rw-rw-   0        0        0     7727 2024-04-17 15:52:38.000000 tehzor-0.0.4/tehzor/api.py
--rw-rw-rw-   0        0        0      748 2024-04-17 06:33:50.000000 tehzor-0.0.4/tehzor/constants.py
--rw-rw-rw-   0        0        0     5679 2024-04-17 16:00:06.000000 tehzor-0.0.4/tehzor/models.py
-drwxrwxrwx   0        0        0        0 2024-04-17 16:03:26.709702 tehzor-0.0.4/tehzor.egg-info/
--rw-rw-rw-   0        0        0     1955 2024-04-17 16:03:26.000000 tehzor-0.0.4/tehzor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2024-04-17 16:03:26.000000 tehzor-0.0.4/tehzor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 16:03:26.000000 tehzor-0.0.4/tehzor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-17 16:03:26.000000 tehzor-0.0.4/tehzor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-17 16:03:26.000000 tehzor-0.0.4/tehzor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 16:03:26.709702 tehzor-0.0.4/tests/
--rw-rw-rw-   0        0        0      531 2024-04-17 06:33:50.000000 tehzor-0.0.4/tests/test_api_create.py
--rw-rw-rw-   0        0        0      927 2024-04-17 06:33:50.000000 tehzor-0.0.4/tests/test_get_problem_id.py
--rw-rw-rw-   0        0        0      915 2024-04-17 13:10:00.000000 tehzor-0.0.4/tests/test_get_space_id.py
--rw-rw-rw-   0        0        0     1399 2024-04-17 15:55:44.000000 tehzor-0.0.4/tests/test_get_space_meters.py
--rw-rw-rw-   0        0        0      975 2024-04-17 06:33:50.000000 tehzor-0.0.4/tests/test_get_work_acceptance.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:46:41.923295 tehzor-0.0.5/
+-rw-rw-rw-   0        0        0     1082 2024-04-12 09:32:26.000000 tehzor-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1955 2024-04-26 15:46:41.923295 tehzor-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1180 2024-04-17 06:48:00.000000 tehzor-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 15:46:41.923295 tehzor-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1028 2024-04-26 15:46:10.000000 tehzor-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:46:41.915470 tehzor-0.0.5/tehzor/
+-rw-rw-rw-   0        0        0       77 2024-04-17 06:33:50.000000 tehzor-0.0.5/tehzor/__init__.py
+-rw-rw-rw-   0        0        0     7727 2024-04-18 10:07:43.000000 tehzor-0.0.5/tehzor/api.py
+-rw-rw-rw-   0        0        0      748 2024-04-17 06:33:50.000000 tehzor-0.0.5/tehzor/constants.py
+-rw-rw-rw-   0        0        0     6119 2024-04-26 15:31:14.000000 tehzor-0.0.5/tehzor/models.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:46:41.923295 tehzor-0.0.5/tehzor.egg-info/
+-rw-rw-rw-   0        0        0     1955 2024-04-26 15:46:41.000000 tehzor-0.0.5/tehzor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-04-26 15:46:41.000000 tehzor-0.0.5/tehzor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 15:46:41.000000 tehzor-0.0.5/tehzor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-26 15:46:41.000000 tehzor-0.0.5/tehzor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 15:46:41.000000 tehzor-0.0.5/tehzor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 15:46:41.923295 tehzor-0.0.5/tests/
+-rw-rw-rw-   0        0        0      531 2024-04-17 06:33:50.000000 tehzor-0.0.5/tests/test_api_create.py
+-rw-rw-rw-   0        0        0      927 2024-04-17 06:33:50.000000 tehzor-0.0.5/tests/test_get_problem_id.py
+-rw-rw-rw-   0        0        0      915 2024-04-17 13:10:00.000000 tehzor-0.0.5/tests/test_get_space_id.py
+-rw-rw-rw-   0        0        0     1399 2024-04-17 15:55:44.000000 tehzor-0.0.5/tests/test_get_space_meters.py
+-rw-rw-rw-   0        0        0      975 2024-04-17 06:33:50.000000 tehzor-0.0.5/tests/test_get_work_acceptance.py
```

### Comparing `tehzor-0.0.4/LICENSE.txt` & `tehzor-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.4/PKG-INFO` & `tehzor-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tehzor
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python API wrapper for Tehzor API
 Home-page: https://github.com/gritsyuk/tehzor
 Download-URL: https://github.com/gritsyuk/tehzor/archive/refs/heads/develop.zip
 Author: Igor Gritsyuk
 Author-email: gritsyuk.igor@gmail.com
 Project-URL: GitHub, https://github.com/gritsyuk/tehzor
 Keywords: tehzor api tehzorapi construction supervision operation inspections constarctionsite building management
```

### Comparing `tehzor-0.0.4/README.md` & `tehzor-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.4/setup.py` & `tehzor-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
   
 
 setup(
   name='tehzor',
-  version='0.0.4',
+  version='0.0.5',
   author='Igor Gritsyuk',
   author_email='gritsyuk.igor@gmail.com',
   description='A Python API wrapper for Tehzor API',
   download_url='https://github.com/gritsyuk/tehzor/archive/refs/heads/develop.zip',
   long_description=long_description,
   long_description_content_type='text/markdown',
   url='https://github.com/gritsyuk/tehzor',
```

### Comparing `tehzor-0.0.4/tehzor/api.py` & `tehzor-0.0.5/tehzor/api.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.4/tehzor/constants.py` & `tehzor-0.0.5/tehzor/constants.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.4/tehzor/models.py` & `tehzor-0.0.5/tehzor/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     id: str
     preview: Optional[dict] = None
     full: Optional[dict] = None
     size: Optional[int] = None
 
 
 class User(BaseModel):
-    id: str
+    id: Optional[str] = None
     fullName: Optional[str] = None
     displayName: Optional[str] = None
     position: Optional[str] = None
     color: Optional[str] = None
 
 
 class Status(BaseModel):
@@ -116,22 +116,28 @@
     unitId: Optional[str] = None
     unitName: Optional[str] = None
 
 
 class WorkAcceptances(Problem):
     objectId: str
     structureIds: List[str]
-    spaceIds: List[str]
+    spaceIds: List[str] = [] 
     acceptanceDate: int
     percent: Optional[float] = 0.0
     comment: Optional[str] = None
     physicalWorkScope: Optional[WorkScope] = None
     type: Optional[str] = None
     frontType: Optional[str]
 
+    @field_validator('createdAt', 'modifiedAt', 'acceptanceDate', mode='after')
+    def convert_timestamps_to_datetime(cls, value):
+        if isinstance(value, int):
+            return datetime.fromtimestamp(value / 1000)
+        return value
+
 
 class Spacetype(BaseModel):
     id: str
     name: str | None = None
     singularName: str | None = None
 
 
@@ -192,10 +198,14 @@
             return datetime.fromtimestamp(value / 1000)
         return value
 
 
 class SpaceMeters(BaseModel):
     id: str
     type: SpaceMeterType | None
-    serialNumber: str
-    description: str
+    serialNumber: str | None = None
+    description: str | None = None
     consumptions: List[SpaceMetersConsumption] | None = None
+    createdBy: User | None = None
+    createdAt: int | None = None
+    modifiedBy: User | None = None
+    modifiedAt: int | None = None
```

### Comparing `tehzor-0.0.4/tehzor.egg-info/PKG-INFO` & `tehzor-0.0.5/tehzor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tehzor
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python API wrapper for Tehzor API
 Home-page: https://github.com/gritsyuk/tehzor
 Download-URL: https://github.com/gritsyuk/tehzor/archive/refs/heads/develop.zip
 Author: Igor Gritsyuk
 Author-email: gritsyuk.igor@gmail.com
 Project-URL: GitHub, https://github.com/gritsyuk/tehzor
 Keywords: tehzor api tehzorapi construction supervision operation inspections constarctionsite building management
```

### Comparing `tehzor-0.0.4/tests/test_api_create.py` & `tehzor-0.0.5/tests/test_api_create.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.4/tests/test_get_problem_id.py` & `tehzor-0.0.5/tests/test_get_problem_id.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.4/tests/test_get_space_id.py` & `tehzor-0.0.5/tests/test_get_space_id.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.4/tests/test_get_space_meters.py` & `tehzor-0.0.5/tests/test_get_space_meters.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.4/tests/test_get_work_acceptance.py` & `tehzor-0.0.5/tests/test_get_work_acceptance.py`

 * *Files identical despite different names*

