# Comparing `tmp/alibabacloud_cloudauth20190307-2.5.0.tar.gz` & `tmp/alibabacloud_cloudauth20190307-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.5.0.tar", last modified: Wed Apr 10 17:14:47 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.6.0.tar", last modified: Fri Apr 26 07:31:47 2024, max compression
```

## Comparing `alibabacloud_cloudauth20190307-2.5.0.tar` & `alibabacloud_cloudauth20190307-2.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/
--rw-r--r--   0 root         (0) root         (0)     1336 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2449 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1119 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1204 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/__init__.py
--rw-r--r--   0 root         (0) root         (0)   113253 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/client.py
--rw-r--r--   0 root         (0) root         (0)   186651 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2449 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2838 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   117681 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/client.py
+-rw-r--r--   0 root         (0) root         (0)   193806 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2838 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/setup.py
```

### Comparing `alibabacloud_cloudauth20190307-2.5.0/LICENSE` & `alibabacloud_cloudauth20190307-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.5.0/PKG-INFO` & `alibabacloud_cloudauth20190307-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth20190307
-Version: 2.5.0
+Version: 2.6.0
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.5.0/README-CN.md` & `alibabacloud_cloudauth20190307-2.6.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.5.0/README.md` & `alibabacloud_cloudauth20190307-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/client.py` & `alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -899,14 +899,120 @@
     async def create_verify_setting_async(
         self,
         request: cloudauth_20190307_models.CreateVerifySettingRequest,
     ) -> cloudauth_20190307_models.CreateVerifySettingResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_verify_setting_with_options_async(request, runtime)
 
+    def credential_verify_with_options(
+        self,
+        request: cloudauth_20190307_models.CredentialVerifyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.CredentialVerifyResponse:
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
+    async def credential_verify_with_options_async(
+        self,
+        request: cloudauth_20190307_models.CredentialVerifyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.CredentialVerifyResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def credential_verify(
+        self,
+        request: cloudauth_20190307_models.CredentialVerifyRequest,
+    ) -> cloudauth_20190307_models.CredentialVerifyResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.credential_verify_with_options(request, runtime)
+
+    async def credential_verify_async(
+        self,
+        request: cloudauth_20190307_models.CredentialVerifyRequest,
+    ) -> cloudauth_20190307_models.CredentialVerifyResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.credential_verify_with_options_async(request, runtime)
+
     def describe_device_info_with_options(
         self,
         request: cloudauth_20190307_models.DescribeDeviceInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeDeviceInfoResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/models.py` & `alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1455,14 +1455,234 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateVerifySettingResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CredentialVerifyRequest(TeaModel):
+    def __init__(
+        self,
+        cert_num: str = None,
+        cred_name: str = None,
+        cred_type: str = None,
+        identify_num: str = None,
+        image_context: str = None,
+        image_url: str = None,
+        is_check: str = None,
+        is_ocr: str = None,
+        user_name: str = None,
+    ):
+        self.cert_num = cert_num
+        self.cred_name = cred_name
+        self.cred_type = cred_type
+        self.identify_num = identify_num
+        self.image_context = image_context
+        self.image_url = image_url
+        self.is_check = is_check
+        self.is_ocr = is_ocr
+        self.user_name = user_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        ocr_info: str = None,
+        result: str = None,
+        risk_score: Dict[str, str] = None,
+        risk_tag: str = None,
+        verify_detail: str = None,
+        verify_result: str = None,
+    ):
+        self.ocr_info = ocr_info
+        self.result = result
+        self.risk_score = risk_score
+        self.risk_tag = risk_tag
+        self.verify_detail = verify_detail
+        self.verify_result = verify_result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+        result_object: CredentialVerifyResponseBodyResultObject = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result_object = result_object
+
+    def validate(self):
+        if self.result_object:
+            self.result_object.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CredentialVerifyResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         biz_type: str = None,
         current_page: int = None,
         device_id: str = None,
         expired_end_day: str = None,
```

### Comparing `alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/PKG-INFO` & `alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth20190307
-Version: 2.5.0
+Version: 2.6.0
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.5.0/setup.py` & `alibabacloud_cloudauth20190307-2.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth20190307.
 
-Created on 10/04/2024
+Created on 26/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth20190307"
 NAME = "alibabacloud_cloudauth20190307" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ID Verification (20190307) SDK Library for Python"
```

