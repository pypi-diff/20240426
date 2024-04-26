# Comparing `tmp/ansys-api-discovery-0.5.1.tar.gz` & `tmp/ansys_api_discovery-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-discovery-0.5.1.tar", last modified: Wed Oct  4 09:18:40 2023, max compression
+gzip compressed data, was "ansys_api_discovery-0.5.2.tar", last modified: Fri Apr 26 14:18:53 2024, max compression
```

## Comparing `ansys-api-discovery-0.5.1.tar` & `ansys_api_discovery-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:18:40.371950 ansys-api-discovery-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-10-04 09:18:40.371950 ansys-api-discovery-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:18:40.367950 ansys-api-discovery-0.5.1/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:18:40.367950 ansys-api-discovery-0.5.1/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:18:40.367950 ansys-api-discovery-0.5.1/ansys/api/discovery/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/ansys/api/discovery/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/ansys/api/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/ansys/api/discovery/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:18:40.371950 ansys-api-discovery-0.5.1/ansys/api/discovery/v0/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/ansys/api/discovery/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/ansys/api/discovery/v0/definedvariationstable.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/ansys/api/discovery/v0/discoverymodels.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/ansys/api/discovery/v0/historytrackparameters.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/ansys/api/discovery/v0/scriptparameters.proto
--rw-r--r--   0 runner    (1001) docker     (127)    45403 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/ansys/api/discovery/v0/units.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:18:40.371950 ansys-api-discovery-0.5.1/ansys_api_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-10-04 09:18:40.000000 ansys-api-discovery-0.5.1/ansys_api_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-10-04 09:18:40.000000 ansys-api-discovery-0.5.1/ansys_api_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 09:18:40.000000 ansys-api-discovery-0.5.1/ansys_api_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-10-04 09:18:40.000000 ansys-api-discovery-0.5.1/ansys_api_discovery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-04 09:18:40.000000 ansys-api-discovery-0.5.1/ansys_api_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-04 09:18:40.000000 ansys-api-discovery-0.5.1/ansys_api_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-04 09:18:40.371950 ansys-api-discovery-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-10-04 09:18:21.000000 ansys-api-discovery-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:18:53.039875 ansys_api_discovery-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-26 14:18:53.039875 ansys_api_discovery-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:18:53.035875 ansys_api_discovery-0.5.2/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:18:53.035875 ansys_api_discovery-0.5.2/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:18:53.035875 ansys_api_discovery-0.5.2/ansys/api/discovery/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:18:53.039875 ansys_api_discovery-0.5.2/ansys/api/discovery/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/v0/conditions.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/v0/definedvariationstable.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/v0/discoverymodels.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/v0/historytrackparameters.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/v0/messaging.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/v0/scriptparameters.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/v0/simulations.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/v0/solution.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    45403 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/ansys/api/discovery/v0/units.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:18:53.039875 ansys_api_discovery-0.5.2/ansys_api_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-26 14:18:53.000000 ansys_api_discovery-0.5.2/ansys_api_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-26 14:18:53.000000 ansys_api_discovery-0.5.2/ansys_api_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:18:53.000000 ansys_api_discovery-0.5.2/ansys_api_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-26 14:18:53.000000 ansys_api_discovery-0.5.2/ansys_api_discovery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 14:18:53.000000 ansys_api_discovery-0.5.2/ansys_api_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 14:18:53.000000 ansys_api_discovery-0.5.2/ansys_api_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:18:53.039875 ansys_api_discovery-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-26 14:18:41.000000 ansys_api_discovery-0.5.2/setup.py
```

### Comparing `ansys-api-discovery-0.5.1/LICENSE` & `ansys_api_discovery-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.5.1/PKG-INFO` & `ansys_api_discovery-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ansys-api-discovery
-Version: 0.5.1
-Summary: Autogenerated python gRPC interface package for ansys-api-discovery, built on 09:18:40 on 04 October 2023
+Version: 0.5.2
+Summary: Autogenerated python gRPC interface package for ansys-api-discovery, built on 14:18:53 on 26 April 2024
 Home-page: https://github.com/ansys/ansys-api-discovery
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: grpcio~=1.47
 Requires-Dist: protobuf<5,>=3.19
