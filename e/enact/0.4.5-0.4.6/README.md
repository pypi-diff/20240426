# Comparing `tmp/enact-0.4.5.tar.gz` & `tmp/enact-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enact-0.4.5.tar", last modified: Mon Apr  8 21:46:07 2024, max compression
+gzip compressed data, was "enact-0.4.6.tar", last modified: Fri Apr 26 20:06:48 2024, max compression
```

## Comparing `enact-0.4.5.tar` & `enact-0.4.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.072802 enact-0.4.5/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    11357 2023-08-07 17:31:37.000000 enact-0.4.5/LICENSE
--rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-04-08 21:46:07.072802 enact-0.4.5/PKG-INFO
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    14497 2023-12-06 01:14:11.000000 enact-0.4.5/README.md
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      550 2024-04-08 21:45:31.000000 enact-0.4.5/pyproject.toml
--rw-rw-r--   0 leo      (824781618) leo      (824781618)       38 2024-04-08 21:46:07.072802 enact-0.4.5/setup.cfg
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.064803 enact-0.4.5/src/
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.068802 enact-0.4.5/src/enact/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3260 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/__init__.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     8742 2024-04-08 21:41:00.000000 enact-0.4.5/src/enact/contexts.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     4062 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/digests.py
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.072802 enact-0.4.5/src/enact/fastapi/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      808 2024-04-02 22:20:36.000000 enact-0.4.5/src/enact/fastapi/__init__.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     4596 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/fastapi/fastapi.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    18263 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/function_wrappers.py
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.072802 enact-0.4.5/src/enact/gradio/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      813 2024-04-02 22:20:36.000000 enact-0.4.5/src/enact/gradio/__init__.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    26488 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/gradio/gradio.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     8972 2024-04-03 21:00:20.000000 enact-0.4.5/src/enact/interfaces.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     7394 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/invocation_generators.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    32624 2023-12-14 01:55:35.000000 enact-0.4.5/src/enact/invocations.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     6992 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/pretty_print.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)        0 2023-08-07 17:31:37.000000 enact-0.4.5/src/enact/py.typed
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    11286 2024-04-03 20:56:13.000000 enact-0.4.5/src/enact/references.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3333 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/registration.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      273 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/resource_digests.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    15763 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/resource_registry.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5024 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/resources.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5760 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/serialization.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5913 2024-02-11 18:04:33.000000 enact-0.4.5/src/enact/type_wrappers.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1440 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/utils.py
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.072802 enact-0.4.5/src/enact.egg-info/
--rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-04-08 21:46:07.000000 enact-0.4.5/src/enact.egg-info/PKG-INFO
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1087 2024-04-08 21:46:07.000000 enact-0.4.5/src/enact.egg-info/SOURCES.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)        1 2024-04-08 21:46:07.000000 enact-0.4.5/src/enact.egg-info/dependency_links.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)       19 2024-04-08 21:46:07.000000 enact-0.4.5/src/enact.egg-info/requires.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)        6 2024-04-08 21:46:07.000000 enact-0.4.5/src/enact.egg-info/top_level.txt
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.072802 enact-0.4.5/tests/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     7465 2024-04-08 21:41:00.000000 enact-0.4.5/tests/test_contexts.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1379 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_digest.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    13705 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_function_wrappers.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3994 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_invocation_generator.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    26951 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_invocations.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1534 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_pretty_print.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     6787 2024-04-03 21:00:20.000000 enact-0.4.5/tests/test_references.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3707 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_registration.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     7559 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_resource_registry.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5680 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_resources.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2271 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_serialize.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2250 2024-02-11 18:04:33.000000 enact-0.4.5/tests/test_type_wrappers.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2538 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_utils.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    11357 2023-08-07 17:31:37.000000 enact-0.4.6/LICENSE
+-rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-04-26 20:06:48.669546 enact-0.4.6/PKG-INFO
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    14497 2023-12-06 01:14:11.000000 enact-0.4.6/README.md
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      550 2024-04-26 19:56:26.000000 enact-0.4.6/pyproject.toml
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)       38 2024-04-26 20:06:48.669546 enact-0.4.6/setup.cfg
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.665546 enact-0.4.6/src/
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/src/enact/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3260 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/__init__.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     8742 2024-04-08 21:41:00.000000 enact-0.4.6/src/enact/contexts.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     4062 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/digests.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/src/enact/fastapi/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      808 2024-04-02 22:20:36.000000 enact-0.4.6/src/enact/fastapi/__init__.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     4596 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/fastapi/fastapi.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    18263 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/function_wrappers.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/src/enact/gradio/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      813 2024-04-02 22:20:36.000000 enact-0.4.6/src/enact/gradio/__init__.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    26488 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/gradio/gradio.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     8972 2024-04-03 21:00:20.000000 enact-0.4.6/src/enact/interfaces.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     7394 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/invocation_generators.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    32624 2023-12-14 01:55:35.000000 enact-0.4.6/src/enact/invocations.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     6992 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/pretty_print.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)        0 2023-08-07 17:31:37.000000 enact-0.4.6/src/enact/py.typed
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    11286 2024-04-03 20:56:13.000000 enact-0.4.6/src/enact/references.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3333 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/registration.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      273 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/resource_digests.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    15966 2024-04-26 19:56:26.000000 enact-0.4.6/src/enact/resource_registry.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5024 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/resources.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5760 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/serialization.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5913 2024-02-11 18:04:33.000000 enact-0.4.6/src/enact/type_wrappers.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1440 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/utils.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/src/enact.egg-info/
+-rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-04-26 20:06:48.000000 enact-0.4.6/src/enact.egg-info/PKG-INFO
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1087 2024-04-26 20:06:48.000000 enact-0.4.6/src/enact.egg-info/SOURCES.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)        1 2024-04-26 20:06:48.000000 enact-0.4.6/src/enact.egg-info/dependency_links.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)       19 2024-04-26 20:06:48.000000 enact-0.4.6/src/enact.egg-info/requires.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)        6 2024-04-26 20:06:48.000000 enact-0.4.6/src/enact.egg-info/top_level.txt
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/tests/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     7525 2024-04-08 21:55:50.000000 enact-0.4.6/tests/test_contexts.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1379 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_digest.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    13705 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_function_wrappers.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3994 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_invocation_generator.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    26951 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_invocations.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1534 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_pretty_print.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     6787 2024-04-03 21:00:20.000000 enact-0.4.6/tests/test_references.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3707 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_registration.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     8670 2024-04-26 19:51:23.000000 enact-0.4.6/tests/test_resource_registry.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5680 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_resources.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2271 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_serialize.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2250 2024-02-11 18:04:33.000000 enact-0.4.6/tests/test_type_wrappers.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2538 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_utils.py
```

### Comparing `enact-0.4.5/LICENSE` & `enact-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/PKG-INFO` & `enact-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enact
-Version: 0.4.5
+Version: 0.4.6
 Summary: A framework for generative software.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enact-0.4.5/README.md` & `enact-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/pyproject.toml` & `enact-0.4.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "enact"
