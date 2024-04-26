# Comparing `tmp/alibabacloud_dms-enterprise20181101_py2-1.19.1.tar.gz` & `tmp/alibabacloud_dms-enterprise20181101_py2-1.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101_py2-1.19.1.tar", last modified: Thu Apr 18 04:31:23 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101_py2-1.20.0.tar", last modified: Fri Apr 26 09:51:02 2024, max compression
```

## Comparing `alibabacloud_dms-enterprise20181101_py2-1.19.1.tar` & `alibabacloud_dms-enterprise20181101_py2-1.20.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/
--rw-r--r--   0 root         (0) root         (0)     1829 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2539 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   364338 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101/client.py
--rw-r--r--   0 root         (0) root         (0)  2041641 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2539 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      528 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2960 2024-04-18 04:31:23.000000 alibabacloud_dms-enterprise20181101_py2-1.19.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/
+-rw-r--r--   0 root         (0) root         (0)     1975 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   366586 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101/client.py
+-rw-r--r--   0 root         (0) root         (0)  2058678 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      528 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2960 2024-04-26 09:51:02.000000 alibabacloud_dms-enterprise20181101_py2-1.20.0/setup.py
```

### Comparing `alibabacloud_dms-enterprise20181101_py2-1.19.1/ChangeLog.md` & `alibabacloud_dms-enterprise20181101_py2-1.20.0/ChangeLog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-04-18 Version: 1.19.1
+- Update API ApproveOrder: add param NewApproverList.
+- Update API GetDataCorrectOrderDetail: update response param.
+
+
 2024-04-16 Version: 1.19.0
 - Support API ListSensitiveColumnInfo.
 
 
 2024-03-27 Version: 1.18.1
 - Update API AddInstance: add param UseSsl.
 - Update API ModifyInstance: add param UseSsl.
