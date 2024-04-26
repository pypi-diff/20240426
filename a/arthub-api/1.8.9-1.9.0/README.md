# Comparing `tmp/arthub_api-1.8.9.tar.gz` & `tmp/arthub_api-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.8.9.tar", last modified: Thu Sep 14 07:31:08 2023, max compression
+gzip compressed data, was "arthub_api-1.9.0.tar", last modified: Fri Apr 26 07:43:12 2024, max compression
```

## Comparing `arthub_api-1.8.9.tar` & `arthub_api-1.9.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-09-14 07:31:08.206853 arthub_api-1.8.9/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.8.9/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.8.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-09-14 07:31:08.206853 arthub_api-1.8.9/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.8.9/README.md
-drwxrwxrwx   0        0        0        0 2023-09-14 07:31:08.186847 arthub_api-1.8.9/arthub_api/
--rw-rw-rw-   0        0        0      675 2023-07-25 13:45:45.000000 arthub_api-1.8.9/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     3049 2023-07-31 12:06:21.000000 arthub_api-1.8.9/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-09-14 07:30:36.000000 arthub_api-1.8.9/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.8.9/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0      104 2023-07-25 13:45:45.000000 arthub_api-1.8.9/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      501 2023-07-25 13:45:45.000000 arthub_api-1.8.9/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    43536 2023-07-25 13:45:45.000000 arthub_api-1.8.9/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     2072 2023-07-25 13:45:45.000000 arthub_api-1.8.9/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    28990 2023-07-25 13:45:45.000000 arthub_api-1.8.9/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.8.9/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1443 2023-07-25 13:45:45.000000 arthub_api-1.8.9/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.8.9/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.8.9/arthub_api/models.py
--rw-rw-rw-   0        0        0    44784 2023-08-01 12:07:16.000000 arthub_api-1.8.9/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    44908 2023-09-14 07:24:32.000000 arthub_api-1.8.9/arthub_api/storage.py
--rw-rw-rw-   0        0        0     9102 2023-07-25 13:45:45.000000 arthub_api-1.8.9/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-09-14 07:31:08.197818 arthub_api-1.8.9/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-09-14 07:31:07.000000 arthub_api-1.8.9/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2023-09-14 07:31:07.000000 arthub_api-1.8.9/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-14 07:31:07.000000 arthub_api-1.8.9/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-09-14 07:31:07.000000 arthub_api-1.8.9/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.8.9/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      164 2023-09-14 07:31:07.000000 arthub_api-1.8.9/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-09-14 07:31:07.000000 arthub_api-1.8.9/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.8.9/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-09-14 07:31:08.206853 arthub_api-1.8.9/setup.cfg
--rw-rw-rw-   0        0        0     3129 2023-09-13 10:09:22.000000 arthub_api-1.8.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-14 07:31:08.204839 arthub_api-1.8.9/tests/
--rw-rw-rw-   0        0        0      176 2023-07-25 13:45:45.000000 arthub_api-1.8.9/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.8.9/tests/_utils.py
--rw-rw-rw-   0        0        0      735 2023-07-25 13:45:45.000000 arthub_api-1.8.9/tests/conftest.py
--rw-rw-rw-   0        0        0     6646 2023-07-25 13:45:45.000000 arthub_api-1.8.9/tests/test_open_api.py
--rw-rw-rw-   0        0        0     2979 2023-07-25 13:45:45.000000 arthub_api-1.8.9/tests/test_storage.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:43:12.947695 arthub_api-1.9.0/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.9.0/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2024-04-26 07:43:12.947695 arthub_api-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 07:43:12.920568 arthub_api-1.9.0/arthub_api/
+-rw-rw-rw-   0        0        0      675 2023-07-25 13:45:45.000000 arthub_api-1.9.0/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     3049 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2024-04-26 07:41:47.000000 arthub_api-1.9.0/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.9.0/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0      128 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      501 2023-07-25 13:45:45.000000 arthub_api-1.9.0/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    43536 2023-07-25 13:45:45.000000 arthub_api-1.9.0/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     2072 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    28990 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.9.0/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1443 2023-07-25 13:45:45.000000 arthub_api-1.9.0/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.9.0/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1465 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/models.py
+-rw-rw-rw-   0        0        0    47472 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    46992 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/storage.py
+-rw-rw-rw-   0        0        0    10006 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:43:12.935168 arthub_api-1.9.0/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-03-14 07:53:40.000000 arthub_api-1.9.0/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      185 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.9.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 07:43:12.947695 arthub_api-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     3157 2024-04-26 07:41:26.000000 arthub_api-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:43:12.944145 arthub_api-1.9.0/tests/
+-rw-rw-rw-   0        0        0      176 2023-07-25 13:45:45.000000 arthub_api-1.9.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.9.0/tests/_utils.py
+-rw-rw-rw-   0        0        0      866 2024-04-26 07:41:26.000000 arthub_api-1.9.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     7139 2024-04-26 07:41:26.000000 arthub_api-1.9.0/tests/test_open_api.py
+-rw-rw-rw-   0        0        0     3471 2024-04-26 07:41:26.000000 arthub_api-1.9.0/tests/test_storage.py
```

### Comparing `arthub_api-1.8.9/LICENSE` & `arthub_api-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.9/PKG-INFO` & `arthub_api-1.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.8.9
+Version: 1.9.0
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.8.9/README.md` & `arthub_api-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.9/arthub_api/__init__.py` & `arthub_api-1.9.0/arthub_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.9/arthub_api/__main__.py` & `arthub_api-1.9.0/arthub_api/__main__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.9/arthub_api/_internal_utils.py` & `arthub_api-1.9.0/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.9/arthub_api/blade_api.py` & `arthub_api-1.9.0/arthub_api/blade_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.9/arthub_api/blade_api_instance.py` & `arthub_api-1.9.0/arthub_api/blade_api_instance.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.9/arthub_api/blade_storage.py` & `arthub_api-1.9.0/arthub_api/blade_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.9/arthub_api/config.py` & `arthub_api-1.9.0/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.9/arthub_api/exception.py` & `arthub_api-1.9.0/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.9/arthub_api/models.py` & `arthub_api-1.9.0/arthub_api/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,7 +45,15 @@
     @property
     def progress_weight(self):
         return self._progress_weight
 
 
 def success_task_result(data, progress_weight=0):
     return TaskResult(succeeded=True, data=data, progress_weight=progress_weight)
