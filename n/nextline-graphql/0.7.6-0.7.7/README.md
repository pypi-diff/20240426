# Comparing `tmp/nextline_graphql-0.7.6.tar.gz` & `tmp/nextline_graphql-0.7.7.tar.gz`

## Comparing `nextline_graphql-0.7.6.tar` & `nextline_graphql-0.7.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/__about__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/py.typed
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/config/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/config/default.toml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/custom/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/custom/strawberry.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/hook/__init__.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/hook/spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/__init__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/__init__.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/test.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/example_script/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/example_script/script.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/example_script/script2.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/example_script/script_asyncio.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/example_script/script_scratch.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/example_script/script_threading.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/mutations/Exec.gql
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/mutations/Reset.gql
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/mutations/RunAndContinue.gql
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/mutations/SendPdbCommand.gql
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/queries/Exception.gql
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/queries/Source.gql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/queries/SourceLine.gql
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/queries/State.gql
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Counter.gql
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Prompting.gql
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/subscriptions/State.gql
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Stdout.gql
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/subscriptions/TraceIds.gql
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/schema/__init__.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/schema/mutation.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/schema/query.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/schema/subscription.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/dev/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/dev/plugin.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/dev/schema/__init__.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/dev/schema/query.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/graphql/__init__.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/graphql/plugin.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/graphql/graphql/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/graphql/graphql/queries/Settings.gql
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/graphql/schema/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/graphql/schema/query.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/graphql/test/__init__.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/nextlinegraphql/plugins/graphql/test/funcs.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/LICENSE
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/README.md
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 nextline_graphql-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/__about__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/__init__.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/py.typed
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/config/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/config/default.toml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/custom/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/custom/strawberry.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/hook/__init__.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/hook/spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/__init__.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/__init__.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/test.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/script.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/script2.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/script_asyncio.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/script_scratch.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/script_threading.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/mutations/Exec.gql
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/mutations/Reset.gql
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/mutations/RunAndContinue.gql
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/mutations/SendPdbCommand.gql
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/queries/Exception.gql
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/queries/Source.gql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/queries/SourceLine.gql
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/queries/State.gql
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Counter.gql
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Prompting.gql
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/subscriptions/State.gql
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Stdout.gql
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/subscriptions/TraceIds.gql
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/__init__.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/mutation.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/query.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/subscription.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/dev/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/dev/plugin.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/dev/schema/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/dev/schema/query.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/__init__.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/plugin.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/graphql/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/graphql/queries/Settings.gql
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/schema/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/schema/query.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/test/__init__.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/test/funcs.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/LICENSE
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/README.md
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/PKG-INFO
```

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/factory.py` & `nextline_graphql-0.7.7/nextlinegraphql/factory.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/config/__init__.py` & `nextline_graphql-0.7.7/nextlinegraphql/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/config/default.toml` & `nextline_graphql-0.7.7/nextlinegraphql/config/default.toml`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/custom/strawberry.py` & `nextline_graphql-0.7.7/nextlinegraphql/custom/strawberry.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/hook/__init__.py` & `nextline_graphql-0.7.7/nextlinegraphql/hook/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/hook/spec.py` & `nextline_graphql-0.7.7/nextlinegraphql/hook/spec.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/__init__.py` & `nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/test.py` & `nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/test.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/graphql/__init__.py` & `nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/schema/mutation.py` & `nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/mutation.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/schema/query.py` & `nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/query.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/plugins/ctrl/schema/subscription.py` & `nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/subscription.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/plugins/graphql/plugin.py` & `nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/nextlinegraphql/plugins/graphql/test/funcs.py` & `nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/test/funcs.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/.gitignore` & `nextline_graphql-0.7.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/LICENSE` & `nextline_graphql-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/README.md` & `nextline_graphql-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.6/pyproject.toml` & `nextline_graphql-0.7.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "nextline>=0.7.3",
+    "nextline>=0.7.4",
     "apluggy>=0.9.9",
     "dynaconf>=3.2",
     "starlette>=0.31",
     "strawberry-graphql>=0.213",
     "websockets>=12.0",
     "rich>=13.6",
 ]
```

### Comparing `nextline_graphql-0.7.6/PKG-INFO` & `nextline_graphql-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.3
 Name: nextline-graphql
-Version: 0.7.6
+Version: 0.7.7
 Summary: A GraphQL API for Nextline
 Project-URL: Homepage, https://github.com/simonsobs/nextline
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: apluggy>=0.9.9
 Requires-Dist: dynaconf>=3.2
-Requires-Dist: nextline>=0.7.3
+Requires-Dist: nextline>=0.7.4
 Requires-Dist: rich>=13.6
 Requires-Dist: starlette>=0.31
 Requires-Dist: strawberry-graphql>=0.213
 Requires-Dist: websockets>=12.0
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
```

