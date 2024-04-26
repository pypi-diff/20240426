# Comparing `tmp/pigeonsai-1.0.6.tar.gz` & `tmp/pigeonsai-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonsai-1.0.6.tar", last modified: Fri Apr 12 00:54:31 2024, max compression
+gzip compressed data, was "pigeonsai-1.0.7.tar", last modified: Fri Apr 26 03:16:45 2024, max compression
```

## Comparing `pigeonsai-1.0.6.tar` & `pigeonsai-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/
--rw-r--r--   0 bs        (1000) bs        (1000)     1882 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/PKG-INFO
--rw-r--r--   0 bs        (1000) bs        (1000)      374 2024-04-10 17:12:16.000000 pigeonsai-1.0.6/README.md
--rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/setup.cfg
--rw-r--r--   0 bs        (1000) bs        (1000)     2075 2024-04-12 00:54:09.000000 pigeonsai-1.0.6/setup.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.791464 pigeonsai-1.0.6/src/
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/src/pigeonsai/
--rw-r--r--   0 bs        (1000) bs        (1000)      479 2024-03-15 16:34:17.000000 pigeonsai-1.0.6/src/pigeonsai/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)     3913 2024-03-22 23:15:49.000000 pigeonsai-1.0.6/src/pigeonsai/_client.py
--rw-r--r--   0 bs        (1000) bs        (1000)       48 2024-04-02 15:06:23.000000 pigeonsai-1.0.6/src/pigeonsai/_constants.py
--rw-r--r--   0 bs        (1000) bs        (1000)     3288 2024-03-16 02:35:35.000000 pigeonsai-1.0.6/src/pigeonsai/_exceptions.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/src/pigeonsai/_utils/
--rw-r--r--   0 bs        (1000) bs        (1000)       39 2024-03-15 17:28:27.000000 pigeonsai-1.0.6/src/pigeonsai/_utils/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)      136 2024-03-15 16:23:51.000000 pigeonsai-1.0.6/src/pigeonsai/_utils/_utils.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/src/pigeonsai/resources/
--rw-r--r--   0 bs        (1000) bs        (1000)      148 2024-03-19 16:08:19.000000 pigeonsai-1.0.6/src/pigeonsai/resources/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)      181 2024-03-19 16:42:03.000000 pigeonsai-1.0.6/src/pigeonsai/resources/anomaly_detector.py
--rw-r--r--   0 bs        (1000) bs        (1000)    10791 2024-04-10 16:56:58.000000 pigeonsai-1.0.6/src/pigeonsai/resources/data_connector.py
--rw-r--r--   0 bs        (1000) bs        (1000)    10537 2024-04-11 21:01:33.000000 pigeonsai-1.0.6/src/pigeonsai/resources/recommender.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/src/pigeonsai.egg-info/
--rw-r--r--   0 bs        (1000) bs        (1000)     1882 2024-04-12 00:54:31.000000 pigeonsai-1.0.6/src/pigeonsai.egg-info/PKG-INFO
--rw-r--r--   0 bs        (1000) bs        (1000)      535 2024-04-12 00:54:31.000000 pigeonsai-1.0.6/src/pigeonsai.egg-info/SOURCES.txt
--rw-r--r--   0 bs        (1000) bs        (1000)        1 2024-04-12 00:54:31.000000 pigeonsai-1.0.6/src/pigeonsai.egg-info/dependency_links.txt
--rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-12 00:54:31.000000 pigeonsai-1.0.6/src/pigeonsai.egg-info/requires.txt
--rw-r--r--   0 bs        (1000) bs        (1000)       10 2024-04-12 00:54:31.000000 pigeonsai-1.0.6/src/pigeonsai.egg-info/top_level.txt
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-26 03:16:45.471752 pigeonsai-1.0.7/
+-rw-r--r--   0 bs        (1000) bs        (1000)     1882 2024-04-26 03:16:45.471752 pigeonsai-1.0.7/PKG-INFO
+-rw-r--r--   0 bs        (1000) bs        (1000)      374 2024-04-10 17:12:16.000000 pigeonsai-1.0.7/README.md
+-rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-26 03:16:45.471752 pigeonsai-1.0.7/setup.cfg
+-rw-r--r--   0 bs        (1000) bs        (1000)     2075 2024-04-26 03:16:42.000000 pigeonsai-1.0.7/setup.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-26 03:16:45.461752 pigeonsai-1.0.7/src/
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-26 03:16:45.461752 pigeonsai-1.0.7/src/pigeonsai/
+-rw-r--r--   0 bs        (1000) bs        (1000)      479 2024-03-15 16:34:17.000000 pigeonsai-1.0.7/src/pigeonsai/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)     3913 2024-03-22 23:15:49.000000 pigeonsai-1.0.7/src/pigeonsai/_client.py
+-rw-r--r--   0 bs        (1000) bs        (1000)       48 2024-04-02 15:06:23.000000 pigeonsai-1.0.7/src/pigeonsai/_constants.py
+-rw-r--r--   0 bs        (1000) bs        (1000)     3288 2024-03-16 02:35:35.000000 pigeonsai-1.0.7/src/pigeonsai/_exceptions.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-26 03:16:45.461752 pigeonsai-1.0.7/src/pigeonsai/_utils/
+-rw-r--r--   0 bs        (1000) bs        (1000)       39 2024-03-15 17:28:27.000000 pigeonsai-1.0.7/src/pigeonsai/_utils/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)      136 2024-03-15 16:23:51.000000 pigeonsai-1.0.7/src/pigeonsai/_utils/_utils.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-26 03:16:45.471752 pigeonsai-1.0.7/src/pigeonsai/resources/
+-rw-r--r--   0 bs        (1000) bs        (1000)      148 2024-03-19 16:08:19.000000 pigeonsai-1.0.7/src/pigeonsai/resources/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)      181 2024-03-19 16:42:03.000000 pigeonsai-1.0.7/src/pigeonsai/resources/anomaly_detector.py
+-rw-r--r--   0 bs        (1000) bs        (1000)    10791 2024-04-10 16:56:58.000000 pigeonsai-1.0.7/src/pigeonsai/resources/data_connector.py
+-rw-r--r--   0 bs        (1000) bs        (1000)    11765 2024-04-25 15:44:53.000000 pigeonsai-1.0.7/src/pigeonsai/resources/recommender.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-26 03:16:45.471752 pigeonsai-1.0.7/src/pigeonsai.egg-info/
+-rw-r--r--   0 bs        (1000) bs        (1000)     1882 2024-04-26 03:16:45.000000 pigeonsai-1.0.7/src/pigeonsai.egg-info/PKG-INFO
+-rw-r--r--   0 bs        (1000) bs        (1000)      535 2024-04-26 03:16:45.000000 pigeonsai-1.0.7/src/pigeonsai.egg-info/SOURCES.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)        1 2024-04-26 03:16:45.000000 pigeonsai-1.0.7/src/pigeonsai.egg-info/dependency_links.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-26 03:16:45.000000 pigeonsai-1.0.7/src/pigeonsai.egg-info/requires.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)       10 2024-04-26 03:16:45.000000 pigeonsai-1.0.7/src/pigeonsai.egg-info/top_level.txt
```

### Comparing `pigeonsai-1.0.6/PKG-INFO` & `pigeonsai-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 1.0.6
+Version: 1.0.7
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://docs.pigeonsai.com/
```

### Comparing `pigeonsai-1.0.6/setup.py` & `pigeonsai-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_desc = """
 PigeonsAI is an ecosystem to build production ready machine learning applications.
 """
 
 setup(
     name="pigeonsai",
-    version="1.0.6",
+    version="1.0.7",
     description="PigeonAI client and SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://www.pigeonsai.com/",
     project_urls={
         "Homepage": "https://www.pigeonsai.com",
```

### Comparing `pigeonsai-1.0.6/src/pigeonsai/_client.py` & `pigeonsai-1.0.7/src/pigeonsai/_client.py`

 * *Files identical despite different names*

### Comparing `pigeonsai-1.0.6/src/pigeonsai/_exceptions.py` & `pigeonsai-1.0.7/src/pigeonsai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pigeonsai-1.0.6/src/pigeonsai/resources/data_connector.py` & `pigeonsai-1.0.7/src/pigeonsai/resources/data_connector.py`

 * *Files identical despite different names*

### Comparing `pigeonsai-1.0.6/src/pigeonsai/resources/recommender.py` & `pigeonsai-1.0.7/src/pigeonsai/resources/recommender.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # resources/recommender.py
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, List, Optional, Union, Dict, Any
 from .._constants import (BASE_URL_V2)
 
 import httpx
 
 if TYPE_CHECKING:
     from .._client import PigeonsAI
     from .data_connector import DataConnector
@@ -61,36 +61,42 @@
         print(f'\033[38;2;85;87;93m Endpoint:\033[0m \033[92m{response_json["data"]["endpoint"]}\033[0m')
         print(f'\033[38;2;85;87;93m Message:\033[0m \033[92m{response_json["message"]}\033[0m')
 
         return response
 
     def _inference(
         self,
-        user_history_ids: Optional[str] = None,
-        user_id: Optional[int] = None,
-        exclude_seen: Optional[bool] = None,
-        k: int = 10,
-        model_endpoint: str = None,
-        model_name: str = None
+        user_id,
+        user_interactions,
+        k,
+        recommend_seen,
+        candidate_ids,
+        model_endpoint,
+        model_name,
     ):
-        if user_history_ids is None and user_id is None:
-            raise ValueError("Either user_id or user_history_ids must be provided.")
+        if not (user_id or user_interactions):
+            raise ValueError("Either user_id or user_interactions must be provided.")
+        if user_id and user_interactions:
+            raise ValueError("Provide either user_id or user_interactions, not both.")
+        if not model_name and not model_endpoint:
+            raise ValueError("Either model_name or model_endpoint must be provided.")
 
-        if model_name and model_endpoint:
-            raise ValueError("Both model_name and model_endpoint are provided. Either one of them will be used.")
+        model_endpoint = _construct_model_url(model_name, model_endpoint, user_id, user_interactions)
 
-        model_endpoint = _construct_model_url(model_endpoint=model_endpoint, model_name=model_name)
-
-        headers = self.client.auth_headers
         data = {
             "k": k,
-            "user_id": user_id,
-            "exclude_seen": exclude_seen,
-            "history_ids": user_history_ids,
+            "recommend_seen": recommend_seen,
+            "candidate_ids": candidate_ids
         }
+        if user_id:
+            data["user_id"] = user_id
+        else:
+            data["user_interactions"] = user_interactions
+
+        headers = self.client.auth_headers
 
         try:
             response = self.client._http_client.post(model_endpoint, headers=headers, json=data, timeout=300.0)
             response.raise_for_status()
             return response.json()
         except httpx.HTTPStatusError as e:
             error_message = f"Status code: {e.response.status_code}, Error: {e.response.text}"
@@ -113,25 +119,26 @@
         data = {
             'unique_identifier': unique_identifier,
             'pull_latest_data': pull_latest_data,
         }
 
         url = BASE_URL_V2 + '/retrain'
         headers = self.client.auth_headers
-        
+
         print(f'\033[38;2;229;192;108m Initializing {unique_identifier} re-training \033[0m')
 
         response = self.client._request("POST", url, headers=headers, data=data)
         response_json = response.json()
-        
+
         print(f'\033[38;2;85;87;93m Re-training job creation successful.\033[0m')
         print(f'\033[38;2;85;87;93m Detail:\033[0m \033[92m{response_json["data"]}\033[0m')
 
         return response
 
+
 class Transformer(BaseModelTrainer):
     def __init__(self, client: PigeonsAI):
         super().__init__(client, model_architecture='transformer')
 
     def train(
         self,
         custom_model_name: str,
@@ -187,36 +194,40 @@
             'optimizer_algorithm': optimizer_algorithm,
             'beta1': beta1,
             'beta2': beta2,
             'weight_decay': weight_decay,
             'subset': subset,
             'threshold': threshold,
         }
-        
-        # get rid of None    
+
+        # get rid of None
         filtered_kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
         return self._train(custom_model_name, train_set_uri, **filtered_kwargs)
 
     def inference(
         self,
-        user_history_ids: Optional[str] = None,
-        user_id: Optional[int] = None,
-        k: int = 10,
+        user_id: Optional[Union[str, int]] = None,
+        user_interactions: Optional[Dict[str, Any]] = None,
+        k: Optional[int] = 10,
+        recommend_seen: Optional[bool] = True,
+        candidate_ids: Optional[List[int]] = None,
         model_endpoint: str = None,
         model_name: str = None
     ):
         return self._inference(
-            user_history_ids=user_history_ids,
             user_id=user_id,
+            user_interactions=user_interactions,
             k=k,
+            recommend_seen=recommend_seen,
+            candidate_ids=candidate_ids,
             model_endpoint=model_endpoint,
             model_name=model_name
         )
-        
+
     def retrain(
         self,
         unique_identifier: str,
         pull_latest_data: bool,
     ):
         return self._retrain(
             unique_identifier=unique_identifier,
@@ -261,49 +272,71 @@
             'eval_user_percent': eval_user_percent,
             'recall_at_k': recall_at_k,
             'eval_iterations': eval_iterations,
             'act_fn': act_fn,
             'likelihood': likelihood,
             'data_subset_percent': data_subset_percent,
         }
-        
+
         # get rid of None
         filtered_kwargs = {k: v for k, v in kwargs.items() if v is not None}
-        
+
         return self._train(custom_model_name, train_set_uri, **filtered_kwargs)
-        
+
     def inference(
         self,
-        user_history_ids: Optional[str] = None,
         user_id: Optional[int] = None,
-        exclude_seen: Optional[bool] = None,
+        user_interactions: Optional[str] = None,
+        recommend_seen: Optional[bool] = None,
         k: int = 10,
         model_endpoint: str = None,
         model_name: str = None
     ):
-        return self._inference(
-            user_history_ids=user_history_ids,
-            user_id=user_id,
-            exclude_seen=exclude_seen,
-            k=k,
-            model_endpoint=model_endpoint,
-            model_name=model_name
-        )
-        
+        if user_interactions is None and user_id is None:
+            raise ValueError("Either user_id or user_history_ids must be provided.")
+
+        if model_name and model_endpoint:
+            raise ValueError("Both model_name and model_endpoint are provided. Either one of them will be used.")
+
+        model_endpoint = _construct_model_url(model_name, model_endpoint, user_id, user_interactions)
+
+        headers = self.client.auth_headers
+        data = {
+            "user_id": user_id,
+            "user_interactions": user_interactions,
+            "k": k,
+            "recommend_seen": recommend_seen,
+        }
+
+        try:
+            response = self.client._http_client.post(model_endpoint, headers=headers, json=data, timeout=300.0)
+            response.raise_for_status()
+            return response.json()
+        except httpx.HTTPStatusError as e:
+            error_message = f"Status code: {e.response.status_code}, Error: {e.response.text}"
+            print(error_message)
+        except Exception as e:
+            raise e
+
     def retrain(
         self,
         unique_identifier: str,
         pull_latest_data: bool,
     ):
         return self._retrain(
             unique_identifier=unique_identifier,
             pull_latest_data=pull_latest_data,
         )
 
 
-def _construct_model_url(model_name: Optional[str] = None, model_endpoint: Optional[str] = None) -> str:
-    if model_name:
-        return f"https://{model_name}.apps.pigeonsai.cloud/recommend"
-    elif model_endpoint:
-        return f"{model_endpoint.rstrip('/')}/recommend"
-    else:
-        raise ValueError("Either model_name or model_endpoint must be provided")
+def _construct_model_url(
+    model_name: Optional[str] = None,
+    model_endpoint: Optional[str] = None,
+    user_id: Optional[str] = None,
+    user_interactions: Optional[Dict[str, Any]] = None
+) -> str:
+    base_endpoint = f"https://{model_name}.apps.pigeonsai.cloud" if model_name else model_endpoint.rstrip('/')
+    if user_interactions:
+        endpoint_suffix = "iid_recommend"
+    elif user_id:
+        endpoint_suffix = "uid_recommend"
+    return f"{base_endpoint}/{endpoint_suffix}"
```

### Comparing `pigeonsai-1.0.6/src/pigeonsai.egg-info/PKG-INFO` & `pigeonsai-1.0.7/src/pigeonsai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 1.0.6
+Version: 1.0.7
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://docs.pigeonsai.com/
```

### Comparing `pigeonsai-1.0.6/src/pigeonsai.egg-info/SOURCES.txt` & `pigeonsai-1.0.7/src/pigeonsai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

