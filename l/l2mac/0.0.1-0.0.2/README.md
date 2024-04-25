# Comparing `tmp/l2mac-0.0.1.tar.gz` & `tmp/l2mac-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2mac-0.0.1.tar", last modified: Tue Apr 23 15:47:27 2024, max compression
+gzip compressed data, was "l2mac-0.0.2.tar", last modified: Thu Apr 25 23:41:10 2024, max compression
```

## Comparing `l2mac-0.0.1.tar` & `l2mac-0.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-23 15:47:27.606848 l2mac-0.0.1/
--rw-r--r--   0 samholt    (501) staff       (20)     1068 2024-04-13 10:40:13.000000 l2mac-0.0.1/LICENSE
--rw-r--r--   0 samholt    (501) staff       (20)     8176 2024-04-23 15:47:27.606541 l2mac-0.0.1/PKG-INFO
--rw-r--r--   0 samholt    (501) staff       (20)     7403 2024-04-23 15:25:45.000000 l2mac-0.0.1/README.md
-drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-23 15:47:27.581858 l2mac-0.0.1/l2mac/
--rw-r--r--   0 samholt    (501) staff       (20)      147 2024-04-22 20:27:55.000000 l2mac-0.0.1/l2mac/__init__.py
--rw-r--r--   0 samholt    (501) staff       (20)     3479 2024-04-23 15:26:38.000000 l2mac-0.0.1/l2mac/config.py
--rw-r--r--   0 samholt    (501) staff       (20)     7932 2024-04-22 14:48:59.000000 l2mac-0.0.1/l2mac/core.py
-drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-23 15:47:27.595109 l2mac-0.0.1/l2mac/envs/
--rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-17 17:57:57.000000 l2mac-0.0.1/l2mac/envs/__init__.py
--rw-r--r--   0 samholt    (501) staff       (20)     1496 2024-04-17 16:20:06.000000 l2mac-0.0.1/l2mac/envs/general.py
--rw-r--r--   0 samholt    (501) staff       (20)    20006 2024-04-22 15:59:18.000000 l2mac-0.0.1/l2mac/l2mac.py
-drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-23 15:47:27.597576 l2mac-0.0.1/l2mac/llm_providers/
--rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-17 17:58:06.000000 l2mac-0.0.1/l2mac/llm_providers/__init__.py
--rw-r--r--   0 samholt    (501) staff       (20)    11124 2024-04-22 01:19:46.000000 l2mac-0.0.1/l2mac/llm_providers/general.py
--rw-r--r--   0 samholt    (501) staff       (20)    16111 2024-04-22 00:56:53.000000 l2mac-0.0.1/l2mac/llm_providers/openai.py
--rw-r--r--   0 samholt    (501) staff       (20)     2025 2024-04-17 16:20:06.000000 l2mac-0.0.1/l2mac/llm_providers/rate_limiter.py
--rw-r--r--   0 samholt    (501) staff       (20)     4154 2024-04-17 16:20:06.000000 l2mac-0.0.1/l2mac/llm_providers/utils.py
-drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-23 15:47:27.599761 l2mac-0.0.1/l2mac/prompts/
--rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-17 17:56:57.000000 l2mac-0.0.1/l2mac/prompts/__init__.py
--rw-r--r--   0 samholt    (501) staff       (20)     6036 2024-04-20 18:23:06.000000 l2mac-0.0.1/l2mac/prompts/book.yaml
--rw-r--r--   0 samholt    (501) staff       (20)     8102 2024-04-21 01:02:40.000000 l2mac-0.0.1/l2mac/prompts/codebase.yaml
--rw-r--r--   0 samholt    (501) staff       (20)     5847 2024-04-20 18:04:03.000000 l2mac-0.0.1/l2mac/prompts/custom.yaml
--rw-r--r--   0 samholt    (501) staff       (20)     1943 2024-04-20 17:58:21.000000 l2mac-0.0.1/l2mac/prompts/load_prompts.py
-drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-23 15:47:27.602889 l2mac-0.0.1/l2mac/tools/
--rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-16 14:06:46.000000 l2mac-0.0.1/l2mac/tools/__init__.py
--rw-r--r--   0 samholt    (501) staff       (20)    10324 2024-04-21 00:10:54.000000 l2mac-0.0.1/l2mac/tools/code_analysis.py
--rw-r--r--   0 samholt    (501) staff       (20)     2372 2024-04-17 16:20:06.000000 l2mac-0.0.1/l2mac/tools/control_unit.py
--rw-r--r--   0 samholt    (501) staff       (20)    11654 2024-04-17 16:20:06.000000 l2mac-0.0.1/l2mac/tools/core.py
--rw-r--r--   0 samholt    (501) staff       (20)     9851 2024-04-17 16:22:23.000000 l2mac-0.0.1/l2mac/tools/read.py
--rw-r--r--   0 samholt    (501) staff       (20)     1621 2024-04-17 16:20:06.000000 l2mac-0.0.1/l2mac/tools/utils.py
--rw-r--r--   0 samholt    (501) staff       (20)    12541 2024-04-20 15:08:47.000000 l2mac-0.0.1/l2mac/tools/write.py
-drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-23 15:47:27.604776 l2mac-0.0.1/l2mac/utils/
--rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-17 17:58:25.000000 l2mac-0.0.1/l2mac/utils/__init__.py
--rw-r--r--   0 samholt    (501) staff       (20)    86112 2024-04-17 16:20:06.000000 l2mac-0.0.1/l2mac/utils/l2mac.py
--rw-r--r--   0 samholt    (501) staff       (20)      978 2024-04-17 16:20:06.000000 l2mac-0.0.1/l2mac/utils/logging.py
--rw-r--r--   0 samholt    (501) staff       (20)     3033 2024-04-22 15:59:18.000000 l2mac-0.0.1/l2mac/utils/run.py
-drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-23 15:47:27.594072 l2mac-0.0.1/l2mac.egg-info/
--rw-r--r--   0 samholt    (501) staff       (20)     8176 2024-04-23 15:47:27.000000 l2mac-0.0.1/l2mac.egg-info/PKG-INFO
--rw-r--r--   0 samholt    (501) staff       (20)      898 2024-04-23 15:47:27.000000 l2mac-0.0.1/l2mac.egg-info/SOURCES.txt
--rw-r--r--   0 samholt    (501) staff       (20)        1 2024-04-23 15:47:27.000000 l2mac-0.0.1/l2mac.egg-info/dependency_links.txt
--rw-r--r--   0 samholt    (501) staff       (20)       41 2024-04-23 15:47:27.000000 l2mac-0.0.1/l2mac.egg-info/entry_points.txt
--rw-r--r--   0 samholt    (501) staff       (20)      136 2024-04-23 15:47:27.000000 l2mac-0.0.1/l2mac.egg-info/requires.txt
--rw-r--r--   0 samholt    (501) staff       (20)        6 2024-04-23 15:47:27.000000 l2mac-0.0.1/l2mac.egg-info/top_level.txt
--rw-r--r--   0 samholt    (501) staff       (20)       38 2024-04-23 15:47:27.606913 l2mac-0.0.1/setup.cfg
--rw-r--r--   0 samholt    (501) staff       (20)     1141 2024-04-23 15:38:40.000000 l2mac-0.0.1/setup.py
-drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-23 15:47:27.605671 l2mac-0.0.1/tests/
--rw-r--r--   0 samholt    (501) staff       (20)       34 2024-04-22 17:28:34.000000 l2mac-0.0.1/tests/test_l2mac.py
--rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-13 09:51:20.000000 l2mac-0.0.1/tests/test_l2mac_tools.py
+drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-25 23:41:10.670099 l2mac-0.0.2/
+-rw-r--r--   0 samholt    (501) staff       (20)     1068 2024-04-13 10:40:13.000000 l2mac-0.0.2/LICENSE
+-rw-r--r--   0 samholt    (501) staff       (20)    19554 2024-04-25 23:41:10.669667 l2mac-0.0.2/PKG-INFO
+-rw-r--r--   0 samholt    (501) staff       (20)    18751 2024-04-23 21:56:12.000000 l2mac-0.0.2/README.md
+drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-25 23:41:10.643115 l2mac-0.0.2/l2mac/
+-rw-r--r--   0 samholt    (501) staff       (20)      147 2024-04-22 20:27:55.000000 l2mac-0.0.2/l2mac/__init__.py
+-rw-r--r--   0 samholt    (501) staff       (20)     3479 2024-04-23 15:26:38.000000 l2mac-0.0.2/l2mac/config.py
+-rw-r--r--   0 samholt    (501) staff       (20)     7932 2024-04-22 14:48:59.000000 l2mac-0.0.2/l2mac/core.py
+drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-25 23:41:10.650564 l2mac-0.0.2/l2mac/envs/
+-rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-17 17:57:57.000000 l2mac-0.0.2/l2mac/envs/__init__.py
+-rw-r--r--   0 samholt    (501) staff       (20)     1496 2024-04-17 16:20:06.000000 l2mac-0.0.2/l2mac/envs/general.py
+-rw-r--r--   0 samholt    (501) staff       (20)    20006 2024-04-22 15:59:18.000000 l2mac-0.0.2/l2mac/l2mac.py
+drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-25 23:41:10.652925 l2mac-0.0.2/l2mac/llm_providers/
+-rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-17 17:58:06.000000 l2mac-0.0.2/l2mac/llm_providers/__init__.py
+-rw-r--r--   0 samholt    (501) staff       (20)    11299 2024-04-25 23:40:52.000000 l2mac-0.0.2/l2mac/llm_providers/general.py
+-rw-r--r--   0 samholt    (501) staff       (20)    16111 2024-04-22 00:56:53.000000 l2mac-0.0.2/l2mac/llm_providers/openai.py
+-rw-r--r--   0 samholt    (501) staff       (20)     2025 2024-04-17 16:20:06.000000 l2mac-0.0.2/l2mac/llm_providers/rate_limiter.py
+-rw-r--r--   0 samholt    (501) staff       (20)     4154 2024-04-17 16:20:06.000000 l2mac-0.0.2/l2mac/llm_providers/utils.py
+drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-25 23:41:10.662091 l2mac-0.0.2/l2mac/prompts/
+-rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-17 17:56:57.000000 l2mac-0.0.2/l2mac/prompts/__init__.py
+-rw-r--r--   0 samholt    (501) staff       (20)     6036 2024-04-20 18:23:06.000000 l2mac-0.0.2/l2mac/prompts/book.yaml
+-rw-r--r--   0 samholt    (501) staff       (20)     8102 2024-04-21 01:02:40.000000 l2mac-0.0.2/l2mac/prompts/codebase.yaml
+-rw-r--r--   0 samholt    (501) staff       (20)     5847 2024-04-20 18:04:03.000000 l2mac-0.0.2/l2mac/prompts/custom.yaml
+-rw-r--r--   0 samholt    (501) staff       (20)     1943 2024-04-20 17:58:21.000000 l2mac-0.0.2/l2mac/prompts/load_prompts.py
+drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-25 23:41:10.665721 l2mac-0.0.2/l2mac/tools/
+-rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-16 14:06:46.000000 l2mac-0.0.2/l2mac/tools/__init__.py
+-rw-r--r--   0 samholt    (501) staff       (20)    10324 2024-04-21 00:10:54.000000 l2mac-0.0.2/l2mac/tools/code_analysis.py
+-rw-r--r--   0 samholt    (501) staff       (20)     2372 2024-04-17 16:20:06.000000 l2mac-0.0.2/l2mac/tools/control_unit.py
+-rw-r--r--   0 samholt    (501) staff       (20)    11654 2024-04-17 16:20:06.000000 l2mac-0.0.2/l2mac/tools/core.py
+-rw-r--r--   0 samholt    (501) staff       (20)     9851 2024-04-17 16:22:23.000000 l2mac-0.0.2/l2mac/tools/read.py
+-rw-r--r--   0 samholt    (501) staff       (20)     1621 2024-04-17 16:20:06.000000 l2mac-0.0.2/l2mac/tools/utils.py
+-rw-r--r--   0 samholt    (501) staff       (20)    12541 2024-04-20 15:08:47.000000 l2mac-0.0.2/l2mac/tools/write.py
+drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-25 23:41:10.667654 l2mac-0.0.2/l2mac/utils/
+-rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-17 17:58:25.000000 l2mac-0.0.2/l2mac/utils/__init__.py
+-rw-r--r--   0 samholt    (501) staff       (20)    86112 2024-04-17 16:20:06.000000 l2mac-0.0.2/l2mac/utils/l2mac.py
+-rw-r--r--   0 samholt    (501) staff       (20)      978 2024-04-17 16:20:06.000000 l2mac-0.0.2/l2mac/utils/logging.py
+-rw-r--r--   0 samholt    (501) staff       (20)     3033 2024-04-22 15:59:18.000000 l2mac-0.0.2/l2mac/utils/run.py
+drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-25 23:41:10.649470 l2mac-0.0.2/l2mac.egg-info/
+-rw-r--r--   0 samholt    (501) staff       (20)    19554 2024-04-25 23:41:10.000000 l2mac-0.0.2/l2mac.egg-info/PKG-INFO
+-rw-r--r--   0 samholt    (501) staff       (20)      898 2024-04-25 23:41:10.000000 l2mac-0.0.2/l2mac.egg-info/SOURCES.txt
+-rw-r--r--   0 samholt    (501) staff       (20)        1 2024-04-25 23:41:10.000000 l2mac-0.0.2/l2mac.egg-info/dependency_links.txt
+-rw-r--r--   0 samholt    (501) staff       (20)       41 2024-04-25 23:41:10.000000 l2mac-0.0.2/l2mac.egg-info/entry_points.txt
+-rw-r--r--   0 samholt    (501) staff       (20)      150 2024-04-25 23:41:10.000000 l2mac-0.0.2/l2mac.egg-info/requires.txt
+-rw-r--r--   0 samholt    (501) staff       (20)        6 2024-04-25 23:41:10.000000 l2mac-0.0.2/l2mac.egg-info/top_level.txt
+-rw-r--r--   0 samholt    (501) staff       (20)       38 2024-04-25 23:41:10.670233 l2mac-0.0.2/setup.cfg
+-rw-r--r--   0 samholt    (501) staff       (20)     1141 2024-04-25 23:40:11.000000 l2mac-0.0.2/setup.py
+drwxr-xr-x   0 samholt    (501) staff       (20)        0 2024-04-25 23:41:10.668691 l2mac-0.0.2/tests/
+-rw-r--r--   0 samholt    (501) staff       (20)       63 2024-04-23 16:10:02.000000 l2mac-0.0.2/tests/test_l2mac.py
+-rw-r--r--   0 samholt    (501) staff       (20)        0 2024-04-13 09:51:20.000000 l2mac-0.0.2/tests/test_l2mac_tools.py
```

### Comparing `l2mac-0.0.1/LICENSE` & `l2mac-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/config.py` & `l2mac-0.0.2/l2mac/config.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/core.py` & `l2mac-0.0.2/l2mac/core.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/envs/general.py` & `l2mac-0.0.2/l2mac/envs/general.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/l2mac.py` & `l2mac-0.0.2/l2mac/l2mac.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/llm_providers/general.py` & `l2mac-0.0.2/l2mac/llm_providers/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         "temperature": config.llm_settings.temperature,
         "top_p": config.llm_settings.top_p,
         "frequency_penalty": config.llm_settings.frequency_penalty,
         "presence_penalty": config.llm_settings.presence_penalty,
         "stop": config.llm_settings.stop,
         "stream": config.llm_settings.api_stream,
         "api_key": config.llm.api_key,
