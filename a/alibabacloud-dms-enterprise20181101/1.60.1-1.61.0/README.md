# Comparing `tmp/alibabacloud_dms-enterprise20181101-1.60.1.tar.gz` & `tmp/alibabacloud_dms-enterprise20181101-1.61.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101-1.60.1.tar", last modified: Thu Apr 18 04:31:55 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101-1.61.0.tar", last modified: Fri Apr 26 09:51:35 2024, max compression
```

## Comparing `alibabacloud_dms-enterprise20181101-1.60.1.tar` & `alibabacloud_dms-enterprise20181101-1.61.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/
--rw-r--r--   0 root         (0) root         (0)     8187 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2479 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1139 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1224 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   882527 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/client.py
--rw-r--r--   0 root         (0) root         (0)  2024361 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2479 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2668 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/
+-rw-r--r--   0 root         (0) root         (0)     8333 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2479 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1224 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   888511 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101/client.py
+-rw-r--r--   0 root         (0) root         (0)  2041183 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2479 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2668 2024-04-26 09:51:35.000000 alibabacloud_dms-enterprise20181101-1.61.0/setup.py
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.1/ChangeLog.md` & `alibabacloud_dms-enterprise20181101-1.61.0/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-04-18 Version: 1.60.1
+- Update API ApproveOrder: add param NewApproverList.
+- Update API GetDataCorrectOrderDetail: update response param.
+
+
 2024-04-16 Version: 1.60.0
 - Support API ListSensitiveColumnInfo.
 
 
 2024-03-27 Version: 1.59.1
 - Update API AddInstance: add param UseSsl.
 - Update API ModifyInstance: add param UseSsl.
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.1/LICENSE` & `alibabacloud_dms-enterprise20181101-1.61.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.60.1/PKG-INFO` & `alibabacloud_dms-enterprise20181101-1.61.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dms-enterprise20181101
-Version: 1.60.1
+Version: 1.61.0
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.1/README-CN.md` & `alibabacloud_dms-enterprise20181101-1.61.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.60.1/README.md` & `alibabacloud_dms-enterprise20181101-1.61.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/client.py` & `alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10173,14 +10173,162 @@
     async def get_table_dbtopology_async(
         self,
         request: dms_enterprise_20181101_models.GetTableDBTopologyRequest,
     ) -> dms_enterprise_20181101_models.GetTableDBTopologyResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_table_dbtopology_with_options_async(request, runtime)
 
