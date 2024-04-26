# Comparing `tmp/alibabacloud_cloudauth20190307_py2-2.3.0.tar.gz` & `tmp/alibabacloud_cloudauth20190307_py2-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth20190307_py2-2.3.0.tar", last modified: Wed Apr 10 17:13:05 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth20190307_py2-2.4.0.tar", last modified: Fri Apr 26 07:31:13 2024, max compression
```

## Comparing `alibabacloud_cloudauth20190307_py2-2.3.0.tar` & `alibabacloud_cloudauth20190307_py2-2.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/
--rw-r--r--   0 root         (0) root         (0)      378 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2514 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49105 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/client.py
--rw-r--r--   0 root         (0) root         (0)   188030 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2514 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      347 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/
+-rw-r--r--   0 root         (0) root         (0)      572 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51003 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307/client.py
+-rw-r--r--   0 root         (0) root         (0)   195222 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      347 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-26 07:31:13.000000 alibabacloud_cloudauth20190307_py2-2.4.0/setup.py
```

### Comparing `alibabacloud_cloudauth20190307_py2-2.3.0/LICENSE` & `alibabacloud_cloudauth20190307_py2-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307_py2-2.3.0/PKG-INFO` & `alibabacloud_cloudauth20190307_py2-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth20190307_py2
-Version: 2.3.0
+Version: 2.4.0
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307_py2-2.3.0/README-CN.md` & `alibabacloud_cloudauth20190307_py2-2.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307_py2-2.3.0/README.md` & `alibabacloud_cloudauth20190307_py2-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/client.py` & `alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,14 +408,60 @@
             self.call_api(params, req, runtime)
         )
 
     def create_verify_setting(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_verify_setting_with_options(request, runtime)
 
+    def credential_verify_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cert_num):
+            query['CertNum'] = request.cert_num
+        if not UtilClient.is_unset(request.cred_name):
+            query['CredName'] = request.cred_name
+        if not UtilClient.is_unset(request.cred_type):
+            query['CredType'] = request.cred_type
+        if not UtilClient.is_unset(request.identify_num):
+            query['IdentifyNum'] = request.identify_num
+        if not UtilClient.is_unset(request.image_url):
+            query['ImageUrl'] = request.image_url
+        if not UtilClient.is_unset(request.is_check):
+            query['IsCheck'] = request.is_check
+        if not UtilClient.is_unset(request.is_ocr):
+            query['IsOCR'] = request.is_ocr
+        if not UtilClient.is_unset(request.user_name):
+            query['UserName'] = request.user_name
+        body = {}
+        if not UtilClient.is_unset(request.image_context):
+            body['ImageContext'] = request.image_context
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CredentialVerify',
+            version='2019-03-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudauth_20190307_models.CredentialVerifyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def credential_verify(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.credential_verify_with_options(request, runtime)
+
     def describe_device_info_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
