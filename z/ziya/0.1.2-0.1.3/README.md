# Comparing `tmp/ziya-0.1.2.tar.gz` & `tmp/ziya-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziya-0.1.2.tar", max compression
+gzip compressed data, was "ziya-0.1.3.tar", max compression
```

## Comparing `ziya-0.1.2.tar` & `ziya-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.2/LICENSE
--rw-r--r--   0        0        0     1714 2024-04-24 04:42:40.757902 ziya-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.2/app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.2/app/agents/__init__.py
--rw-r--r--   0        0        0     4266 2024-04-24 04:42:40.748800 ziya-0.1.2/app/agents/agent.py
--rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.2/app/agents/prompts.py
--rw-r--r--   0        0        0     1688 2024-04-24 04:42:40.748995 ziya-0.1.2/app/main.py
--rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.2/app/server.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.2/app/utils/__init__.py
--rw-r--r--   0        0        0     2278 2024-04-24 04:42:40.749189 ziya-0.1.2/app/utils/directory_util.py
--rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.2/app/utils/gitignore_parser.py
--rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.2/app/utils/logging_utils.py
--rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.2/app/utils/print_tree_util.py
--rw-r--r--   0        0        0      716 2024-04-24 04:43:41.685380 ziya-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3622 2024-04-24 04:42:38.591520 ziya-0.1.2/static/app.js
--rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.2/static/favicon.ico
--rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.2/static/sendPayload.js
--rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.2/static/ziya.css
--rw-r--r--   0        0        0      800 2024-04-23 01:33:44.760779 ziya-0.1.2/templates/index.html
--rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 ziya-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2072 2024-04-26 01:28:16.357186 ziya-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.3/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.3/app/agents/__init__.py
+-rw-r--r--   0        0        0     4266 2024-04-24 04:42:40.748800 ziya-0.1.3/app/agents/agent.py
+-rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.3/app/agents/prompts.py
+-rw-r--r--   0        0        0     1704 2024-04-26 01:28:16.352143 ziya-0.1.3/app/main.py
+-rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.3/app/server.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.3/app/utils/__init__.py
+-rw-r--r--   0        0        0     2278 2024-04-24 04:42:40.749189 ziya-0.1.3/app/utils/directory_util.py
+-rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.3/app/utils/gitignore_parser.py
+-rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.3/app/utils/logging_utils.py
+-rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.3/app/utils/print_tree_util.py
+-rw-r--r--   0        0        0      716 2024-04-26 01:28:16.352353 ziya-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3622 2024-04-24 04:42:38.591520 ziya-0.1.3/static/app.js
+-rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.3/static/favicon.ico
+-rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.3/static/sendPayload.js
+-rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.3/static/ziya.css
+-rw-r--r--   0        0        0      800 2024-04-23 01:33:44.760779 ziya-0.1.3/templates/index.html
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 ziya-0.1.3/PKG-INFO
```

### Comparing `ziya-0.1.2/LICENSE` & `ziya-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/README.md` & `ziya-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -49,18 +49,20 @@
         ├── main.py
         └── server.py
 ...
 ```
 
 ### Options
 
-`--exclude`: Comma-separated list of files or directories to exclude from the codebase.
+`--exclude`: Comma-separated list of files or directories or file suffix patterns to exclude from the codebase. Eg: `--exclude 'tst,build,*.py'`
+
+`--include`: Comma-separated list of directories to include. By default, it only searches for current directory for code files, but you can specify a list of subset directories under current folder to search instead of the entire folder. Eg: `--include='app,src/mappers'`
 
 `--profile`: AWS profile to use for the Bedrock LLM.
 
 `--model`: The AWS Bedrock Model to use, one of `haiku`(default), `sonnet` or `opus`.
 
 `--port`: The port number for frontend app. Default is `6969`.
 
 ```bash
-ziya --exclude='tst,build,*.py' --profile=ziya --model=sonnet --port=8080
+ziya --include='app,src/mappers' --exclude='tst,build,*.py' --profile=ziya --model=sonnet --port=8080
 ```
```

