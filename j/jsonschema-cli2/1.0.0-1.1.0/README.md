# Comparing `tmp/jsonschema_cli2-1.0.0.tar.gz` & `tmp/jsonschema_cli2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_cli2-1.0.0.tar", max compression
+gzip compressed data, was "jsonschema_cli2-1.1.0.tar", max compression
```

## Comparing `jsonschema_cli2-1.0.0.tar` & `jsonschema_cli2-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/LICENSE
--rw-r--r--   0        0        0     2953 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/jsonschema_cli2/__init__.py
--rw-r--r--   0        0        0      110 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/jsonschema_cli2/__main__.py
--rw-r--r--   0        0        0     2221 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/jsonschema_cli2/args.py
--rw-r--r--   0        0        0      377 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/jsonschema_cli2/cli.py
--rw-r--r--   0        0        0       99 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/jsonschema_cli2/exceptions.py
--rw-r--r--   0        0        0      550 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/jsonschema_cli2/handlers.py
--rw-r--r--   0        0        0      910 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/jsonschema_cli2/load.py
--rw-r--r--   0        0        0      269 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/jsonschema_cli2/resolvers.py
--rw-r--r--   0        0        0     3831 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/jsonschema_cli2/tests/test_cli.py
--rw-r--r--   0        0        0     1751 2024-04-25 20:59:15.965629 jsonschema_cli2-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4304 1970-01-01 00:00:00.000000 jsonschema_cli2-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-26 14:08:14.134468 jsonschema_cli2-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2953 2024-04-26 14:08:14.138468 jsonschema_cli2-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 14:08:14.138468 jsonschema_cli2-1.1.0/jsonschema_cli2/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-26 14:08:14.138468 jsonschema_cli2-1.1.0/jsonschema_cli2/__main__.py
+-rw-r--r--   0        0        0     2219 2024-04-26 14:08:14.138468 jsonschema_cli2-1.1.0/jsonschema_cli2/args.py
+-rw-r--r--   0        0        0      377 2024-04-26 14:08:14.138468 jsonschema_cli2-1.1.0/jsonschema_cli2/cli.py
+-rw-r--r--   0        0        0       99 2024-04-26 14:08:14.138468 jsonschema_cli2-1.1.0/jsonschema_cli2/exceptions.py
+-rw-r--r--   0        0        0      550 2024-04-26 14:08:14.138468 jsonschema_cli2-1.1.0/jsonschema_cli2/handlers.py
+-rw-r--r--   0        0        0      910 2024-04-26 14:08:14.138468 jsonschema_cli2-1.1.0/jsonschema_cli2/load.py
+-rw-r--r--   0        0        0      269 2024-04-26 14:08:14.138468 jsonschema_cli2-1.1.0/jsonschema_cli2/resolvers.py
+-rw-r--r--   0        0        0     3831 2024-04-26 14:08:14.138468 jsonschema_cli2-1.1.0/jsonschema_cli2/tests/test_cli.py
+-rw-r--r--   0        0        0     1751 2024-04-26 14:08:14.138468 jsonschema_cli2-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4304 1970-01-01 00:00:00.000000 jsonschema_cli2-1.1.0/PKG-INFO
```

### Comparing `jsonschema_cli2-1.0.0/LICENSE` & `jsonschema_cli2-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_cli2-1.0.0/README.md` & `jsonschema_cli2-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jsonschema_cli2-1.0.0/jsonschema_cli2/args.py` & `jsonschema_cli2-1.1.0/jsonschema_cli2/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,9 +66,7 @@
 
 def schema_validate(args):
     path, schema = load_schema(args.schema_file_or_string)
     instance = load_instance(args.data_file_or_string)
     resolver = relative_path_resolver(schema, base_path=path)
 
     jsonschema.Draft7Validator(schema, resolver=resolver).validate(instance=instance)
-
-
```

### Comparing `jsonschema_cli2-1.0.0/jsonschema_cli2/handlers.py` & `jsonschema_cli2-1.1.0/jsonschema_cli2/handlers.py`

 * *Files identical despite different names*

### Comparing `jsonschema_cli2-1.0.0/jsonschema_cli2/load.py` & `jsonschema_cli2-1.1.0/jsonschema_cli2/load.py`

 * *Files identical despite different names*

### Comparing `jsonschema_cli2-1.0.0/jsonschema_cli2/tests/test_cli.py` & `jsonschema_cli2-1.1.0/jsonschema_cli2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jsonschema_cli2-1.0.0/pyproject.toml` & `jsonschema_cli2-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.scripts]
 jsonschema-cli2 = 'jsonschema_cli2.cli:run'
 
 [tool.poetry]
 name = "jsonschema-cli2"
-version = "1.0.0"
+version = "1.1.0"
 description = "A thin wrapper over to allow validating schemas easily using simple CLI commands."
 authors = ["solairen <solairen@solairen.tech>"]
 readme = 'README.md'
 classifiers = [
   "Development Status :: 5 - Production/Stable",
+  "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+  "Operating System :: OS Independent",
+  "Intended Audience :: Developers",
+  "Environment :: Console",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
-  "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-  "Operating System :: OS Independent",
-  "Intended Audience :: Developers",
-  "Environment :: Console"
+  "Programming Language :: Python :: Implementation :: PyPy"
 ]
 
 [tool.poetry.urls]
 Homepage = "https://github.com/solairen/jsonschema_cli2"
 Source = "https://github.com/solairen/jsonschema_cli2"
 Issues = "https://github.com/solairen/jsonschema_cli2/issues"
```

### Comparing `jsonschema_cli2-1.0.0/PKG-INFO` & `jsonschema_cli2-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-cli2
-Version: 1.0.0
+Version: 1.1.0
 Summary: A thin wrapper over to allow validating schemas easily using simple CLI commands.
 Author: solairen
 Author-email: solairen@solairen.tech
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

