# Comparing `tmp/docx-asn1-1.0.6.tar.gz` & `tmp/docx_asn1-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx-asn1-1.0.6.tar", last modified: Wed Mar 13 17:47:19 2024, max compression
+gzip compressed data, was "docx_asn1-1.0.7.tar", last modified: Fri Apr 26 14:59:22 2024, max compression
```

## Comparing `docx-asn1-1.0.6.tar` & `docx_asn1-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-03-13 17:47:19.674867 docx-asn1-1.0.6/
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     1061 2024-03-13 16:42:04.000000 docx-asn1-1.0.6/LICENSE
--rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2177 2024-03-13 17:47:19.674867 docx-asn1-1.0.6/PKG-INFO
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      388 2024-03-13 17:24:22.000000 docx-asn1-1.0.6/README.md
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-03-13 17:47:19.674867 docx-asn1-1.0.6/docx_asn1/
--rwxrwxr-x   0 n4n5      (1000) n4n5      (1000)       90 2024-03-13 17:10:15.000000 docx-asn1-1.0.6/docx_asn1/__init__.py
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      111 2024-03-13 16:55:43.000000 docx-asn1-1.0.6/docx_asn1/__main__.py
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     1246 2024-03-13 17:46:28.000000 docx-asn1-1.0.6/docx_asn1/utils.py
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-03-13 17:47:19.674867 docx-asn1-1.0.6/docx_asn1.egg-info/
--rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2177 2024-03-13 17:47:19.000000 docx-asn1-1.0.6/docx_asn1.egg-info/PKG-INFO
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      227 2024-03-13 17:47:19.000000 docx-asn1-1.0.6/docx_asn1.egg-info/SOURCES.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)        1 2024-03-13 17:47:19.000000 docx-asn1-1.0.6/docx_asn1.egg-info/dependency_links.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       10 2024-03-13 17:47:19.000000 docx-asn1-1.0.6/docx_asn1.egg-info/top_level.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      698 2024-03-13 17:39:05.000000 docx-asn1-1.0.6/pyproject.toml
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       38 2024-03-13 17:47:19.674867 docx-asn1-1.0.6/setup.cfg
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-04-26 14:59:22.021237 docx_asn1-1.0.7/
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     1061 2024-03-13 16:42:04.000000 docx_asn1-1.0.7/LICENSE
+-rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2177 2024-04-26 14:59:22.021237 docx_asn1-1.0.7/PKG-INFO
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      388 2024-03-13 17:24:22.000000 docx_asn1-1.0.7/README.md
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-04-26 14:59:22.021237 docx_asn1-1.0.7/docx_asn1/
+-rwxrwxr-x   0 n4n5      (1000) n4n5      (1000)       90 2024-03-13 17:10:15.000000 docx_asn1-1.0.7/docx_asn1/__init__.py
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      111 2024-03-13 16:55:43.000000 docx_asn1-1.0.7/docx_asn1/__main__.py
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     1336 2024-04-26 14:57:48.000000 docx_asn1-1.0.7/docx_asn1/utils.py
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-04-26 14:59:22.021237 docx_asn1-1.0.7/docx_asn1.egg-info/
+-rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2177 2024-04-26 14:59:22.000000 docx_asn1-1.0.7/docx_asn1.egg-info/PKG-INFO
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      227 2024-04-26 14:59:22.000000 docx_asn1-1.0.7/docx_asn1.egg-info/SOURCES.txt
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)        1 2024-04-26 14:59:22.000000 docx_asn1-1.0.7/docx_asn1.egg-info/dependency_links.txt
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       10 2024-04-26 14:59:22.000000 docx_asn1-1.0.7/docx_asn1.egg-info/top_level.txt
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      698 2024-04-26 14:58:27.000000 docx_asn1-1.0.7/pyproject.toml
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       38 2024-04-26 14:59:22.021237 docx_asn1-1.0.7/setup.cfg
```

### Comparing `docx-asn1-1.0.6/LICENSE` & `docx_asn1-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `docx-asn1-1.0.6/PKG-INFO` & `docx_asn1-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx-asn1
-Version: 1.0.6
+Version: 1.0.7
 Summary: Extract ASN.1 from DOCX files
 Author-email: n4n5 <its.just.n4n5@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 n4n5
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `docx-asn1-1.0.6/docx_asn1/utils.py` & `docx_asn1-1.0.7/docx_asn1/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from docx import Document
 from sys import argv, stderr
 from os.path import isfile
 
 
-def extract_text_from_docx(filename):
+def extract_text_from_docx(
+    filename, start_text="-- ASN1START", stop_text="-- ASN1STOP"
+):
     """extract asn1 from a docx file"""
     if not isfile(filename):
         print(f"File {filename} not found", file=stderr)
         return None
     doc = Document(filename)
     full_text = []
     inside_range = False
     for para in doc.paragraphs:
-        if "-- ASN1START" in para.text:
+        if start_text in para.text:
             inside_range = True
             continue
-        elif "-- ASN1STOP" in para.text:
+        elif stop_text in para.text:
+            full_text.append(para.text)
             inside_range = False
             continue
 
         # Add the paragraph text if inside the desired range
         if inside_range:
             full_text.append(para.text)
     return "\n".join(full_text)
```

### Comparing `docx-asn1-1.0.6/docx_asn1.egg-info/PKG-INFO` & `docx_asn1-1.0.7/docx_asn1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx-asn1
-Version: 1.0.6
+Version: 1.0.7
 Summary: Extract ASN.1 from DOCX files
 Author-email: n4n5 <its.just.n4n5@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 n4n5
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `docx-asn1-1.0.6/pyproject.toml` & `docx_asn1-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docx-asn1"
-version = "1.0.6"
+version = "1.0.7"
 description = "Extract ASN.1 from DOCX files"
 readme = "README.md"
 authors = [{ name = "n4n5", email = "its.just.n4n5@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

