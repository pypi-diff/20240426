# Comparing `tmp/log10_io-0.8.2.tar.gz` & `tmp/log10_io-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log10_io-0.8.2.tar", max compression
+gzip compressed data, was "log10_io-0.8.3.tar", max compression
```

## Comparing `log10_io-0.8.2.tar` & `log10_io-0.8.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1083 2024-04-24 22:32:57.779244 log10_io-0.8.2/LICENSE
--rw-r--r--   0        0        0     9613 2024-04-24 22:32:57.779244 log10_io-0.8.2/README.md
--rw-r--r--   0        0        0        0 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/__init__.py
--rw-r--r--   0        0        0     1550 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/__main__.py
--rw-r--r--   0        0        0    11700 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/_httpx_utils.py
--rw-r--r--   0        0        0     9112 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/agents/camel.py
--rw-r--r--   0        0        0      722 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     6079 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/anthropic.py
--rw-r--r--   0        0        0     2578 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/bigquery.py
--rw-r--r--   0        0        0      719 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/cli_utils.py
--rw-r--r--   0        0        0    22337 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/completions/completions.py
--rw-r--r--   0        0        0     2648 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/evals.py
--rw-r--r--   0        0        0     5459 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/feedback/_summary_feedback_utils.py
--rw-r--r--   0        0        0     4487 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/feedback/autofeedback.py
--rw-r--r--   0        0        0     8357 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/feedback/feedback.py
--rw-r--r--   0        0        0     4880 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/feedback/feedback_task.py
--rw-r--r--   0        0        0     9274 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/langchain.py
--rw-r--r--   0        0        0     4432 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/litellm.py
--rw-r--r--   0        0        0     7967 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/llm.py
--rw-r--r--   0        0        0    39884 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/load.py
--rw-r--r--   0        0        0     2886 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/mosaicml.py
--rw-r--r--   0        0        0     3217 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/openai.py
--rw-r--r--   0        0        0     6915 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/prompt_analyzer.py
--rw-r--r--   0        0        0     1020 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/schemas/bigquery.json
--rw-r--r--   0        0        0     2654 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/together.py
--rw-r--r--   0        0        0     2101 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/tools.py
--rw-r--r--   0        0        0     1211 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/utils.py
--rw-r--r--   0        0        0     2242 2024-04-24 22:32:57.787244 log10_io-0.8.2/pyproject.toml
--rw-r--r--   0        0        0    11109 1970-01-01 00:00:00.000000 log10_io-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-26 00:11:42.135162 log10_io-0.8.3/LICENSE
+-rw-r--r--   0        0        0     9613 2024-04-26 00:11:42.135162 log10_io-0.8.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/__init__.py
+-rw-r--r--   0        0        0     1550 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/__main__.py
+-rw-r--r--   0        0        0    11352 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/_httpx_utils.py
+-rw-r--r--   0        0        0     9112 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/agents/camel.py
+-rw-r--r--   0        0        0      722 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     6079 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/anthropic.py
+-rw-r--r--   0        0        0     2578 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/bigquery.py
+-rw-r--r--   0        0        0      719 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/cli_utils.py
+-rw-r--r--   0        0        0    22337 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/completions/completions.py
+-rw-r--r--   0        0        0     2648 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/evals.py
+-rw-r--r--   0        0        0     5459 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/feedback/_summary_feedback_utils.py
+-rw-r--r--   0        0        0     4487 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/feedback/autofeedback.py
+-rw-r--r--   0        0        0     8357 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/feedback/feedback.py
+-rw-r--r--   0        0        0     4880 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/feedback/feedback_task.py
+-rw-r--r--   0        0        0     9274 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/langchain.py
+-rw-r--r--   0        0        0     4432 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/litellm.py
+-rw-r--r--   0        0        0     7967 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/llm.py
+-rw-r--r--   0        0        0    39993 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/load.py
+-rw-r--r--   0        0        0     2886 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/mosaicml.py
+-rw-r--r--   0        0        0     3217 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/openai.py
+-rw-r--r--   0        0        0     6915 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/prompt_analyzer.py
+-rw-r--r--   0        0        0     1020 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0     2654 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/together.py
+-rw-r--r--   0        0        0     2101 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/tools.py
+-rw-r--r--   0        0        0     1211 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/utils.py
+-rw-r--r--   0        0        0     2242 2024-04-26 00:11:42.143162 log10_io-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0    11109 1970-01-01 00:00:00.000000 log10_io-0.8.3/PKG-INFO
```

### Comparing `log10_io-0.8.2/LICENSE` & `log10_io-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/README.md` & `log10_io-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/__main__.py` & `log10_io-0.8.3/log10/__main__.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/_httpx_utils.py` & `log10_io-0.8.3/log10/_httpx_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         full_response = ""
         finished = False
         async for chunk in super().aiter_bytes(*args, **kwargs):
             full_response += chunk.decode(errors="ignore")
 
             if "data: [DONE]" in full_response:
                 finished = True
