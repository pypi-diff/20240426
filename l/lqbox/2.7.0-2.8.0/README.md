# Comparing `tmp/lqbox-2.7.0.tar.gz` & `tmp/lqbox-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqbox-2.7.0.tar", max compression
+gzip compressed data, was "lqbox-2.8.0.tar", max compression
```

## Comparing `lqbox-2.7.0.tar` & `lqbox-2.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1091 2024-03-20 09:46:12.799882 lqbox-2.7.0/LICENSE
--rw-r--r--   0        0        0      322 2024-04-17 09:22:35.882463 lqbox-2.7.0/pyproject.toml
--rw-r--r--   0        0        0       30 2024-03-20 09:46:12.799882 lqbox-2.7.0/README.md
--rw-r--r--   0        0        0      143 2024-03-20 09:46:12.801882 lqbox-2.7.0/src/lqbox/__init__.py
--rw-r--r--   0        0        0     2705 2024-04-09 01:53:28.324154 lqbox-2.7.0/src/lqbox/ali/__init__.py
--rw-r--r--   0        0        0     1289 2024-03-20 09:46:12.801882 lqbox-2.7.0/src/lqbox/base/__init__.py
--rw-r--r--   0        0        0     2970 2024-04-10 08:12:43.668992 lqbox-2.7.0/src/lqbox/bidp/__init__.py
--rw-r--r--   0        0        0     2975 2024-03-20 09:46:12.802882 lqbox-2.7.0/src/lqbox/elihu/__init__.py
--rw-r--r--   0        0        0     1834 2024-03-20 09:46:12.802882 lqbox-2.7.0/src/lqbox/mc/__init__.py
--rw-r--r--   0        0        0     2421 2024-04-11 07:20:15.936012 lqbox-2.7.0/src/lqbox/oc/__init__.py
--rw-r--r--   0        0        0     2324 2024-03-20 09:46:12.803882 lqbox-2.7.0/src/lqbox/open_bidp/__init__.py
--rw-r--r--   0        0        0     4031 2024-04-17 09:22:35.887463 lqbox-2.7.0/src/lqbox/open_elihu/__init__.py
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 lqbox-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-03-20 09:46:12.799882 lqbox-2.8.0/LICENSE
+-rw-r--r--   0        0        0      322 2024-04-26 07:44:51.325533 lqbox-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2024-03-20 09:46:12.799882 lqbox-2.8.0/README.md
+-rw-r--r--   0        0        0      143 2024-03-20 09:46:12.801882 lqbox-2.8.0/src/lqbox/__init__.py
+-rw-r--r--   0        0        0     2705 2024-04-09 01:53:28.324154 lqbox-2.8.0/src/lqbox/ali/__init__.py
+-rw-r--r--   0        0        0     1289 2024-03-20 09:46:12.801882 lqbox-2.8.0/src/lqbox/base/__init__.py
+-rw-r--r--   0        0        0     2970 2024-04-10 08:12:43.668992 lqbox-2.8.0/src/lqbox/bidp/__init__.py
+-rw-r--r--   0        0        0     2975 2024-03-20 09:46:12.802882 lqbox-2.8.0/src/lqbox/elihu/__init__.py
+-rw-r--r--   0        0        0     1834 2024-03-20 09:46:12.802882 lqbox-2.8.0/src/lqbox/mc/__init__.py
+-rw-r--r--   0        0        0     2421 2024-04-11 07:20:15.936012 lqbox-2.8.0/src/lqbox/oc/__init__.py
+-rw-r--r--   0        0        0     3037 2024-04-26 07:44:26.309415 lqbox-2.8.0/src/lqbox/open_bidp/__init__.py
+-rw-r--r--   0        0        0     4031 2024-04-17 09:22:35.887463 lqbox-2.8.0/src/lqbox/open_elihu/__init__.py
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 lqbox-2.8.0/PKG-INFO
```

### Comparing `lqbox-2.7.0/LICENSE` & `lqbox-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lqbox-2.7.0/src/lqbox/ali/__init__.py` & `lqbox-2.8.0/src/lqbox/ali/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.7.0/src/lqbox/base/__init__.py` & `lqbox-2.8.0/src/lqbox/base/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.7.0/src/lqbox/bidp/__init__.py` & `lqbox-2.8.0/src/lqbox/bidp/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.7.0/src/lqbox/elihu/__init__.py` & `lqbox-2.8.0/src/lqbox/elihu/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.7.0/src/lqbox/mc/__init__.py` & `lqbox-2.8.0/src/lqbox/mc/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.7.0/src/lqbox/oc/__init__.py` & `lqbox-2.8.0/src/lqbox/oc/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.7.0/src/lqbox/open_bidp/__init__.py` & `lqbox-2.8.0/src/lqbox/open_bidp/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 @Project : lqbox 
 @File    : __init__.py
 @Date    : 2023/8/31 13:01:27
 @Author  : zhchen
 @Desc    : 
 """
 import uuid
+from typing import Optional
 
 from requests import Response
 
 from lqbox.base import BaseBox
 
 
 class OpenBidpBox(BaseBox):
@@ -51,8 +52,25 @@
         if platform_code is not None:
             d['platformCode'] = platform_code
         return self.request_open_api('AccountOpenApi/getAccountsWithoutLongSession', body=d)
 
     def call_search_data_fetch_records(self, request_entity: dict):
         """检查之前的数据落盘记录，在补录场景下可以减少重复取数"""
         # request_entity的key: shovelProject, shovelClass, limit, aspect, partKey, timeRange, mizarGroupId
-        return self.request_open_api('RecordOpenApiController/searchDataFetchRecords', body=request_entity)
+        return self.request_open_api('RecordOpenApiController/searchDataFetchRecords', body=request_entity)
+
+    def call_get_account_related_available_sessions(
+            self, account_id: int, platform_code: str,
+            status: Optional[str] = None, limit: Optional[int] = None):
+        """查找某个账号是否有可用会话 (获取session)"""
+        dictionary = {
+            'accountId': account_id,
+            'platformCode': platform_code,
+        }
+        if status is not None:
+            dictionary['status'] = status
+        if limit is not None:
+            dictionary['limit'] = limit
+        else:
+            dictionary['limit'] = 1
+
+        return self.request_open_api("AccountOpenApi/getAccountRelatedAvailableSessions", body=dictionary)
```

### Comparing `lqbox-2.7.0/src/lqbox/open_elihu/__init__.py` & `lqbox-2.8.0/src/lqbox/open_elihu/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.7.0/PKG-INFO` & `lqbox-2.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqbox
-Version: 2.7.0
+Version: 2.8.0
 Summary: lqbox
 License: MIT
 Author: luke9012
 Author-email: luke781520097@163.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

