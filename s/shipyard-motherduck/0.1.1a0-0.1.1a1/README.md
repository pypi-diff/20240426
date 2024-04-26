# Comparing `tmp/shipyard_motherduck-0.1.1a0.tar.gz` & `tmp/shipyard_motherduck-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_motherduck-0.1.1a0.tar", max compression
+gzip compressed data, was "shipyard_motherduck-0.1.1a1.tar", max compression
```

## Comparing `shipyard_motherduck-0.1.1a0.tar` & `shipyard_motherduck-0.1.1a1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1389 2024-04-19 17:49:25.468173 shipyard_motherduck-0.1.1a0/README.md
--rw-r--r--   0        0        0      618 2024-04-24 20:34:17.815450 shipyard_motherduck-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-19 17:49:25.469225 shipyard_motherduck-0.1.1a0/shipyard_motherduck/__init__.py
--rw-r--r--   0        0        0      857 2024-04-23 20:50:28.199375 shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/authtest.py
--rw-r--r--   0        0        0     1088 2024-04-19 17:49:25.469563 shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/execute.py
--rw-r--r--   0        0        0     1880 2024-04-19 17:49:25.469691 shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/fetch.py
--rw-r--r--   0        0        0     3061 2024-04-19 17:49:25.469825 shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/upload.py
--rw-r--r--   0        0        0      865 2024-04-19 17:49:25.469968 shipyard_motherduck-0.1.1a0/shipyard_motherduck/exceptions.py
--rw-r--r--   0        0        0     7097 2024-04-19 17:49:25.470169 shipyard_motherduck-0.1.1a0/shipyard_motherduck/motherduck.py
--rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 shipyard_motherduck-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1389 2024-04-19 17:49:25.468173 shipyard_motherduck-0.1.1a1/README.md
+-rw-r--r--   0        0        0      618 2024-04-25 21:18:27.702028 shipyard_motherduck-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-19 17:49:25.469225 shipyard_motherduck-0.1.1a1/shipyard_motherduck/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-25 21:17:15.112818 shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/authtest.py
+-rw-r--r--   0        0        0     1088 2024-04-19 17:49:25.469563 shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/execute.py
+-rw-r--r--   0        0        0     1880 2024-04-19 17:49:25.469691 shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/fetch.py
+-rw-r--r--   0        0        0     3061 2024-04-19 17:49:25.469825 shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/upload.py
+-rw-r--r--   0        0        0      865 2024-04-19 17:49:25.469968 shipyard_motherduck-0.1.1a1/shipyard_motherduck/exceptions.py
+-rw-r--r--   0        0        0     7097 2024-04-19 17:49:25.470169 shipyard_motherduck-0.1.1a1/shipyard_motherduck/motherduck.py
+-rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 shipyard_motherduck-0.1.1a1/PKG-INFO
```

### Comparing `shipyard_motherduck-0.1.1a0/README.md` & `shipyard_motherduck-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.1a0/pyproject.toml` & `shipyard_motherduck-0.1.1a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-motherduck"
-version = "0.1.1a0"
+version = "0.1.1a1"
 description = "A local client for working with Python and MotherDuck"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shipyard-templates = "^0.8.2"
```

### Comparing `shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/execute.py` & `shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/execute.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/fetch.py` & `shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/upload.py` & `shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.1a0/shipyard_motherduck/exceptions.py` & `shipyard_motherduck-0.1.1a1/shipyard_motherduck/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.1a0/shipyard_motherduck/motherduck.py` & `shipyard_motherduck-0.1.1a1/shipyard_motherduck/motherduck.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.1a0/PKG-INFO` & `shipyard_motherduck-0.1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-motherduck
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: A local client for working with Python and MotherDuck
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

