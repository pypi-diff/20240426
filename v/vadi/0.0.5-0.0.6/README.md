# Comparing `tmp/vadi-0.0.5.tar.gz` & `tmp/vadi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vadi-0.0.5.tar", max compression
+gzip compressed data, was "vadi-0.0.6.tar", max compression
```

## Comparing `vadi-0.0.5.tar` & `vadi-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1074 2024-04-07 18:58:17.517436 vadi-0.0.5/LICENSE
--rw-r--r--   0        0        0     2864 2024-04-23 10:07:30.746937 vadi-0.0.5/README.md
--rw-r--r--   0        0        0     2033 2024-04-26 05:39:38.976723 vadi-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 18:58:47.327273 vadi-0.0.5/src/utils/__init__.py
--rw-r--r--   0        0        0      801 2024-04-26 05:38:55.976722 vadi-0.0.5/src/utils/console.py
--rw-r--r--   0        0        0      188 2024-04-08 16:57:12.949917 vadi-0.0.5/src/utils/constants.py
--rw-r--r--   0        0        0      239 2024-04-22 15:13:33.966777 vadi-0.0.5/src/utils/helpers.py
--rw-r--r--   0        0        0       57 2024-04-07 19:51:41.123190 vadi-0.0.5/src/utils/py.typed
--rw-r--r--   0        0        0        0 2024-04-07 18:58:17.517436 vadi-0.0.5/src/vadi/__init__.py
--rw-r--r--   0        0        0     3789 2024-04-22 15:12:06.623443 vadi-0.0.5/src/vadi/interpreter.py
--rw-r--r--   0        0        0     2066 2024-04-22 15:12:06.623443 vadi-0.0.5/src/vadi/lexer.py
--rw-r--r--   0        0        0      454 2024-04-22 15:12:06.623443 vadi-0.0.5/src/vadi/memory.py
--rw-r--r--   0        0        0     2997 2024-04-22 15:12:06.623443 vadi-0.0.5/src/vadi/parser.py
--rw-r--r--   0        0        0       57 2024-04-07 19:51:41.123190 vadi-0.0.5/src/vadi/py.typed
--rw-r--r--   0        0        0     1054 2024-04-26 05:18:47.546704 vadi-0.0.5/src/vadi/repl.py
--rw-r--r--   0        0        0      747 2024-04-08 03:01:51.703473 vadi-0.0.5/src/vadi/tokens.py
--rw-r--r--   0        0        0      484 2024-04-22 15:13:33.966777 vadi-0.0.5/src/vadi/typedef.py
--rw-r--r--   0        0        0     3696 1970-01-01 00:00:00.000000 vadi-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-26 07:07:22.684275 vadi-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2864 2024-04-26 07:07:22.684275 vadi-0.0.6/README.md
+-rw-r--r--   0        0        0     2033 2024-04-26 07:07:41.960305 vadi-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-26 07:07:22.688275 vadi-0.0.6/src/utils/__init__.py
+-rw-r--r--   0        0        0      801 2024-04-26 07:07:22.688275 vadi-0.0.6/src/utils/console.py
+-rw-r--r--   0        0        0      188 2024-04-26 07:07:22.688275 vadi-0.0.6/src/utils/constants.py
+-rw-r--r--   0        0        0      239 2024-04-26 07:07:22.688275 vadi-0.0.6/src/utils/helpers.py
+-rw-r--r--   0        0        0       57 2024-04-26 07:07:22.688275 vadi-0.0.6/src/utils/py.typed
+-rw-r--r--   0        0        0        0 2024-04-26 07:07:22.688275 vadi-0.0.6/src/vadi/__init__.py
+-rw-r--r--   0        0        0     3789 2024-04-26 07:07:22.688275 vadi-0.0.6/src/vadi/interpreter.py
+-rw-r--r--   0        0        0     2066 2024-04-26 07:07:22.688275 vadi-0.0.6/src/vadi/lexer.py
+-rw-r--r--   0        0        0      454 2024-04-26 07:07:22.688275 vadi-0.0.6/src/vadi/memory.py
+-rw-r--r--   0        0        0     2997 2024-04-26 07:07:22.688275 vadi-0.0.6/src/vadi/parser.py
+-rw-r--r--   0        0        0       57 2024-04-26 07:07:22.688275 vadi-0.0.6/src/vadi/py.typed
+-rw-r--r--   0        0        0     1054 2024-04-26 07:07:22.688275 vadi-0.0.6/src/vadi/repl.py
+-rw-r--r--   0        0        0      747 2024-04-26 07:07:22.688275 vadi-0.0.6/src/vadi/tokens.py
+-rw-r--r--   0        0        0      484 2024-04-26 07:07:22.688275 vadi-0.0.6/src/vadi/typedef.py
+-rw-r--r--   0        0        0     3696 1970-01-01 00:00:00.000000 vadi-0.0.6/PKG-INFO
```

### Comparing `vadi-0.0.5/LICENSE` & `vadi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vadi-0.0.5/README.md` & `vadi-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `vadi-0.0.5/pyproject.toml` & `vadi-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vadi"
-version = "0.0.5"
+version = "0.0.6"
 description = "REPL of a simple, interpreted and statically-typed programming language."
 authors = ["Shivam Shandilya <fvyogami@gmail.com>"]
 repository = "https://github.com/vyogami/Vadi"
 documentation = "https://github.com/vyogami/Vadi/blob/main/CONTRIBUTING.md"
 readme = "README.md"
 packages = [
   { include = "vadi", from = "src" },
```

### Comparing `vadi-0.0.5/src/utils/console.py` & `vadi-0.0.6/src/utils/console.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.5/src/vadi/interpreter.py` & `vadi-0.0.6/src/vadi/interpreter.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.5/src/vadi/lexer.py` & `vadi-0.0.6/src/vadi/lexer.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.5/src/vadi/parser.py` & `vadi-0.0.6/src/vadi/parser.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.5/src/vadi/repl.py` & `vadi-0.0.6/src/vadi/repl.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.5/src/vadi/tokens.py` & `vadi-0.0.6/src/vadi/tokens.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.5/PKG-INFO` & `vadi-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vadi
-Version: 0.0.5
+Version: 0.0.6
 Summary: REPL of a simple, interpreted and statically-typed programming language.
 Home-page: https://github.com/vyogami/Vadi
 Author: Shivam Shandilya
 Author-email: fvyogami@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

