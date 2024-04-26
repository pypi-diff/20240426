# Comparing `tmp/scrapegraphaisub-0.0.12b2.tar.gz` & `tmp/scrapegraphaisub-0.0.12b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphaisub-0.0.12b2.tar", max compression
+gzip compressed data, was "scrapegraphaisub-0.0.12b3.tar", max compression
```

## Comparing `scrapegraphaisub-0.0.12b2.tar` & `scrapegraphaisub-0.0.12b3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1065 2024-04-21 12:50:35.483405 scrapegraphaisub-0.0.12b2/LICENSE
--rw-r--r--   0        0        0     5439 2024-04-21 12:50:35.483405 scrapegraphaisub-0.0.12b2/README.md
--rw-r--r--   0        0        0     1622 2024-04-21 12:50:53.895467 scrapegraphaisub-0.0.12b2/pyproject.toml
--rw-r--r--   0        0        0       57 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/__init__.py
--rw-r--r--   0        0        0       90 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/builders/__init__.py
--rw-r--r--   0        0        0     6673 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/builders/graph_builder.py
--rw-r--r--   0        0        0       95 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/evaluators/__init__.py
--rw-r--r--   0        0        0     2837 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/evaluators/trulens_evaluator.py
--rw-r--r--   0        0        0      167 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/graphs/__init__.py
--rw-r--r--   0        0        0     3041 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/graphs/base_graph.py
--rw-r--r--   0        0        0     4587 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     5141 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/graphs/speech_graph.py
--rw-r--r--   0        0        0      164 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/helpers/__init__.py
--rw-r--r--   0        0        0      406 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/helpers/models_tokens.py
--rw-r--r--   0        0        0     3459 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/helpers/nodes_metadata.py
--rw-r--r--   0        0        0     2372 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/helpers/schemas.py
--rw-r--r--   0        0        0      187 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/models/__init__.py
--rw-r--r--   0        0        0      615 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/models/gemini.py
--rw-r--r--   0        0        0      575 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/models/openai_tts.py
--rw-r--r--   0        0        0      395 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/__init__.py
--rw-r--r--   0        0        0     7486 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/conditional_node.py
--rw-r--r--   0        0        0     3284 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/fetch_node.py
--rw-r--r--   0        0        0     5611 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     4023 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1243 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3269 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/parse_node.py
--rw-r--r--   0        0        0     4127 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/rag_node.py
--rw-r--r--   0        0        0     1638 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      191 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/__init__.py
--rw-r--r--   0        0        0     1271 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1268 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/convert_to_json.py
--rw-r--r--   0        0        0     3564 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/parse_state_keys.py
--rw-r--r--   0        0        0      877 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/remover.py
--rw-r--r--   0        0        0      574 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1353 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/test_node.py
--rw-r--r--   0        0        0      990 2024-04-21 12:50:35.495405 scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/token_calculator.py
--rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 scrapegraphaisub-0.0.12b2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-26 12:47:13.022388 scrapegraphaisub-0.0.12b3/LICENSE
+-rw-r--r--   0        0        0     5439 2024-04-26 12:47:13.022388 scrapegraphaisub-0.0.12b3/README.md
+-rw-r--r--   0        0        0     1622 2024-04-26 12:47:31.386376 scrapegraphaisub-0.0.12b3/pyproject.toml
+-rw-r--r--   0        0        0       57 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/builders/__init__.py
+-rw-r--r--   0        0        0     6673 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/builders/graph_builder.py
+-rw-r--r--   0        0        0       95 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/evaluators/__init__.py
+-rw-r--r--   0        0        0     2837 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/evaluators/trulens_evaluator.py
+-rw-r--r--   0        0        0      167 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/graphs/__init__.py
+-rw-r--r--   0        0        0     3041 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/graphs/base_graph.py
+-rw-r--r--   0        0        0     4587 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     5141 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/graphs/speech_graph.py
+-rw-r--r--   0        0        0      164 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/helpers/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3459 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0     2372 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/helpers/schemas.py
+-rw-r--r--   0        0        0      187 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/models/__init__.py
+-rw-r--r--   0        0        0      615 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/models/gemini.py
+-rw-r--r--   0        0        0      575 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/models/openai_tts.py
+-rw-r--r--   0        0        0      395 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/__init__.py
+-rw-r--r--   0        0        0     7486 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3284 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/fetch_node.py
+-rw-r--r--   0        0        0     5611 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     4023 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1243 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3269 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/parse_node.py
+-rw-r--r--   0        0        0     4127 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/rag_node.py
+-rw-r--r--   0        0        0     1638 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      191 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/__init__.py
+-rw-r--r--   0        0        0     1271 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1268 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3564 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      877 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/remover.py
+-rw-r--r--   0        0        0      574 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1353 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/test_node.py
+-rw-r--r--   0        0        0      990 2024-04-26 12:47:13.034388 scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/token_calculator.py
+-rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 scrapegraphaisub-0.0.12b3/PKG-INFO
```

### Comparing `scrapegraphaisub-0.0.12b2/LICENSE` & `scrapegraphaisub-0.0.12b3/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/README.md` & `scrapegraphaisub-0.0.12b3/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/pyproject.toml` & `scrapegraphaisub-0.0.12b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphaisub"
-version = "0.0.12b2"
+version = "0.0.12b3"
 description = "A first semantic versioned Scrapegraph fork by subzero team"
 authors = [
     "simone pulcini <pulcini@prova.prova>",
     "luigi corollo <corollo@prova.prova>"
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/builders/graph_builder.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/evaluators/trulens_evaluator.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/evaluators/trulens_evaluator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/graphs/base_graph.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/graphs/smart_scraper_graph.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/graphs/speech_graph.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/helpers/nodes_metadata.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/helpers/schemas.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/models/gemini.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/models/openai.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/models/openai_itt.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/models/openai_tts.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/base_node.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/conditional_node.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/fetch_node.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/generate_answer_node.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/get_probable_tags_node.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/image_to_text_node.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/parse_node.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/rag_node.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/nodes/text_to_speech_node.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/convert_to_csv.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/convert_to_json.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/parse_state_keys.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/remover.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/save_audio_from_bytes.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/test_node.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/test_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/scrapegraphaisub/utils/token_calculator.py` & `scrapegraphaisub-0.0.12b3/scrapegraphaisub/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphaisub-0.0.12b2/PKG-INFO` & `scrapegraphaisub-0.0.12b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphaisub
-Version: 0.0.12b2
+Version: 0.0.12b3
 Summary: A first semantic versioned Scrapegraph fork by subzero team
 Home-page: https://github.com/subzero-team/Scrapegraph-ai
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: simone pulcini
 Author-email: pulcini@prova.prova
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*, !=3.12.*
```

