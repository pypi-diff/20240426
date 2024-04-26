# Comparing `tmp/typedllm-0.2.3.tar.gz` & `tmp/typedllm-0.2.4.tar.gz`

## Comparing `typedllm-0.2.3.tar` & `typedllm-0.2.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.2.3/HISTORY.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/test_client.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/test_interop.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/test_prompt.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/test_tool.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedllm-0.2.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedllm-0.2.3/LICENSE
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 typedllm-0.2.3/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 typedllm-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 typedllm-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.2.4/HISTORY.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 typedllm-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 typedllm-0.2.4/tests/test_client.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 typedllm-0.2.4/tests/test_interop.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 typedllm-0.2.4/tests/test_prompt.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 typedllm-0.2.4/tests/test_tool.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedllm-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedllm-0.2.4/LICENSE
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 typedllm-0.2.4/README.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 typedllm-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 typedllm-0.2.4/PKG-INFO
```

### Comparing `typedllm-0.2.3/tests/conftest.py` & `typedllm-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.3/tests/test_client.py` & `typedllm-0.2.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.3/tests/test_interop.py` & `typedllm-0.2.4/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.3/tests/test_prompt.py` & `typedllm-0.2.4/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.3/tests/test_tool.py` & `typedllm-0.2.4/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.3/.gitignore` & `typedllm-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.3/LICENSE` & `typedllm-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.3/pyproject.toml` & `typedllm-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 authors = [
     {name = "Todd Cullen", email = "todd@100-x.ai"},
 ]
 dependencies = [
     "pydantic>=2.1.0",
     "httpx>=0.27.0",
     "litellm>=1.34.25",
-    "typedtemplate>=0.1.6"
+    "typedtemplate>=0.1.6",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 license = {text = "MIT"}
 dynamic = ["version"]
 
 [build-system]
```

