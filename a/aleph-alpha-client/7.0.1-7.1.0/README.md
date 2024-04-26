# Comparing `tmp/aleph-alpha-client-7.0.1.tar.gz` & `tmp/aleph_alpha_client-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-alpha-client-7.0.1.tar", last modified: Wed Feb 21 10:02:00 2024, max compression
+gzip compressed data, was "aleph_alpha_client-7.1.0.tar", last modified: Fri Apr 26 07:07:28 2024, max compression
```

## Comparing `aleph-alpha-client-7.0.1.tar` & `aleph_alpha_client-7.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:02:00.205979 aleph-alpha-client-7.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-02-21 10:02:00.205979 aleph-alpha-client-7.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:02:00.201979 aleph-alpha-client-7.0.1/aleph_alpha_client/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44675 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/aleph_alpha_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17164 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/detokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/document.py
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    19721 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/explanation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16765 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/summarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/aleph_alpha_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:02:00.201979 aleph-alpha-client-7.0.1/aleph_alpha_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-02-21 10:02:00.000000 aleph-alpha-client-7.0.1/aleph_alpha_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-21 10:02:00.000000 aleph-alpha-client-7.0.1/aleph_alpha_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 10:02:00.000000 aleph-alpha-client-7.0.1/aleph_alpha_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-21 10:02:00.000000 aleph-alpha-client-7.0.1/aleph_alpha_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-21 10:02:00.000000 aleph-alpha-client-7.0.1/aleph_alpha_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 10:02:00.205979 aleph-alpha-client-7.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:02:00.201979 aleph-alpha-client-7.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_complete.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_detokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_explanation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-21 10:01:52.000000 aleph-alpha-client-7.0.1/tests/test_wildcard_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:28.833220 aleph_alpha_client-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-26 07:07:28.833220 aleph_alpha_client-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:28.829219 aleph_alpha_client-7.1.0/aleph_alpha_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45155 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/aleph_alpha_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17164 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/detokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19721 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/explanation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16765 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/aleph_alpha_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:28.833220 aleph_alpha_client-7.1.0/aleph_alpha_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-26 07:07:28.000000 aleph_alpha_client-7.1.0/aleph_alpha_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-26 07:07:28.000000 aleph_alpha_client-7.1.0/aleph_alpha_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:07:28.000000 aleph_alpha_client-7.1.0/aleph_alpha_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 07:07:28.000000 aleph_alpha_client-7.1.0/aleph_alpha_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 07:07:28.000000 aleph_alpha_client-7.1.0/aleph_alpha_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 07:07:28.833220 aleph_alpha_client-7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:28.833220 aleph_alpha_client-7.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-26 07:07:21.000000 aleph_alpha_client-7.1.0/tests/test_wildcard_import.py
```

### Comparing `aleph-alpha-client-7.0.1/LICENSE` & `aleph_alpha_client-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/PKG-INFO` & `aleph_alpha_client-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 7.0.1
+Version: 7.1.0
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aleph-alpha-client-7.0.1/README.md` & `aleph_alpha_client-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/__init__.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     TokenControl,
     Tokens,
 )
 from .prompt_template import PromptTemplate
 from .aleph_alpha_client import (
     POOLING_OPTIONS,
     AsyncClient,
+    BusyError,
     Client,
     QuotaError,
 )
 from .completion import CompletionRequest, CompletionResponse
 from .detokenization import DetokenizationRequest, DetokenizationResponse
 from .document import Document
 from .embedding import (
@@ -51,14 +52,15 @@
 from .utils import load_base64_from_file, load_base64_from_url
 from .version import __version__
 
 __all__ = [
     "AsyncClient",
     "BatchSemanticEmbeddingRequest",
     "BatchSemanticEmbeddingResponse",
+    "BusyError",
     "Client",
     "CompletionRequest",
     "CompletionResponse",
     "ControlTokenOverlap",
     "CustomGranularity",
     "DetokenizationRequest",
     "DetokenizationResponse",
```

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/aleph_alpha_client.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/aleph_alpha_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,17 @@
         nice(bool, required, default False):
             Setting this to True, will signal to the API that you intend to be nice to other users
             by de-prioritizing your request below concurrent ones.
 
         verify_ssl(bool, optional, default True)
             Setting this to False will disable checking for SSL when doing requests.
 
+        tags(Optional[Sequence[str]], optional, default None)
+            Internal feature.
+
     Example usage:
         >>> request = CompletionRequest(
                 prompt=Prompt.from_text(f"Request"), maximum_tokens=64
             )
         >>> client = Client(token=os.environ["AA_TOKEN"])
         >>> response: CompletionResponse = client.complete(request, "luminous-base")
     """
@@ -159,22 +162,24 @@
         token: str,
         host: str = "https://api.aleph-alpha.com",
         hosting: Optional[str] = None,
         request_timeout_seconds: int = DEFAULT_REQUEST_TIMEOUT,
         total_retries: int = 8,
         nice: bool = False,
         verify_ssl=True,
+        tags: Optional[Sequence[str]] = None,
     ) -> None:
         if host[-1] != "/":
             host += "/"
         self.host = host
         self.hosting = hosting
         self.request_timeout_seconds = request_timeout_seconds
         self.token = token
         self.nice = nice
+        self.tags = tags
 
         retry_strategy = Retry(
             total=total_retries,
             backoff_factor=0.25,
             status_forcelist=RETRY_STATUS_CODES,
             allowed_methods=["POST", "GET"],
             raise_on_status=False,
@@ -238,14 +243,16 @@
     ) -> Mapping[str, Any]:
         json_body = dict(request.to_json())
 
         if model is not None:
             json_body["model"] = model
         if self.hosting is not None:
             json_body["hosting"] = self.hosting
+        if self.tags is not None:
+            json_body["tags"] = self.tags
         return json_body
 
     def models(self) -> List[Mapping[str, Any]]:
         """
         Queries all models which are currently available.
 
         For documentation of the response, see https://docs.aleph-alpha.com/api/available-models/
@@ -628,14 +635,17 @@
         nice(bool, required, default False):
             Setting this to True, will signal to the API that you intend to be nice to other users
             by de-prioritizing your request below concurrent ones.
 
         verify_ssl(bool, optional, default True)
             Setting this to False will disable checking for SSL when doing requests.
 
+        tags(Optional[Sequence[str]], optional, default None)
+            Internal feature.
+
     Example usage:
         >>> request = CompletionRequest(prompt=Prompt.from_text(f"Request"), maximum_tokens=64)
         >>> async with AsyncClient(token=os.environ["AA_TOKEN"]) as client:
                 response: CompletionResponse = await client.complete(request, "luminous-base")
     """
 
     def __init__(
@@ -643,22 +653,24 @@
         token: str,
         host: str = "https://api.aleph-alpha.com",
         hosting: Optional[str] = None,
         request_timeout_seconds: int = DEFAULT_REQUEST_TIMEOUT,
         total_retries: int = 8,
         nice: bool = False,
         verify_ssl=True,
+        tags: Optional[Sequence[str]] = None,
     ) -> None:
         if host[-1] != "/":
             host += "/"
         self.host = host
         self.hosting = hosting
         self.request_timeout_seconds = request_timeout_seconds
         self.token = token
         self.nice = nice
+        self.tags = tags
 
         retry_options = ExponentialRetry(
             attempts=total_retries + 1,
             exceptions={aiohttp.ClientConnectionError},
             start_timeout=0.25,
             statuses=set(RETRY_STATUS_CODES),
         )
@@ -758,14 +770,16 @@
     ) -> Mapping[str, Any]:
         json_body = dict(request.to_json())
 
         if model is not None:
             json_body["model"] = model
         if self.hosting is not None:
             json_body["hosting"] = self.hosting
+        if self.tags is not None:
+            json_body["tags"] = self.tags
         return json_body
 
     async def models(self) -> List[Mapping[str, Any]]:
         """
         Queries all models which are currently available.
 
         For documentation of the response, see https://docs.aleph-alpha.com/api/available-models/
```

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/completion.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/completion.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/detokenization.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/detokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/document.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/document.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/embedding.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/embedding.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/evaluation.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/evaluation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/explanation.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/explanation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/prompt.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/prompt_template.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/prompt_template.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/qa.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/summarization.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/summarization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client/tokenization.py` & `aleph_alpha_client-7.1.0/aleph_alpha_client/tokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client.egg-info/PKG-INFO` & `aleph_alpha_client-7.1.0/aleph_alpha_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 7.0.1
+Version: 7.1.0
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aleph-alpha-client-7.0.1/aleph_alpha_client.egg-info/SOURCES.txt` & `aleph_alpha_client-7.1.0/aleph_alpha_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/setup.py` & `aleph_alpha_client-7.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         "aiodns >= 3.0.0",
         "aiohttp-retry >= 2.8.3",
         "tokenizers >= 0.13.2",
         "typing_extensions >= 4.5.0",
         "Pillow >= 9.2.0",
         "tqdm >= v4.62.0",
         "python-liquid >= 1.9.4",
-        "packaging >= 23.2"
+        "packaging >= 23.2",
     ],
     tests_require=tests_require,
     extras_require={
         "test": tests_require,
         "types": types_require,
         "dev": dev_require,
         "docs": docs_require,
```

### Comparing `aleph-alpha-client-7.0.1/tests/test_clients.py` & `aleph_alpha_client-7.1.0/tests/test_clients.py`

 * *Files 23% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     try:
         _ = await client.complete(request, model=model_name)
     finally:
         await client.close()
 
 
 def test_nice_flag_on_client(httpserver: HTTPServer):
-    httpserver.expect_request("/version").respond_with_data("OK")
+    httpserver.expect_request("/version").respond_with_data(MIN_API_VERSION)
 
     httpserver.expect_request(
         "/complete", query_string={"nice": "true"}
     ).respond_with_json(
         CompletionResponse(
             "model_version",
             [
@@ -75,15 +75,15 @@
     client = Client(host=httpserver.url_for(""), token="AA_TOKEN", nice=True)
 
     request = CompletionRequest(prompt=Prompt.from_text("Hello world"))
     client.complete(request, model="luminous")
 
 
 async def test_nice_flag_on_async_client(httpserver: HTTPServer):
-    httpserver.expect_request("/version").respond_with_data("OK")
+    httpserver.expect_request("/version").respond_with_data(MIN_API_VERSION)
 
     httpserver.expect_request(
         "/complete",
         query_string={"nice": "true"},
     ).respond_with_json(
         CompletionResponse(
             "model_version",
@@ -92,15 +92,71 @@
             num_tokens_generated=1,
         ).to_json()
     )
 
     request = CompletionRequest(prompt=Prompt.from_text("Hello world"))
 
     async with AsyncClient(
-        host=httpserver.url_for(""), token="AA_TOKEN", nice=True
+        host=httpserver.url_for(""),
+        token="AA_TOKEN",
+        nice=True,
+        request_timeout_seconds=1,
+    ) as client:
+        await client.complete(request, model="luminous")
+
+
+def test_tags_on_client(httpserver: HTTPServer):
+    httpserver.expect_request("/version").respond_with_data(MIN_API_VERSION)
+
+    request = CompletionRequest(prompt=Prompt.from_text("Hello world"))
+    body = {k: v for k, v in request.to_json().items() if v is not None}
+    body["tags"] = ["tim-tagger"]
+    body["model"] = "luminous"
+    httpserver.expect_request("/complete", json=body).respond_with_json(
+        CompletionResponse(
+            "model_version",
+            [
+                CompletionResult(
+                    log_probs=[],
+                    completion="foo",
+                )
+            ],
+            num_tokens_prompt_total=2,
+            num_tokens_generated=1,
+        ).to_json()
+    )
+
+    client = Client(
+        host=httpserver.url_for(""),
+        request_timeout_seconds=1,
+        token="AA_TOKEN",
+        tags=["tim-tagger"],
+    )
+
+    client.complete(request, model="luminous")
+
+
+async def test_tags_on_async_client(httpserver: HTTPServer):
+    httpserver.expect_request("/version").respond_with_data(MIN_API_VERSION)
+
+    request = CompletionRequest(prompt=Prompt.from_text("Hello world"))
+    body = {k: v for k, v in request.to_json().items() if v is not None}
+    body["tags"] = ["tim-tagger"]
+    body["model"] = "luminous"
+    httpserver.expect_request("/complete", json=body).respond_with_json(
+        CompletionResponse(
+            "model_version",
+            [CompletionResult(log_probs=[], completion="foo")],
+            num_tokens_prompt_total=2,
+            num_tokens_generated=1,
+        ).to_json()
+    )
+
+    async with AsyncClient(
+        host=httpserver.url_for(""), token="AA_TOKEN", tags=["tim-tagger"]
     ) as client:
         await client.complete(request, model="luminous")
 
 
 @pytest.mark.system_test
 def test_available_models_sync_client(sync_client: Client, model_name: str):
     models = sync_client.models()
```

### Comparing `aleph-alpha-client-7.0.1/tests/test_complete.py` & `aleph_alpha_client-7.1.0/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/tests/test_detokenize.py` & `aleph_alpha_client-7.1.0/tests/test_detokenize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/tests/test_embed.py` & `aleph_alpha_client-7.1.0/tests/test_embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from pytest_httpserver import HTTPServer
 
 from aleph_alpha_client import EmbeddingRequest
 from aleph_alpha_client.aleph_alpha_client import AsyncClient, Client
 from aleph_alpha_client.embedding import (
     BatchSemanticEmbeddingRequest,
     SemanticEmbeddingRequest,
-    SemanticRepresentation, BatchSemanticEmbeddingResponse,
+    SemanticRepresentation,
+    BatchSemanticEmbeddingResponse,
 )
 from aleph_alpha_client.prompt import Prompt
 from tests.common import (
     sync_client,
     async_client,
     model_name,
 )
@@ -57,23 +58,28 @@
 @pytest.mark.parametrize("num_prompts", [1, 100, 101])
 @pytest.mark.parametrize("batch_size", [1, 32, 100])
 async def test_batch_embed_semantic_with_async_client(
     async_client: AsyncClient, sync_client: Client, num_prompts: int, batch_size: int
 ):
     words = ["car", "elephant", "kitchen sink", "rubber", "sun"]
     r = random.Random(4082)
-    prompts = list([Prompt.from_text(words[r.randint(0, 4)]) for i in range(num_prompts)])
+    prompts = list(
+        [Prompt.from_text(words[r.randint(0, 4)]) for i in range(num_prompts)]
+    )
 
     request = BatchSemanticEmbeddingRequest(
         prompts=prompts,
         representation=SemanticRepresentation.Symmetric,
         compress_to_size=128,
     )
     result = await async_client.batch_semantic_embed(
-        request=request, num_concurrent_requests=10, batch_size=batch_size, model="luminous-base"
+        request=request,
+        num_concurrent_requests=10,
+        batch_size=batch_size,
+        model="luminous-base",
     )
 
     # We have no control over the exact tokenizer used in the backend, so we cannot know the exact
     # number of tokens. We do know, however, that there must be at least one token per prompt.
     assert result.num_tokens_prompt_total >= num_prompts
 
     assert len(result.embeddings) == num_prompts
@@ -123,15 +129,19 @@
     model_name = "test_model"
     expected_body = {
         **request.to_json(),
         "model": model_name,
     }
     httpserver.expect_ordered_request(
         "/batch_semantic_embed", method="POST", data=json.dumps(expected_body)
-    ).respond_with_json(BatchSemanticEmbeddingResponse(model_version="1", embeddings=[], num_tokens_prompt_total=1).to_json())
+    ).respond_with_json(
+        BatchSemanticEmbeddingResponse(
+            model_version="1", embeddings=[], num_tokens_prompt_total=1
+        ).to_json()
+    )
     async_client = AsyncClient(token="", host=httpserver.url_for(""), total_retries=1)
     await async_client.batch_semantic_embed(request, model=model_name)
 
 
 # Client
 
 
@@ -222,10 +232,14 @@
         prompts=[Prompt.from_text("hello")],
         representation=SemanticRepresentation.Symmetric,
     )
     model_name = "test_model"
     expected_body = {**request.to_json(), "model": model_name}
     httpserver.expect_ordered_request(
         "/batch_semantic_embed", method="POST", data=json.dumps(expected_body)
-    ).respond_with_json(BatchSemanticEmbeddingResponse(model_version="1", embeddings=[], num_tokens_prompt_total=1).to_json())
+    ).respond_with_json(
+        BatchSemanticEmbeddingResponse(
+            model_version="1", embeddings=[], num_tokens_prompt_total=1
+        ).to_json()
+    )
     sync_client = Client(token="", host=httpserver.url_for(""), total_retries=1)
     sync_client.batch_semantic_embed(request, model=model_name)
