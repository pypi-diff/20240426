# Comparing `tmp/PerplexiPy-1.0.3-py3-none-any.whl.zip` & `tmp/PerplexiPy-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11647 bytes, number of entries: 10
+Zip file size: 11711 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     9253 b- defN 24-Apr-22 04:33 perplexipy/__init__.py
--rw-r--r--  2.0 unx     9179 b- defN 24-Apr-22 04:33 perplexipy/codex.py
+-rw-r--r--  2.0 unx     9490 b- defN 24-Apr-26 04:59 perplexipy/codex.py
 -rw-r--r--  2.0 unx      283 b- defN 24-Mar-01 20:13 perplexipy/errors.py
 -rw-r--r--  2.0 unx      684 b- defN 24-Apr-13 17:06 perplexipy/responses.py
--rw-r--r--  2.0 unx     1514 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6833 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/RECORD
-10 files, 28711 bytes uncompressed, 10255 bytes compressed:  64.3%
+-rw-r--r--  2.0 unx     1514 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6833 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/RECORD
+10 files, 29022 bytes uncompressed, 10319 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: perplexipy/errors.py
 Comment: 
 
 Filename: perplexipy/responses.py
 Comment: 
 
-Filename: PerplexiPy-1.0.3.dist-info/LICENSE.txt
+Filename: PerplexiPy-1.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.3.dist-info/METADATA
+Filename: PerplexiPy-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: PerplexiPy-1.0.3.dist-info/WHEEL
+Filename: PerplexiPy-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: PerplexiPy-1.0.3.dist-info/entry_points.txt
+Filename: PerplexiPy-1.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.3.dist-info/top_level.txt
+Filename: PerplexiPy-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.3.dist-info/RECORD
+Filename: PerplexiPy-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perplexipy/codex.py

```diff
@@ -30,15 +30,15 @@
 @private
 """
 CONFIG_FILE_NAME = os.path.join(CONFIG_PATH, 'codex-repl.yaml')
 """
 @private
 """
 
-DEFAULT_LLM = 'mixtral-8x7b-instruct'
+DEFAULT_MODEL_NAME = 'mixtral-8x7b-instruct'
 DEFAULT_VIM_EDIT_MODE = True
 """
 @private
 """
 
 QUERY_CRISP = 'Concise, code only reply to this prompt: '
 """
@@ -50,18 +50,32 @@
 @private
 """
 
 
 # *** globals ***
 
 _client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
-_client.model = DEFAULT_LLM
+_client.model = DEFAULT_MODEL_NAME
 _queryCodeStyle = True
 
 
+# *** classes and objects ***
+
+class CodexREPL:
+
+    def __init__(self):
+        self._client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
+        self._client.model = DEFAULT_MODEL_NAME
+        self._queryCodeStyle = True
+
+
+    def run(self):
+        pass
+
+
 # *** implementation ***
 
 def _die(msg: str, exitCode: int = 99):
     click.echo(msg)
     sys.exit(99)
 
 
@@ -84,15 +98,15 @@
     """
     global _client
 
     result = None
     if userQuery:
         if not _client:
             _client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
-            _client.model = DEFAULT_LLM
+            _client.model = DEFAULT_MODEL_NAME
         result = _client.query(userQuery)
 
     return result
 
 
 def _stdinHasData() -> bool:
     """
@@ -210,15 +224,15 @@
 
 def _loadConfigFrom(fileName: str = CONFIG_FILE_NAME, pathName = CONFIG_PATH) -> dict:
     if os.path.exists(fileName):
         with open(fileName, 'r') as inputFile:
             config = yaml.safe_load(inputFile)
     else:
         config = {
-            'activeModel': 3,
+            'activeModel': DEFAULT_MODEL_NAME,
             'editingMode': 'vi',
             'queryCodeStyle': _queryCodeStyle,
         }
         _saveConfigTo(config, fileName, pathName)
     return config
```