```

### Comparing `alibabacloud_dms-enterprise20181101_py2-1.19.1/LICENSE` & `alibabacloud_dms-enterprise20181101_py2-1.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101_py2-1.19.1/PKG-INFO` & `alibabacloud_dms-enterprise20181101_py2-1.20.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dms-enterprise20181101_py2
-Version: 1.19.1
+Version: 1.20.0
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101_py2-1.19.1/README-CN.md` & `alibabacloud_dms-enterprise20181101_py2-1.20.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101_py2-1.19.1/README.md` & `alibabacloud_dms-enterprise20181101_py2-1.20.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101/client.py` & `alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4521,14 +4521,74 @@
             self.call_api(params, req, runtime)
         )
 
     def get_table_dbtopology(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_table_dbtopology_with_options(request, runtime)
 
+    def get_table_design_project_flow_with_options(self, request, runtime):
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
+    def get_table_design_project_flow(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_table_design_project_flow_with_options(request, runtime)
+
+    def get_table_design_project_info_with_options(self, request, runtime):
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
+    def get_table_design_project_info(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_table_design_project_info_with_options(request, runtime)
+
     def get_table_topology_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.table_guid):
             query['TableGuid'] = request.table_guid
         if not UtilClient.is_unset(request.tid):
             query['Tid'] = request.tid
```

### Comparing `alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101/models.py` & `alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -24977,14 +24977,460 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetTableDBTopologyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetTableDesignProjectFlowRequest(TeaModel):
+    def __init__(self, order_id=None, tid=None):
+        self.order_id = order_id  # type: long
+        self.tid = tid  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetTableDesignProjectFlowRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetTableDesignProjectFlowResponseBodyProjectFlowFlowNodeArray(TeaModel):
+    def __init__(self, back_to_design=None, can_skip=None, node_role=None, node_title=None, position=None,
+                 publish_anchor=None, publish_strategies=None):
+        self.back_to_design = back_to_design  # type: bool
+        self.can_skip = can_skip  # type: bool
+        self.node_role = node_role  # type: str
+        self.node_title = node_title  # type: str
+        self.position = position  # type: int
+        self.publish_anchor = publish_anchor  # type: bool
+        self.publish_strategies = publish_strategies  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetTableDesignProjectFlowResponseBodyProjectFlowFlowNodeArray, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, current_position=None, flow_node_array=None, rule_comment=None, rule_name=None):
+        self.current_position = current_position  # type: int
+        self.flow_node_array = flow_node_array  # type: list[GetTableDesignProjectFlowResponseBodyProjectFlowFlowNodeArray]
+        self.rule_comment = rule_comment  # type: str
+        self.rule_name = rule_name  # type: str
+
+    def validate(self):
+        if self.flow_node_array:
+            for k in self.flow_node_array:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(GetTableDesignProjectFlowResponseBodyProjectFlow, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, error_code=None, error_message=None, project_flow=None, request_id=None, success=None):
+        self.error_code = error_code  # type: str
+        self.error_message = error_message  # type: str
+        self.project_flow = project_flow  # type: GetTableDesignProjectFlowResponseBodyProjectFlow
+        self.request_id = request_id  # type: str
+        self.success = success  # type: bool
+
+    def validate(self):
+        if self.project_flow:
+            self.project_flow.validate()
+
+    def to_map(self):
+        _map = super(GetTableDesignProjectFlowResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetTableDesignProjectFlowResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetTableDesignProjectFlowResponse, self).to_map()
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
+            temp_model = GetTableDesignProjectFlowResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetTableDesignProjectInfoRequest(TeaModel):
+    def __init__(self, order_id=None, tid=None):
+        self.order_id = order_id  # type: long
+        self.tid = tid  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetTableDesignProjectInfoRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetTableDesignProjectInfoResponseBodyProjectInfoBaseDatabase(TeaModel):
+    def __init__(self, alias=None, db_id=None, db_type=None, env_type=None, logic=None, schema_name=None,
+                 search_name=None):
+        self.alias = alias  # type: str
+        self.db_id = db_id  # type: int
+        self.db_type = db_type  # type: str
+        self.env_type = env_type  # type: str
+        self.logic = logic  # type: bool
+        self.schema_name = schema_name  # type: str
+        self.search_name = search_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetTableDesignProjectInfoResponseBodyProjectInfoBaseDatabase, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, base_database=None, creator_id=None, description=None, gmt_create=None, gmt_modified=None,
+                 order_id=None, project_id=None, status=None, title=None):
+        self.base_database = base_database  # type: GetTableDesignProjectInfoResponseBodyProjectInfoBaseDatabase
+        self.creator_id = creator_id  # type: long
+        self.description = description  # type: str
+        self.gmt_create = gmt_create  # type: str
+        self.gmt_modified = gmt_modified  # type: str
+        self.order_id = order_id  # type: long
+        self.project_id = project_id  # type: long
+        self.status = status  # type: str
+        self.title = title  # type: str
+
+    def validate(self):
+        if self.base_database:
+            self.base_database.validate()
+
+    def to_map(self):
+        _map = super(GetTableDesignProjectInfoResponseBodyProjectInfo, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, error_code=None, error_message=None, project_info=None, request_id=None, success=None):
+        self.error_code = error_code  # type: str
+        self.error_message = error_message  # type: str
+        self.project_info = project_info  # type: GetTableDesignProjectInfoResponseBodyProjectInfo
+        self.request_id = request_id  # type: str
+        self.success = success  # type: bool
+
+    def validate(self):
+        if self.project_info:
+            self.project_info.validate()
+
+    def to_map(self):
+        _map = super(GetTableDesignProjectInfoResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetTableDesignProjectInfoResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetTableDesignProjectInfoResponse, self).to_map()
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
+            temp_model = GetTableDesignProjectInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetTableTopologyRequest(TeaModel):
     def __init__(self, table_guid=None, tid=None):
         # The GUID of the table in Data Management (DMS).
         # 
         # > 
         # > - You can call the [ListLogicTables](~~141875~~) operation with ReturnGuid set to true to query the GUIDs of logical tables in a specific logical database.
         # > - You can call the [ListTables](~~141878~~) operation with ReturnGuid set to true to query the GUIDs of tables in a specific physical database.
```

### Comparing `alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101_py2.egg-info/PKG-INFO` & `alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dms-enterprise20181101-py2
-Version: 1.19.1
+Version: 1.20.0
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101_py2-1.19.1/alibabacloud_dms_enterprise20181101_py2.egg-info/SOURCES.txt` & `alibabacloud_dms-enterprise20181101_py2-1.20.0/alibabacloud_dms_enterprise20181101_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101_py2-1.19.1/setup.py` & `alibabacloud_dms-enterprise20181101_py2-1.20.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dms-enterprise20181101_py2.
 
-Created on 18/04/2024
+Created on 26/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dms_enterprise20181101"
 NAME = "alibabacloud_dms-enterprise20181101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dms-enterprise (20181101) SDK Library for Python2"
```

