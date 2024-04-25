# Comparing `tmp/onstats-0.9.1.tar.gz` & `tmp/onstats-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onstats-0.9.1.tar", max compression
+gzip compressed data, was "onstats-0.9.2.tar", max compression
```

## Comparing `onstats-0.9.1.tar` & `onstats-0.9.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      455 2024-04-25 21:25:25.136066 onstats-0.9.1/README.md
--rw-r--r--   0        0        0        0 2024-04-25 18:47:55.240859 onstats-0.9.1/onstats/__init__.py
--rw-r--r--   0        0        0     7464 2024-04-25 21:37:14.634127 onstats-0.9.1/onstats/stats.py
--rw-r--r--   0        0        0     1381 2024-04-25 21:35:59.433892 onstats-0.9.1/onstats/util.py
--rw-r--r--   0        0        0      751 2024-04-25 22:09:47.161954 onstats-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 onstats-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      921 2024-04-25 22:15:54.211990 onstats-0.9.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 18:47:55.240859 onstats-0.9.2/onstats/__init__.py
+-rw-r--r--   0        0        0     7464 2024-04-25 21:37:14.634127 onstats-0.9.2/onstats/stats.py
+-rw-r--r--   0        0        0     1381 2024-04-25 21:35:59.433892 onstats-0.9.2/onstats/util.py
+-rw-r--r--   0        0        0      751 2024-04-25 22:16:28.560293 onstats-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 onstats-0.9.2/PKG-INFO
```

### Comparing `onstats-0.9.1/onstats/stats.py` & `onstats-0.9.2/onstats/stats.py`

 * *Files identical despite different names*

### Comparing `onstats-0.9.1/onstats/util.py` & `onstats-0.9.2/onstats/util.py`

 * *Files identical despite different names*

### Comparing `onstats-0.9.1/pyproject.toml` & `onstats-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onstats"
-version = "0.9.1"
+version = "0.9.2"
 description = "Online stats in python, based in generators with send"
 authors = ["Pablo Ruiz <pablo.r.c@live.com>"]
 readme = "README.md"
 repository = "https://github.com/PabloRuizCuevas/onstats"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

