# Comparing `tmp/ollama-0.1.8.tar.gz` & `tmp/ollama-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama-0.1.8.tar", max compression
+gzip compressed data, was "ollama-0.1.9.tar", max compression
```

## Comparing `ollama-0.1.8.tar` & `ollama-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1058 2024-03-27 17:38:54.820834 ollama-0.1.8/LICENSE
--rw-r--r--   0        0        0     3063 2024-03-27 17:38:54.820834 ollama-0.1.8/README.md
--rw-r--r--   0        0        0      720 2024-03-27 17:38:54.820834 ollama-0.1.8/ollama/__init__.py
--rw-r--r--   0        0        0    23826 2024-03-27 17:38:54.820834 ollama-0.1.8/ollama/_client.py
--rw-r--r--   0        0        0     3399 2024-03-27 17:38:54.820834 ollama-0.1.8/ollama/_types.py
--rw-r--r--   0        0        0      835 2024-03-27 17:39:04.480806 ollama-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 ollama-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-04-26 00:13:08.529790 ollama-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3062 2024-04-26 00:13:08.529790 ollama-0.1.9/README.md
+-rw-r--r--   0        0        0      720 2024-04-26 00:13:08.529790 ollama-0.1.9/ollama/__init__.py
+-rw-r--r--   0        0        0    23836 2024-04-26 00:13:08.529790 ollama-0.1.9/ollama/_client.py
+-rw-r--r--   0        0        0     3399 2024-04-26 00:13:08.529790 ollama-0.1.9/ollama/_types.py
+-rw-r--r--   0        0        0      855 2024-04-26 00:13:18.773812 ollama-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 ollama-0.1.9/PKG-INFO
```

### Comparing `ollama-0.1.8/LICENSE` & `ollama-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama-0.1.8/README.md` & `ollama-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 ```python
 ollama.push('user/llama2')
 ```
 
 ### Embeddings
 
 ```python
-ollama.embeddings(model='llama2', prompt='They sky is blue because of rayleigh scattering')
+ollama.embeddings(model='llama2', prompt='The sky is blue because of rayleigh scattering')
 ```
 
 ## Custom client
 
 A custom client can be created with the following fields:
 
 - `host`: The Ollama host to connect to
```

### Comparing `ollama-0.1.8/ollama/__init__.py` & `ollama-0.1.9/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `ollama-0.1.8/ollama/_client.py` & `ollama-0.1.9/ollama/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
       raise RequestError('must provide a model')
 
     for message in messages or []:
       if not isinstance(message, dict):
         raise TypeError('messages must be a list of Message or dict-like objects')
       if not (role := message.get('role')) or role not in ['system', 'user', 'assistant']:
         raise RequestError('messages must contain a role and it must be one of "system", "user", or "assistant"')
-      if not message.get('content'):
+      if 'content' not in message:
         raise RequestError('messages must contain content')
       if images := message.get('images'):
         message['images'] = [_encode_image(image) for image in images]
 
     return self._request_stream(
       'POST',
       '/api/chat',
@@ -190,15 +190,15 @@
 
   def embeddings(
     self,
     model: str = '',
     prompt: str = '',
     options: Optional[Options] = None,
     keep_alive: Optional[Union[float, str]] = None,
-  ) -> Sequence[float]:
+  ) -> Mapping[str, Sequence[float]]:
     return self._request(
       'POST',
       '/api/embeddings',
       json={
         'model': model,
         'prompt': prompt,
         'options': options or {},
@@ -445,15 +445,15 @@
       raise RequestError('must provide a model')
 
     for message in messages or []:
       if not isinstance(message, dict):
         raise TypeError('messages must be a list of strings')
       if not (role := message.get('role')) or role not in ['system', 'user', 'assistant']:
         raise RequestError('messages must contain a role and it must be one of "system", "user", or "assistant"')
-      if not message.get('content'):
+      if 'content' not in message:
         raise RequestError('messages must contain content')
       if images := message.get('images'):
         message['images'] = [_encode_image(image) for image in images]
 
     return await self._request_stream(
       'POST',
       '/api/chat',
```

### Comparing `ollama-0.1.8/ollama/_types.py` & `ollama-0.1.9/ollama/_types.py`

 * *Files identical despite different names*

### Comparing `ollama-0.1.8/pyproject.toml` & `ollama-0.1.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "ollama"
-version = "0.1.8"
+version = "0.1.9"
 description = "The official Python client for Ollama."
 authors = ["Ollama <hello@ollama.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://ollama.ai"
 repository = "https://github.com/jmorganca/ollama-python"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.27.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.3"
+pytest = ">=7.4.3,<9.0.0"
 pytest-asyncio = "^0.23.2"
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 pytest-httpserver = "^1.0.8"
 pillow = "^10.2.0"
-ruff = "^0.1.8"
+ruff = ">=0.1.8,<0.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 999
```

### Comparing `ollama-0.1.8/PKG-INFO` & `ollama-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama
-Version: 0.1.8
+Version: 0.1.9
 Summary: The official Python client for Ollama.
 Home-page: https://ollama.ai
 License: MIT
 Author: Ollama
 Author-email: hello@ollama.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -120,15 +120,15 @@
 ```python
 ollama.push('user/llama2')
 ```
 
 ### Embeddings
 
 ```python
-ollama.embeddings(model='llama2', prompt='They sky is blue because of rayleigh scattering')
+ollama.embeddings(model='llama2', prompt='The sky is blue because of rayleigh scattering')
 ```
 
 ## Custom client
 
 A custom client can be created with the following fields:
 
 - `host`: The Ollama host to connect to
```

