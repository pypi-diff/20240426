# Comparing `tmp/pyfivetran-2024.3.5.1.tar.gz` & `tmp/pyfivetran-2024.4.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfivetran-2024.3.5.1.tar", max compression
+gzip compressed data, was "pyfivetran-2024.4.26.1.tar", max compression
```

## Comparing `pyfivetran-2024.3.5.1.tar` & `pyfivetran-2024.4.26.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       34 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/__init__.py
--rw-r--r--   0        0        0     2580 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/client.py
--rw-r--r--   0        0        0      663 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/endpoints/__init__.py
--rw-r--r--   0        0        0     2301 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/endpoints/base.py
--rw-r--r--   0        0        0     9563 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/endpoints/certificate.py
--rw-r--r--   0        0        0    12494 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/endpoints/connector.py
--rw-r--r--   0        0        0     7489 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/endpoints/destination.py
--rw-r--r--   0        0        0     7563 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/endpoints/group.py
--rw-r--r--   0        0        0     2992 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/endpoints/logs.py
--rw-r--r--   0        0        0     1059 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/endpoints/roles.py
--rw-r--r--   0        0        0     8780 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/endpoints/schema.py
--rw-r--r--   0        0        0     6136 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/endpoints/users.py
--rw-r--r--   0        0        0     3262 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/endpoints/webhook.py
--rw-r--r--   0        0        0      509 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/shed.py
--rw-r--r--   0        0        0     1224 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyfivetran/utils.py
--rw-r--r--   0        0        0     1124 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/pyproject.toml
--rw-r--r--   0        0        0     1454 2024-03-06 02:59:25.315733 pyfivetran-2024.3.5.1/readme.md
--rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 pyfivetran-2024.3.5.1/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/__init__.py
+-rw-r--r--   0        0        0     2580 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/client.py
+-rw-r--r--   0        0        0      663 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/endpoints/__init__.py
+-rw-r--r--   0        0        0     2301 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/endpoints/base.py
+-rw-r--r--   0        0        0     9563 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/endpoints/certificate.py
+-rw-r--r--   0        0        0    12494 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/endpoints/connector.py
+-rw-r--r--   0        0        0     7489 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/endpoints/destination.py
+-rw-r--r--   0        0        0     7563 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/endpoints/group.py
+-rw-r--r--   0        0        0     2992 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/endpoints/logs.py
+-rw-r--r--   0        0        0     1059 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/endpoints/roles.py
+-rw-r--r--   0        0        0     8780 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/endpoints/schema.py
+-rw-r--r--   0        0        0     6136 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/endpoints/users.py
+-rw-r--r--   0        0        0     3262 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/endpoints/webhook.py
+-rw-r--r--   0        0        0      509 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/shed.py
+-rw-r--r--   0        0        0     1224 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyfivetran/utils.py
+-rw-r--r--   0        0        0     1206 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/pyproject.toml
+-rw-r--r--   0        0        0     1454 2024-04-26 20:05:20.832343 pyfivetran-2024.4.26.1/readme.md
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 pyfivetran-2024.4.26.1/PKG-INFO
```

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/client.py` & `pyfivetran-2024.4.26.1/pyfivetran/client.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/endpoints/__init__.py` & `pyfivetran-2024.4.26.1/pyfivetran/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/endpoints/base.py` & `pyfivetran-2024.4.26.1/pyfivetran/endpoints/base.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/endpoints/certificate.py` & `pyfivetran-2024.4.26.1/pyfivetran/endpoints/certificate.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/endpoints/connector.py` & `pyfivetran-2024.4.26.1/pyfivetran/endpoints/connector.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/endpoints/destination.py` & `pyfivetran-2024.4.26.1/pyfivetran/endpoints/destination.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/endpoints/group.py` & `pyfivetran-2024.4.26.1/pyfivetran/endpoints/group.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/endpoints/logs.py` & `pyfivetran-2024.4.26.1/pyfivetran/endpoints/logs.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/endpoints/roles.py` & `pyfivetran-2024.4.26.1/pyfivetran/endpoints/roles.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/endpoints/schema.py` & `pyfivetran-2024.4.26.1/pyfivetran/endpoints/schema.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/endpoints/users.py` & `pyfivetran-2024.4.26.1/pyfivetran/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/endpoints/webhook.py` & `pyfivetran-2024.4.26.1/pyfivetran/endpoints/webhook.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyfivetran/utils.py` & `pyfivetran-2024.4.26.1/pyfivetran/utils.py`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/pyproject.toml` & `pyfivetran-2024.4.26.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [tool.poetry]
 name = "pyfivetran"
-version = "2024.03.05.01"
+version = "2024.04.26.01"
 description = "Pythonic interface to the fivetran API"
 authors = ["Khari Gardner <kharigardner@protonmail.com>"]
 license = "MIT"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = "^3.8, <3.12"
 httpx = "^0.25.1"
 lazy = "^1.6"
 pytz = "^2024.1"
 python-dateutil = "^2.9.0.post0"
 
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.docs]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 mypy = "^1.7.0"
 ruff = "^0.1.6"
 pre-commit = "^3.5.0"
 pytest-mock = "^3.12.0"
```

### Comparing `pyfivetran-2024.3.5.1/readme.md` & `pyfivetran-2024.4.26.1/readme.md`

 * *Files identical despite different names*

### Comparing `pyfivetran-2024.3.5.1/PKG-INFO` & `pyfivetran-2024.4.26.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfivetran
-Version: 2024.3.5.1
+Version: 2024.4.26.1
 Summary: Pythonic interface to the fivetran API
 License: MIT
 Author: Khari Gardner
 Author-email: kharigardner@protonmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

