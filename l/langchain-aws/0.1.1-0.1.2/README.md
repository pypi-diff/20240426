# Comparing `tmp/langchain_aws-0.1.1.tar.gz` & `tmp/langchain_aws-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_aws-0.1.1.tar", max compression
+gzip compressed data, was "langchain_aws-0.1.2.tar", max compression
```

## Comparing `langchain_aws-0.1.1.tar` & `langchain_aws-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1072 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/LICENSE
--rw-r--r--   0        0        0     1534 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/README.md
--rw-r--r--   0        0        0      611 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/__init__.py
--rw-r--r--   0        0        0      113 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/chat_models/__init__.py
--rw-r--r--   0        0        0    13294 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/chat_models/bedrock.py
--rw-r--r--   0        0        0       96 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/embeddings/__init__.py
--rw-r--r--   0        0        0     7282 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/embeddings/bedrock.py
--rw-r--r--   0        0        0      191 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/graphs/__init__.py
--rw-r--r--   0        0        0    14347 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/graphs/neptune_graph.py
--rw-r--r--   0        0        0    10331 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/graphs/neptune_rdf_graph.py
--rw-r--r--   0        0        0      297 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/llms/__init__.py
--rw-r--r--   0        0        0    31691 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/llms/bedrock.py
--rw-r--r--   0        0        0    13595 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0        0 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/py.typed
--rw-r--r--   0        0        0      251 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/retrievers/__init__.py
--rw-r--r--   0        0        0     4654 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/retrievers/bedrock.py
--rw-r--r--   0        0        0    15189 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/retrievers/kendra.py
--rw-r--r--   0        0        0     1033 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/langchain_aws/utils.py
--rw-r--r--   0        0        0     2728 2024-04-24 19:16:06.999034 langchain_aws-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2376 1970-01-01 00:00:00.000000 langchain_aws-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1534 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/README.md
+-rw-r--r--   0        0        0      611 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/__init__.py
+-rw-r--r--   0        0        0      113 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/chat_models/__init__.py
+-rw-r--r--   0        0        0    13294 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/chat_models/bedrock.py
+-rw-r--r--   0        0        0       96 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/embeddings/__init__.py
+-rw-r--r--   0        0        0     7282 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/embeddings/bedrock.py
+-rw-r--r--   0        0        0      191 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/graphs/__init__.py
+-rw-r--r--   0        0        0    14347 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/graphs/neptune_graph.py
+-rw-r--r--   0        0        0    10331 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/graphs/neptune_rdf_graph.py
+-rw-r--r--   0        0        0      297 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/llms/__init__.py
+-rw-r--r--   0        0        0    31691 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/llms/bedrock.py
+-rw-r--r--   0        0        0    13595 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0        0 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/py.typed
+-rw-r--r--   0        0        0      251 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/retrievers/__init__.py
+-rw-r--r--   0        0        0     4654 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/retrievers/bedrock.py
+-rw-r--r--   0        0        0    15189 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/retrievers/kendra.py
+-rw-r--r--   0        0        0     1033 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/utils.py
+-rw-r--r--   0        0        0     2737 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2377 1970-01-01 00:00:00.000000 langchain_aws-0.1.2/PKG-INFO
```

### Comparing `langchain_aws-0.1.1/LICENSE` & `langchain_aws-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/README.md` & `langchain_aws-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/langchain_aws/__init__.py` & `langchain_aws-0.1.2/langchain_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/langchain_aws/chat_models/bedrock.py` & `langchain_aws-0.1.2/langchain_aws/chat_models/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/langchain_aws/embeddings/bedrock.py` & `langchain_aws-0.1.2/langchain_aws/embeddings/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/langchain_aws/graphs/neptune_graph.py` & `langchain_aws-0.1.2/langchain_aws/graphs/neptune_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/langchain_aws/graphs/neptune_rdf_graph.py` & `langchain_aws-0.1.2/langchain_aws/graphs/neptune_rdf_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/langchain_aws/llms/bedrock.py` & `langchain_aws-0.1.2/langchain_aws/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/langchain_aws/llms/sagemaker_endpoint.py` & `langchain_aws-0.1.2/langchain_aws/llms/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/langchain_aws/retrievers/bedrock.py` & `langchain_aws-0.1.2/langchain_aws/retrievers/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/langchain_aws/retrievers/kendra.py` & `langchain_aws-0.1.2/langchain_aws/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/langchain_aws/utils.py` & `langchain_aws-0.1.2/langchain_aws/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.1/pyproject.toml` & `langchain_aws-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-aws"
-version = "0.1.1"
+version = "0.1.2"
 description = "An integration package connecting AWS and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-aws"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-aws/tree/main/libs/aws"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain-core = "^0.1.45"
-boto3 = "^1.34.72"
+boto3 = ">=1.34.51,<1.35.0"
 numpy = "^1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.3"
```

### Comparing `langchain_aws-0.1.1/PKG-INFO` & `langchain_aws-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-aws
-Version: 0.1.1
+Version: 0.1.2
 Summary: An integration package connecting AWS and LangChain
 Home-page: https://github.com/langchain-ai/langchain-aws
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: boto3 (>=1.34.72,<2.0.0)
+Requires-Dist: boto3 (>=1.34.51,<1.35.0)
 Requires-Dist: langchain-core (>=0.1.45,<0.2.0)
 Requires-Dist: numpy (>=1,<2)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-aws
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-aws/tree/main/libs/aws
 Description-Content-Type: text/markdown
 
 # langchain-aws
```

