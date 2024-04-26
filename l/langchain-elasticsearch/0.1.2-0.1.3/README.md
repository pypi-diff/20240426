# Comparing `tmp/langchain_elasticsearch-0.1.2.tar.gz` & `tmp/langchain_elasticsearch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_elasticsearch-0.1.2.tar", max compression
+gzip compressed data, was "langchain_elasticsearch-0.1.3.tar", max compression
```

## Comparing `langchain_elasticsearch-0.1.2.tar` & `langchain_elasticsearch-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/LICENSE
--rw-r--r--   0        0        0     3272 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/README.md
--rw-r--r--   0        0        0      618 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/__init__.py
--rw-r--r--   0        0        0     4075 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/_utilities.py
--rw-r--r--   0        0        0     5417 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/chat_history.py
--rw-r--r--   0        0        0     1094 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/client.py
--rw-r--r--   0        0        0     7862 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/py.typed
--rw-r--r--   0        0        0     4764 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/retrievers.py
--rw-r--r--   0        0        0    49912 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/vectorstores.py
--rw-r--r--   0        0        0     2315 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 langchain_elasticsearch-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-26 09:50:55.686820 langchain_elasticsearch-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5805 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/README.md
+-rw-r--r--   0        0        0      705 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4075 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/_utilities.py
+-rw-r--r--   0        0        0     7748 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/cache.py
+-rw-r--r--   0        0        0     5417 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/chat_history.py
+-rw-r--r--   0        0        0     1094 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/client.py
+-rw-r--r--   0        0        0     7862 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/py.typed
+-rw-r--r--   0        0        0     4764 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/retrievers.py
+-rw-r--r--   0        0        0    49930 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/vectorstores.py
+-rw-r--r--   0        0        0     2618 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6691 1970-01-01 00:00:00.000000 langchain_elasticsearch-0.1.3/PKG-INFO
```

### Comparing `langchain_elasticsearch-0.1.2/LICENSE` & `langchain_elasticsearch-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.2/langchain_elasticsearch/__init__.py` & `langchain_elasticsearch-0.1.3/langchain_elasticsearch/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from langchain_elasticsearch.cache import ElasticsearchCache
 from langchain_elasticsearch.chat_history import ElasticsearchChatMessageHistory
 from langchain_elasticsearch.embeddings import ElasticsearchEmbeddings
 from langchain_elasticsearch.retrievers import ElasticsearchRetriever
 from langchain_elasticsearch.vectorstores import (
     ApproxRetrievalStrategy,
     ElasticsearchStore,
     ExactRetrievalStrategy,
     SparseRetrievalStrategy,
 )
 
 __all__ = [
     "ApproxRetrievalStrategy",
+    "ElasticsearchCache",
     "ElasticsearchChatMessageHistory",
     "ElasticsearchEmbeddings",
     "ElasticsearchRetriever",
     "ElasticsearchStore",
     "ExactRetrievalStrategy",
     "SparseRetrievalStrategy",
 ]
```

### Comparing `langchain_elasticsearch-0.1.2/langchain_elasticsearch/_utilities.py` & `langchain_elasticsearch-0.1.3/langchain_elasticsearch/_utilities.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.2/langchain_elasticsearch/chat_history.py` & `langchain_elasticsearch-0.1.3/langchain_elasticsearch/chat_history.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.2/langchain_elasticsearch/client.py` & `langchain_elasticsearch-0.1.3/langchain_elasticsearch/client.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.2/langchain_elasticsearch/embeddings.py` & `langchain_elasticsearch-0.1.3/langchain_elasticsearch/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.2/langchain_elasticsearch/retrievers.py` & `langchain_elasticsearch-0.1.3/langchain_elasticsearch/retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.2/langchain_elasticsearch/vectorstores.py` & `langchain_elasticsearch-0.1.3/langchain_elasticsearch/vectorstores.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,16 +147,16 @@
             "filter": filter,
             "field": vector_query_field,
             "k": k,
             "num_candidates": fetch_k,
         }
 
         # Embedding provided via the embedding function
