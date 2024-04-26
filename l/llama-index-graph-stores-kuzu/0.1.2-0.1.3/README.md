# Comparing `tmp/llama_index_graph_stores_kuzu-0.1.2.tar.gz` & `tmp/llama_index_graph_stores_kuzu-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_graph_stores_kuzu-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_graph_stores_kuzu-0.1.3.tar", max compression
```

## Comparing `llama_index_graph_stores_kuzu-0.1.2.tar` & `llama_index_graph_stores_kuzu-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       44 2024-02-13 13:53:01.640140 llama_index_graph_stores_kuzu-0.1.2/README.md
--rw-r--r--   0        0        0       92 2024-02-13 13:53:01.640337 llama_index_graph_stores_kuzu-0.1.2/llama_index/graph_stores/kuzu/__init__.py
--rw-r--r--   0        0        0     8711 2024-02-13 13:53:01.640423 llama_index_graph_stores_kuzu-0.1.2/llama_index/graph_stores/kuzu/base.py
--rw-r--r--   0        0        0     1463 2024-02-21 17:10:29.861202 llama_index_graph_stores_kuzu-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 llama_index_graph_stores_kuzu-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-04-26 15:45:20.627714 llama_index_graph_stores_kuzu-0.1.3/README.md
+-rw-r--r--   0        0        0       92 2024-04-26 15:45:20.627714 llama_index_graph_stores_kuzu-0.1.3/llama_index/graph_stores/kuzu/__init__.py
+-rw-r--r--   0        0        0     8690 2024-04-26 15:45:20.627714 llama_index_graph_stores_kuzu-0.1.3/llama_index/graph_stores/kuzu/base.py
+-rw-r--r--   0        0        0     1463 2024-04-26 15:45:20.627714 llama_index_graph_stores_kuzu-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 llama_index_graph_stores_kuzu-0.1.3/PKG-INFO
```

### Comparing `llama_index_graph_stores_kuzu-0.1.2/llama_index/graph_stores/kuzu/base.py` & `llama_index_graph_stores_kuzu-0.1.3/llama_index/graph_stores/kuzu/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Kùzu graph store index."""
+
 from typing import Any, Dict, List, Optional
 
 from llama_index.core.graph_stores.types import GraphStore
 
 import kuzu
 
 
@@ -47,15 +48,15 @@
             MATCH (n1:%s)-[r:%s]->(n2:%s)
             WHERE n1.ID = $subj
             RETURN r.predicate, n2.ID;
         """
         prepared_statement = self.connection.prepare(
             query % (self.node_table_name, self.rel_table_name, self.node_table_name)
         )
-        query_result = self.connection.execute(prepared_statement, [("subj", subj)])
+        query_result = self.connection.execute(prepared_statement, {"subj": subj})
         retval = []
         while query_result.has_next():
             row = query_result.get_next()
             retval.append([row[0], row[1]])
         return retval
 
     def get_rel_map(
@@ -78,15 +79,15 @@
                     where_clause += " OR n1.ID = $%d" % i
                 params.append((str(i), curr_subj))
         else:
             where_clause = ""
         query = f"{match_clause} {where_clause} {return_clause}"
         prepared_statement = self.connection.prepare(query)
         if subjs is not None:
-            query_result = self.connection.execute(prepared_statement, params)
+            query_result = self.connection.execute(prepared_statement, dict(params))
         else:
             query_result = self.connection.execute(prepared_statement)
         retval: Dict[str, List[List[str]]] = {}
         while query_result.has_next():
             row = query_result.get_next()
             curr_path = []
             subj = row[0]
@@ -111,45 +112,45 @@
 
     def upsert_triplet(self, subj: str, rel: str, obj: str) -> None:
         """Add triplet."""
 
         def check_entity_exists(connection: Any, entity: str) -> bool:
             is_exists_result = connection.execute(
                 "MATCH (n:%s) WHERE n.ID = $entity RETURN n.ID" % self.node_table_name,
-                [("entity", entity)],
+                {"entity": entity},
             )
             return is_exists_result.has_next()
 
         def create_entity(connection: Any, entity: str) -> None:
             connection.execute(
                 "CREATE (n:%s {ID: $entity})" % self.node_table_name,
-                [("entity", entity)],
+                {"entity": entity},
             )
 
         def check_rel_exists(connection: Any, subj: str, obj: str, rel: str) -> bool:
             is_exists_result = connection.execute(
                 (
                     "MATCH (n1:{})-[r:{}]->(n2:{}) WHERE n1.ID = $subj AND n2.ID = "
                     "$obj AND r.predicate = $pred RETURN r.predicate"
                 ).format(
                     self.node_table_name, self.rel_table_name, self.node_table_name
                 ),
-                [("subj", subj), ("obj", obj), ("pred", rel)],
+                {"subj": subj, "obj": obj, "pred": rel},
             )
             return is_exists_result.has_next()
 
         def create_rel(connection: Any, subj: str, obj: str, rel: str) -> None:
             connection.execute(
                 (
                     "MATCH (n1:{}), (n2:{}) WHERE n1.ID = $subj AND n2.ID = $obj "
                     "CREATE (n1)-[r:{} {{predicate: $pred}}]->(n2)"
                 ).format(
                     self.node_table_name, self.node_table_name, self.rel_table_name
                 ),
-                [("subj", subj), ("obj", obj), ("pred", rel)],
+                {"subj": subj, "obj": obj, "pred": rel},
             )
 
         is_subj_exists = check_entity_exists(self.connection, subj)
         is_obj_exists = check_entity_exists(self.connection, obj)
 
         if not is_subj_exists:
             create_entity(self.connection, subj)
@@ -170,29 +171,29 @@
             connection.execute(
                 (
                     "MATCH (n1:{})-[r:{}]->(n2:{}) WHERE n1.ID = $subj AND n2.ID"
                     " = $obj AND r.predicate = $pred DELETE r"
                 ).format(
                     self.node_table_name, self.rel_table_name, self.node_table_name
                 ),
-                [("subj", subj), ("obj", obj), ("pred", rel)],
+                {"subj": subj, "obj": obj, "pred": rel},
             )
 
         def delete_entity(connection: Any, entity: str) -> None:
             connection.execute(
                 "MATCH (n:%s) WHERE n.ID = $entity DELETE n" % self.node_table_name,
-                [("entity", entity)],
+                {"entity": entity},
             )
 
         def check_edges(connection: Any, entity: str) -> bool:
             is_exists_result = connection.execute(
                 "MATCH (n1:{})-[r:{}]-(n2:{}) WHERE n2.ID = $entity RETURN r.predicate".format(
                     self.node_table_name, self.rel_table_name, self.node_table_name
                 ),
-                [("entity", entity)],
+                {"entity": entity},
             )
             return is_exists_result.has_next()
 
         delete_rel(self.connection, subj, obj, rel)
         if not check_edges(self.connection, subj):
             delete_entity(self.connection, subj)
         if not check_edges(self.connection, obj):
```

### Comparing `llama_index_graph_stores_kuzu-0.1.2/pyproject.toml` & `llama_index_graph_stores_kuzu-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index graph stores kuzu integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-graph-stores-kuzu"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 kuzu = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_graph_stores_kuzu-0.1.2/PKG-INFO` & `llama_index_graph_stores_kuzu-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-graph-stores-kuzu
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index graph stores kuzu integration
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
 Requires-Dist: kuzu (>=0.1.0,<0.2.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Graph Stores Integration: Kuzu
```

