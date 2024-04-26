# Comparing `tmp/arcee_py-1.0.4.tar.gz` & `tmp/arcee_py-1.0.6.tar.gz`

## Comparing `arcee_py-1.0.4.tar` & `arcee_py-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.0.4/.python-version
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.0.4/tasks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.0.4/.github/CODEOWNERS
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.0.4/.github/iced/test.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/__init__.py
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/api.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/api_handler.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/cli.py
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/cli_handler.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/config.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/dalm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/schemas/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/schemas/doc.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 arcee_py-1.0.4/arcee/schemas/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.4/tests/conftest.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.0.4/tests/test_api_handler.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.0.4/.gitignore
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 arcee_py-1.0.4/README.md
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 arcee_py-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 arcee_py-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.0.6/.python-version
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.0.6/tasks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.0.6/.github/CODEOWNERS
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.0.6/.github/iced/test.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.0.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/__init__.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/api.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/api_handler.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/cli.py
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/cli_handler.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/config.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/dalm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/schemas/__init__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/schemas/doc.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/schemas/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.6/tests/conftest.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.0.6/tests/test_api_handler.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.0.6/.gitignore
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 arcee_py-1.0.6/README.md
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 arcee_py-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 arcee_py-1.0.6/PKG-INFO
```

### Comparing `arcee_py-1.0.4/tasks.py` & `arcee_py-1.0.6/tasks.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/.github/iced/test.yml` & `arcee_py-1.0.6/.github/iced/test.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/.github/workflows/publish.yml` & `arcee_py-1.0.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/arcee/__init__.py` & `arcee_py-1.0.6/arcee/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.4"
+__version__ = "1.0.6"
 
 import os
 
 from arcee import config
 from arcee.api import upload_docs, upload_corpus_folder, upload_qa_pairs, start_alignment, start_pretraining, start_retriever_training, get_retriever_status, start_deployment, stop_deployment, generate, retrieve, delete_corpus, upload_alignment
 from arcee.dalm import DALM, DALMFilter
```

### Comparing `arcee_py-1.0.4/arcee/api.py` & `arcee_py-1.0.6/arcee/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,16 +135,16 @@
     data = {"deployment_name": deployment_name}
     return make_request("post", Route.deployment+"/stopDeployment", data)
 
 def generate(deployment_name: str, query: str):
     data = {"deployment_name": deployment_name, "query": query}
     return make_request("post", Route.deployment+"/generate", data)
 
-def retrieve(deployment_name: str, query: str):
-    data = {"deployment_name": deployment_name, "query": query}
+def retrieve(deployment_name: str, query: str, size: Optional[int] = 5):
+    data = {"deployment_name": deployment_name, "query": query, "size": size}
     return make_request("post", Route.deployment+"/retrieve", data)
 
 def embed(deployment_name: str, query: str):
     data = {"deployment_name": deployment_name, "query": query}
     return make_request("post", Route.deployment+"/embed", data)
 
 def get_current_org() -> str:
```

### Comparing `arcee_py-1.0.4/arcee/api_handler.py` & `arcee_py-1.0.6/arcee/api_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/arcee/cli.py` & `arcee_py-1.0.6/arcee/cli.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/arcee/cli_handler.py` & `arcee_py-1.0.6/arcee/cli_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/arcee/config.py` & `arcee_py-1.0.6/arcee/config.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/arcee/dalm.py` & `arcee_py-1.0.6/arcee/dalm.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/tests/test_api_handler.py` & `arcee_py-1.0.6/tests/test_api_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/.gitignore` & `arcee_py-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/README.md` & `arcee_py-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/pyproject.toml` & `arcee_py-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.4/PKG-INFO` & `arcee_py-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcee-py
-Version: 1.0.4
+Version: 1.0.6
 Project-URL: Home, https://arcee.ai
 Author-email: Jacob Solowetz <jacob@arcee.ai>, Ben Epstein <ben@arcee.ai>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: pydantic<3.0,>=2.4.2
 Requires-Dist: requests
 Requires-Dist: rich
```

