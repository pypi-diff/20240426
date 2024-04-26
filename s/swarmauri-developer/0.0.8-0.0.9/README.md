# Comparing `tmp/swarmauri_developer-0.0.8.tar.gz` & `tmp/swarmauri_developer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarmauri_developer-0.0.8.tar", last modified: Wed Apr 24 17:40:02 2024, max compression
+gzip compressed data, was "swarmauri_developer-0.0.9.tar", last modified: Fri Apr 26 09:54:41 2024, max compression
```

## Comparing `swarmauri_developer-0.0.8.tar` & `swarmauri_developer-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:40:02.595650 swarmauri_developer-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-24 17:40:02.595650 swarmauri_developer-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-24 17:39:54.000000 swarmauri_developer-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 17:40:02.595650 swarmauri_developer-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-24 17:39:54.000000 swarmauri_developer-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:40:02.595650 swarmauri_developer-0.0.8/swarmauri_developer/
--rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-04-24 17:39:54.000000 swarmauri_developer-0.0.8/swarmauri_developer/DeveloperAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-24 17:39:54.000000 swarmauri_developer-0.0.8/swarmauri_developer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:40:02.595650 swarmauri_developer-0.0.8/swarmauri_developer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-24 17:40:02.000000 swarmauri_developer-0.0.8/swarmauri_developer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 17:40:02.000000 swarmauri_developer-0.0.8/swarmauri_developer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:40:02.000000 swarmauri_developer-0.0.8/swarmauri_developer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 17:40:02.000000 swarmauri_developer-0.0.8/swarmauri_developer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 17:40:02.000000 swarmauri_developer-0.0.8/swarmauri_developer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 17:40:02.000000 swarmauri_developer-0.0.8/swarmauri_developer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:41.783247 swarmauri_developer-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-26 09:54:41.779247 swarmauri_developer-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-26 09:54:32.000000 swarmauri_developer-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:54:41.783247 swarmauri_developer-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-26 09:54:32.000000 swarmauri_developer-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:41.779247 swarmauri_developer-0.0.9/swarmauri_developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-04-26 09:54:32.000000 swarmauri_developer-0.0.9/swarmauri_developer/DeveloperAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-26 09:54:32.000000 swarmauri_developer-0.0.9/swarmauri_developer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:54:41.779247 swarmauri_developer-0.0.9/swarmauri_developer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-26 09:54:41.000000 swarmauri_developer-0.0.9/swarmauri_developer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-26 09:54:41.000000 swarmauri_developer-0.0.9/swarmauri_developer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:54:41.000000 swarmauri_developer-0.0.9/swarmauri_developer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 09:54:41.000000 swarmauri_developer-0.0.9/swarmauri_developer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 09:54:41.000000 swarmauri_developer-0.0.9/swarmauri_developer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 09:54:41.000000 swarmauri_developer-0.0.9/swarmauri_developer.egg-info/top_level.txt
```

### Comparing `swarmauri_developer-0.0.8/PKG-INFO` & `swarmauri_developer-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri_developer
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Swarmauri Developer Assistant is part of the swarmaURI framework and is designed to enable developers to rapidly develop with the Swarmauri Sdk.. This tool is designed to enhance software development workflows by integrating an advanced AI with pretrained vectorizers and document retrieval. The assistant features a web gui with chatbot, file explorer and editor, and code interpreter.
 Home-page: http://github.com/swarmauri/developer_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `swarmauri_developer-0.0.8/README.md` & `swarmauri_developer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `swarmauri_developer-0.0.8/setup.py` & `swarmauri_developer-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `swarmauri_developer-0.0.8/swarmauri_developer/DeveloperAssistant.py` & `swarmauri_developer-0.0.9/swarmauri_developer/DeveloperAssistant.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,22 +223,26 @@
     def launch(self):
         self.app.launch(share=True)
 
 def main():
     import argparse
     parser = argparse.ArgumentParser(description="Swarmauri Developer Assistant Command Line Tool")
     parser.add_argument('-api_key', '--api_key', type=str, help='OPENAI_API_KEY', required=True)
+    parser.add_argument('-share', '--share', type=bool, help='Deploy a live app on gradio', required=False)
     parser.add_argument('-db_path', '--db_path', type=str, help='path to sqlite3 db', required=False)
     parser.add_argument('-vector_store_path', '--vector_store_path', type=str, help='path to vector store artifacts', required=False)
     args = parser.parse_args()
 
     api_key = args.api_key
     
     assistant = DeveloperAssistant(api_key=api_key)
     if args.db_path:
         assistant.db_path = args.db_path
     if args.vector_store_path:
         assistant.vector_store_path = args.vector_store_path
-    assistant.launch()
-
+    if args.share:
+        assistant.launch(share=args.share)
+    else:
+        assistant.launch(share=False)
+        
 if __name__ == "__main__":
     main()
```

### Comparing `swarmauri_developer-0.0.8/swarmauri_developer/__init__.py` & `swarmauri_developer-0.0.9/swarmauri_developer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __short_desc__ = """The Swarmauri Developer Assistant is part of the swarmaURI framework and is designed to enable developers to rapidly develop with the Swarmauri Sdk.. This tool is designed to enhance software development workflows by integrating an advanced AI with pretrained vectorizers and document retrieval. The assistant features a web gui with chatbot, file explorer and editor, and code interpreter."""
 __long_desc__ = """# Swarmauri Developer Assistant
 
 ## Overview
 The Swarmauri Developer Assistant is part of the swarmaURI framework and is designed to enable developers to rapidly develop with the Swarmauri Sdk.. This tool is designed to enhance software development workflows by integrating an advanced AI with pretrained vectorizers and document retrieval. The assistant features a web gui with chatbot, file explorer and editor, and code interpreter.
 
 ## Features
```

### Comparing `swarmauri_developer-0.0.8/swarmauri_developer.egg-info/PKG-INFO` & `swarmauri_developer-0.0.9/swarmauri_developer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri_developer
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Swarmauri Developer Assistant is part of the swarmaURI framework and is designed to enable developers to rapidly develop with the Swarmauri Sdk.. This tool is designed to enhance software development workflows by integrating an advanced AI with pretrained vectorizers and document retrieval. The assistant features a web gui with chatbot, file explorer and editor, and code interpreter.
 Home-page: http://github.com/swarmauri/developer_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

