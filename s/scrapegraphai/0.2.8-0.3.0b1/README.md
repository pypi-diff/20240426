# Comparing `tmp/scrapegraphai-0.2.8.tar.gz` & `tmp/scrapegraphai-0.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.2.8.tar", max compression
+gzip compressed data, was "scrapegraphai-0.3.0b1.tar", max compression
```

## Comparing `scrapegraphai-0.2.8.tar` & `scrapegraphai-0.3.0b1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.2.8/LICENSE
--rw-r--r--   0        0        0     7907 2024-04-25 10:10:10.131040 scrapegraphai-0.2.8/README.md
--rw-r--r--   0        0        0     1644 2024-04-25 10:12:24.944918 scrapegraphai-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.2.8/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.2.8/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.2.8/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      258 2024-04-20 20:58:42.218942 scrapegraphai-0.2.8/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     3623 2024-04-25 10:10:10.154362 scrapegraphai-0.2.8/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     4628 2024-04-25 10:11:59.645944 scrapegraphai-0.2.8/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2494 2024-04-25 10:10:10.154636 scrapegraphai-0.2.8/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2191 2024-04-12 10:59:59.484979 scrapegraphai-0.2.8/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2380 2024-04-20 20:58:42.219513 scrapegraphai-0.2.8/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3120 2024-04-20 20:58:42.219606 scrapegraphai-0.2.8/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      202 2024-04-25 10:11:59.646772 scrapegraphai-0.2.8/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      829 2024-04-25 10:10:10.154906 scrapegraphai-0.2.8/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-09 11:20:43.626222 scrapegraphai-0.2.8/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-04-25 10:11:59.647049 scrapegraphai-0.2.8/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.2.8/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      290 2024-04-12 10:59:59.485515 scrapegraphai-0.2.8/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-09 11:20:43.626608 scrapegraphai-0.2.8/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.2.8/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      839 2024-04-12 10:59:59.485625 scrapegraphai-0.2.8/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.2.8/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.2.8/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.2.8/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.2.8/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      539 2024-04-25 10:11:59.647387 scrapegraphai-0.2.8/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.2.8/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-20 20:58:42.219990 scrapegraphai-0.2.8/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3375 2024-04-25 10:10:10.155199 scrapegraphai-0.2.8/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6893 2024-04-24 08:02:38.694607 scrapegraphai-0.2.8/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7236 2024-04-25 10:10:10.155594 scrapegraphai-0.2.8/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-20 20:58:42.221320 scrapegraphai-0.2.8/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-20 20:58:42.221535 scrapegraphai-0.2.8/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-20 20:58:42.221690 scrapegraphai-0.2.8/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5165 2024-04-25 10:11:59.648032 scrapegraphai-0.2.8/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6444 2024-04-25 10:11:59.648364 scrapegraphai-0.2.8/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4507 2024-04-25 10:10:10.156452 scrapegraphai-0.2.8/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     1635 2024-04-22 19:30:38.104934 scrapegraphai-0.2.8/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      242 2024-04-12 10:55:27.494820 scrapegraphai-0.2.8/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1742 2024-04-25 10:10:10.156867 scrapegraphai-0.2.8/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1443 2024-04-25 10:10:10.157249 scrapegraphai-0.2.8/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.2.8/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0     1504 2024-04-12 11:30:08.598599 scrapegraphai-0.2.8/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     1070 2024-04-25 10:10:10.157483 scrapegraphai-0.2.8/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.2.8/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.2.8/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.2.8/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     9532 1970-01-01 00:00:00.000000 scrapegraphai-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-26 17:16:41.541549 scrapegraphai-0.3.0b1/LICENSE
+-rw-r--r--   0        0        0     7907 2024-04-26 17:16:41.541549 scrapegraphai-0.3.0b1/README.md
+-rw-r--r--   0        0        0     1646 2024-04-26 17:17:00.325693 scrapegraphai-0.3.0b1/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      258 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     3623 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     4628 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2494 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2191 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2380 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3120 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      202 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      290 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      839 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      539 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3375 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6893 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7236 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-26 17:16:41.569549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5165 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6444 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4507 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     1635 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      242 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1443 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0     1504 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     1070 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-04-26 17:16:41.573549 scrapegraphai-0.3.0b1/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     9534 1970-01-01 00:00:00.000000 scrapegraphai-0.3.0b1/PKG-INFO
```

### Comparing `scrapegraphai-0.2.8/LICENSE` & `scrapegraphai-0.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/README.md` & `scrapegraphai-0.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/pyproject.toml` & `scrapegraphai-0.3.0b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.2.8"
+version = "0.3.0b1"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `scrapegraphai-0.2.8/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.3.0b1/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.3.0b1/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.3.0b1/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.3.0b1/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.3.0b1/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.3.0b1/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.3.0b1/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.3.0b1/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.3.0b1/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.3.0b1/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.3.0b1/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/models/gemini.py` & `scrapegraphai-0.3.0b1/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.3.0b1/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/models/ollama.py` & `scrapegraphai-0.3.0b1/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/models/openai.py` & `scrapegraphai-0.3.0b1/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.3.0b1/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.3.0b1/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.3.0b1/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.3.0b1/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.3.0b1/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.3.0b1/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.3.0b1/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/utils/remover.py` & `scrapegraphai-0.3.0b1/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.3.0b1/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.3.0b1/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.3.0b1/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.2.8/PKG-INFO` & `scrapegraphai-0.3.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.2.8
+Version: 0.3.0b1
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >3.9,<4.0
```