```

### Comparing `alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/models.py` & `alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1269,14 +1269,206 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateVerifySettingResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CredentialVerifyRequest(TeaModel):
+    def __init__(self, cert_num=None, cred_name=None, cred_type=None, identify_num=None, image_context=None,
+                 image_url=None, is_check=None, is_ocr=None, user_name=None):
+        self.cert_num = cert_num  # type: str
+        self.cred_name = cred_name  # type: str
+        self.cred_type = cred_type  # type: str
+        self.identify_num = identify_num  # type: str
+        self.image_context = image_context  # type: str
+        self.image_url = image_url  # type: str
+        self.is_check = is_check  # type: str
+        self.is_ocr = is_ocr  # type: str
+        self.user_name = user_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CredentialVerifyRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cert_num is not None:
+            result['CertNum'] = self.cert_num
+        if self.cred_name is not None:
+            result['CredName'] = self.cred_name
+        if self.cred_type is not None:
+            result['CredType'] = self.cred_type
+        if self.identify_num is not None:
+            result['IdentifyNum'] = self.identify_num
+        if self.image_context is not None:
+            result['ImageContext'] = self.image_context
+        if self.image_url is not None:
+            result['ImageUrl'] = self.image_url
+        if self.is_check is not None:
+            result['IsCheck'] = self.is_check
+        if self.is_ocr is not None:
+            result['IsOCR'] = self.is_ocr
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CertNum') is not None:
+            self.cert_num = m.get('CertNum')
+        if m.get('CredName') is not None:
+            self.cred_name = m.get('CredName')
+        if m.get('CredType') is not None:
+            self.cred_type = m.get('CredType')
+        if m.get('IdentifyNum') is not None:
+            self.identify_num = m.get('IdentifyNum')
+        if m.get('ImageContext') is not None:
+            self.image_context = m.get('ImageContext')
+        if m.get('ImageUrl') is not None:
+            self.image_url = m.get('ImageUrl')
+        if m.get('IsCheck') is not None:
+            self.is_check = m.get('IsCheck')
+        if m.get('IsOCR') is not None:
+            self.is_ocr = m.get('IsOCR')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        return self
+
+
+class CredentialVerifyResponseBodyResultObject(TeaModel):
+    def __init__(self, ocr_info=None, result=None, risk_score=None, risk_tag=None, verify_detail=None,
+                 verify_result=None):
+        self.ocr_info = ocr_info  # type: str
+        self.result = result  # type: str
+        self.risk_score = risk_score  # type: dict[str, str]
+        self.risk_tag = risk_tag  # type: str
+        self.verify_detail = verify_detail  # type: str
+        self.verify_result = verify_result  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CredentialVerifyResponseBodyResultObject, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ocr_info is not None:
+            result['OcrInfo'] = self.ocr_info
+        if self.result is not None:
+            result['Result'] = self.result
+        if self.risk_score is not None:
+            result['RiskScore'] = self.risk_score
+        if self.risk_tag is not None:
+            result['RiskTag'] = self.risk_tag
+        if self.verify_detail is not None:
+            result['VerifyDetail'] = self.verify_detail
+        if self.verify_result is not None:
+            result['VerifyResult'] = self.verify_result
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('OcrInfo') is not None:
+            self.ocr_info = m.get('OcrInfo')
+        if m.get('Result') is not None:
+            self.result = m.get('Result')
+        if m.get('RiskScore') is not None:
+            self.risk_score = m.get('RiskScore')
+        if m.get('RiskTag') is not None:
+            self.risk_tag = m.get('RiskTag')
+        if m.get('VerifyDetail') is not None:
+            self.verify_detail = m.get('VerifyDetail')
+        if m.get('VerifyResult') is not None:
+            self.verify_result = m.get('VerifyResult')
+        return self
+
+
+class CredentialVerifyResponseBody(TeaModel):
+    def __init__(self, code=None, message=None, request_id=None, result_object=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+        self.result_object = result_object  # type: CredentialVerifyResponseBodyResultObject
+
+    def validate(self):
+        if self.result_object:
+            self.result_object.validate()
+
+    def to_map(self):
+        _map = super(CredentialVerifyResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result_object is not None:
+            result['ResultObject'] = self.result_object.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResultObject') is not None:
+            temp_model = CredentialVerifyResponseBodyResultObject()
+            self.result_object = temp_model.from_map(m['ResultObject'])
+        return self
+
+
+class CredentialVerifyResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CredentialVerifyResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CredentialVerifyResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CredentialVerifyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeDeviceInfoRequest(TeaModel):
     def __init__(self, biz_type=None, current_page=None, device_id=None, expired_end_day=None,
                  expired_start_day=None, page_size=None, user_device_id=None):
         self.biz_type = biz_type  # type: str
         self.current_page = current_page  # type: int
         self.device_id = device_id  # type: str
         self.expired_end_day = expired_end_day  # type: str
```

### Comparing `alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/PKG-INFO` & `alibabacloud_cloudauth20190307_py2-2.4.0/alibabacloud_cloudauth20190307_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth20190307-py2
-Version: 2.3.0
+Version: 2.4.0
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307_py2-2.3.0/setup.py` & `alibabacloud_cloudauth20190307_py2-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth20190307_py2.
 
-Created on 10/04/2024
+Created on 26/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth20190307"
 NAME = "alibabacloud_cloudauth20190307_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ID Verification (20190307) SDK Library for Python2"
```

