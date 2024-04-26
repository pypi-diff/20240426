# Comparing `tmp/e2enetworks-1.2.2.tar.gz` & `tmp/e2enetworks-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-1.2.2.tar", last modified: Wed Apr 17 10:20:46 2024, max compression
+gzip compressed data, was "e2enetworks-1.2.3.tar", last modified: Fri Apr 26 12:50:45 2024, max compression
```

## Comparing `e2enetworks-1.2.2.tar` & `e2enetworks-1.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-17 10:20:46.289658 e2enetworks-1.2.2/
--rw-r--r--   0 jagga      (501) staff       (20)    10786 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/LICENSE.txt
--rw-r--r--   0 jagga      (501) staff       (20)     1418 2024-04-17 10:20:46.289445 e2enetworks-1.2.2/PKG-INFO
--rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/README.rst
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-17 10:20:46.284177 e2enetworks-1.2.2/e2enetworks/
--rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/__init__.py
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-17 10:20:46.285296 e2enetworks-1.2.2/e2enetworks/cloud/
--rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/__init__.py
--rw-r--r--   0 jagga      (501) staff       (20)      147 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/test.py
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-17 10:20:46.288985 e2enetworks-1.2.2/e2enetworks/cloud/tir/
--rw-r--r--   0 jagga      (501) staff       (20)     2290 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/__init__.py
--rw-r--r--   0 jagga      (501) staff       (20)     9305 2024-04-17 10:17:07.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/api_client.py
--rw-r--r--   0 jagga      (501) staff       (20)     2794 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/apitoken.py
--rw-r--r--   0 jagga      (501) staff       (20)     9405 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/client.py
--rw-r--r--   0 jagga      (501) staff       (20)     7401 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/constants.py
--rw-r--r--   0 jagga      (501) staff       (20)     5788 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/datasets.py
--rw-r--r--   0 jagga      (501) staff       (20)    13823 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/endpoints.py
--rw-r--r--   0 jagga      (501) staff       (20)     2619 2024-04-17 10:17:07.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/helpers.py
--rw-r--r--   0 jagga      (501) staff       (20)     1368 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/images.py
--rw-r--r--   0 jagga      (501) staff       (20)     2105 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/minio_service.py
--rw-r--r--   0 jagga      (501) staff       (20)     6455 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/models.py
--rw-r--r--   0 jagga      (501) staff       (20)     6022 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/notebook.py
--rw-r--r--   0 jagga      (501) staff       (20)     9999 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/pipelines.py
--rw-r--r--   0 jagga      (501) staff       (20)     2849 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/projects.py
--rw-r--r--   0 jagga      (501) staff       (20)     4268 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/skus.py
--rw-r--r--   0 jagga      (501) staff       (20)     2391 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/teams.py
--rw-r--r--   0 jagga      (501) staff       (20)     1159 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/utils.py
--rw-r--r--   0 jagga      (501) staff       (20)       23 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/version.py
--rw-r--r--   0 jagga      (501) staff       (20)     1517 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/constants.py
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-17 10:20:46.289195 e2enetworks-1.2.2/e2enetworks.egg-info/
--rw-r--r--   0 jagga      (501) staff       (20)     1418 2024-04-17 10:20:46.000000 e2enetworks-1.2.2/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 jagga      (501) staff       (20)      914 2024-04-17 10:20:46.000000 e2enetworks-1.2.2/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 jagga      (501) staff       (20)        1 2024-04-17 10:20:46.000000 e2enetworks-1.2.2/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 jagga      (501) staff       (20)      138 2024-04-17 10:20:46.000000 e2enetworks-1.2.2/e2enetworks.egg-info/requires.txt
--rw-r--r--   0 jagga      (501) staff       (20)       12 2024-04-17 10:20:46.000000 e2enetworks-1.2.2/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 jagga      (501) staff       (20)       38 2024-04-17 10:20:46.289710 e2enetworks-1.2.2/setup.cfg
--rw-r--r--   0 jagga      (501) staff       (20)     1829 2024-04-17 10:17:07.000000 e2enetworks-1.2.2/setup.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-26 12:50:45.184798 e2enetworks-1.2.3/
+-rw-r--r--   0 jagga      (501) staff       (20)    10786 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/LICENSE.txt
+-rw-r--r--   0 jagga      (501) staff       (20)     1418 2024-04-26 12:50:45.184532 e2enetworks-1.2.3/PKG-INFO
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/README.rst
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-26 12:50:45.178562 e2enetworks-1.2.3/e2enetworks/
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/__init__.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-26 12:50:45.179627 e2enetworks-1.2.3/e2enetworks/cloud/
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/__init__.py
+-rw-r--r--   0 jagga      (501) staff       (20)      147 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/test.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-26 12:50:45.183981 e2enetworks-1.2.3/e2enetworks/cloud/tir/
+-rw-r--r--   0 jagga      (501) staff       (20)     2290 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/__init__.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9305 2024-04-17 10:17:07.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/api_client.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2794 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/apitoken.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9405 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/client.py
+-rw-r--r--   0 jagga      (501) staff       (20)     8779 2024-04-26 12:46:31.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/constants.py
+-rw-r--r--   0 jagga      (501) staff       (20)     5788 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/datasets.py
+-rw-r--r--   0 jagga      (501) staff       (20)    13823 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/endpoints.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2619 2024-04-17 10:17:07.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/helpers.py
+-rw-r--r--   0 jagga      (501) staff       (20)     1368 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/images.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2105 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/minio_service.py
+-rw-r--r--   0 jagga      (501) staff       (20)     6455 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/models.py
+-rw-r--r--   0 jagga      (501) staff       (20)     6022 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/notebook.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9999 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/pipelines.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2849 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/projects.py
+-rw-r--r--   0 jagga      (501) staff       (20)     4268 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/skus.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2391 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/teams.py
+-rw-r--r--   0 jagga      (501) staff       (20)     1159 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/utils.py
+-rw-r--r--   0 jagga      (501) staff       (20)       23 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/version.py
+-rw-r--r--   0 jagga      (501) staff       (20)     1561 2024-04-26 12:43:02.000000 e2enetworks-1.2.3/e2enetworks/constants.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-26 12:50:45.184229 e2enetworks-1.2.3/e2enetworks.egg-info/
+-rw-r--r--   0 jagga      (501) staff       (20)     1418 2024-04-26 12:50:45.000000 e2enetworks-1.2.3/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 jagga      (501) staff       (20)      914 2024-04-26 12:50:45.000000 e2enetworks-1.2.3/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 jagga      (501) staff       (20)        1 2024-04-26 12:50:45.000000 e2enetworks-1.2.3/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 jagga      (501) staff       (20)      138 2024-04-26 12:50:45.000000 e2enetworks-1.2.3/e2enetworks.egg-info/requires.txt
+-rw-r--r--   0 jagga      (501) staff       (20)       12 2024-04-26 12:50:45.000000 e2enetworks-1.2.3/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 jagga      (501) staff       (20)       38 2024-04-26 12:50:45.184851 e2enetworks-1.2.3/setup.cfg
+-rw-r--r--   0 jagga      (501) staff       (20)     1829 2024-04-26 12:49:58.000000 e2enetworks-1.2.3/setup.py
```

### Comparing `e2enetworks-1.2.2/LICENSE.txt` & `e2enetworks-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/PKG-INFO` & `e2enetworks-1.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 1.2.2
+Version: 1.2.3
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
```

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/__init__.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/__init__.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/api_client.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/api_client.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/apitoken.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/apitoken.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/client.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/client.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/constants.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,83 @@
 
-from e2enetworks.constants import WHISPER_LARGE_V3,LLAMA_2_13B_CHAT, STABLE_DIFFUSION_2_1,MIXTRAL_8X7B_INSTRUCT, CODELLAMA_13B_INSTRUCT, E5_MISTRAL_7B_INSTRUCT
-ARGUMENT_IS_MANDATORY = "IS MANDATORY" 
+from e2enetworks.constants import WHISPER_LARGE_V3, LLAMA_2_13B_CHAT, STABLE_DIFFUSION_2_1, MIXTRAL_8X7B_INSTRUCT, \
+    CODELLAMA_13B_INSTRUCT, E5_MISTRAL_7B_INSTRUCT, LLAMA_3_8B_INSTRUCT
+
+ARGUMENT_IS_MANDATORY = "IS MANDATORY"
     
 MODEL_NAME_TO_URL_PATH_MAPPING = {
     LLAMA_2_13B_CHAT : "project/{namespace}/v1/llama-2-13b-chat/infer",
     STABLE_DIFFUSION_2_1 : "project/{namespace}/v1/stable-diffusion-2-1/infer",
     MIXTRAL_8X7B_INSTRUCT: "project/{namespace}/v1/mixtral-8x7b-instruct/infer",
     CODELLAMA_13B_INSTRUCT : "project/{namespace}/v1/codellama-13b-instruct/infer",
     WHISPER_LARGE_V3 : "project/{namespace}/v1/whisper-large-v3/infer",
-    E5_MISTRAL_7B_INSTRUCT: "project/{namespace}/v1/e5-mistral-7b-instruct/infer"
+    E5_MISTRAL_7B_INSTRUCT: "project/{namespace}/v1/e5-mistral-7b-instruct/infer",
+    LLAMA_3_8B_INSTRUCT: "project/{namespace}/v1/llama-3-8b-instruct/infer",
 }
 MODEL_API_DEFAULT_DATA = {"inputs": []}
 
 MODELS_API_DATA_FORMATS = {
     LLAMA_2_13B_CHAT: {
         "prompt": {
             "name": "prompt",
             "shape": [1],
             "datatype": "BYTES",
             "data": [],
         },
         "system_prompt": {
+            "name": "system_prompt",
+            "shape": [1],
+            "datatype": "BYTES",
+            "data": [],
+        },
+        "max_new_tokens": {
+            "name": "max_new_tokens",
+            "shape": [1],
+            "datatype": "INT32",
+            "data": [],
+        },
+        "top_k": {
+            "name": "top_k",
+            "shape": [1],
+            "datatype": "INT32",
+            "data": [],
+        },
+        "top_p": {
+            "name": "top_p",
+            "shape": [1],
+            "datatype": "FP32",
+            "data": [],
+        },
+        "temperature": {
+            "name": "temperature",
+            "shape": [1],
+            "datatype": "FP32",
+            "data": [],
+        },
+        "num_return_sequences": {
+            "name": "num_return_sequences",
+            "shape": [1],
+            "datatype": "INT32",
+            "data": [],
+        },
+        "repetition_penalty": {
+            "name": "repetition_penalty",
+            "shape": [1],
+            "datatype": "FP32",
+            "data": [],
+        },
+    },
+    LLAMA_3_8B_INSTRUCT: {
+        "prompt": {
+            "name": "prompt",
+            "shape": [1],
+            "datatype": "BYTES",
+            "data": [],
+        },
+        "system_prompt": {
             "name": "system_prompt",
             "shape": [1],
             "datatype": "BYTES",
             "data": [],
         },
         "max_new_tokens": {
             "name": "max_new_tokens",
```

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/datasets.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/datasets.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/endpoints.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/endpoints.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/helpers.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/helpers.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/images.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/images.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/minio_service.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/minio_service.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/models.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/models.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/notebook.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/notebook.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/pipelines.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/pipelines.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/projects.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/projects.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/skus.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/skus.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/teams.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/teams.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/cloud/tir/utils.py` & `e2enetworks-1.2.3/e2enetworks/cloud/tir/utils.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/e2enetworks/constants.py` & `e2enetworks-1.2.3/e2enetworks/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 
 WHISPER_DATA_LIMIT_BYTES = 50000000
 WHISPER_LARGE_V3 = "whisper-large-v3"
 LLAMA_2_13B_CHAT = "llama-2-13b-chat"
 STABLE_DIFFUSION_2_1 = "stable-diffusion-2-1"
 MIXTRAL_8X7B_INSTRUCT = "mixtral-8x7b-instruct"
 CODELLAMA_13B_INSTRUCT = "codellama-13b-instruct"
-E5_MISTRAL_7B_INSTRUCT = "e5-mistral-7b-instruct"
+E5_MISTRAL_7B_INSTRUCT = "e5-mistral-7b-instruct"
+LLAMA_3_8B_INSTRUCT = "llama-3-8b-instruct"
```

### Comparing `e2enetworks-1.2.2/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-1.2.3/e2enetworks.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 1.2.2
+Version: 1.2.3
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
```

### Comparing `e2enetworks-1.2.2/e2enetworks.egg-info/SOURCES.txt` & `e2enetworks-1.2.3/e2enetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.2/setup.py` & `e2enetworks-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "1.2.2"
+version = "1.2.3"
 install_requires = [
     "requests~=2.30.0",
     "urllib3==1.26.6",
     "kfp==1.8.22",
     "kfp-pipeline-spec==0.1.16",
     "kfp-server-api==1.8.5",
     "minio==7.1.3",
```