```

### Comparing `aleph-alpha-client-7.0.1/tests/test_error_handling.py` & `aleph_alpha_client-7.1.0/tests/test_error_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,13 +107,18 @@
         httpserver.expect_ordered_request(re.compile("^/")).respond_with_data(
             f"error({i})", status=status_code or choice(list(RETRY_STATUS_CODES))
         )
 
 
 def expect_valid_completion(httpserver: HTTPServer) -> None:
     httpserver.expect_ordered_request("/complete").respond_with_json(
-        CompletionResponse(model_version="1", completions=[], num_tokens_prompt_total=0, num_tokens_generated=0).to_json()
+        CompletionResponse(
+            model_version="1",
+            completions=[],
+            num_tokens_prompt_total=0,
+            num_tokens_generated=0,
+        ).to_json()
     )
 
 
 def expect_valid_version(httpserver: HTTPServer) -> None:
     httpserver.expect_ordered_request("/version").respond_with_data("ok", status=200)
```

### Comparing `aleph-alpha-client-7.0.1/tests/test_evaluate.py` & `aleph_alpha_client-7.1.0/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/tests/test_explanation.py` & `aleph_alpha_client-7.1.0/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/tests/test_image.py` & `aleph_alpha_client-7.1.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/tests/test_prompt.py` & `aleph_alpha_client-7.1.0/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/tests/test_prompt_template.py` & `aleph_alpha_client-7.1.0/tests/test_prompt_template.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/tests/test_qa.py` & `aleph_alpha_client-7.1.0/tests/test_qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/tests/test_summarize.py` & `aleph_alpha_client-7.1.0/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-7.0.1/tests/test_tokenize.py` & `aleph_alpha_client-7.1.0/tests/test_tokenize.py`

 * *Files identical despite different names*