## Comparing `PerplexiPy-1.0.3.dist-info/LICENSE.txt` & `PerplexiPy-1.0.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PerplexiPy-1.0.3.dist-info/METADATA` & `PerplexiPy-1.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PerplexiPy
-Version: 1.0.3
+Version: 1.0.4
 Summary: PerplexiPy - A robust Perplexity AI API client
 Author-email: CIME Software Ltd <perplexipy@cime.net>
 License: BSD-3
 Project-URL: homepage, https://cime-software.github.io/perplexipy/
 Project-URL: Documentation, https://cime-software.github.io/perplexipy/
 Project-URL: Bug Tracker, https://github.com/CIME-Software/perplexipy/issues
 Project-URL: Source, https://github.com/CIME-Software/perplexipy
@@ -22,15 +22,15 @@
 Requires-Dist: appdirs
 Requires-Dist: click
 Requires-Dist: openai (>=1.12.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 
-% perplexipy(3) Version 1.0.3 | Perplexity AI high level API documentation
+% perplexipy(3) Version 1.0.4 | Perplexity AI high level API documentation
 
 Name
 ====
 
 **PerplexiPy** - Perplexity AI high level library
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.3 Summary: PerplexiPy - A
+Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.4 Summary: PerplexiPy - A
 robust Perplexity AI API client Author-email: CIME Software Ltd
 cime.net> License: BSD-3 Project-URL: homepage, https://cime-
 software.github.io/perplexipy/ Project-URL: Documentation, https://cime-
 software.github.io/perplexipy/ Project-URL: Bug Tracker, https://github.com/
 CIME-Software/perplexipy/issues Project-URL: Source, https://github.com/CIME-
 Software/perplexipy Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: appdirs Requires-Dist: click Requires-Dist: openai
 (>=1.12.0) Requires-Dist: prompt-toolkit Requires-Dist: python-dotenv Requires-
-Dist: pyyaml % perplexipy(3) Version 1.0.3 | Perplexity AI high level API
+Dist: pyyaml % perplexipy(3) Version 1.0.4 | Perplexity AI high level API
 documentation Name ==== **PerplexiPy** - Perplexity AI high level library
 [https://images2.imgbox.com/57/94/AsI1WSfy_o.png]Synopsis ======== ```python
 client = PerplexityClient() \ print(client.query('What is the meaning of 42?')
 \ for result in client.queryStreamable('List of all US presidents'): \ print
 (result) ``` Description =========== **PerplexiPy** is a high-level,
 convenience library for interacting with the Perplexity API from any Python
 3.9+ application. The library aims to simplify interactions with Perplexity
```

## Comparing `PerplexiPy-1.0.3.dist-info/RECORD` & `PerplexiPy-1.0.4.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 perplexipy/__init__.py,sha256=jex9IfNCEyLV3rtpq7L3VEfs75NmHXZki8l6wD-wohA,9253
-perplexipy/codex.py,sha256=ll0VrHpaSPjV4F8R9KejOfQMqRlS8loYsDStMcC10ls,9179
+perplexipy/codex.py,sha256=RpiWJeNE7oBwd2gyE9LUulRRr_ef99QOKeL9uRERqoc,9490
 perplexipy/errors.py,sha256=YM4dVV9q2aLm_ZJdhyCjhejLXdo8mEffx93zlP_7lOs,283
 perplexipy/responses.py,sha256=1OrBpZxGHaVvlE5x9ZtdQhoXP5RbmKOXtHGt6Nm7g2I,684
-PerplexiPy-1.0.3.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
-PerplexiPy-1.0.3.dist-info/METADATA,sha256=65rwMxA4ytU5fb9reFB592XzTk_-4xZpMofVg7XH950,6833
-PerplexiPy-1.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-PerplexiPy-1.0.3.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
-PerplexiPy-1.0.3.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
-PerplexiPy-1.0.3.dist-info/RECORD,,
+PerplexiPy-1.0.4.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
+PerplexiPy-1.0.4.dist-info/METADATA,sha256=lt80TVmlSkeKDnOywyrPU1-6dVppUXnJH9znhLVWvXo,6833
+PerplexiPy-1.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+PerplexiPy-1.0.4.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
+PerplexiPy-1.0.4.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
+PerplexiPy-1.0.4.dist-info/RECORD,,
```

