# Comparing `tmp/llama_index_tools_google-0.1.3.tar.gz` & `tmp/llama_index_tools_google-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_tools_google-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_tools_google-0.1.4.tar", max compression
```

## Comparing `llama_index_tools_google-0.1.3.tar` & `llama_index_tools_google-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       39 2024-02-13 13:53:01.941395 llama_index_tools_google-0.1.3/README.md
--rw-r--r--   0        0        0      351 2024-02-13 13:53:01.942129 llama_index_tools_google-0.1.3/llama_index/tools/google/__init__.py
--rw-r--r--   0        0        0        0 2024-02-13 13:53:01.942240 llama_index_tools_google-0.1.3/llama_index/tools/google/calendar/__init__.py
--rw-r--r--   0        0        0     7158 2024-02-13 13:53:01.942312 llama_index_tools_google-0.1.3/llama_index/tools/google/calendar/base.py
--rw-r--r--   0        0        0        0 2024-02-13 13:53:01.942431 llama_index_tools_google-0.1.3/llama_index/tools/google/gmail/__init__.py
--rw-r--r--   0        0        0     9163 2024-02-13 13:53:01.942520 llama_index_tools_google-0.1.3/llama_index/tools/google/gmail/base.py
--rw-r--r--   0        0        0        7 2024-02-13 13:53:01.942660 llama_index_tools_google-0.1.3/llama_index/tools/google/search/__init__.py
--rw-r--r--   0        0        0     1449 2024-02-13 13:53:01.942728 llama_index_tools_google-0.1.3/llama_index/tools/google/search/base.py
--rw-r--r--   0        0        0     1719 2024-02-21 22:17:26.578481 llama_index_tools_google-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 llama_index_tools_google-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/README.md
+-rw-r--r--   0        0        0      351 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/calendar/__init__.py
+-rw-r--r--   0        0        0     7162 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/calendar/base.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/gmail/__init__.py
+-rw-r--r--   0        0        0     9163 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/gmail/base.py
+-rw-r--r--   0        0        0        7 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/search/__init__.py
+-rw-r--r--   0        0        0     1449 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/search/base.py
+-rw-r--r--   0        0        0     1688 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 llama_index_tools_google-0.1.4/PKG-INFO
```

### Comparing `llama_index_tools_google-0.1.3/llama_index/tools/google/calendar/base.py` & `llama_index_tools_google-0.1.4/llama_index/tools/google/calendar/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,20 +162,20 @@
         credentials = self._get_credentials()
         service = build("calendar", "v3", credentials=credentials)
 
         attendees_list = []
         for attendee in attendees:
             attendees_list.append({"email": attendee})
         start_time = (
-            datetime.datetime.strptime(start_datetime, "%Y-%m-%dT%H:%M:%S")
+            datetime.datetime.strptime(start_datetime, "%Y-%m-%dT%H:%M:%S%z")
             .astimezone()
             .strftime("%Y-%m-%dT%H:%M:%S.%f%z")
         )
         end_time = (
-            datetime.datetime.strptime(end_datetime, "%Y-%m-%dT%H:%M:%S")
+            datetime.datetime.strptime(end_datetime, "%Y-%m-%dT%H:%M:%S%z")
             .astimezone()
             .strftime("%Y-%m-%dT%H:%M:%S.%f%z")
         )
 
         event = {
             "summary": title,
             "location": location,
```

### Comparing `llama_index_tools_google-0.1.3/llama_index/tools/google/gmail/base.py` & `llama_index_tools_google-0.1.4/llama_index/tools/google/gmail/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_tools_google-0.1.3/llama_index/tools/google/search/base.py` & `llama_index_tools_google-0.1.4/llama_index/tools/google/search/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_tools_google-0.1.3/pyproject.toml` & `llama_index_tools_google-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 contains_example = false
 import_path = "llama_index.tools.google"
 
 [tool.llamahub.class_authors]
 GmailToolSpec = "ajhofmann"
 GoogleCalendarToolSpec = "ajhofmann"
 GoogleSearchToolSpec = "ajhofmann"
-QUERY_URL_TMPL = "llama-index"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
@@ -28,15 +27,15 @@
 description = "llama-index tools google integration"
 exclude = ["**/BUILD"]
 keywords = ["email", "gmail"]
 license = "MIT"
 maintainers = ["ajhofmann"]
 name = "llama-index-tools-google"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 google-api-python-client = "^2.115.0"
 google-auth-httplib2 = "^0.2.0"
 google-auth-oauthlib = "^1.2.0"
```

### Comparing `llama_index_tools_google-0.1.3/PKG-INFO` & `llama_index_tools_google-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: llama-index-tools-google
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index tools google integration
 License: MIT
 Keywords: email,gmail
 Author: Your Name
 Author-email: you@example.com
 Maintainer: ajhofmann
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: google-api-python-client (>=2.115.0,<3.0.0)
 Requires-Dist: google-auth-httplib2 (>=0.2.0,<0.3.0)
 Requires-Dist: google-auth-oauthlib (>=1.2.0,<2.0.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
```

