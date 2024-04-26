# Comparing `tmp/llama_index_vector_stores_lantern-0.1.2.tar.gz` & `tmp/llama_index_vector_stores_lantern-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_lantern-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_lantern-0.1.3.tar", max compression
```

## Comparing `llama_index_vector_stores_lantern-0.1.2.tar` & `llama_index_vector_stores_lantern-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       48 2024-02-13 13:53:02.007952 llama_index_vector_stores_lantern-0.1.2/README.md
--rw-r--r--   0        0        0      104 2024-02-13 13:53:02.008146 llama_index_vector_stores_lantern-0.1.2/llama_index/vector_stores/lantern/__init__.py
--rw-r--r--   0        0        0    21333 2024-02-13 13:53:02.008219 llama_index_vector_stores_lantern-0.1.2/llama_index/vector_stores/lantern/base.py
--rw-r--r--   0        0        0     1590 2024-02-21 23:29:00.142996 llama_index_vector_stores_lantern-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 llama_index_vector_stores_lantern-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-04-26 15:45:09.584683 llama_index_vector_stores_lantern-0.1.3/README.md
+-rw-r--r--   0        0        0      104 2024-04-26 15:45:09.584683 llama_index_vector_stores_lantern-0.1.3/llama_index/vector_stores/lantern/__init__.py
+-rw-r--r--   0        0        0    22257 2024-04-26 15:45:09.584683 llama_index_vector_stores_lantern-0.1.3/llama_index/vector_stores/lantern/base.py
+-rw-r--r--   0        0        0     1590 2024-04-26 15:45:09.584683 llama_index_vector_stores_lantern-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 llama_index_vector_stores_lantern-0.1.3/PKG-INFO
```

### Comparing `llama_index_vector_stores_lantern-0.1.2/llama_index/vector_stores/lantern/base.py` & `llama_index_vector_stores_lantern-0.1.3/llama_index/vector_stores/lantern/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,27 +108,57 @@
             (AbstractData,),
             {"__tablename__": tablename, "__table_args__": {"schema": schema_name}},
         )
 
     Index(
         hnsw_indexname,
         model.embedding,  # type: ignore
-        postgresql_using="hnsw",
+        postgresql_using="lantern_hnsw",
         postgresql_with={
             "m": m,
             "ef_construction": ef_construction,
             "ef": ef,
             "dim": embed_dim,
         },
         postgresql_ops={"embedding": "dist_cos_ops"},
     )
     return model
 
 
 class LanternVectorStore(BasePydanticVectorStore):
+    """Latern vector store.
+
+    Examples:
+        `pip install llama-index-vector-stores-lantern`
+
+        ```python
+        from llama_index.vector_stores.lantern import LanternVectorStore
+
+        # Set up connection details
+        connection_string = "postgresql://postgres:postgres@localhost:5432"
+        db_name = "postgres"
+        url = make_url(connection_string)
+
+        # Create an instance of LanternVectorStore
+        vector_store = LanternVectorStore.from_params(
+            database=db_name,
+            host=url.host,
+            password=url.password,
+            port=url.port,
+            user=url.username,
+            table_name="your_table_name",
+            embed_dim=1536,  # openai embedding dimension
+            m=16,  # HNSW M parameter
+            ef_construction=128,  # HNSW ef construction parameter
+            ef=64,  # HNSW ef search parameter
+        )
+        ```
+
+    """
+
     from sqlalchemy.sql.selectable import Select
 
     stores_text = True
     flat_metadata = False
 
     connection_string: str
     async_connection_string: str
```

### Comparing `llama_index_vector_stores_lantern-0.1.2/pyproject.toml` & `llama_index_vector_stores_lantern-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores lantern integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-lantern"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 psycopg2-binary = "^2.9.9"
 asyncpg = "^0.29.0"
```

### Comparing `llama_index_vector_stores_lantern-0.1.2/PKG-INFO` & `llama_index_vector_stores_lantern-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-lantern
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index vector_stores lantern integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Requires-Dist: sqlalchemy[asyncio] (>=2.0.25,<3.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Vector_Stores Integration: Lantern
```