+
+
+class RemoteNodeInfo(object):
+    def __init__(self, node_id, parent_id=-1, origin_url=""):
+        self.id = node_id
+        self.parent_id = parent_id
+        self.origin_url = origin_url
+
```

### Comparing `arthub_api-1.8.9/arthub_api/open_api.py` & `arthub_api-1.9.0/arthub_api/open_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from . import _internal_utils
 from . import exception
 from xml.etree import ElementTree
 from . import arthub_api_config
 from .config import api_config_oa
 from .utils import get_config_by_name, logger
 import os
+import json
 
 
 def _node_query_metas(simplified_meta=True):
     metas = [
         "name",
         "file_format",
         "node_type",
@@ -36,14 +37,15 @@
             "confirmed_asset_id",
             "preview_url",
             "status",
             "crc64",
             "updated_date",
             "description",
             "total_leaf_count"
+            "last_modifier"
         ]
     return metas
 
 
 class APIError(Exception):
     pass
 
@@ -282,14 +284,16 @@
         self._public_token = ""
         self._cookies = None
         self._api_version_depot = "v2"
         self._api_version_gateway = "v2"
         self._api_version_account = "v3"
         self._cached_account_name = ""
         self._cached_password = ""
+        self._cached_business_type = "default"
+        self._cached_terminal_type = "default"
         self._auto_login = False
         self._current_account_info = None
         self._in_blade_env = False
         if apply_blade_env:
             self._apply_blade_env_value()
         if get_token_from_cache:
             self.get_token_from_cache()
@@ -455,15 +459,18 @@
 
     def _try_auto_login(self):
         # Use the cached account password to log in again to get the token
         if not self._auto_login:
             return False
         if len(self._cached_password) == 0 or len(self._cached_account_name) == 0:
             return False