-Requires-Dist: ansys-api-dbu==0.2.1
+Requires-Dist: ansys-api-dbu==0.3.0
 
 ### ansys-api-discovery gRPC Interface Package
 
 This repository provides the auto-generated gRPC Python interface files
 for Discovery/SpaceClaim.
```

### Comparing `ansys-api-discovery-0.5.1/README.md` & `ansys_api_discovery-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.5.1/ansys/api/discovery/v0/definedvariationstable.proto` & `ansys_api_discovery-0.5.2/ansys/api/discovery/v0/definedvariationstable.proto`

 * *Files 1% similar despite different names*

```diff
@@ -123,13 +123,14 @@
 
 ///UPDATES
 //
 
 message UpdateResponse{
   // The result
   bool result = 1;
+  string message = 2;
 }
 
 message IsSolvingResponse{
   // The result
   bool is_solving = 1;
 }
```

### Comparing `ansys-api-discovery-0.5.1/ansys/api/discovery/v0/historytrackparameters.proto` & `ansys_api_discovery-0.5.2/ansys/api/discovery/v0/historytrackparameters.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.5.1/ansys/api/discovery/v0/scriptparameters.proto` & `ansys_api_discovery-0.5.2/ansys/api/discovery/v0/scriptparameters.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.5.1/ansys/api/discovery/v0/units.proto` & `ansys_api_discovery-0.5.2/ansys/api/discovery/v0/units.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.5.1/ansys_api_discovery.egg-info/PKG-INFO` & `ansys_api_discovery-0.5.2/ansys_api_discovery.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ansys-api-discovery
-Version: 0.5.1
-Summary: Autogenerated python gRPC interface package for ansys-api-discovery, built on 09:18:40 on 04 October 2023
+Version: 0.5.2
+Summary: Autogenerated python gRPC interface package for ansys-api-discovery, built on 14:18:53 on 26 April 2024
 Home-page: https://github.com/ansys/ansys-api-discovery
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: grpcio~=1.47
 Requires-Dist: protobuf<5,>=3.19
-Requires-Dist: ansys-api-dbu==0.2.1
+Requires-Dist: ansys-api-dbu==0.3.0
 
 ### ansys-api-discovery gRPC Interface Package
 
 This repository provides the auto-generated gRPC Python interface files
 for Discovery/SpaceClaim.
```

### Comparing `ansys-api-discovery-0.5.1/ansys_api_discovery.egg-info/SOURCES.txt` & `ansys_api_discovery-0.5.2/ansys_api_discovery.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 README.md
 pyproject.toml
 setup.py
 ansys/api/discovery/VERSION
 ansys/api/discovery/__init__.py
 ansys/api/discovery/py.typed
 ansys/api/discovery/v0/__init__.py
+ansys/api/discovery/v0/conditions.proto
 ansys/api/discovery/v0/definedvariationstable.proto
 ansys/api/discovery/v0/discoverymodels.proto
 ansys/api/discovery/v0/historytrackparameters.proto
+ansys/api/discovery/v0/messaging.proto
 ansys/api/discovery/v0/scriptparameters.proto
+ansys/api/discovery/v0/simulations.proto
+ansys/api/discovery/v0/solution.proto
 ansys/api/discovery/v0/units.proto
 ansys_api_discovery.egg-info/PKG-INFO
 ansys_api_discovery.egg-info/SOURCES.txt
 ansys_api_discovery.egg-info/dependency_links.txt
 ansys_api_discovery.egg-info/entry_points.txt
 ansys_api_discovery.egg-info/requires.txt
 ansys_api_discovery.egg-info/top_level.txt
```

### Comparing `ansys-api-discovery-0.5.1/setup.py` & `ansys_api_discovery-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         author_email='support@ansys.com',
         description=description,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url=f"https://github.com/ansys/{package_name}",
         license="MIT",
         python_requires=">=3.7",
-        install_requires=["grpcio~=1.47", "protobuf>=3.19,<5", "ansys-api-dbu==0.2.1"],
+        install_requires=["grpcio~=1.47", "protobuf>=3.19,<5", "ansys-api-dbu==0.3.0"],
         packages=setuptools.find_namespace_packages(".", include=("ansys.*",)),
         package_data={
             "": ["*.proto", "*.pyi", "py.typed", "VERSION"],
         },
         entry_points={
             "ansys.tools.protoc_helper.proto_provider": [
                 f"{dot_package_name}={dot_package_name}"
```

