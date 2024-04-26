# Comparing `tmp/openlit-0.0.3.tar.gz` & `tmp/openlit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlit-0.0.3.tar", max compression
+gzip compressed data, was "openlit-1.0.0.tar", max compression
```

## Comparing `openlit-0.0.3.tar` & `openlit-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2024-04-19 15:03:28.223177 openlit-0.0.3/LICENSE
--rw-r--r--   0        0        0     9238 2024-04-19 15:03:28.223177 openlit-0.0.3/README.md
--rw-r--r--   0        0        0      927 2024-04-19 15:03:28.223177 openlit-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4651 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/__helpers.py
--rw-r--r--   0        0        0     8795 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/__init__.py
--rw-r--r--   0        0        0     1955 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0    15993 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/anthropic/anthropic.py
--rw-r--r--   0        0        0    16035 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/anthropic/async_anthropic.py
--rw-r--r--   0        0        0     3253 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0    10374 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/chroma/chroma.py
--rw-r--r--   0        0        0     1920 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0    20348 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/cohere/cohere.py
--rw-r--r--   0        0        0     2531 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     7609 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/langchain/langchain.py
--rw-r--r--   0        0        0     3156 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/mistral/__init__.py
--rw-r--r--   0        0        0    21328 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/mistral/async_mistral.py
--rw-r--r--   0        0        0    21179 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/mistral/mistral.py
--rw-r--r--   0        0        0    16265 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0    46297 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/openai/async_azure_openai.py
--rw-r--r--   0        0        0    45841 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/openai/async_openai.py
--rw-r--r--   0        0        0    46091 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/openai/azure_openai.py
--rw-r--r--   0        0        0    46522 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/openai/openai.py
--rw-r--r--   0        0        0     2526 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     8732 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/pinecone/pinecone.py
--rw-r--r--   0        0        0     1478 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/transformers/__init__.py
--rw-r--r--   0        0        0     7592 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/instrumentation/transformers/transformers.py
--rw-r--r--   0        0        0     4293 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/otel/metrics.py
--rw-r--r--   0        0        0     3612 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/otel/tracing.py
--rw-r--r--   0        0        0     5686 2024-04-19 15:03:28.227177 openlit-0.0.3/src/openlit/semcov/__init__.py
--rw-r--r--   0        0        0    10457 1970-01-01 00:00:00.000000 openlit-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-26 04:48:14.563522 openlit-1.0.0/LICENSE
+-rw-r--r--   0        0        0     9235 2024-04-26 04:48:14.563522 openlit-1.0.0/README.md
+-rw-r--r--   0        0        0      927 2024-04-26 04:48:14.563522 openlit-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4651 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/__helpers.py
+-rw-r--r--   0        0        0     8795 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/__init__.py
+-rw-r--r--   0        0        0     1955 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0    15993 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/anthropic/anthropic.py
+-rw-r--r--   0        0        0    16035 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/anthropic/async_anthropic.py
+-rw-r--r--   0        0        0     3253 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0    10374 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/chroma/chroma.py
+-rw-r--r--   0        0        0     1920 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0    20348 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/cohere/cohere.py
+-rw-r--r--   0        0        0     2531 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     7609 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/langchain/langchain.py
+-rw-r--r--   0        0        0     3156 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/mistral/__init__.py
+-rw-r--r--   0        0        0    21328 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/mistral/async_mistral.py
+-rw-r--r--   0        0        0    21179 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/mistral/mistral.py
+-rw-r--r--   0        0        0    16265 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0    46297 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/openai/async_azure_openai.py
+-rw-r--r--   0        0        0    45841 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/openai/async_openai.py
+-rw-r--r--   0        0        0    46091 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/openai/azure_openai.py
+-rw-r--r--   0        0        0    46522 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/openai/openai.py
+-rw-r--r--   0        0        0     2526 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     8732 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/pinecone/pinecone.py
+-rw-r--r--   0        0        0     1478 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/transformers/__init__.py
+-rw-r--r--   0        0        0     7592 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/instrumentation/transformers/transformers.py
+-rw-r--r--   0        0        0     4293 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/otel/metrics.py
+-rw-r--r--   0        0        0     3612 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/otel/tracing.py
+-rw-r--r--   0        0        0     5686 2024-04-26 04:48:14.563522 openlit-1.0.0/src/openlit/semcov/__init__.py
+-rw-r--r--   0        0        0    10454 1970-01-01 00:00:00.000000 openlit-1.0.0/PKG-INFO
```

### Comparing `openlit-0.0.3/LICENSE` & `openlit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/README.md` & `openlit-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <img src="https://github.com/openlit/.github/blob/main/profile/assets/wide-logo-no-bg.png?raw=true" alt="OpenLIT Logo" width="30%"><h1>
 OpenTelemetry Auto-Instrumentation for GenAI & LLM Applications</h1>
 
 **[Documentation](https://docs.openlit.io/) | [Quickstart](#-getting-started) | [Python SDK](https://github.com/openlit/openlit/tree/main/sdk/python)**
 
 [![OpenLIT](https://img.shields.io/badge/OpenLIT-orange)](https://github.com/openlit/openlit)
 [![License](https://img.shields.io/github/license/openlit/openlit?label=License&logo=github&color=f80&logoColor=white)](https://github.com/openlit/openlit/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/badge/dokumetry/month)](https://pepy.tech/project/dokumetry)
+[![Downloads](https://static.pepy.tech/badge/openlit/month)](https://pepy.tech/project/openlit)
 [![GitHub Last Commit](https://img.shields.io/github/last-commit/openlit/openlit)](https://github.com/openlit/openlit/pulse)
 [![GitHub Contributors](https://img.shields.io/github/contributors/openlit/openlit)](https://github.com/openlit/openlit/graphs/contributors)
 
 [![Slack](https://img.shields.io/badge/Slack-4A154B?logo=slack&logoColor=white)](https://join.slack.com/t/openlit/shared_invite/zt-2etnfttwg-TjP_7BZXfYg84oAukY8QRQ)
 [![X](https://img.shields.io/badge/follow-%40OpenLIT-1DA1F2?logo=x&style=social)](https://twitter.com/openlit_io)
 
 </div>
@@ -144,8 +144,8 @@
 ## 💚 Community & Support
 
 Connect with the OpenLIT community and maintainers for support, discussions, and updates:
 
 - 🌟 If you like it, Leave a star on our [GitHub](https://github.com/openlit/openlit/)
 - 🌍 Join our [Slack](https://join.slack.com/t/openlit/shared_invite/zt-2etnfttwg-TjP_7BZXfYg84oAukY8QRQ) Community for live interactions and questions.
 - 🐞 Report bugs on our [GitHub Issues](https://github.com/openlit/openlit/issues) to help us improve OpenLIT.
-- 𝕏 Follow us on [X](https://twitter.com/openlit) for the latest updates and news.
+- 𝕏 Follow us on [X](https://twitter.com/openlit) for the latest updates and news.
```

### Comparing `openlit-0.0.3/pyproject.toml` & `openlit-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openlit"
-version = "0.0.3"
+version = "1.0.0"
 description = "OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects"
 authors = ["OpenLIT"]
 repository = "https://github.com/openlit/openlit/tree/main/openlit/python"
 readme = "README.md"
 homepage = "https://github.com/openlit/openlit/tree/main/openlit/python"
 keywords = ["OpenTelemetry", "otel", "otlp","llm", "tracing", "openai", "anthropic", "claude", "cohere", "llm monitoring", "observability", "monitoring", "gpt", "Generative AI", "chatGPT"]
```

### Comparing `openlit-0.0.3/src/openlit/__helpers.py` & `openlit-1.0.0/src/openlit/__helpers.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/__init__.py` & `openlit-1.0.0/src/openlit/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/anthropic/__init__.py` & `openlit-1.0.0/src/openlit/instrumentation/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/anthropic/anthropic.py` & `openlit-1.0.0/src/openlit/instrumentation/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/anthropic/async_anthropic.py` & `openlit-1.0.0/src/openlit/instrumentation/anthropic/async_anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/chroma/__init__.py` & `openlit-1.0.0/src/openlit/instrumentation/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/chroma/chroma.py` & `openlit-1.0.0/src/openlit/instrumentation/chroma/chroma.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/cohere/__init__.py` & `openlit-1.0.0/src/openlit/instrumentation/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/cohere/cohere.py` & `openlit-1.0.0/src/openlit/instrumentation/cohere/cohere.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/langchain/__init__.py` & `openlit-1.0.0/src/openlit/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/langchain/langchain.py` & `openlit-1.0.0/src/openlit/instrumentation/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/mistral/__init__.py` & `openlit-1.0.0/src/openlit/instrumentation/mistral/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/mistral/async_mistral.py` & `openlit-1.0.0/src/openlit/instrumentation/mistral/async_mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/mistral/mistral.py` & `openlit-1.0.0/src/openlit/instrumentation/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/openai/__init__.py` & `openlit-1.0.0/src/openlit/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/openai/async_azure_openai.py` & `openlit-1.0.0/src/openlit/instrumentation/openai/async_azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/openai/async_openai.py` & `openlit-1.0.0/src/openlit/instrumentation/openai/async_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/openai/azure_openai.py` & `openlit-1.0.0/src/openlit/instrumentation/openai/azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/openai/openai.py` & `openlit-1.0.0/src/openlit/instrumentation/openai/openai.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/pinecone/__init__.py` & `openlit-1.0.0/src/openlit/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/pinecone/pinecone.py` & `openlit-1.0.0/src/openlit/instrumentation/pinecone/pinecone.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/transformers/__init__.py` & `openlit-1.0.0/src/openlit/instrumentation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/instrumentation/transformers/transformers.py` & `openlit-1.0.0/src/openlit/instrumentation/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/otel/metrics.py` & `openlit-1.0.0/src/openlit/otel/metrics.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/otel/tracing.py` & `openlit-1.0.0/src/openlit/otel/tracing.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/src/openlit/semcov/__init__.py` & `openlit-1.0.0/src/openlit/semcov/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-0.0.3/PKG-INFO` & `openlit-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlit
-Version: 0.0.3
+Version: 1.0.0
 Summary: OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects
 Home-page: https://github.com/openlit/openlit/tree/main/openlit/python
 Keywords: OpenTelemetry,otel,otlp,llm,tracing,openai,anthropic,claude,cohere,llm monitoring,observability,monitoring,gpt,Generative AI,chatGPT
 Author: OpenLIT
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -25,15 +25,15 @@
 <img src="https://github.com/openlit/.github/blob/main/profile/assets/wide-logo-no-bg.png?raw=true" alt="OpenLIT Logo" width="30%"><h1>
 OpenTelemetry Auto-Instrumentation for GenAI & LLM Applications</h1>
 
 **[Documentation](https://docs.openlit.io/) | [Quickstart](#-getting-started) | [Python SDK](https://github.com/openlit/openlit/tree/main/sdk/python)**
 
 [![OpenLIT](https://img.shields.io/badge/OpenLIT-orange)](https://github.com/openlit/openlit)
 [![License](https://img.shields.io/github/license/openlit/openlit?label=License&logo=github&color=f80&logoColor=white)](https://github.com/openlit/openlit/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/badge/dokumetry/month)](https://pepy.tech/project/dokumetry)
+[![Downloads](https://static.pepy.tech/badge/openlit/month)](https://pepy.tech/project/openlit)
 [![GitHub Last Commit](https://img.shields.io/github/last-commit/openlit/openlit)](https://github.com/openlit/openlit/pulse)
 [![GitHub Contributors](https://img.shields.io/github/contributors/openlit/openlit)](https://github.com/openlit/openlit/graphs/contributors)
 
 [![Slack](https://img.shields.io/badge/Slack-4A154B?logo=slack&logoColor=white)](https://join.slack.com/t/openlit/shared_invite/zt-2etnfttwg-TjP_7BZXfYg84oAukY8QRQ)
 [![X](https://img.shields.io/badge/follow-%40OpenLIT-1DA1F2?logo=x&style=social)](https://twitter.com/openlit_io)
 
 </div>
@@ -168,7 +168,8 @@
 
 Connect with the OpenLIT community and maintainers for support, discussions, and updates:
 
 - 🌟 If you like it, Leave a star on our [GitHub](https://github.com/openlit/openlit/)
 - 🌍 Join our [Slack](https://join.slack.com/t/openlit/shared_invite/zt-2etnfttwg-TjP_7BZXfYg84oAukY8QRQ) Community for live interactions and questions.
 - 🐞 Report bugs on our [GitHub Issues](https://github.com/openlit/openlit/issues) to help us improve OpenLIT.
 - 𝕏 Follow us on [X](https://twitter.com/openlit) for the latest updates and news.
+
```