-        if query_vector and not self.query_model_id:
-            knn["query_vector"] = query_vector
+        if query_vector is not None and not self.query_model_id:
+            knn["query_vector"] = list(query_vector)
 
         # Case 2: Used when model has been deployed to
         # Elasticsearch and can infer the query vector from the query text
         elif query and self.query_model_id:
             knn["query_vector_builder"] = {
                 "text_embedding": {
                     "model_id": self.query_model_id,  # use 'model_id' argument
@@ -885,28 +885,28 @@
             source=True,
             source_includes=fields,
         )
 
         def default_doc_builder(hit: Dict) -> Document:
             return Document(
                 page_content=hit["_source"].get(self.query_field, ""),
-                metadata=hit["_source"]["metadata"],
+                metadata=hit["_source"].get("metadata", {}),
             )
 
         doc_builder = doc_builder or default_doc_builder
 
         docs_and_scores = []
         for hit in response["hits"]["hits"]:
             for field in fields:
+                if "metadata" not in hit["_source"]:
+                    hit["_source"]["metadata"] = {}
                 if field in hit["_source"] and field not in [
                     "metadata",
                     self.query_field,
                 ]:
-                    if "metadata" not in hit["_source"]:
-                        hit["_source"]["metadata"] = {}
                     hit["_source"]["metadata"][field] = hit["_source"][field]
 
             docs_and_scores.append(
                 (
                     doc_builder(hit),
                     hit["_score"],
                 )
```

### Comparing `langchain_elasticsearch-0.1.2/pyproject.toml` & `langchain_elasticsearch-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-elasticsearch"
-version = "0.1.2"
+version = "0.1.3"
 description = "An integration package connecting Elasticsearch and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-elastic"
 license = "MIT"
 
 [tool.poetry.urls]
@@ -24,14 +24,15 @@
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain = "^0.1.13"
 langchain-text-splitters = ">=0.0.1,<0.1"
+langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -39,19 +40,21 @@
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
+langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
+langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
```

### Comparing `langchain_elasticsearch-0.1.2/PKG-INFO` & `langchain_elasticsearch-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: langchain-elasticsearch
-Version: 0.1.2
-Summary: An integration package connecting Elasticsearch and LangChain
-Home-page: https://github.com/langchain-ai/langchain-elastic
-License: MIT
-Requires-Python: >=3.8.1,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: elasticsearch (>=8.12.0,<9.0.0)
-Requires-Dist: langchain-core (>=0.1,<0.2)
-Requires-Dist: numpy (>=1,<2)
-Project-URL: Repository, https://github.com/langchain-ai/langchain-elastic
-Project-URL: Source Code, https://github.com/langchain-ai/langchain-elastic/tree/main/libs/elasticsearch
-Description-Content-Type: text/markdown
-
 # langchain-elasticsearch
 
 This package contains the LangChain integration with Elasticsearch.
 
 ## Installation
 
 ```bash
@@ -127,7 +107,89 @@
     index="your-index-name",
     session_id="your-session-id",
     es_cloud_id="your-cloud-id",
     es_api_key="your-api-key",
 )
 ```
 
+
+### ElasticsearchCache
+
+A caching layer for LLMs that uses Elasticsearch.
+
+Simple example:
+
+```python
+from elasticsearch import Elasticsearch
+from langchain.globals import set_llm_cache
+
+from langchain_elasticsearch import ElasticsearchCache
+
+es_client = Elasticsearch(hosts="http://localhost:9200")
+set_llm_cache(
+    ElasticsearchCache(
+        es_connection=es_client,
+        index_name="llm-chat-cache",
+        metadata={"project": "my_chatgpt_project"},
+    )
+)
+```
+
+The `index_name` parameter can also accept aliases. This allows to use the 
+[ILM: Manage the index lifecycle](https://www.elastic.co/guide/en/elasticsearch/reference/current/index-lifecycle-management.html)
+that we suggest to consider for managing retention and controlling cache growth.
+
+Look at the class docstring for all parameters.
+
+#### Index the generated text
+
+The cached data won't be searchable by default.
+The developer can customize the building of the Elasticsearch document in order to add indexed text fields,
+where to put, for example, the text generated by the LLM.
+
+This can be done by subclassing end overriding methods.
+The new cache class can be applied also to a pre-existing cache index:
+
+```python
+import json
+from typing import Any, Dict, List
+
+from elasticsearch import Elasticsearch
+from langchain.globals import set_llm_cache
+from langchain_core.caches import RETURN_VAL_TYPE
+
+from langchain_elasticsearch import ElasticsearchCache
+
+
+class SearchableElasticsearchCache(ElasticsearchCache):
+    @property
+    def mapping(self) -> Dict[str, Any]:
+        mapping = super().mapping
+        mapping["mappings"]["properties"]["parsed_llm_output"] = {
+            "type": "text",
+            "analyzer": "english",
+        }
+        return mapping
+
+    def build_document(
+        self, prompt: str, llm_string: str, return_val: RETURN_VAL_TYPE
+    ) -> Dict[str, Any]:
+        body = super().build_document(prompt, llm_string, return_val)
+        body["parsed_llm_output"] = self._parse_output(body["llm_output"])
+        return body
+
+    @staticmethod
+    def _parse_output(data: List[str]) -> List[str]:
+        return [
+            json.loads(output)["kwargs"]["message"]["kwargs"]["content"]
+            for output in data
+        ]
+
+
+es_client = Elasticsearch(hosts="http://localhost:9200")
+set_llm_cache(
+    SearchableElasticsearchCache(es_connection=es_client, index_name="llm-chat-cache")
+)
+```
+
+When overriding the mapping and the document building, 
+please only make additive modifications, keeping the base mapping intact.
```

