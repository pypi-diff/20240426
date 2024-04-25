# Comparing `tmp/gcr_chat-0.1.1.tar.gz` & `tmp/gcr_chat-0.1.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcr_chat-0.1.1.tar", max compression
+gzip compressed data, was "gcr_chat-0.1.1.dev1.tar", max compression
```

## Comparing `gcr_chat-0.1.1.tar` & `gcr_chat-0.1.1.dev1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      729 2024-04-25 23:29:32.617216 gcr_chat-0.1.1/README.md
--rw-r--r--   0        0        0      471 2024-04-25 23:29:32.617711 gcr_chat-0.1.1/gcr_chat/__init__.py
--rw-r--r--   0        0        0      322 2024-04-25 23:29:32.617838 gcr_chat-0.1.1/gcr_chat/chatbot/__init__.py
--rw-r--r--   0        0        0     6374 2024-04-25 23:29:32.617957 gcr_chat-0.1.1/gcr_chat/chatbot/client.py
--rw-r--r--   0        0        0     2417 2024-04-25 23:29:32.618060 gcr_chat-0.1.1/gcr_chat/chatbot/command.py
--rw-r--r--   0        0        0      447 2024-04-25 23:29:32.618149 gcr_chat-0.1.1/gcr_chat/chatbot/exceptions.py
--rw-r--r--   0        0        0      699 2024-04-25 23:29:32.618246 gcr_chat-0.1.1/gcr_chat/models.py
--rw-r--r--   0        0        0     2020 2024-04-25 23:30:13.644472 gcr_chat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 gcr_chat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      729 2024-04-25 23:29:32.617216 gcr_chat-0.1.1.dev1/README.md
+-rw-r--r--   0        0        0      471 2024-04-25 23:29:32.617711 gcr_chat-0.1.1.dev1/gcr_chat/__init__.py
+-rw-r--r--   0        0        0      322 2024-04-25 23:29:32.617838 gcr_chat-0.1.1.dev1/gcr_chat/chatbot/__init__.py
+-rw-r--r--   0        0        0     6374 2024-04-25 23:29:32.617957 gcr_chat-0.1.1.dev1/gcr_chat/chatbot/client.py
+-rw-r--r--   0        0        0     2417 2024-04-25 23:29:32.618060 gcr_chat-0.1.1.dev1/gcr_chat/chatbot/command.py
+-rw-r--r--   0        0        0      447 2024-04-25 23:29:32.618149 gcr_chat-0.1.1.dev1/gcr_chat/chatbot/exceptions.py
+-rw-r--r--   0        0        0      699 2024-04-25 23:29:32.618246 gcr_chat-0.1.1.dev1/gcr_chat/models.py
+-rw-r--r--   0        0        0     2026 2024-04-25 23:29:32.618965 gcr_chat-0.1.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 gcr_chat-0.1.1.dev1/PKG-INFO
```

### Comparing `gcr_chat-0.1.1/README.md` & `gcr_chat-0.1.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `gcr_chat-0.1.1/gcr_chat/chatbot/client.py` & `gcr_chat-0.1.1.dev1/gcr_chat/chatbot/client.py`

 * *Files identical despite different names*

### Comparing `gcr_chat-0.1.1/gcr_chat/chatbot/command.py` & `gcr_chat-0.1.1.dev1/gcr_chat/chatbot/command.py`

 * *Files identical despite different names*

### Comparing `gcr_chat-0.1.1/gcr_chat/models.py` & `gcr_chat-0.1.1.dev1/gcr_chat/models.py`

 * *Files identical despite different names*

### Comparing `gcr_chat-0.1.1/pyproject.toml` & `gcr_chat-0.1.1.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcr_chat"
-version = "0.1.1"
+version = "0.1.1-dev.1"
 description = "Chatbot command parsing library to be used in conjunction with Google Cloud Run and GSuite Chat."
 authors = ["Sam Kenney <sam.kenney@me.com>"]
 readme = "README.md"
 packages = [{ include = "gcr_chat" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `gcr_chat-0.1.1/PKG-INFO` & `gcr_chat-0.1.1.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcr_chat
-Version: 0.1.1
+Version: 0.1.1.dev1
 Summary: Chatbot command parsing library to be used in conjunction with Google Cloud Run and GSuite Chat.
 Author: Sam Kenney
 Author-email: sam.kenney@me.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: examples
```