-        return self.login(self._cached_account_name, self._cached_password).is_succeeded()
+        return self.login(account_name=self._cached_account_name,
+                          password=self._cached_password,
+                          terminal_type=self._cached_terminal_type,
+                          business_type=self._cached_business_type).is_succeeded()
 
     def _make_api_request(self, url, data=None, method='POST', content_type='application/json',
                           try_login_on_expired=True):
         # set token to headers
         headers = {}
         if self._token:
             headers["arthubtoken"] = self._token
@@ -499,46 +506,72 @@
         cookies_str = os.environ.get("BLADE_API_COOKIES")
         if cookies_str:
             self.set_cookies(cookies_str, True)
 
     def add_headers(self, headers):
         pass
 
-    def login(self, account_name, password, set_auto_login=True, save_token_to_cache=True):
+    @staticmethod
+    def generate_login_ticket(req_payload, public_key_str):
+        plain_text = req_payload["nounce"] + json.dumps(req_payload)
+        return utils.encrypt(public_key_str, plain_text)
+
+    def login(self, account_name, password,
+              terminal_type="default",
+              business_type="default",
+              verification_code=None,
+              login_public_keys=None,
+              set_auto_login=True,
+              save_token_to_cache=True):
         r"""Login by email/mobile and password. You can visit https://arthub.qq.com to register.
 
         :param account_name: str. email or mobile.
         :param password: str. If you forget, visit https://arthub.qq.com/reset-password to reset
+        :param terminal_type: str.
+        :param business_type: str.
+        :param verification_code: str.
+        :param login_public_keys: str.
         :param set_auto_login: (optional) bool. After successful login, save the account and password,
                and login automatically after the login status expires
         :param save_token_to_cache: (optional) bool. After successful login, save the token to local cache
         :rtype: arthub_api.APIResponse
         """
 
-        url = self._account_url("login")
         req_payload = {
             "account_name": account_name,
             "account_type": "mobile" if account_name.isdigit() else "email",
             "password": password,
+            "terminal_type": terminal_type,
+            "business_type": business_type,
             "current_time": utils.current_milli_time(),
             "nounce": utils.get_random_string(8),
             "oauth_type": "password",
             "login_type": "arthub_token"
         }
+
+        url = self._account_url("login")
+        if not login_public_keys:
+            req_payload["verification_code"] = verification_code
+        else:
+            url = self._account_url("open-secret-login")
+            req_payload["ticket"] = self.generate_login_ticket(req_payload, login_public_keys)
+
         res = self._make_api_request(url, req_payload, try_login_on_expired=False)
         if res.is_succeeded():
             r = res.results.get(0)
             token = r["arthub_token"]
             self.set_token(token, save_token_to_cache)
 
             self._auto_login = set_auto_login
             # save account and password for auto login
             if set_auto_login:
                 self._cached_account_name = account_name
                 self._cached_password = password
+                self._cached_terminal_type = terminal_type
+                self._cached_business_type = business_type
 
         return res
 
     def _account_value(self, key):
         account_info = self.current_account_info
         if account_info:
             return account_info.get(key)
@@ -919,14 +952,31 @@
         if not res or not res.ok:
             error_message = "request complete S3 multipart upload failed, url: %s, code: %d" % (
                 signed_url, res.status_code)
             logger.error("[API] %s" % error_message)
             return models.failure_result(error_message)
         return models.success_result(None)
 