### Comparing `ziya-0.1.2/app/agents/agent.py` & `ziya-0.1.3/app/agents/agent.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/app/agents/prompts.py` & `ziya-0.1.3/app/agents/prompts.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/app/main.py` & `ziya-0.1.3/app/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 def main():
     os.environ["ZIYA_USER_CODEBASE_DIR"] = os.getcwd()
 
     parser = argparse.ArgumentParser(description="Run with custom options")
     parser.add_argument("--exclude", default=[], type=lambda x: x.split(','),
                         help="List of files or directories to exclude (e.g., --exclude 'tst,build,*.py')")
-    parser.add_argument("--include-dirs", default=[], type=lambda x: x.split(','),
-                        help="List of directories to include (e.g., --include 'src,static')")
+    parser.add_argument("--include", default=[], type=lambda x: x.split(','),
+                        help="List of directories to include (e.g., --include 'src,static'). Only directories for now")
     parser.add_argument("--profile", type=str, default=None,
                         help="AWS profile to use (e.g., --profile ziya)")
     parser.add_argument("--model", type=str, choices=["sonnet", "haiku", "opus"], default="haiku",
                         help="AWS Bedrock Model to use  (e.g., --model sonnet)")
     parser.add_argument("--port", type=int, default=6969,
                         help="Port number to run Ziya frontend on (e.g., --port 8080)")
     args = parser.parse_args()
 
     additional_excluded_dirs = ','.join([item for item in args.exclude])
     os.environ["ZIYA_ADDITIONAL_EXCLUDE_DIRS"] = additional_excluded_dirs
 
-    additional_included_dirs = ','.join([item for item in args.include_dirs])
+    additional_included_dirs = ','.join([item for item in args.include])
     os.environ["ZIYA_ADDITIONAL_INCLUDE_DIRS"] = additional_included_dirs
 
     if args.profile:
         os.environ["ZIYA_AWS_PROFILE"] = args.profile
     if args.model:
         os.environ["ZIYA_AWS_MODEL"] = args.model
```

### Comparing `ziya-0.1.2/app/server.py` & `ziya-0.1.3/app/server.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/app/utils/directory_util.py` & `ziya-0.1.3/app/utils/directory_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/app/utils/gitignore_parser.py` & `ziya-0.1.3/app/utils/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/app/utils/print_tree_util.py` & `ziya-0.1.3/app/utils/print_tree_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/pyproject.toml` & `ziya-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziya"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Vishnu Krishnaprasad <vishnukool@gmail.com>"]
 readme = "README.md"
 include = ["static/**/*", "templates/**/*", "pyproject.toml"]
 packages = [
     { include = "app" },
 ]
```

### Comparing `ziya-0.1.2/static/app.js` & `ziya-0.1.3/static/app.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/static/favicon.ico` & `ziya-0.1.3/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/static/sendPayload.js` & `ziya-0.1.3/static/sendPayload.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/static/ziya.css` & `ziya-0.1.3/static/ziya.css`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/templates/index.html` & `ziya-0.1.3/templates/index.html`

 * *Files identical despite different names*

### Comparing `ziya-0.1.2/PKG-INFO` & `ziya-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziya
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Vishnu Krishnaprasad
 Author-email: vishnukool@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -73,18 +73,20 @@
         ├── main.py
         └── server.py
 ...
 ```
 
 ### Options
 
-`--exclude`: Comma-separated list of files or directories to exclude from the codebase.
+`--exclude`: Comma-separated list of files or directories or file suffix patterns to exclude from the codebase. Eg: `--exclude 'tst,build,*.py'`
+
+`--include`: Comma-separated list of directories to include. By default, it only searches for current directory for code files, but you can specify a list of subset directories under current folder to search instead of the entire folder. Eg: `--include='app,src/mappers'`
 
 `--profile`: AWS profile to use for the Bedrock LLM.
 
 `--model`: The AWS Bedrock Model to use, one of `haiku`(default), `sonnet` or `opus`.
 
 `--port`: The port number for frontend app. Default is `6969`.
 
 ```bash
-ziya --exclude='tst,build,*.py' --profile=ziya --model=sonnet --port=8080
+ziya --include='app,src/mappers' --exclude='tst,build,*.py' --profile=ziya --model=sonnet --port=8080
 ```
```

