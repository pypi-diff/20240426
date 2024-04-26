# Comparing `tmp/langchain_zhipu-4.1.2.tar.gz` & `tmp/langchain_zhipu-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_zhipu-4.1.2.tar", max compression
+gzip compressed data, was "langchain_zhipu-4.1.3.tar", max compression
```

## Comparing `langchain_zhipu-4.1.2.tar` & `langchain_zhipu-4.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     4221 2024-04-19 01:27:50.154822 langchain_zhipu-4.1.2/README.md
--rw-r--r--   0        0        0      971 2024-04-20 11:17:13.232062 langchain_zhipu-4.1.2/langchain_zhipu/__init__.py
--rw-r--r--   0        0        0       23 2024-04-20 11:12:51.678450 langchain_zhipu-4.1.2/langchain_zhipu/__version__.py
--rw-r--r--   0        0        0        0 2024-03-28 15:37:31.905694 langchain_zhipu-4.1.2/langchain_zhipu/http/__init__.py
--rw-r--r--   0        0        0     4844 2024-04-20 11:05:25.768200 langchain_zhipu-4.1.2/langchain_zhipu/http/api.py
--rw-r--r--   0        0        0    13779 2024-04-13 06:21:01.194348 langchain_zhipu-4.1.2/langchain_zhipu/http/base.py
--rw-r--r--   0        0        0     7825 2024-04-13 06:21:17.673386 langchain_zhipu-4.1.2/langchain_zhipu/http/chat.py
--rw-r--r--   0        0        0     1714 2024-04-13 03:17:37.336032 langchain_zhipu-4.1.2/langchain_zhipu/http/embeddings.py
--rw-r--r--   0        0        0      500 2024-04-02 14:02:48.067993 langchain_zhipu-4.1.2/langchain_zhipu/http/enum.py
--rw-r--r--   0        0        0      382 2024-04-09 02:22:51.583321 langchain_zhipu-4.1.2/langchain_zhipu/http/env.py
--rw-r--r--   0        0        0     8994 2024-04-09 02:58:49.863351 langchain_zhipu-4.1.2/langchain_zhipu/http/manager.py
--rw-r--r--   0        0        0     4099 2024-04-06 13:39:34.256771 langchain_zhipu-4.1.2/langchain_zhipu/http/types.py
--rw-r--r--   0        0        0     1721 2024-03-26 15:19:10.785090 langchain_zhipu-4.1.2/langchain_zhipu/utils.py
--rw-r--r--   0        0        0      750 2024-04-20 11:12:58.052250 langchain_zhipu-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     5066 1970-01-01 00:00:00.000000 langchain_zhipu-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4221 2024-04-19 01:27:50.154822 langchain_zhipu-4.1.3/README.md
+-rw-r--r--   0        0        0      971 2024-04-20 11:17:13.232062 langchain_zhipu-4.1.3/langchain_zhipu/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-26 14:01:10.986554 langchain_zhipu-4.1.3/langchain_zhipu/__version__.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:37:31.905694 langchain_zhipu-4.1.3/langchain_zhipu/http/__init__.py
+-rw-r--r--   0        0        0     4844 2024-04-20 11:05:25.768200 langchain_zhipu-4.1.3/langchain_zhipu/http/api.py
+-rw-r--r--   0        0        0    13692 2024-04-26 13:59:03.840626 langchain_zhipu-4.1.3/langchain_zhipu/http/base.py
+-rw-r--r--   0        0        0     7825 2024-04-13 06:21:17.673386 langchain_zhipu-4.1.3/langchain_zhipu/http/chat.py
+-rw-r--r--   0        0        0     1714 2024-04-13 03:17:37.336032 langchain_zhipu-4.1.3/langchain_zhipu/http/embeddings.py
+-rw-r--r--   0        0        0      500 2024-04-02 14:02:48.067993 langchain_zhipu-4.1.3/langchain_zhipu/http/enum.py
+-rw-r--r--   0        0        0      382 2024-04-09 02:22:51.583321 langchain_zhipu-4.1.3/langchain_zhipu/http/env.py
+-rw-r--r--   0        0        0     8994 2024-04-09 02:58:49.863351 langchain_zhipu-4.1.3/langchain_zhipu/http/manager.py
+-rw-r--r--   0        0        0     4099 2024-04-06 13:39:34.256771 langchain_zhipu-4.1.3/langchain_zhipu/http/types.py
+-rw-r--r--   0        0        0     1721 2024-03-26 15:19:10.785090 langchain_zhipu-4.1.3/langchain_zhipu/utils.py
+-rw-r--r--   0        0        0      750 2024-04-26 14:01:14.853856 langchain_zhipu-4.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5066 1970-01-01 00:00:00.000000 langchain_zhipu-4.1.3/PKG-INFO
```

### Comparing `langchain_zhipu-4.1.2/README.md` & `langchain_zhipu-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.2/langchain_zhipu/__init__.py` & `langchain_zhipu-4.1.3/langchain_zhipu/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.2/langchain_zhipu/http/api.py` & `langchain_zhipu-4.1.3/langchain_zhipu/http/api.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.2/langchain_zhipu/http/base.py` & `langchain_zhipu-4.1.3/langchain_zhipu/http/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,17 +118,14 @@
 
         if self.model:
             attributes["model"] = self.model
 
         if self.streaming:
             attributes["streaming"] = self.streaming
 
-        if self.return_type:
-            attributes["return_type"] = self.return_type
-
         return attributes
 
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
         """Get the namespace of the langchain object."""
         return ["langchain", "chat_models", "ZhipuAI"]
```

### Comparing `langchain_zhipu-4.1.2/langchain_zhipu/http/chat.py` & `langchain_zhipu-4.1.3/langchain_zhipu/http/chat.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.2/langchain_zhipu/http/embeddings.py` & `langchain_zhipu-4.1.3/langchain_zhipu/http/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.2/langchain_zhipu/http/manager.py` & `langchain_zhipu-4.1.3/langchain_zhipu/http/manager.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.2/langchain_zhipu/http/types.py` & `langchain_zhipu-4.1.3/langchain_zhipu/http/types.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.2/langchain_zhipu/utils.py` & `langchain_zhipu-4.1.3/langchain_zhipu/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.2/pyproject.toml` & `langchain_zhipu-4.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain_zhipu"
-version = "4.1.2"
+version = "4.1.3"
 description = "将智谱AI集成到LangChain"
 license = "MIT"
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/langchain_zhipuai"
 repository = "https://github.com/arcstep/langchain_zhipuai.git"
 readme = "README.md"
```

### Comparing `langchain_zhipu-4.1.2/PKG-INFO` & `langchain_zhipu-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_zhipu
-Version: 4.1.2
+Version: 4.1.3
 Summary: 将智谱AI集成到LangChain
 Home-page: https://github.com/arcstep/langchain_zhipuai
 License: MIT
 Author: arcstep
 Author-email: 43801@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

