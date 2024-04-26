# Comparing `tmp/dimentyy_tl_parse-0.0.1.dev1.tar.gz` & `tmp/dimentyy_tl_parse-0.0.1.dev2.tar.gz`

## Comparing `dimentyy_tl_parse-0.0.1.dev1.tar` & `dimentyy_tl_parse-0.0.1.dev2.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev1/LICENSE.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev1/README.md
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev1/pyproject.toml
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/fake-src/dimentyy/tl/parse/__init__.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/fake-src/dimentyy/tl/parse/container.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/fake-src/dimentyy/tl/parse/new_html.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/fake-src/dimentyy/tl/parse/types.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/LICENSE.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/PKG-INFO
```

### Comparing `dimentyy_tl_parse-0.0.1.dev1/LICENSE.md` & `dimentyy_tl_parse-0.0.1.dev2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dimentyy_tl_parse-0.0.1.dev1/pyproject.toml` & `dimentyy_tl_parse-0.0.1.dev2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
-packages = ["dimentyy"]
+packages = ["fake-src/dimentyy"]
 
 [tool.hatch.build.targets.sdist]
-only-include = ["dimentyy"]
+only-include = ["fake-src/dimentyy"]
 
 [project]
 name = "dimentyy.tl-parse"
 description = "Better parsing modes for telethon.TelegramClient"
-version = "0.0.1dev1"
+version = "0.0.1dev2"
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 authors = [
   { name = "dimentyy" },
 ]
 classifiers = [
```

### Comparing `dimentyy_tl_parse-0.0.1.dev1/PKG-INFO` & `dimentyy_tl_parse-0.0.1.dev2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dimentyy.tl-parse
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Better parsing modes for telethon.TelegramClient
 Project-URL: Source, https://github.com/dimentyy/tl-parse.py
 Project-URL: Author, https://t.me/dimentyy
 Author: dimentyy
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
```