+    def get_table_design_project_flow_with_options(
+        self,
+        request: dms_enterprise_20181101_models.GetTableDesignProjectFlowRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetTableDesignProjectFlowResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetTableDesignProjectFlow',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetTableDesignProjectFlowResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_table_design_project_flow_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.GetTableDesignProjectFlowRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetTableDesignProjectFlowResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetTableDesignProjectFlow',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetTableDesignProjectFlowResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_table_design_project_flow(
+        self,
+        request: dms_enterprise_20181101_models.GetTableDesignProjectFlowRequest,
+    ) -> dms_enterprise_20181101_models.GetTableDesignProjectFlowResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_table_design_project_flow_with_options(request, runtime)
+
+    async def get_table_design_project_flow_async(
+        self,
+        request: dms_enterprise_20181101_models.GetTableDesignProjectFlowRequest,
+    ) -> dms_enterprise_20181101_models.GetTableDesignProjectFlowResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_table_design_project_flow_with_options_async(request, runtime)
+
+    def get_table_design_project_info_with_options(
+        self,
+        request: dms_enterprise_20181101_models.GetTableDesignProjectInfoRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetTableDesignProjectInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetTableDesignProjectInfo',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetTableDesignProjectInfoResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_table_design_project_info_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.GetTableDesignProjectInfoRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetTableDesignProjectInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetTableDesignProjectInfo',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetTableDesignProjectInfoResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_table_design_project_info(
+        self,
+        request: dms_enterprise_20181101_models.GetTableDesignProjectInfoRequest,
+    ) -> dms_enterprise_20181101_models.GetTableDesignProjectInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_table_design_project_info_with_options(request, runtime)
+
+    async def get_table_design_project_info_async(
+        self,
+        request: dms_enterprise_20181101_models.GetTableDesignProjectInfoRequest,
+    ) -> dms_enterprise_20181101_models.GetTableDesignProjectInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_table_design_project_info_with_options_async(request, runtime)
+
     def get_table_topology_with_options(
         self,
         request: dms_enterprise_20181101_models.GetTableTopologyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetTableTopologyResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/models.py` & `alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -28116,14 +28116,524 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetTableDBTopologyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetTableDesignProjectFlowRequest(TeaModel):
+    def __init__(
+        self,
+        order_id: int = None,
+        tid: int = None,
+    ):
+        self.order_id = order_id
+        self.tid = tid
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
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetTableDesignProjectFlowResponseBodyProjectFlowFlowNodeArray(TeaModel):
+    def __init__(
+        self,
+        back_to_design: bool = None,
+        can_skip: bool = None,
+        node_role: str = None,
+        node_title: str = None,
+        position: int = None,
+        publish_anchor: bool = None,
+        publish_strategies: List[str] = None,
+    ):
+        self.back_to_design = back_to_design
+        self.can_skip = can_skip
+        self.node_role = node_role
+        self.node_title = node_title
+        self.position = position
+        self.publish_anchor = publish_anchor
+        self.publish_strategies = publish_strategies
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
+        if self.back_to_design is not None:
+            result['BackToDesign'] = self.back_to_design
+        if self.can_skip is not None:
+            result['CanSkip'] = self.can_skip
+        if self.node_role is not None:
+            result['NodeRole'] = self.node_role
+        if self.node_title is not None:
+            result['NodeTitle'] = self.node_title
+        if self.position is not None:
+            result['Position'] = self.position
+        if self.publish_anchor is not None:
+            result['PublishAnchor'] = self.publish_anchor
+        if self.publish_strategies is not None:
+            result['PublishStrategies'] = self.publish_strategies
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BackToDesign') is not None:
+            self.back_to_design = m.get('BackToDesign')
+        if m.get('CanSkip') is not None:
+            self.can_skip = m.get('CanSkip')
+        if m.get('NodeRole') is not None:
+            self.node_role = m.get('NodeRole')
+        if m.get('NodeTitle') is not None:
+            self.node_title = m.get('NodeTitle')
+        if m.get('Position') is not None:
+            self.position = m.get('Position')
+        if m.get('PublishAnchor') is not None:
+            self.publish_anchor = m.get('PublishAnchor')
+        if m.get('PublishStrategies') is not None:
+            self.publish_strategies = m.get('PublishStrategies')
+        return self
+
+
+class GetTableDesignProjectFlowResponseBodyProjectFlow(TeaModel):
+    def __init__(
+        self,
+        current_position: int = None,
+        flow_node_array: List[GetTableDesignProjectFlowResponseBodyProjectFlowFlowNodeArray] = None,
+        rule_comment: str = None,
+        rule_name: str = None,
+    ):
+        self.current_position = current_position
+        self.flow_node_array = flow_node_array
+        self.rule_comment = rule_comment
+        self.rule_name = rule_name
+
+    def validate(self):
+        if self.flow_node_array:
+            for k in self.flow_node_array:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_position is not None:
+            result['CurrentPosition'] = self.current_position
+        result['FlowNodeArray'] = []
+        if self.flow_node_array is not None:
+            for k in self.flow_node_array:
+                result['FlowNodeArray'].append(k.to_map() if k else None)
+        if self.rule_comment is not None:
+            result['RuleComment'] = self.rule_comment
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CurrentPosition') is not None:
+            self.current_position = m.get('CurrentPosition')
+        self.flow_node_array = []
+        if m.get('FlowNodeArray') is not None:
+            for k in m.get('FlowNodeArray'):
+                temp_model = GetTableDesignProjectFlowResponseBodyProjectFlowFlowNodeArray()
+                self.flow_node_array.append(temp_model.from_map(k))
+        if m.get('RuleComment') is not None:
+            self.rule_comment = m.get('RuleComment')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        return self
+
+
+class GetTableDesignProjectFlowResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_code: str = None,
+        error_message: str = None,
+        project_flow: GetTableDesignProjectFlowResponseBodyProjectFlow = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.error_code = error_code
+        self.error_message = error_message
+        self.project_flow = project_flow
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.project_flow:
+            self.project_flow.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.project_flow is not None:
+            result['ProjectFlow'] = self.project_flow.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('ProjectFlow') is not None:
+            temp_model = GetTableDesignProjectFlowResponseBodyProjectFlow()
+            self.project_flow = temp_model.from_map(m['ProjectFlow'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetTableDesignProjectFlowResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetTableDesignProjectFlowResponseBody = None,
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
+            temp_model = GetTableDesignProjectFlowResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetTableDesignProjectInfoRequest(TeaModel):
+    def __init__(
+        self,
+        order_id: int = None,
+        tid: int = None,
+    ):
+        self.order_id = order_id
+        self.tid = tid
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
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetTableDesignProjectInfoResponseBodyProjectInfoBaseDatabase(TeaModel):
+    def __init__(
+        self,
+        alias: str = None,
+        db_id: int = None,
+        db_type: str = None,
+        env_type: str = None,
+        logic: bool = None,
+        schema_name: str = None,
+        search_name: str = None,
+    ):
+        self.alias = alias
+        self.db_id = db_id
+        self.db_type = db_type
+        self.env_type = env_type
+        self.logic = logic
+        self.schema_name = schema_name
+        self.search_name = search_name
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
+        if self.alias is not None:
+            result['Alias'] = self.alias
+        if self.db_id is not None:
+            result['DbId'] = self.db_id
+        if self.db_type is not None:
+            result['DbType'] = self.db_type
+        if self.env_type is not None:
+            result['EnvType'] = self.env_type
+        if self.logic is not None:
+            result['Logic'] = self.logic
+        if self.schema_name is not None:
+            result['SchemaName'] = self.schema_name
+        if self.search_name is not None:
+            result['SearchName'] = self.search_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Alias') is not None:
+            self.alias = m.get('Alias')
+        if m.get('DbId') is not None:
+            self.db_id = m.get('DbId')
+        if m.get('DbType') is not None:
+            self.db_type = m.get('DbType')
+        if m.get('EnvType') is not None:
+            self.env_type = m.get('EnvType')
+        if m.get('Logic') is not None:
+            self.logic = m.get('Logic')
+        if m.get('SchemaName') is not None:
+            self.schema_name = m.get('SchemaName')
+        if m.get('SearchName') is not None:
+            self.search_name = m.get('SearchName')
+        return self
+
+
+class GetTableDesignProjectInfoResponseBodyProjectInfo(TeaModel):
+    def __init__(
+        self,
+        base_database: GetTableDesignProjectInfoResponseBodyProjectInfoBaseDatabase = None,
+        creator_id: int = None,
+        description: str = None,
+        gmt_create: str = None,
+        gmt_modified: str = None,
+        order_id: int = None,
+        project_id: int = None,
+        status: str = None,
+        title: str = None,
+    ):
+        self.base_database = base_database
+        self.creator_id = creator_id
+        self.description = description
+        self.gmt_create = gmt_create
+        self.gmt_modified = gmt_modified
+        self.order_id = order_id
+        self.project_id = project_id
+        self.status = status
+        self.title = title
+
+    def validate(self):
+        if self.base_database:
+            self.base_database.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.base_database is not None:
+            result['BaseDatabase'] = self.base_database.to_map()
+        if self.creator_id is not None:
+            result['CreatorId'] = self.creator_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.gmt_create is not None:
+            result['GmtCreate'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.project_id is not None:
+            result['ProjectId'] = self.project_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.title is not None:
+            result['Title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BaseDatabase') is not None:
+            temp_model = GetTableDesignProjectInfoResponseBodyProjectInfoBaseDatabase()
+            self.base_database = temp_model.from_map(m['BaseDatabase'])
+        if m.get('CreatorId') is not None:
+            self.creator_id = m.get('CreatorId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('GmtCreate') is not None:
+            self.gmt_create = m.get('GmtCreate')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('ProjectId') is not None:
+            self.project_id = m.get('ProjectId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        return self
+
+
+class GetTableDesignProjectInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_code: str = None,
+        error_message: str = None,
+        project_info: GetTableDesignProjectInfoResponseBodyProjectInfo = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.error_code = error_code
+        self.error_message = error_message
+        self.project_info = project_info
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.project_info:
+            self.project_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.project_info is not None:
+            result['ProjectInfo'] = self.project_info.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('ProjectInfo') is not None:
+            temp_model = GetTableDesignProjectInfoResponseBodyProjectInfo()
+            self.project_info = temp_model.from_map(m['ProjectInfo'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetTableDesignProjectInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetTableDesignProjectInfoResponseBody = None,
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
+            temp_model = GetTableDesignProjectInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetTableTopologyRequest(TeaModel):
     def __init__(
         self,
         table_guid: str = None,
         tid: int = None,
     ):
         # The GUID of the table in Data Management (DMS).
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO` & `alibabacloud_dms-enterprise20181101-1.61.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dms-enterprise20181101
-Version: 1.60.1
+Version: 1.61.0
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.1/setup.py` & `alibabacloud_dms-enterprise20181101-1.61.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dms-enterprise20181101.
 
-Created on 18/04/2024
+Created on 26/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dms_enterprise20181101"
 NAME = "alibabacloud_dms-enterprise20181101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dms-enterprise (20181101) SDK Library for Python"
```

