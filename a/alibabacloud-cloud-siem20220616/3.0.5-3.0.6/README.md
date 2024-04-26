# Comparing `tmp/alibabacloud_cloud-siem20220616-3.0.5.tar.gz` & `tmp/alibabacloud_cloud-siem20220616-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloud-siem20220616-3.0.5.tar", last modified: Wed Apr 17 17:15:00 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloud-siem20220616-3.0.6.tar", last modified: Fri Apr 26 17:08:51 2024, max compression
```

## Comparing `alibabacloud_cloud-siem20220616-3.0.5.tar` & `alibabacloud_cloud-siem20220616-3.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/
--rw-r--r--   0 root         (0) root         (0)      840 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2450 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1123 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1208 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/__init__.py
--rw-r--r--   0 root         (0) root         (0)   385500 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/client.py
--rw-r--r--   0 root         (0) root         (0)   887867 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2450 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 17:15:00.000000 alibabacloud_cloud-siem20220616-3.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2648 2024-04-17 17:14:59.000000 alibabacloud_cloud-siem20220616-3.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:08:51.000000 alibabacloud_cloud-siem20220616-3.0.6/
+-rw-r--r--   0 root         (0) root         (0)     9464 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-26 17:08:51.000000 alibabacloud_cloud-siem20220616-3.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:08:51.000000 alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   386320 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616/client.py
+-rw-r--r--   0 root         (0) root         (0)   888817 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:08:51.000000 alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-26 17:08:51.000000 alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 17:08:51.000000 alibabacloud_cloud-siem20220616-3.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-04-26 17:08:50.000000 alibabacloud_cloud-siem20220616-3.0.6/setup.py
```

### Comparing `alibabacloud_cloud-siem20220616-3.0.5/LICENSE` & `alibabacloud_cloud-siem20220616-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616-3.0.5/PKG-INFO` & `alibabacloud_cloud-siem20220616-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloud-siem20220616
-Version: 3.0.5
+Version: 3.0.6
 Summary: Alibaba Cloud cloud-siem (20220616) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloud-siem20220616-3.0.5/README-CN.md` & `alibabacloud_cloud-siem20220616-3.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616-3.0.5/README.md` & `alibabacloud_cloud-siem20220616-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/client.py` & `alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -7502,14 +7502,18 @@
         request: cloud_siem_20220616_models.ListUserProdLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.ListUserProdLogsResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.source_log_code):
             body['SourceLogCode'] = request.source_log_code
         if not UtilClient.is_unset(request.source_prod_code):
             body['SourceProdCode'] = request.source_prod_code
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -7534,14 +7538,18 @@
         request: cloud_siem_20220616_models.ListUserProdLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.ListUserProdLogsResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.source_log_code):
             body['SourceLogCode'] = request.source_log_code
         if not UtilClient.is_unset(request.source_prod_code):
             body['SourceProdCode'] = request.source_prod_code
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -7580,14 +7588,18 @@
         request: cloud_siem_20220616_models.ListUsersByProdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.ListUsersByProdResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.source_prod_code):
             body['SourceProdCode'] = request.source_prod_code
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListUsersByProd',
@@ -7610,14 +7622,18 @@
         request: cloud_siem_20220616_models.ListUsersByProdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_siem_20220616_models.ListUsersByProdResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.role_for):
+            body['RoleFor'] = request.role_for
+        if not UtilClient.is_unset(request.role_type):
+            body['RoleType'] = request.role_type
         if not UtilClient.is_unset(request.source_prod_code):
             body['SourceProdCode'] = request.source_prod_code
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ListUsersByProd',
```

### Comparing `alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616/models.py` & `alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -22314,22 +22314,26 @@
         return self
 
 
 class ListUserProdLogsRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         source_log_code: str = None,
         source_prod_code: str = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The log code.
         self.source_log_code = source_log_code
         # The code of the cloud service.
         self.source_prod_code = source_prod_code
 
     def validate(self):
         pass
@@ -22338,24 +22342,32 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.source_log_code is not None:
             result['SourceLogCode'] = self.source_log_code
         if self.source_prod_code is not None:
             result['SourceProdCode'] = self.source_prod_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('SourceLogCode') is not None:
             self.source_log_code = m.get('SourceLogCode')
         if m.get('SourceProdCode') is not None:
             self.source_prod_code = m.get('SourceProdCode')
         return self
 
 
@@ -22543,43 +22555,55 @@
         return self
 
 
 class ListUsersByProdRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
+        role_for: int = None,
+        role_type: int = None,
         source_prod_code: str = None,
     ):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id
+        self.role_for = role_for
+        self.role_type = role_type
         # The code of the cloud service.
         self.source_prod_code = source_prod_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.role_for is not None:
+            result['RoleFor'] = self.role_for
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
         if self.source_prod_code is not None:
             result['SourceProdCode'] = self.source_prod_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RoleFor') is not None:
+            self.role_for = m.get('RoleFor')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
         if m.get('SourceProdCode') is not None:
             self.source_prod_code = m.get('SourceProdCode')
         return self
 
 
 class ListUsersByProdResponseBodyData(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_cloud-siem20220616-3.0.5/alibabacloud_cloud_siem20220616.egg-info/PKG-INFO` & `alibabacloud_cloud-siem20220616-3.0.6/alibabacloud_cloud_siem20220616.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloud-siem20220616
-Version: 3.0.5
+Version: 3.0.6
 Summary: Alibaba Cloud cloud-siem (20220616) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloud-siem20220616-3.0.5/setup.py` & `alibabacloud_cloud-siem20220616-3.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloud-siem20220616.
 
-Created on 17/04/2024
+Created on 26/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloud_siem20220616"
 NAME = "alibabacloud_cloud-siem20220616" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cloud-siem (20220616) SDK Library for Python"
```