+        "base_url": config.llm.base_url,
         "_open_ai_rate_limit_requests_per_minute": config.llm_settings.rate_limit_requests_per_minute,
         "_logger": logger,
         "_name": name,
         "_rate_limiter": rate_limiter,
         "_retry_with_exponential_backoff__initial_delay": config.llm_settings.api_retry_with_exponential_backoff__initial_delay,
         "_retry_with_exponential_backoff__exponential_base": config.llm_settings.api_retry_with_exponential_backoff__exponential_base,
         "_retry_with_exponential_backoff__jitter": config.llm_settings.api_retry_with_exponential_backoff__jitter,
@@ -176,30 +177,32 @@
 
 
 async def async_chat_completion_rl_inner(**kwargs):
     kwargs.get("_logger", None)
     kwargs.get("_name", None)
     rate_limiter = kwargs.get("_rate_limiter", None)
     api_type = kwargs.get("api_type", ApiType.openai)
+    base_url = kwargs.get("base_url")
     if api_type == ApiType.openai:
-        aclient = AsyncOpenAI(api_key=kwargs["api_key"])
+        aclient = AsyncOpenAI(api_key=kwargs["api_key"], base_url=kwargs["base_url"])
     elif api_type == ApiType.azure:
         aclient = AsyncAzureOpenAI(
             api_key=kwargs["api_key"], api_version=kwargs["api_version"], azure_endpoint=kwargs["azure_endpoint"]
         )
     keys_to_remove = {
         "_open_ai_rate_limit_requests_per_minute",
         "_logger",
         "_name",
         "api_key",
         "api_version",
         "azure_endpoint",
         "_rate_limiter",
         "stream",
         "api_type",
+        "base_url"
     }
     kwargs = {k: v for k, v in kwargs.items() if k not in keys_to_remove}
     perf_counter()
     # if logger:
     #     logger.info(f"[{name}][OpenAI API Request] {kwargs}")
     # pretty_print_chat_messages(kwargs['messages'])
 
