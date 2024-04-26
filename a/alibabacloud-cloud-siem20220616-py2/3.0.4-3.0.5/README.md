# Comparing `tmp/alibabacloud_cloud-siem20220616_py2-3.0.4.tar.gz` & `tmp/alibabacloud_cloud-siem20220616_py2-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloud-siem20220616_py2-3.0.4.tar", last modified: Wed Apr 17 17:12:44 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloud-siem20220616_py2-3.0.5.tar", last modified: Fri Apr 26 17:08:07 2024, max compression
```

## Comparing `alibabacloud_cloud-siem20220616_py2-3.0.4.tar` & `alibabacloud_cloud-siem20220616_py2-3.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/
--rw-r--r--   0 root         (0) root         (0)      699 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2514 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1054 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/__init__.py
--rw-r--r--   0 root         (0) root         (0)   156866 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/client.py
--rw-r--r--   0 root         (0) root         (0)   893445 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2514 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2940 2024-04-17 17:12:44.000000 alibabacloud_cloud-siem20220616_py2-3.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:08:07.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/
+-rw-r--r--   0 root         (0) root         (0)     9323 2024-04-26 17:08:06.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-26 17:08:06.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-26 17:08:06.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-26 17:08:07.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-26 17:08:06.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-26 17:08:06.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:08:07.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-26 17:08:06.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   157276 2024-04-26 17:08:06.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616/client.py
+-rw-r--r--   0 root         (0) root         (0)   894389 2024-04-26 17:08:06.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:08:07.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-26 17:08:07.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2024-04-26 17:08:07.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 17:08:07.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-26 17:08:07.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-26 17:08:07.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 17:08:07.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2940 2024-04-26 17:08:06.000000 alibabacloud_cloud-siem20220616_py2-3.0.5/setup.py
```

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.4/LICENSE` & `alibabacloud_cloud-siem20220616_py2-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.4/PKG-INFO` & `alibabacloud_cloud-siem20220616_py2-3.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloud-siem20220616_py2
-Version: 3.0.4
+Version: 3.0.5
 Summary: Alibaba Cloud cloud-siem (20220616) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.4/README-CN.md` & `alibabacloud_cloud-siem20220616_py2-3.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.4/README.md` & `alibabacloud_cloud-siem20220616_py2-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/client.py` & `alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3143,14 +3143,18 @@
         return self.list_rd_users_with_options(request, runtime)
 
     def list_user_prod_logs_with_options(self, request, runtime):
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
@@ -3175,14 +3179,18 @@
         return self.list_user_prod_logs_with_options(request, runtime)
 
     def list_users_by_prod_with_options(self, request, runtime):
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

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616/models.py` & `alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -19841,20 +19841,22 @@
         if m.get('body') is not None:
             temp_model = ListRdUsersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListUserProdLogsRequest(TeaModel):
-    def __init__(self, region_id=None, source_log_code=None, source_prod_code=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None, source_log_code=None, source_prod_code=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The log code.
         self.source_log_code = source_log_code  # type: str
         # The code of the cloud service.
         self.source_prod_code = source_prod_code  # type: str
 
     def validate(self):
         pass
@@ -19863,24 +19865,32 @@
         _map = super(ListUserProdLogsRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
 
 
@@ -20045,42 +20055,52 @@
         if m.get('body') is not None:
             temp_model = ListUserProdLogsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListUsersByProdRequest(TeaModel):
-    def __init__(self, region_id=None, source_prod_code=None):
+    def __init__(self, region_id=None, role_for=None, role_type=None, source_prod_code=None):
         # The region in which the data management center of the threat analysis feature resides. Specify this parameter based on the regions in which your assets reside. Valid values:
         # 
         # *   cn-hangzhou: Your assets reside in regions in China.
         # *   ap-southeast-1: Your assets reside in regions outside China.
         self.region_id = region_id  # type: str
+        self.role_for = role_for  # type: long
+        self.role_type = role_type  # type: int
         # The code of the cloud service.
         self.source_prod_code = source_prod_code  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListUsersByProdRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, cloud_code=None, imported=None, log_mds_code=None, main_user_id=None, source_log_code=None,
```

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.4/alibabacloud_cloud_siem20220616_py2.egg-info/PKG-INFO` & `alibabacloud_cloud-siem20220616_py2-3.0.5/alibabacloud_cloud_siem20220616_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloud-siem20220616-py2
-Version: 3.0.4
+Version: 3.0.5
 Summary: Alibaba Cloud cloud-siem (20220616) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloud-siem20220616_py2-3.0.4/setup.py` & `alibabacloud_cloud-siem20220616_py2-3.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloud-siem20220616_py2.
 
-Created on 17/04/2024
+Created on 26/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloud_siem20220616"
 NAME = "alibabacloud_cloud-siem20220616_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cloud-siem (20220616) SDK Library for Python2"
```

