# Comparing `tmp/markdown_convert-1.1.3.tar.gz` & `tmp/markdown_convert-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-1.1.3.tar", max compression
+gzip compressed data, was "markdown_convert-1.1.4.tar", max compression
```

## Comparing `markdown_convert-1.1.3.tar` & `markdown_convert-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.1.3/LICENSE
--rw-r--r--   0        0        0     2452 2024-04-18 14:09:49.066892 markdown_convert-1.1.3/README.md
--rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.1.3/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.1.3/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.1.3/markdown_convert/code.css
--rw-r--r--   0        0        0     5344 2024-04-10 06:55:23.607495 markdown_convert-1.1.3/markdown_convert/default.css
--rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.1.3/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.1.3/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     5711 2024-04-16 12:03:21.481233 markdown_convert-1.1.3/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.1.3/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.1.3/markdown_convert/modules/utils.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.1.3/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      680 2024-04-18 14:09:53.383079 markdown_convert-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 markdown_convert-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2452 2024-04-18 14:09:49.066892 markdown_convert-1.1.4/README.md
+-rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.1.4/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.1.4/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.1.4/markdown_convert/code.css
+-rw-r--r--   0        0        0     5585 2024-04-26 13:21:52.381584 markdown_convert-1.1.4/markdown_convert/default.css
+-rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.1.4/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.1.4/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     5711 2024-04-16 12:03:21.481233 markdown_convert-1.1.4/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.1.4/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.1.4/markdown_convert/modules/utils.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.1.4/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      680 2024-04-26 13:24:49.922502 markdown_convert-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 markdown_convert-1.1.4/PKG-INFO
```

### Comparing `markdown_convert-1.1.3/LICENSE` & `markdown_convert-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.3/README.md` & `markdown_convert-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.3/markdown_convert/__main__.py` & `markdown_convert-1.1.4/markdown_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.3/markdown_convert/code.css` & `markdown_convert-1.1.4/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.3/markdown_convert/default.css` & `markdown_convert-1.1.4/markdown_convert/default.css`

 * *Files 24% similar despite different names*

```diff
@@ -94,45 +94,56 @@
 
 /* Print media css */
 @page {
   size: A4;
   margin: 2.54cm;
 }
 
+:root {
+  --top-margin: 1em;
+  --bottom-margin: 0;
+  --left-margin: 1.5em;
+
+  --top-margin-small: 0;
+  --left-margin-small: 1em;
+
+  --bottom-margin-big: 0.5em;
+  --left-margin-big: 2em;
+}
+
 /* Document structure */
 body {
-  margin: 0 0 0 0;
-  padding: 0 0 0 0;
+  margin: 0;
+  padding: 0;
   font-family: "Cantarell Web", sans-serif;
   color: #333;
-  line-height: 1;
 }
 
 /* Headers and paragraphs */
 h1,
 h2,
 h3,
 h4,
 h5 {
   color: #333;
   font-weight: 400;
 }
 
 h1 {
-  margin-top: 0;
-  margin-bottom: 0.5em;
+  margin-top: var(--top-margin-small);
+  margin-bottom: var(--bottom-margin-big);
 }
 
 h2,
 h3,
 h4,
 h5,
 p {
-  margin-top: 1em;
-  margin-bottom: 0;
+  margin-top: var(--top-margin);
+  margin-bottom: var(--bottom-margin);
 }
 
 h1 {
   font-size: 48px;
 }
 
 h2 {
@@ -149,57 +160,44 @@
 
 h5 {
   font-size: 14px;
 }
 
 p {
   font-size: 12px;
-  line-height: 1.5em;
 }
 
 /* Links */
 a {
   color: #09f;
   margin: 0;
   vertical-align: baseline;
 }
 
 /* Lists */
 ul,
 ol {
   font-size: 12px;
-  line-height: 1.5em;
-  margin: 1em 0 0 1.5em;
   padding: 0;
-}
-
-li > ul,
-li > ol {
-  margin-top: 0;
-}
-
-li {
-  line-height: 1.5em;
-}
-
-li ul {
-  margin-left: 1.5em;
+  margin-top: var(--top-margin);
+  margin-right: 0;
+  margin-bottom: var(--bottom-margin);
+  margin-left: var(--left-margin-big);
 }
 
 /* Code blocks */
 pre {
-  padding: 0 2em;
+  padding: 0;
   white-space: pre-wrap;
 }
 
 code {
   font-family: "JetBrains Mono", "Courier New", Courier, monospace;
   font-size: 10px;
   background-color: #eee;
-  line-height: 1.5em;
   padding-left: 0.4em;
   padding-right: 0.4em;
   display: inline-block;
   border-radius: 0.3em;
 }
 
 h1 code,
@@ -208,38 +206,38 @@
 h4 code,
 h5 code {
   font-size: 0.8em; /* Adjust the font size as needed */
 }
 
 /* Quotes */
 blockquote {
-  margin-top: 1em;
-  margin-left: 2em;
+  margin-top: var(--top-margin);
+  margin-left: var(--left-margin);
   max-width: 30em;
   border-left: 4px solid #ccc;
   padding-left: 0.5em;
   color: #666;
 }
 
 blockquote > blockquote {
-  margin-left: 1em;
+  margin-left: var(--left-margin-small);
 }
 
 /* Figures */
 img {
   display: block;
   margin: 2em auto;
   max-width: 80%;
 }
 
 /* Tables */
 table {
   font-size: 10px;
   border-collapse: collapse;
-  margin-top: 1em;
+  margin-top: var(--top-margin);
   text-align: left;
   table-layout: auto;
 }
 
 thead {
   background-color: #eee;
 }
@@ -252,19 +250,19 @@
 td {
   padding: 0.5em 0.75em;
   border: 1px solid #ccc;
   white-space: nowrap;
 }
 
 col {
-  width: auto !important;
+  width: auto;
 }
 
 /* Page breaks */
 .pagebreak {
   clear: both;
   page-break-after: always;
 }
 
 .pagebreak + * {
-  margin-top: 0;
+  margin-top: var(--top-margin-small);
 }
```

### Comparing `markdown_convert-1.1.3/markdown_convert/modules/convert.py` & `markdown_convert-1.1.4/markdown_convert/modules/convert.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.3/markdown_convert/modules/resources.py` & `markdown_convert-1.1.4/markdown_convert/modules/resources.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.3/markdown_convert/modules/utils.py` & `markdown_convert-1.1.4/markdown_convert/modules/utils.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.3/markdown_convert/modules/validate.py` & `markdown_convert-1.1.4/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.3/pyproject.toml` & `markdown_convert-1.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "1.1.3"
+version = "1.1.4"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
```

### Comparing `markdown_convert-1.1.3/PKG-INFO` & `markdown_convert-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 1.1.3
+Version: 1.1.4
 Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