+    def depot_set_asset_confirmed_version_id(self, asset_hub, multi_asset_id, confirmed_asset_id):
+        r"""Set the confirmed version of a multi asset.
+
+        :param asset_hub: str. Example: "trial".
+        :param multi_asset_id: int. Example: 1234.
+        :param confirmed_asset_id: int. Example: 1234.
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "set-asset-confirmed-version-id")
+        req_payload = [{
+            "id": multi_asset_id,
+            "confirmed_asset_id": confirmed_asset_id,
+        }]
+        res = self._make_api_request(url, req_payload)
+        return res
+
     def depot_get_child_node_count(self, asset_hub, ids, query_filters=[], is_recursive=False):
         r"""Get the child node count of node in depot.
 
         :param asset_hub: str. Example: "trial".
         :param ids: list<int>. Example: [1234].
         :param query_filters: (optional) list<query_filter (dict) >. Example: [{"meta": "type", "condition": "x != project"}].
                 {
@@ -944,37 +994,43 @@
             "is_recursive": is_recursive
         }
         res = self._make_api_request(url, req_payload)
         res.set_result_by_key("count")
         return res
 
     def depot_get_child_node_id_in_range(self, asset_hub, parent_id, offset, count, query_filters=[],
-                                         is_recursive=False):
+                                         is_recursive=False, order=None):
         r"""Get the child node count of node in depot.
 
         :param asset_hub: str. Example: "trial".
         :param parent_id: int. Example: 1234.
         :param offset: int. range offset: 0.
         :param count: int. range count: 100.
         :param query_filters: list<query_filter (dict) >. Example: [{"meta": "type", "condition": "x != project"}].
                 {
                     "meta": filters meta,
                     "condition": filters condition
                 }
         :param is_recursive: (optional) bool, Whether to query recursively
+        :param order: (optional) dict >. Example:
+                {
+                    "meta": "updated_date",
+                    "type": "descend"
+                }
         :rtype: arthub_api.APIResponse
         """
 
         url = self._depot_url(asset_hub, "get-child-node-id-in-range")
         req_payload = {
             "parent_id": parent_id,
             "offset": offset,
             "count": count,
             "filter": query_filters,
-            "is_recursive": is_recursive
+            "is_recursive": is_recursive,
+            "order": order
         }
         res = self._make_api_request(url, req_payload)
         res.set_result_by_key("nodes")
         return res
 
     def depot_get_node_brief_by_path(self, asset_hub, root_id, path, simplified_meta=False):
         r"""Get the brief of node by path in depot.
@@ -1187,14 +1243,28 @@
         url = self._depot_url(asset_hub, "add-asset-tag")
         req_payload = {
             "asset_id": asset_id,
             "tag_name": tag_name
         }
         return self._make_api_request(url, req_payload)
 
+    def depot_get_asset_tag(self, asset_hub, asset_id):
+        r"""get tags on asset node in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param asset_id: int. Example: 110347249345071.
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "get-tag-by-asset-id")
+        req_payload = {
+            "asset_id": asset_id
+        }
+        return self._make_api_request(url, req_payload)
+
     def depot_update_directory_by_id(self, asset_hub, payloads):
         r"""update metas of directory in depot .
 
         :param asset_hub: str. Example: "trial".
         :param payloads: list<payload (dict) >.
                 {
                     "id": int, node id,
```

### Comparing `arthub_api-1.8.9/arthub_api/storage.py` & `arthub_api-1.9.0/arthub_api/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         self._remote_parent_dir_id = remote_parent_dir_id
         self._local_path = local_path
         self._same_name_override = same_name_override
         self._need_convert = need_convert
         self._tags_to_create = tags_to_create
         self._remote_node_name = os.path.basename(self._local_path)
         self._asset_id = -1
-        self._origin_url = -1
+        self._origin_url = ""
         self._upload_id = -1
         self._description = description
 
     class UploadChunk(object):
         def __init__(self, part_num, offset, length):
             self.part_num = part_num
             self.offset = offset
@@ -347,15 +347,18 @@
         elif os.path.isfile(self._local_path):
             res = self._upload_file()
             if not res.is_succeeded():
                 return res
             uploaded_node_id = res.data
             progress_weight = 1
 
-        return models.success_task_result(uploaded_node_id, progress_weight)
+        node_info = models.RemoteNodeInfo(node_id=uploaded_node_id,
+                                          parent_id=self._remote_parent_dir_id,
+                                          origin_url=self._origin_url)
+        return models.success_task_result(node_info, progress_weight)
 
 
 class TreeNode(object):
     def __init__(self, brief, parent):
         self.brief = brief
         self.parent = parent
         self.children = []
@@ -365,21 +368,33 @@
         return Storage.is_node_directory(self.brief)
 
     @property
     def is_file(self):
         return Storage.is_node_file(self.brief)
 
     @property
+    def is_multi_asset(self):
+        return Storage.is_multi_asset(self.brief)
+
+    @property
     def fullname(self):
         return Storage.node_full_name(self.brief)
 
     @property
     def id(self):
         return self.brief["id"]
 
+    @property
+    def last_modifier(self):
+        return self.brief["last_modifier"]
+
+    @property
+    def updated_date(self):
+        return self.brief["updated_date"]
+
 
 class Storage(object):
     def __init__(self, open_api):
         r"""Used to perform ArtHub storage operations, such as uploading and downloading files.
 
         :param open_api: class: arthub_api.API.
         """
@@ -399,14 +414,18 @@
         return node.get("type") == "directory" or node.get("type") == "project"
 
     @staticmethod
     def is_node_file(node):
         return node.get("type") == "asset" or node.get("type") == "multiasset"
 
     @staticmethod
+    def is_multi_asset(node):
+        return node.get("type") == "multiasset"
+
+    @staticmethod
     def get_child_node_relative_path(child_node_brief, root_id):
         full_path_id = child_node_brief.get("full_path_id")
         full_path_name = child_node_brief.get("full_path_name")
         find_root = False
         root_pos = 0
         for i in range(len(full_path_id)):
             if full_path_id[i] == root_id:
@@ -420,40 +439,46 @@
         for i in range(root_pos + 1, len(full_path_name)):
             relative_paths.append(full_path_name[i])
 
         relative_paths.append(Storage.node_full_name(child_node_brief))
         return models.success_result(relative_paths)
 
     def get_child_nodes_brief_by_id(self, asset_hub, parent_node_id, query_filters=[], is_recursive=False,
-                                    simplified_meta=True):
+                                    simplified_meta=True, order=None):
         r"""Get child nodes brief under parent dir node by parent id.
         """
         res = self.open_api.depot_get_node_brief_by_ids(asset_hub, [parent_node_id], True)
         if not res.is_succeeded():
             return models.failure_result(
                 "get parent node info by %d failed, %s" % (parent_node_id, res.error_message()))
 
         if not self.is_node_directory(res.first_result()):
             return models.failure_result("target parent node %d is not a directory" % parent_node_id)
-        return self.get_child_nodes_brief(asset_hub, res.first_result(), query_filters, is_recursive, simplified_meta)
+        return self.get_child_nodes_brief(asset_hub, res.first_result(), query_filters, is_recursive, simplified_meta,
+                                          order)
 
-    def get_child_nodes_brief(self, asset_hub, parent_node, query_filters=[], is_recursive=False, simplified_meta=True):
+    def get_child_nodes_brief(self, asset_hub, parent_node, query_filters=[], is_recursive=False, simplified_meta=True,
+                              order=None):
         r"""Get child nodes brief under parent dir node.
 
         :param asset_hub: str. Example: "trial".
         :param parent_node: dic. dir type node brief.
         :param simplified_meta: (optional) bool. Just basic meta, lower bandwidth consumption.
         :param query_filters: (optional) list<query_filter (dict) >. Example: [{"meta": "type",
                                                                                 "condition": "x != project"}].
                 {
                     "meta": filters meta,
                     "condition": filters condition
                 }
         :param is_recursive: (optional) bool, Whether to query recursively
