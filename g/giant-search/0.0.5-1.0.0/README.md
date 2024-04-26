# Comparing `tmp/giant_search-0.0.5.tar.gz` & `tmp/giant_search-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant_search-0.0.5.tar", max compression
+gzip compressed data, was "giant_search-1.0.0.tar", max compression
```

## Comparing `giant_search-0.0.5.tar` & `giant_search-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5504 2024-03-13 10:08:37.327474 giant_search-0.0.5/README.md
--rw-r--r--   0        0        0        0 2024-03-13 08:44:36.496013 giant_search-0.0.5/giant_search/__init__.py
--rw-r--r--   0        0        0     3869 2024-03-13 08:44:36.496013 giant_search-0.0.5/giant_search/adapter.py
--rw-r--r--   0        0        0     1238 2024-03-13 08:44:36.496013 giant_search-0.0.5/giant_search/apps.py
--rw-r--r--   0        0        0     2547 2024-03-13 08:44:36.496013 giant_search-0.0.5/giant_search/mixins.py
--rw-r--r--   0        0        0     1882 2024-03-13 09:49:37.727359 giant_search-0.0.5/giant_search/templates/search/results.html
--rw-r--r--   0        0        0        0 2024-03-13 08:44:36.496013 giant_search-0.0.5/giant_search/tests/__init__.py
--rw-r--r--   0        0        0      625 2024-03-13 08:44:36.496013 giant_search-0.0.5/giant_search/tests/test_views.py
--rw-r--r--   0        0        0      163 2024-03-13 08:44:36.496013 giant_search-0.0.5/giant_search/urls.py
--rw-r--r--   0        0        0     1569 2024-03-13 08:44:36.496013 giant_search-0.0.5/giant_search/utils.py
--rw-r--r--   0        0        0      446 2024-03-13 09:57:53.035334 giant_search-0.0.5/giant_search/views.py
--rw-r--r--   0        0        0      560 2024-03-13 10:03:45.754714 giant_search-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     6271 1970-01-01 00:00:00.000000 giant_search-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     5504 2024-04-26 10:14:43.292369 giant_search-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-23 10:04:44.268895 giant_search-1.0.0/giant_search/__init__.py
+-rw-r--r--   0        0        0     3869 2024-03-06 12:35:03.635806 giant_search-1.0.0/giant_search/adapter.py
+-rw-r--r--   0        0        0     1238 2024-02-23 10:04:44.268895 giant_search-1.0.0/giant_search/apps.py
+-rw-r--r--   0        0        0     2547 2024-03-06 10:03:08.429780 giant_search-1.0.0/giant_search/mixins.py
+-rw-r--r--   0        0        0     1882 2024-04-26 10:14:43.293368 giant_search-1.0.0/giant_search/templates/search/results.html
+-rw-r--r--   0        0        0        0 2024-02-23 10:04:44.269894 giant_search-1.0.0/giant_search/tests/__init__.py
+-rw-r--r--   0        0        0      625 2024-03-01 11:46:42.917097 giant_search-1.0.0/giant_search/tests/test_views.py
+-rw-r--r--   0        0        0      163 2024-02-23 10:04:44.269894 giant_search-1.0.0/giant_search/urls.py
+-rw-r--r--   0        0        0     1569 2024-03-04 11:41:57.520249 giant_search-1.0.0/giant_search/utils.py
+-rw-r--r--   0        0        0      446 2024-04-26 10:14:43.293368 giant_search-1.0.0/giant_search/views.py
+-rw-r--r--   0        0        0      560 2024-04-26 10:24:29.159262 giant_search-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6322 1970-01-01 00:00:00.000000 giant_search-1.0.0/PKG-INFO
```

### Comparing `giant_search-0.0.5/README.md` & `giant_search-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `giant_search-0.0.5/giant_search/adapter.py` & `giant_search-1.0.0/giant_search/adapter.py`

 * *Files identical despite different names*

### Comparing `giant_search-0.0.5/giant_search/apps.py` & `giant_search-1.0.0/giant_search/apps.py`

 * *Files identical despite different names*

### Comparing `giant_search-0.0.5/giant_search/mixins.py` & `giant_search-1.0.0/giant_search/mixins.py`

 * *Files identical despite different names*

### Comparing `giant_search-0.0.5/giant_search/templates/search/results.html` & `giant_search-1.0.0/giant_search/templates/search/results.html`

 * *Files identical despite different names*

### Comparing `giant_search-0.0.5/giant_search/tests/test_views.py` & `giant_search-1.0.0/giant_search/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `giant_search-0.0.5/giant_search/utils.py` & `giant_search-1.0.0/giant_search/utils.py`

 * *Files identical despite different names*

### Comparing `giant_search-0.0.5/pyproject.toml` & `giant_search-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-search"
-version = "0.0.5"
+version = "1.0.0"
 description = "Provides a nice abstraction layer on top of the django-watson search library."
 authors = ["Scott Pashley <scott.pashley@giantdigital.co.uk>"]
 readme = "README.md"
 packages = [{ include = "giant_search" }]
 license = "MIT"
 homepage = "https://www.giantdigital.co.uk"
```

### Comparing `giant_search-0.0.5/PKG-INFO` & `giant_search-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: giant-search
-Version: 0.0.5
+Version: 1.0.0
 Summary: Provides a nice abstraction layer on top of the django-watson search library.
 Home-page: https://www.giantdigital.co.uk
 License: MIT
 Author: Scott Pashley
 Author-email: scott.pashley@giantdigital.co.uk
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django-cms (<4.0)
 Requires-Dist: django-watson (>=1.6.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Giant Search
 
 This library provides a nice abstraction layer on top of the `django-watson` search library. It allows developers to
```