@@ -238,29 +241,30 @@
 
 def chat_completion_rl_inner(**kwargs):
     kwargs.get("_logger", None)
     kwargs.get("_name", None)
     rate_limiter = kwargs.get("_rate_limiter", None)
     api_type = kwargs.get("api_type", ApiType.openai)
     if api_type == ApiType.openai:
-        client = OpenAI(api_key=kwargs["api_key"])
+        client = OpenAI(api_key=kwargs["api_key"], base_url=kwargs["base_url"])
     elif api_type == ApiType.azure:
         client = AzureOpenAI(
             api_key=kwargs["api_key"], api_version=kwargs["api_version"], azure_endpoint=kwargs["azure_endpoint"]
         )
     keys_to_remove = {
         "_open_ai_rate_limit_requests_per_minute",
         "_logger",
         "_name",
         "api_key",
         "api_version",
         "azure_endpoint",
         "_rate_limiter",
         "stream",
         "api_type",
+        "base_url"
     }
     kwargs = {k: v for k, v in kwargs.items() if k not in keys_to_remove}
     perf_counter()
     # if logger:
     #     logger.info(f"[{name}][OpenAI API Request] {kwargs}")
     # pretty_print_chat_messages(kwargs['messages'])
     if rate_limiter:
```

### Comparing `l2mac-0.0.1/l2mac/llm_providers/openai.py` & `l2mac-0.0.2/l2mac/llm_providers/openai.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/llm_providers/rate_limiter.py` & `l2mac-0.0.2/l2mac/llm_providers/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/llm_providers/utils.py` & `l2mac-0.0.2/l2mac/llm_providers/utils.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/prompts/book.yaml` & `l2mac-0.0.2/l2mac/prompts/book.yaml`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/prompts/codebase.yaml` & `l2mac-0.0.2/l2mac/prompts/codebase.yaml`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/prompts/custom.yaml` & `l2mac-0.0.2/l2mac/prompts/custom.yaml`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/prompts/load_prompts.py` & `l2mac-0.0.2/l2mac/prompts/load_prompts.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/tools/code_analysis.py` & `l2mac-0.0.2/l2mac/tools/code_analysis.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/tools/control_unit.py` & `l2mac-0.0.2/l2mac/tools/control_unit.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/tools/core.py` & `l2mac-0.0.2/l2mac/tools/core.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/tools/read.py` & `l2mac-0.0.2/l2mac/tools/read.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/tools/utils.py` & `l2mac-0.0.2/l2mac/tools/utils.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/tools/write.py` & `l2mac-0.0.2/l2mac/tools/write.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/utils/l2mac.py` & `l2mac-0.0.2/l2mac/utils/l2mac.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/utils/logging.py` & `l2mac-0.0.2/l2mac/utils/logging.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac/utils/run.py` & `l2mac-0.0.2/l2mac/utils/run.py`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/l2mac.egg-info/SOURCES.txt` & `l2mac-0.0.2/l2mac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `l2mac-0.0.1/setup.py` & `l2mac-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 extras_require = {}
 extras_require = {"dev": ["pylint~=3.0.3", "black~=23.3.0", "isort~=5.12.0", "pre-commit~=3.6.0"]}
 
 setup(
     name="l2mac",
-    version="0.0.1",
+    version="0.0.2",
     description="The LLM Automatic Computer Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/samholt/l2mac",
     author="Sam Holt",
     author_email="samuel.holt.direct@gmail.com",
     license="MIT",
```