-
+        :param order: (optional) dict >. Example:
+                {
+                    "meta": "updated_date",
+                    "type": "descend"
+                }
         :rtype: arthub_api.Result
                 arthub_api.Result.data: list<dict>. child nodes brief
         """
 
         if not self.is_node_directory(parent_node):
             return models.failure_result("node type error")
         parent_id = parent_node.get("id")
@@ -478,15 +503,16 @@
         batch_count = 1000
         offset = 0
         while offset < child_count:
             next_offset = child_count if (offset + batch_count) > child_count else (offset + batch_count)
             r = self.open_api.depot_get_child_node_id_in_range(asset_hub, parent_id, offset,
                                                                next_offset - offset,
                                                                query_filters=query_filters,
-                                                               is_recursive=is_recursive)
+                                                               is_recursive=is_recursive,
+                                                               order=order)
             if not r.is_succeeded():
                 return models.failure_result("get child node ids of %d failed, %s" % (parent_id, r.error_message()))
             child_ids += r.direct_result
             offset = next_offset
 
         # step3: get brief of child node
         child_nodes = []
@@ -499,27 +525,33 @@
             if not r.is_succeeded():
                 return models.failure_result("get child node brief failed, %s" % r.error_message())
             child_nodes += list(r.results.values())
             offset = next_offset
 
         return models.success_result(child_nodes)
 
-    def get_child_nodes(self, asset_hub, parent_path, query_filters=[], is_recursive=False, simplified_meta=True):
+    def get_child_nodes(self, asset_hub, parent_path, query_filters=[], is_recursive=False, simplified_meta=True,
+                        order=None):
         r"""Get child nodes under parent path.
 
         :param asset_hub: str. Example: "trial".
         :param parent_path: str. remote node path to query info. Example: "sdk/1/2".
         :param simplified_meta: (optional) bool. Just basic meta, lower bandwidth consumption.
         :param query_filters: (optional) list<query_filter (dict) >. Example: [{"meta": "type",
                                                                                 "condition": "x != project"}].
                 {
                     "meta": filters meta,
                     "condition": filters condition
                 }
         :param is_recursive: (optional) bool, Whether to query recursively
