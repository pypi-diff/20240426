# Comparing `tmp/closurizer-0.5.1.tar.gz` & `tmp/closurizer-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "closurizer-0.5.1.tar", max compression
+gzip compressed data, was "closurizer-0.6.0.tar", max compression
```

## Comparing `closurizer-0.5.1.tar` & `closurizer-0.6.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1827 2024-02-16 01:43:54.818404 closurizer-0.5.1/closurizer/cli.py
--rw-r--r--   0        0        0     6777 2024-02-16 01:43:54.818404 closurizer-0.5.1/closurizer/closurizer.py
--rw-r--r--   0        0        0      464 2024-02-16 01:43:54.818404 closurizer-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 closurizer-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1827 2024-04-26 01:28:26.715390 closurizer-0.6.0/closurizer/cli.py
+-rw-r--r--   0        0        0     6902 2024-04-26 01:28:26.715390 closurizer-0.6.0/closurizer/closurizer.py
+-rw-r--r--   0        0        0      521 2024-04-26 01:28:26.715390 closurizer-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 closurizer-0.6.0/PKG-INFO
```

### Comparing `closurizer-0.5.1/closurizer/cli.py` & `closurizer-0.6.0/closurizer/cli.py`

 * *Files identical despite different names*

### Comparing `closurizer-0.5.1/closurizer/closurizer.py` & `closurizer-0.6.0/closurizer/closurizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,24 +53,26 @@
            and {field}_edges.predicate = 'biolink:{field}'
       left outer join closure_id as {field}_closure
         on {field}_edges.object = {field}_closure.id
       left outer join closure_label as {field}_closure_label
         on {field}_edges.object = {field}_closure_label.id
     """
 
+
 def grouping_key(grouping_fields):
     fragments = []
     for field in grouping_fields:
         if field == 'negated':
-            fragments.append(f"coalesce({field}.replace('True','NOT'), '')")
+            fragments.append(f"coalesce(cast({field} as varchar).replace('true','NOT'), '')")
         else:
             fragments.append(field)
     grouping_key_fragments = ", ".join(fragments)
     return f"concat_ws('|', {grouping_key_fragments}) as grouping_key"
 
+
 def add_closure(kg_archive: str,
                 closure_file: str,
                 nodes_output_file: str,
                 edges_output_file: str,
                 node_fields: List[str] = None,
                 edge_fields: List[str] = ['subject', 'object'],
                 additional_node_constraints: str = None,
@@ -141,21 +143,22 @@
            {grouping_key(grouping_fields)}  
     from edges
         {"".join([edge_joins(field) for field in edge_fields])}
     """
 
     print(edges_query)
 
+    additional_node_constraints = f"where {additional_node_constraints}" if additional_node_constraints else ""
     nodes_query = f"""        
     create or replace table denormalized_nodes as
     select nodes.*, 
         {"".join([node_columns(node_field) for node_field in node_fields])}
     from nodes
         {node_joins('has_phenotype')}
-    where {additional_node_constraints}
+    {additional_node_constraints}
     group by nodes.*
     """
     print(nodes_query)
 
     if not dry_run:
         db.query(edges_query)
         db.query(f"""
```

### Comparing `closurizer-0.5.1/PKG-INFO` & `closurizer-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: closurizer
-Version: 0.5.1
+Version: 0.6.0
 Summary: Add closure expansion fields to kgx files following the Golr pattern
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: SQLAlchemy (>=1.4.37,<2.0.0)
 Requires-Dist: click (>=8,<9)
-Requires-Dist: duckdb (>=0.9.1,<0.10.0)
+Requires-Dist: duckdb (>=0.10.2,<0.11.0)
```