-version = "0.4.5"
+version = "0.4.6"
 dependencies = [
   "numpy",
   "Pillow",
   "wrapt",
 ]
 description = "A framework for generative software."
 readme = "README.md"
```

### Comparing `enact-0.4.5/src/enact/__init__.py` & `enact-0.4.6/src/enact/__init__.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/contexts.py` & `enact-0.4.6/src/enact/contexts.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/digests.py` & `enact-0.4.6/src/enact/digests.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/fastapi/__init__.py` & `enact-0.4.6/src/enact/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/fastapi/fastapi.py` & `enact-0.4.6/src/enact/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/function_wrappers.py` & `enact-0.4.6/src/enact/function_wrappers.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/gradio/__init__.py` & `enact-0.4.6/src/enact/gradio/__init__.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/gradio/gradio.py` & `enact-0.4.6/src/enact/gradio/gradio.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/interfaces.py` & `enact-0.4.6/src/enact/interfaces.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/invocation_generators.py` & `enact-0.4.6/src/enact/invocation_generators.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/invocations.py` & `enact-0.4.6/src/enact/invocations.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/pretty_print.py` & `enact-0.4.6/src/enact/pretty_print.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/references.py` & `enact-0.4.6/src/enact/references.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/registration.py` & `enact-0.4.6/src/enact/registration.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/resource_registry.py` & `enact-0.4.6/src/enact/resource_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,14 +184,21 @@
     return dict
 
   @classmethod
   def set_wrapped_value(cls, target: dict, src: dict):
     target.clear()
     target.update(src)
 