+        :param order: (optional) dict >. Example:
+                {
+                    "meta": "updated_date",
+                    "type": "descend"
+                }
 
         :rtype: arthub_api.Result
                 arthub_api.Result.data: TreeNode, node of parent
         """
 
         # query root directory node
         res = self.get_node_by_path(asset_hub=asset_hub,
@@ -534,15 +566,16 @@
         def _query_children(parent_node):
             if not parent_node.is_directory:
                 return models.success_result(None)
             _res = self.get_child_nodes_brief(asset_hub=asset_hub,
                                               parent_node=parent_node.brief,
                                               query_filters=query_filters,
                                               is_recursive=False,
-                                              simplified_meta=simplified_meta)
+                                              simplified_meta=simplified_meta,
+                                              order=order)
             if not _res.is_succeeded():
                 return models.failure_result("query children nodes failed")
             for child_brief in _res.data:
                 child_node = TreeNode(brief=child_brief, parent=parent_node)
                 if is_recursive:
                     _res_2 = _query_children(child_node)
                     if not _res_2.is_succeeded():
@@ -634,15 +667,31 @@
 
         res = self.open_api.depot_get_root_id(asset_hub)
         if not res.is_succeeded():
             r_ = models.failure_result("get depot root id failed, %s" % res.error_message())
             r_.set_data({"not_exist": False})
             return r_
         root_id = res.first_result()
-        res = self.open_api.depot_get_node_brief_by_path(asset_hub, root_id, remote_node_path,
+        return self.get_node_by_path_from_id(asset_hub, root_id, remote_node_path, simplified_meta)
+
+    def get_node_by_path_from_id(self, asset_hub_name, asset_hub_id, remote_node_path, simplified_meta=False):
+        r"""Get node info by path in depot under asset hub id.
+
+        :param asset_hub_name: str. Example: "trial".
+        :param asset_hub_id: str. Example: 123.
+        :param remote_node_path: str. remote node path to query info. Example: "sdk/1/2".
+        :param simplified_meta: (optional) bool. Just basic meta, lower bandwidth consumption.
+
+        :rtype: arthub_api.Result
+                arthub_api.Result.is_succeeded(): True when query successful
+                arthub_api.Result.is_succeeded(): False when query fail, or node doesn't exist
+                arthub_api.Result.data: dic. info of dir
+        """
+
+        res = self.open_api.depot_get_node_brief_by_path(asset_hub_name, asset_hub_id, remote_node_path,
                                                          simplified_meta=simplified_meta)
         if not res.is_succeeded():
             r_ = models.failure_result("get node info by \"%s\" failed, %s" % (
                 remote_node_path, res.error_message()))
             r_.set_data({"not_exist": res.is_node_not_exist()})
             return r_
         return models.success_result(res.first_result())
```

### Comparing `arthub_api-1.8.9/arthub_api/utils.py` & `arthub_api-1.9.0/arthub_api/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 """
 arthub_api.utils
 ~~~~~~~~~~~~~~
 
 This module provides utilities that are used within API
 """
 import logging
@@ -15,16 +16,20 @@
 from platformdirs import user_cache_dir
 from .config import (
     api_config_oa,
     api_config_qq,
     api_config_oa_test,
     api_config_qq_test
 )
-from .__version__ import __title__
+from base64 import b64encode, b64decode
+from Crypto.PublicKey import RSA
+from Crypto.Cipher import PKCS1_OAEP
+from Crypto.Hash import SHA256
 
+from .__version__ import __title__
 
 logger = logging.getLogger(__title__)
 
 
 def _path_preprocess(path):
     path = path.strip()
     path = path.rstrip("\\/")
@@ -218,18 +223,16 @@
             cookies[_pair[0]] = _pair[1]
     return cookies
 
 
 def rename_path(src, dest):
     if not mkdir(os.path.dirname(dest)):
         return False
-    if os.path.exists(dest):
-        remove(dest)
     try:
-        os.rename(src, dest)
+        shutil.move(src, dest)
     except Exception:
         return False
     return True
 
 
 def count_files(root_path):
     total_files = 0
@@ -258,42 +261,42 @@
 
 
 def get_cache_dir(api_host):
     root = user_cache_dir(appname="arthub", opinion=False)
     d = os.path.join(root, api_host)
     try:
         os.makedirs(d)
-    except Exception:
+    except Exception as e:
         pass
     return d
 
 
 def get_token_cache_file(api_host):
     root = get_cache_dir(api_host)
     return os.path.join(root, "arthub_token")
 
 
 def get_token_from_cache(api_host):
     token_file = get_token_cache_file(api_host)
     try:
         if os.path.exists(token_file):
             return read_file(token_file)
-    except Exception:
+    except Exception as e:
         logger.warning("[TokenCache] get token from file \"%s\" error: %s",
-                        token_file, str(e))
+                       token_file, str(e))
     return ""
 
 
 def save_token_to_cache(token, api_host):
     token_file = get_token_cache_file(api_host)
     try:
         write_file(token_file, token)
-    except Exception:
+    except Exception as e:
         logger.warning("[TokenCache] save token to file \"%s\" error: %s",
-                        token_file, str(e))
+                       token_file, str(e))
 
 
 def remove_token_cache_file(api_host):
     remove(get_token_cache_file(api_host))
 
 
 def get_config_by_name(env, default_config=None):
@@ -306,7 +309,27 @@
     c = _env_map.get(env)
     if not c:
         if default_config:
             return default_config
         return api_config_oa
     return c
 
+
+def encrypt(public_key_str, plain_text):
+    try:
+        public_key_bytes = b64decode(public_key_str)
+        public_key = RSA.import_key(public_key_bytes)
+
+        block_size = 256 - 2 * 32 - 2
+        plain_text_blocks = [plain_text[i:i + block_size] for i in range(0, len(plain_text), block_size)]
+
+        encrypted_blocks = []
+        for block in plain_text_blocks:
+            cipher = PKCS1_OAEP.new(public_key, hashAlgo=SHA256)
+            encrypted_block = cipher.encrypt(block.encode())
+            encrypted_blocks.append(b64encode(encrypted_block).decode())
+
+        encrypted_text = ".".join(encrypted_blocks)
+        return encrypted_text
+    except Exception as e:
+        print("Error during encryption:", str(e))
+        return ""
```

### Comparing `arthub_api-1.8.9/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.9.0/arthub_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.8.9
+Version: 1.9.0
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.8.9/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.9.0/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.9/setup.py` & `arthub_api-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 requires = [
     'requests>=2.25.1',
     'platformdirs==2.0.2',
     'tenacity==5.0.*; python_version < "3"',
     'tenacity>=8; python_version >= "3"',
     'six==1.16.*',
+    'pycryptodome==3.16.0'
 ]
 
 test_requirements = [
     "pytest",
 ]
 
 about = {}
```

### Comparing `arthub_api-1.8.9/tests/conftest.py` & `arthub_api-1.9.0/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 def env(request):
     return request.config.getoption("--env")
 
 
 @pytest.fixture()
 def open_api(env):
     _c = _utils.get_config(env)
-    open_api = OpenAPI(_c, False)
+    open_api = OpenAPI(config=_c,
+                       get_token_from_cache=False,
+                       login_public_keys=arthub_api_config.login_public_keys)
     res = open_api.login(arthub_api_config.account_email, arthub_api_config.password)
     assert res.is_succeeded()
     return open_api
 
 
 @pytest.fixture()
 def storage(open_api):
```

### Comparing `arthub_api-1.8.9/tests/test_open_api.py` & `arthub_api-1.9.0/tests/test_open_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,21 +124,35 @@
         assert 0
 
     node = res.results.get(0)
     logging.info("[TEST][API] \"%s\" success, name: %s" % (res.url, node["name"]))
 
 
 def test_depot_add_asset_tag(open_api):
-    res = open_api.depot_add_asset_tag(TEST_DEPOT_NAME, asset_id=120347220059344, tag_name=[utils.get_random_string(5)])
+    new_tag_name = utils.get_random_string(5)
+    res = open_api.depot_add_asset_tag(TEST_DEPOT_NAME, asset_id=120347220059344, tag_name=[new_tag_name])
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
-    node = res.results.get(0)
-    logging.info("[TEST][API] \"%s\" success, tag id: %d" % (res.url, node))
+    new_tag_id = res.results.get(0)
+    logging.info("[TEST][API] \"%s\" success, new tag id: %d" % (res.url, new_tag_id))
+
+    res = open_api.depot_get_asset_tag(TEST_DEPOT_NAME, asset_id=120347220059344)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+    find_new_tag = False
+    for tag in res.result:
+        if tag["id"] == new_tag_id and tag["tag_name"] == new_tag_name:
+            find_new_tag = True
+            break
+    if not find_new_tag:
+        assert 0
+    logging.info("[TEST][API] \"%s\" success" % res.url)
 
 
 def test_get_account_detail(open_api):
     res = open_api.get_account_detail()
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
```

### Comparing `arthub_api-1.8.9/tests/test_storage.py` & `arthub_api-1.9.0/tests/test_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 import logging
 import time
 
 TEST_DEPOT_NAME = "apg"
 
+
 def on_api_failed(res):
     logging.error("[TEST][STORAGE] \"%s\" failed, error: %s" % (res.url, res.error_message()))
 
 
 def on_operation_failed(operation, error_message):
     logging.error("[TEST][STORAGE] %s failed, error: %s" % (operation, error_message))
 
@@ -31,14 +32,15 @@
     logging.info("[TEST][STORAGE] download success, local downloaded path: %s, spend: %f s"
                  % (local_downloaded_path, time.time() - since))
     since = time.time()
 
     # upload downloaded dir
     def upload_progress_cb(completed, total):
         print("upload progress: %d/%d" % (completed, total))
+
     res = storage.upload_to_directory_by_path(asset_hub=TEST_DEPOT_NAME,
                                               remote_dir_path="arthub_api_test/storage_test/upload",
                                               local_path=local_downloaded_path,
                                               tags_to_create=["sdk_test"],
                                               same_name_override=False,
                                               need_convert=True,
                                               progress_cb=upload_progress_cb)
@@ -59,7 +61,18 @@
 
 def test_delete_node_by_path(storage):
     res = storage.delete_node_by_path(asset_hub=TEST_DEPOT_NAME, remote_node_path="arthub_api_test/storage_test/upload")
     if not res.is_succeeded():
         on_operation_failed("delete remote node info", res.error_message())
         assert 0
     logging.info("[TEST][STORAGE] delete remote node %d success" % res.data)
+
+
+def test_get_child_nodes(storage):
+    res = storage.get_child_nodes(asset_hub=TEST_DEPOT_NAME, parent_path="arthub_api_test/storage_test/download/child",
+                                  order={"meta": "name", "type": "descend"})
+    if not res.is_succeeded():
+        on_operation_failed("get child nodes", res.error_message())
+        assert 0
+    children_nodes = res.data.children
+    assert len(children_nodes) == 3
+    logging.info("[TEST][STORAGE] get child nodes")
```