+                duration = int(time.time() - self.request.started) * 1000
 
                 completion_id = self.request.headers.get("x-log10-completion-id", "")
                 if finished and completion_id:
                     current_stack_frame = traceback.extract_stack()
                     stacktrace = [
                         {
                             "file": frame.filename,
@@ -200,42 +201,36 @@
                             if tc[0].get("id", ""):
                                 tool_calls.append(tc[0])
                             elif tc[0].get("function", {}).get("arguments", ""):
                                 idx = tc[0].get("index")
                                 tool_calls[idx]["function"]["arguments"] += tc[0]["function"]["arguments"]
 
                     response_json = r_json.copy()
-                    response_json["object"] = "completion"
+                    response_json["object"] = "chat.completion"
                     # r_json is the last response before "data: [DONE]"
-                    # it contains the finish_reason
-                    finish_reason = response_json["choices"][0]["finish_reason"]
 
-                    # If finish_reason is function_call - don't log the response
-                    if not (
-                        "choices" in response_json
-                        and response_json["choices"]
-                        and response_json["choices"][0]["finish_reason"] in ["function_call", "tool_calls"]
-                    ):
+                    if full_content:
                         response_json["choices"][0]["message"] = {"role": "assistant", "content": full_content}
-                    elif finish_reason == "function_call":
-                        response_json["choices"][0]["function_call"] = {
-                            "name": function_name,
-                            "arguments": full_argument,
-                        }
-                    elif finish_reason == "tool_calls":
+                    elif tool_calls:
                         response_json["choices"][0]["message"] = {
                             "content": None,
                             "role": "assistant",
                             "tool_calls": tool_calls,
                         }
+                    elif function_name and full_argument:
+                        # function is deprecated in openai api
+                        response_json["choices"][0]["function_call"] = {
+                            "name": function_name,
+                            "arguments": full_argument,
+                        }
 
                     log_row = {
                         "response": json.dumps(response_json),
                         "status": "finished",
-                        "duration": int(time.time() - self.request.started) * 1000,
+                        "duration": duration,
                         "stacktrace": json.dumps(stacktrace),
                         "kind": "chat",
                         "request": self.request.content.decode("utf-8"),
                         "session_id": sessionID,
                     }
                     if get_log10_session_tags():
                         log_row["tags"] = get_log10_session_tags()
@@ -250,15 +245,15 @@
     async def handle_async_request(self, request: httpx.Request) -> httpx.Response:
         response = await self.transport.handle_async_request(request)
 
         completion_id = request.headers.get("x-log10-completion-id", "")
         if not completion_id:
             return response
 
-        if response.headers.get("content-type") == "application/json":
+        if response.headers.get("content-type").startswith("application/json"):
             await response.aread()
             llm_response = response.json()
 
             current_stack_frame = traceback.extract_stack()
             stacktrace = [
                 {
                     "file": frame.filename,
```

### Comparing `log10_io-0.8.2/log10/agents/camel.py` & `log10_io-0.8.3/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/agents/scrape_summarizer.py` & `log10_io-0.8.3/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/anthropic.py` & `log10_io-0.8.3/log10/anthropic.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/bigquery.py` & `log10_io-0.8.3/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/cli_utils.py` & `log10_io-0.8.3/log10/cli_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/completions/completions.py` & `log10_io-0.8.3/log10/completions/completions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/evals.py` & `log10_io-0.8.3/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/feedback/_summary_feedback_utils.py` & `log10_io-0.8.3/log10/feedback/_summary_feedback_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/feedback/autofeedback.py` & `log10_io-0.8.3/log10/feedback/autofeedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/feedback/feedback.py` & `log10_io-0.8.3/log10/feedback/feedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/feedback/feedback_task.py` & `log10_io-0.8.3/log10/feedback/feedback_task.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/langchain.py` & `log10_io-0.8.3/log10/langchain.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/litellm.py` & `log10_io-0.8.3/log10/litellm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/llm.py` & `log10_io-0.8.3/log10/llm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/load.py` & `log10_io-0.8.3/log10/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,14 +529,17 @@
         log_row["kind"] = "chat"
         kwargs_copy.update(
             {"model": args[1]["model_name"], "messages": [{"role": "user", "content": args[1]["prompt"]}]}
         )
     elif "mistralai" in func.__module__:
         log_row["kind"] = "chat"
     elif "openai" in func.__module__:
+        from openai._utils._utils import strip_not_given
+
+        kwargs_copy = strip_not_given(kwargs_copy)
         kind = "chat" if "chat" in func.__module__ else "completion"
         log_row["kind"] = kind
     elif "google.generativeai" in func.__module__:
         if func.__name__ == "send_message":
             log_row["kind"] = "chat"
             history_messages = []
             if system_instruction := args[0].model._system_instruction:
```

### Comparing `log10_io-0.8.2/log10/mosaicml.py` & `log10_io-0.8.3/log10/mosaicml.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/openai.py` & `log10_io-0.8.3/log10/openai.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/prompt_analyzer.py` & `log10_io-0.8.3/log10/prompt_analyzer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/schemas/bigquery.json` & `log10_io-0.8.3/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/together.py` & `log10_io-0.8.3/log10/together.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/tools.py` & `log10_io-0.8.3/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/log10/utils.py` & `log10_io-0.8.3/log10/utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.2/pyproject.toml` & `log10_io-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "log10-io"
 
-version = "0.8.2"
+version = "0.8.3"
 authors = ["log10 team"]
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `log10_io-0.8.2/PKG-INFO` & `log10_io-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.8.2
+Version: 0.8.3
 Summary: Unified LLM data management
 License: MIT
 Author: log10 team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

