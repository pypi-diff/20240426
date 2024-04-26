# Comparing `tmp/md2weasypdf-0.0.7.tar.gz` & `tmp/md2weasypdf-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2weasypdf-0.0.7.tar", last modified: Thu Apr 25 09:41:19 2024, max compression
+gzip compressed data, was "md2weasypdf-0.0.8.tar", last modified: Thu Apr 25 13:40:05 2024, max compression
```

## Comparing `md2weasypdf-0.0.7.tar` & `md2weasypdf-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:19.689788 md2weasypdf-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 09:41:19.689788 md2weasypdf-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:19.685788 md2weasypdf-0.0.7/md2weasypdf/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:19.689788 md2weasypdf-0.0.7/md2weasypdf/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/footnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/textbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/toa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/toc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:19.689788 md2weasypdf-0.0.7/md2weasypdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-25 09:41:19.689788 md2weasypdf-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:40:05.392287 md2weasypdf-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 13:40:05.392287 md2weasypdf-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:40:05.388287 md2weasypdf-0.0.8/md2weasypdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:40:05.392287 md2weasypdf-0.0.8/md2weasypdf/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/toa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/toc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:40:05.392287 md2weasypdf-0.0.8/md2weasypdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-25 13:40:05.392287 md2weasypdf-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/setup.py
```

### Comparing `md2weasypdf-0.0.7/LICENSE` & `md2weasypdf-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.7/PKG-INFO` & `md2weasypdf-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2weasypdf
-Version: 0.0.7
+Version: 0.0.8
 Summary: Print PDFs from Markdown Files using Weasyprint
 Home-page: https://github.com/mstingl/md2weasypdf
 Author: Manuel Stingl
 Author-email: contact@stingl.st
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `md2weasypdf-0.0.7/README.md` & `md2weasypdf-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.7/md2weasypdf/__main__.py` & `md2weasypdf-0.0.8/md2weasypdf/__main__.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.7/md2weasypdf/extensions/checkbox.py` & `md2weasypdf-0.0.8/md2weasypdf/extensions/checkbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.7/md2weasypdf/extensions/footnotes.py` & `md2weasypdf-0.0.8/md2weasypdf/extensions/footnotes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import xml.etree.ElementTree as etree
+from collections import OrderedDict
 from dataclasses import dataclass
 from typing import Dict
 
 from markdown import Markdown
 from markdown.extensions import footnotes
 from markdown.inlinepatterns import InlineProcessor
 
@@ -38,15 +39,18 @@
                 el.text = str(footnote.index)
 
             return el, m.start(0), m.end(0)
 
 
 class FootnoteExtension(footnotes.FootnoteExtension):
     def __init__(self):
-        self.footnotes: Dict[str, Footnote] = {}
+        self.footnotes: OrderedDict[str, Footnote] = OrderedDict()
+        self.unique_prefix = 0
+        self.found_refs: dict[str, int] = {}
+        self.used_refs: set[str] = set()
 
     def setFootnote(self, id, text):
         self.footnotes[id] = Footnote(text, len(self.footnotes) + 1)
 
     def extendMarkdown(self, md: Markdown):
         md.registerExtension(self)
         self.parser = md.parser
```

### Comparing `md2weasypdf-0.0.7/md2weasypdf/extensions/textbox.py` & `md2weasypdf-0.0.8/md2weasypdf/extensions/textbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.7/md2weasypdf/extensions/toa.py` & `md2weasypdf-0.0.8/md2weasypdf/extensions/toa.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.7/md2weasypdf/extensions/toc.py` & `md2weasypdf-0.0.8/md2weasypdf/extensions/toc.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.7/md2weasypdf/printer.py` & `md2weasypdf-0.0.8/md2weasypdf/printer.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.7/md2weasypdf.egg-info/PKG-INFO` & `md2weasypdf-0.0.8/md2weasypdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2weasypdf
-Version: 0.0.7
+Version: 0.0.8
 Summary: Print PDFs from Markdown Files using Weasyprint
 Home-page: https://github.com/mstingl/md2weasypdf
 Author: Manuel Stingl
 Author-email: contact@stingl.st
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `md2weasypdf-0.0.7/md2weasypdf.egg-info/SOURCES.txt` & `md2weasypdf-0.0.8/md2weasypdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.7/setup.cfg` & `md2weasypdf-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = md2weasypdf
-version = 0.0.7
+version = 0.0.8
 author = Manuel Stingl
 author_email = contact@stingl.st
 description = Print PDFs from Markdown Files using Weasyprint
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU LGPLv2.1
 classifiers =
```