+class ResourceTypeWrapper(FieldValueWrapper[type]):
+  """Wrapper for type-valued fields."""
+
+  @classmethod
+  def wrapped_type(cls) -> Type[type]:
+    return type
+
 
 FunctionWrapperT = TypeVar('FunctionWrapperT', bound='FunctionWrapper')
 MethodWrapperT = TypeVar('MethodWrapperT', bound='MethodWrapper')
 
 
 class FunctionWrapper(interfaces.ResourceBase):
   """Base class for function wrappers.
@@ -289,14 +296,15 @@
     self.register(IntWrapper)
     self.register(FloatWrapper)
     self.register(BoolWrapper)
     self.register(StrWrapper)
     self.register(BytesWrapper)
     self.register(ListWrapper)
     self.register(DictWrapper)
+    self.register(ResourceTypeWrapper)
 
   def register(self, resource: Type[interfaces.ResourceBase]):
     """Registers the resource type."""
     if not issubclass(resource, interfaces.ResourceBase):
       raise RegistryError(
         f'Cannot register non-resource type: {resource}')
     type_id = resource.type_id()
```

### Comparing `enact-0.4.5/src/enact/resources.py` & `enact-0.4.6/src/enact/resources.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/serialization.py` & `enact-0.4.6/src/enact/serialization.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/type_wrappers.py` & `enact-0.4.6/src/enact/type_wrappers.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact/utils.py` & `enact-0.4.6/src/enact/utils.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/src/enact.egg-info/PKG-INFO` & `enact-0.4.6/src/enact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enact
-Version: 0.4.5
+Version: 0.4.6
 Summary: A framework for generative software.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enact-0.4.5/src/enact.egg-info/SOURCES.txt` & `enact-0.4.6/src/enact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/tests/test_contexts.py` & `enact-0.4.6/tests/test_contexts.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     return cls.permissive_init
 
   def __init__(self):
     super().__init__()
     self.depth: Optional[int] = None
 
   def enter(self):
+    assert self.depth is None
     cur = SimpleContext.get_current()
     if cur:
       assert cur.depth is not None
       self.depth = cur.depth + 1
     else:
       self.depth = 1
 
@@ -52,14 +53,15 @@
   """An async context object for testing."""
 
   def __init__(self):
     super().__init__()
     self.depth: Optional[int] = None
 
   async def aenter(self):
+    assert self.depth is None
     cur = AsyncSimpleContext.get_current()
     if cur:
       assert cur.depth is not None
       self.depth = cur.depth + 1
     else:
       self.depth = 1
```

### Comparing `enact-0.4.5/tests/test_digest.py` & `enact-0.4.6/tests/test_digest.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/tests/test_function_wrappers.py` & `enact-0.4.6/tests/test_function_wrappers.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/tests/test_invocation_generator.py` & `enact-0.4.6/tests/test_invocation_generator.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/tests/test_invocations.py` & `enact-0.4.6/tests/test_invocations.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/tests/test_pretty_print.py` & `enact-0.4.6/tests/test_pretty_print.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/tests/test_references.py` & `enact-0.4.6/tests/test_references.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/tests/test_registration.py` & `enact-0.4.6/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/tests/test_resource_registry.py` & `enact-0.4.6/tests/test_resource_registry.py`

 * *Files 17% similar despite different names*

```diff
@@ -216,14 +216,50 @@
     self.assertEqual(unwrapped_method.__self__, instance)
     self.assertEqual(unwrapped_method.__func__, MyClass.foo_wrapper)
 
     # Check that original instance and self are aliased.
     instance.y = 420
     self.assertEqual(unwrapped_method.__self__.y, 420)
 
+  def test_wrap_type_value(self):
+    """Tests that wrapping methods works."""
+    @enact.register
+    class MyResource(enact.Resource):
+      pass
+
+    # Test for resource subclasses.
+    self.assertIsInstance(
+      enact.wrap(MyResource),
+      resource_registry.ResourceTypeWrapper)
+
+    # Test for types that have associated wrappers.
+    self.assertIsInstance(
+      enact.wrap(int),
+      resource_registry.ResourceTypeWrapper)
+
+    with enact.Store():
+      resource_type_ref = enact.commit(MyResource)
+      int_type_ref = enact.commit(int)
+
+      # Clear cache
+      resource_type_ref = enact.Ref.from_id(resource_type_ref.id)
+      int_type_ref = enact.Ref.from_id(int_type_ref.id)
+
+      # Checkout
+      self.assertEqual(resource_type_ref.checkout(), MyResource)
+      self.assertEqual(int_type_ref.checkout(), int)
+
+  def test_wrap_unregistered_type_fails(self):
+    """Tests that wrapping an unregistered type fails."""
+    class MyUnregisteredClass:
+      pass
+    with enact.Store():
+      with self.assertRaises(resource_registry.MissingWrapperError):
+        enact.wrap(MyUnregisteredClass)
+
   def test_deepcopy_primitives(self):
     """Tests that deep copying primitives works."""
     primitives = [1, 1.0, 'a', bytes([1, 2, 3]), True, False, None]
     for p in primitives:
       with self.subTest(str(p)):
         self.assertEqual(resource_registry.deepcopy(p), p)
```

### Comparing `enact-0.4.5/tests/test_resources.py` & `enact-0.4.6/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/tests/test_serialize.py` & `enact-0.4.6/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/tests/test_type_wrappers.py` & `enact-0.4.6/tests/test_type_wrappers.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.5/tests/test_utils.py` & `enact-0.4.6/tests/test_utils.py`

 * *Files identical despite different names*

