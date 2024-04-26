# Comparing `tmp/mkdocs_autoapi-0.1.2.tar.gz` & `tmp/mkdocs_autoapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mkdocs_autoapi-0.1.2.tar", last modified: Fri Apr 26 19:42:51 2024, max compression
+gzip compressed data, was "dist\mkdocs_autoapi-0.1.3.tar", last modified: Fri Apr 26 19:45:30 2024, max compression
```

## Comparing `mkdocs_autoapi-0.1.2.tar` & `mkdocs_autoapi-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 19:42:51.387610 mkdocs_autoapi-0.1.2/
--rw-rw-rw-   0        0        0     1087 2024-04-24 18:09:42.000000 mkdocs_autoapi-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      809 2024-04-26 19:42:51.386610 mkdocs_autoapi-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-26 19:42:51.366605 mkdocs_autoapi-0.1.2/mkdocs_autoapi/
--rw-rw-rw-   0        0        0      129 2024-04-25 15:57:28.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/__init__.py
--rw-rw-rw-   0        0        0     4623 2024-04-25 21:10:53.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/autoapi.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:42:51.379608 mkdocs_autoapi-0.1.2/mkdocs_autoapi/generate_files/
--rw-rw-rw-   0        0        0      246 2024-04-25 16:00:19.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/generate_files/__init__.py
--rw-rw-rw-   0        0        0     4734 2024-04-25 19:48:07.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/generate_files/editor.py
--rw-rw-rw-   0        0        0     4233 2024-04-25 20:24:30.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/generate_files/nav.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:42:51.382609 mkdocs_autoapi-0.1.2/mkdocs_autoapi/literate_nav/
--rw-rw-rw-   0        0        0      127 2024-04-25 15:18:25.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/literate_nav/__init__.py
--rw-rw-rw-   0        0        0       82 2024-04-25 22:36:44.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/literate_nav/exceptions.py
--rw-rw-rw-   0        0        0     1989 2024-04-25 22:25:22.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/literate_nav/globber.py
--rw-rw-rw-   0        0        0    12458 2024-04-26 02:29:25.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/literate_nav/parser.py
--rw-rw-rw-   0        0        0     2121 2024-04-26 02:48:59.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/literate_nav/resolve.py
--rw-rw-rw-   0        0        0     5864 2024-04-26 18:55:38.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/plugin.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:42:51.385609 mkdocs_autoapi-0.1.2/mkdocs_autoapi/section_index/
--rw-rw-rw-   0        0        0      128 2024-04-26 18:43:21.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/section_index/__init__.py
--rw-rw-rw-   0        0        0     5288 2024-04-26 18:49:20.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/section_index/rewrite.py
--rw-rw-rw-   0        0        0      902 2024-04-26 18:55:38.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi/section_index/section_page.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:42:51.386610 mkdocs_autoapi-0.1.2/mkdocs_autoapi.egg-info/
--rw-rw-rw-   0        0        0      809 2024-04-26 19:42:51.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      767 2024-04-26 19:42:51.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 19:42:51.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-26 19:42:51.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2024-04-26 19:42:51.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-26 19:42:51.000000 mkdocs_autoapi-0.1.2/mkdocs_autoapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 19:42:51.387610 mkdocs_autoapi-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1172 2024-04-26 19:42:38.000000 mkdocs_autoapi-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 19:45:30.461482 mkdocs_autoapi-0.1.3/
+-rw-rw-rw-   0        0        0     1087 2024-04-24 18:09:42.000000 mkdocs_autoapi-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      809 2024-04-26 19:45:30.460481 mkdocs_autoapi-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 19:45:30.439477 mkdocs_autoapi-0.1.3/mkdocs_autoapi/
+-rw-rw-rw-   0        0        0      129 2024-04-25 15:57:28.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/__init__.py
+-rw-rw-rw-   0        0        0     4623 2024-04-25 21:10:53.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/autoapi.py
+drwxrwxrwx   0        0        0        0 2024-04-26 19:45:30.453480 mkdocs_autoapi-0.1.3/mkdocs_autoapi/generate_files/
+-rw-rw-rw-   0        0        0      246 2024-04-25 16:00:19.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/generate_files/__init__.py
+-rw-rw-rw-   0        0        0     4734 2024-04-25 19:48:07.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/generate_files/editor.py
+-rw-rw-rw-   0        0        0     4233 2024-04-25 20:24:30.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/generate_files/nav.py
+drwxrwxrwx   0        0        0        0 2024-04-26 19:45:30.457481 mkdocs_autoapi-0.1.3/mkdocs_autoapi/literate_nav/
+-rw-rw-rw-   0        0        0      127 2024-04-25 15:18:25.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/literate_nav/__init__.py
+-rw-rw-rw-   0        0        0       82 2024-04-25 22:36:44.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/literate_nav/exceptions.py
+-rw-rw-rw-   0        0        0     1989 2024-04-25 22:25:22.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/literate_nav/globber.py
+-rw-rw-rw-   0        0        0    12458 2024-04-26 02:29:25.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/literate_nav/parser.py
+-rw-rw-rw-   0        0        0     2121 2024-04-26 02:48:59.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/literate_nav/resolve.py
+-rw-rw-rw-   0        0        0     5837 2024-04-26 19:45:08.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/plugin.py
+drwxrwxrwx   0        0        0        0 2024-04-26 19:45:30.459481 mkdocs_autoapi-0.1.3/mkdocs_autoapi/section_index/
+-rw-rw-rw-   0        0        0      128 2024-04-26 18:43:21.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/section_index/__init__.py
+-rw-rw-rw-   0        0        0     5288 2024-04-26 18:49:20.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/section_index/rewrite.py
+-rw-rw-rw-   0        0        0      902 2024-04-26 18:55:38.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi/section_index/section_page.py
+drwxrwxrwx   0        0        0        0 2024-04-26 19:45:30.460481 mkdocs_autoapi-0.1.3/mkdocs_autoapi.egg-info/
+-rw-rw-rw-   0        0        0      809 2024-04-26 19:45:30.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2024-04-26 19:45:30.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 19:45:30.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-26 19:45:30.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2024-04-26 19:45:30.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-26 19:45:30.000000 mkdocs_autoapi-0.1.3/mkdocs_autoapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 19:45:30.461482 mkdocs_autoapi-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1172 2024-04-26 19:45:19.000000 mkdocs_autoapi-0.1.3/setup.py
```

### Comparing `mkdocs_autoapi-0.1.2/LICENSE` & `mkdocs_autoapi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_autoapi-0.1.2/PKG-INFO` & `mkdocs_autoapi-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-autoapi
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/jcayers20/django-postgres-loader
 Download-URL: https://github.com/jcayers20/django-postgres-loader/archive/refs/tags/0.1.2.tar.gz
 Author: Jacob Ayers
 Author-email: jcayers20@gmail.com
 License: MIT
 Keywords: MkDocs,AutoAPI
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mkdocs_autoapi-0.1.2/mkdocs_autoapi/autoapi.py` & `mkdocs_autoapi-0.1.3/mkdocs_autoapi/autoapi.py`

 * *Files identical despite different names*

### Comparing `mkdocs_autoapi-0.1.2/mkdocs_autoapi/generate_files/editor.py` & `mkdocs_autoapi-0.1.3/mkdocs_autoapi/generate_files/editor.py`

 * *Files identical despite different names*

### Comparing `mkdocs_autoapi-0.1.2/mkdocs_autoapi/generate_files/nav.py` & `mkdocs_autoapi-0.1.3/mkdocs_autoapi/generate_files/nav.py`

 * *Files identical despite different names*

### Comparing `mkdocs_autoapi-0.1.2/mkdocs_autoapi/literate_nav/globber.py` & `mkdocs_autoapi-0.1.3/mkdocs_autoapi/literate_nav/globber.py`

 * *Files identical despite different names*

### Comparing `mkdocs_autoapi-0.1.2/mkdocs_autoapi/literate_nav/parser.py` & `mkdocs_autoapi-0.1.3/mkdocs_autoapi/literate_nav/parser.py`

 * *Files identical despite different names*

### Comparing `mkdocs_autoapi-0.1.2/mkdocs_autoapi/literate_nav/resolve.py` & `mkdocs_autoapi-0.1.3/mkdocs_autoapi/literate_nav/resolve.py`

 * *Files identical despite different names*

### Comparing `mkdocs_autoapi-0.1.2/mkdocs_autoapi/plugin.py` & `mkdocs_autoapi-0.1.3/mkdocs_autoapi/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 
         Returns:
             The updated MkDocs files object.
         """
         # Step 1
         self._dir = tempfile.TemporaryDirectory(
             prefix="autoapi",
-            delete=False,
         )
 
         # Step 2
         exclude = self.config.exclude.copy()
         if "venv/**/*.py" not in self.config.exclude:
             exclude.append("**/venv/**/*.py")
```

### Comparing `mkdocs_autoapi-0.1.2/mkdocs_autoapi/section_index/rewrite.py` & `mkdocs_autoapi-0.1.3/mkdocs_autoapi/section_index/rewrite.py`

 * *Files identical despite different names*

### Comparing `mkdocs_autoapi-0.1.2/mkdocs_autoapi/section_index/section_page.py` & `mkdocs_autoapi-0.1.3/mkdocs_autoapi/section_index/section_page.py`

 * *Files identical despite different names*

### Comparing `mkdocs_autoapi-0.1.2/mkdocs_autoapi.egg-info/PKG-INFO` & `mkdocs_autoapi-0.1.3/mkdocs_autoapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-autoapi
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/jcayers20/django-postgres-loader
 Download-URL: https://github.com/jcayers20/django-postgres-loader/archive/refs/tags/0.1.2.tar.gz
 Author: Jacob Ayers
 Author-email: jcayers20@gmail.com
 License: MIT
 Keywords: MkDocs,AutoAPI
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mkdocs_autoapi-0.1.2/mkdocs_autoapi.egg-info/SOURCES.txt` & `mkdocs_autoapi-0.1.3/mkdocs_autoapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_autoapi-0.1.2/setup.py` & `mkdocs_autoapi-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Package configuration details."""
 
 # built-in imports
 from setuptools import setup, find_packages
 
 setup(
     name="mkdocs-autoapi",
-    version="0.1.2",
+    version="0.1.3",
     license="MIT",
     author="Jacob Ayers",
     author_email="jcayers20@gmail.com",
     url="https://github.com/jcayers20/django-postgres-loader",
     download_url="https://github.com/jcayers20/django-postgres-loader/archive/refs/tags/0.1.2.tar.gz",
     packages=find_packages(),
     keywords=["MkDocs", "AutoAPI"],
```

