# Comparing `tmp/vadi-0.0.4.tar.gz` & `tmp/vadi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vadi-0.0.4.tar", max compression
+gzip compressed data, was "vadi-0.0.5.tar", max compression
```

## Comparing `vadi-0.0.4.tar` & `vadi-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1074 2024-04-07 18:58:17.517436 vadi-0.0.4/LICENSE
--rw-r--r--   0        0        0     2864 2024-04-23 10:07:30.746937 vadi-0.0.4/README.md
--rw-r--r--   0        0        0     2006 2024-04-23 10:08:09.846938 vadi-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 18:58:47.327273 vadi-0.0.4/src/utils/__init__.py
--rw-r--r--   0        0        0      430 2024-04-22 15:10:35.660108 vadi-0.0.4/src/utils/console.py
--rw-r--r--   0        0        0      188 2024-04-08 16:57:12.949917 vadi-0.0.4/src/utils/constants.py
--rw-r--r--   0        0        0      239 2024-04-22 15:13:33.966777 vadi-0.0.4/src/utils/helpers.py
--rw-r--r--   0        0        0       57 2024-04-07 19:51:41.123190 vadi-0.0.4/src/utils/py.typed
--rw-r--r--   0        0        0        0 2024-04-07 18:58:17.517436 vadi-0.0.4/src/vadi/__init__.py
--rw-r--r--   0        0        0     3789 2024-04-22 15:12:06.623443 vadi-0.0.4/src/vadi/interpreter.py
--rw-r--r--   0        0        0     2066 2024-04-22 15:12:06.623443 vadi-0.0.4/src/vadi/lexer.py
--rw-r--r--   0        0        0      454 2024-04-22 15:12:06.623443 vadi-0.0.4/src/vadi/memory.py
--rw-r--r--   0        0        0     2997 2024-04-22 15:12:06.623443 vadi-0.0.4/src/vadi/parser.py
--rw-r--r--   0        0        0       57 2024-04-07 19:51:41.123190 vadi-0.0.4/src/vadi/py.typed
--rw-r--r--   0        0        0     1054 2024-04-22 15:10:35.660108 vadi-0.0.4/src/vadi/repl.py
--rw-r--r--   0        0        0      747 2024-04-08 03:01:51.703473 vadi-0.0.4/src/vadi/tokens.py
--rw-r--r--   0        0        0      484 2024-04-22 15:13:33.966777 vadi-0.0.4/src/vadi/typedef.py
--rw-r--r--   0        0        0     3648 1970-01-01 00:00:00.000000 vadi-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-07 18:58:17.517436 vadi-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2864 2024-04-23 10:07:30.746937 vadi-0.0.5/README.md
+-rw-r--r--   0        0        0     2033 2024-04-26 05:39:38.976723 vadi-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 18:58:47.327273 vadi-0.0.5/src/utils/__init__.py
+-rw-r--r--   0        0        0      801 2024-04-26 05:38:55.976722 vadi-0.0.5/src/utils/console.py
+-rw-r--r--   0        0        0      188 2024-04-08 16:57:12.949917 vadi-0.0.5/src/utils/constants.py
+-rw-r--r--   0        0        0      239 2024-04-22 15:13:33.966777 vadi-0.0.5/src/utils/helpers.py
+-rw-r--r--   0        0        0       57 2024-04-07 19:51:41.123190 vadi-0.0.5/src/utils/py.typed
+-rw-r--r--   0        0        0        0 2024-04-07 18:58:17.517436 vadi-0.0.5/src/vadi/__init__.py
+-rw-r--r--   0        0        0     3789 2024-04-22 15:12:06.623443 vadi-0.0.5/src/vadi/interpreter.py
+-rw-r--r--   0        0        0     2066 2024-04-22 15:12:06.623443 vadi-0.0.5/src/vadi/lexer.py
+-rw-r--r--   0        0        0      454 2024-04-22 15:12:06.623443 vadi-0.0.5/src/vadi/memory.py
+-rw-r--r--   0        0        0     2997 2024-04-22 15:12:06.623443 vadi-0.0.5/src/vadi/parser.py
+-rw-r--r--   0        0        0       57 2024-04-07 19:51:41.123190 vadi-0.0.5/src/vadi/py.typed
+-rw-r--r--   0        0        0     1054 2024-04-26 05:18:47.546704 vadi-0.0.5/src/vadi/repl.py
+-rw-r--r--   0        0        0      747 2024-04-08 03:01:51.703473 vadi-0.0.5/src/vadi/tokens.py
+-rw-r--r--   0        0        0      484 2024-04-22 15:13:33.966777 vadi-0.0.5/src/vadi/typedef.py
+-rw-r--r--   0        0        0     3696 1970-01-01 00:00:00.000000 vadi-0.0.5/PKG-INFO
```

### Comparing `vadi-0.0.4/LICENSE` & `vadi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vadi-0.0.4/README.md` & `vadi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `vadi-0.0.4/pyproject.toml` & `vadi-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vadi"
-version = "0.0.4"
+version = "0.0.5"
 description = "REPL of a simple, interpreted and statically-typed programming language."
 authors = ["Shivam Shandilya <fvyogami@gmail.com>"]
 repository = "https://github.com/vyogami/Vadi"
 documentation = "https://github.com/vyogami/Vadi/blob/main/CONTRIBUTING.md"
 readme = "README.md"
 packages = [
   { include = "vadi", from = "src" },
@@ -12,14 +12,15 @@
   { include = "utils", from = "src" },
   { include = "utils/py.typed", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 rich = "^13.7.1"
+prompt-toolkit = "^3.0.43"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.12.0"
 mypy = "^1.5.1"
 pre-commit = "^3.4.0"
```

### Comparing `vadi-0.0.4/src/vadi/interpreter.py` & `vadi-0.0.5/src/vadi/interpreter.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.4/src/vadi/lexer.py` & `vadi-0.0.5/src/vadi/lexer.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.4/src/vadi/parser.py` & `vadi-0.0.5/src/vadi/parser.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.4/src/vadi/repl.py` & `vadi-0.0.5/src/vadi/repl.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.4/src/vadi/tokens.py` & `vadi-0.0.5/src/vadi/tokens.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.4/PKG-INFO` & `vadi-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: vadi
-Version: 0.0.4
+Version: 0.0.5
 Summary: REPL of a simple, interpreted and statically-typed programming language.
 Home-page: https://github.com/vyogami/Vadi
 Author: Shivam Shandilya
 Author-email: fvyogami@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Project-URL: Documentation, https://github.com/vyogami/Vadi/blob/main/CONTRIBUTING.md
 Project-URL: Repository, https://github.com/vyogami/Vadi
 Description-Content-Type: text/markdown
 
 ![Banner](https://raw.githubusercontent.com/Vyogami/Vadi/main/assets/banner.png)
```

