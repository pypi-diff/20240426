# Comparing `tmp/onstats-0.9.0.tar.gz` & `tmp/onstats-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onstats-0.9.0.tar", max compression
+gzip compressed data, was "onstats-0.9.1.tar", max compression
```

## Comparing `onstats-0.9.0.tar` & `onstats-0.9.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      455 2024-04-25 21:25:25.136066 onstats-0.9.0/README.md
--rw-r--r--   0        0        0        0 2024-04-25 18:47:55.240859 onstats-0.9.0/onstats/__init__.py
--rw-r--r--   0        0        0     7464 2024-04-25 21:37:14.634127 onstats-0.9.0/onstats/stats.py
--rw-r--r--   0        0        0     1381 2024-04-25 21:35:59.433892 onstats-0.9.0/onstats/util.py
--rw-r--r--   0        0        0      693 2024-04-25 21:40:26.330821 onstats-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 onstats-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      455 2024-04-25 21:25:25.136066 onstats-0.9.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 18:47:55.240859 onstats-0.9.1/onstats/__init__.py
+-rw-r--r--   0        0        0     7464 2024-04-25 21:37:14.634127 onstats-0.9.1/onstats/stats.py
+-rw-r--r--   0        0        0     1381 2024-04-25 21:35:59.433892 onstats-0.9.1/onstats/util.py
+-rw-r--r--   0        0        0      751 2024-04-25 22:09:47.161954 onstats-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 onstats-0.9.1/PKG-INFO
```

### Comparing `onstats-0.9.0/onstats/stats.py` & `onstats-0.9.1/onstats/stats.py`

 * *Files identical despite different names*

### Comparing `onstats-0.9.0/onstats/util.py` & `onstats-0.9.1/onstats/util.py`

 * *Files identical despite different names*

### Comparing `onstats-0.9.0/pyproject.toml` & `onstats-0.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "onstats"
-version = "0.9.0"
+version = "0.9.1"
 description = "Online stats in python, based in generators with send"
 authors = ["Pablo Ruiz <pablo.r.c@live.com>"]
 readme = "README.md"
+repository = "https://github.com/PabloRuizCuevas/onstats"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.26.4"
 genbadge = "^1.1.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `onstats-0.9.0/PKG-INFO` & `onstats-0.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: onstats
-Version: 0.9.0
+Version: 0.9.1
 Summary: Online stats in python, based in generators with send
+Home-page: https://github.com/PabloRuizCuevas/onstats
 Author: Pablo Ruiz
 Author-email: pablo.r.c@live.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: genbadge (>=1.1.1,<2.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Project-URL: Repository, https://github.com/PabloRuizCuevas/onstats
 Description-Content-Type: text/markdown
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Tests Status](./reports/coverage/coverage-badge.svg?dummy=8484744)](./reports/junit/report.html)
 
 ## Generators Based Online Statistics
```

