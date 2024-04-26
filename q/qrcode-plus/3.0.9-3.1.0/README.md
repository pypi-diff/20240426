# Comparing `tmp/qrcode_plus-3.0.9.tar.gz` & `tmp/qrcode_plus-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrcode_plus-3.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qrcode_plus-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qrcode_plus-3.0.9.tar` & `qrcode_plus-3.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1505 2024-04-13 16:10:05.922714 qrcode_plus-3.0.9/LICENSE
--rw-r--r--   0        0        0     1003 2024-03-14 15:29:45.816329 qrcode_plus-3.0.9/README.rst
--rw-r--r--   0        0        0     1783 2024-04-17 13:47:04.650282 qrcode_plus-3.0.9/pyproject.toml
--rw-r--r--   0        0        0    16797 2024-04-17 13:45:44.788089 qrcode_plus-3.0.9/qrcode_plus.py
--rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 qrcode_plus-3.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1505 2024-04-13 16:10:05.922714 qrcode_plus-3.1.0/LICENSE
+-rw-r--r--   0        0        0     1003 2024-03-14 15:29:45.816329 qrcode_plus-3.1.0/README.rst
+-rw-r--r--   0        0        0     1783 2024-04-26 08:57:15.479609 qrcode_plus-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16797 2024-04-17 13:45:44.788089 qrcode_plus-3.1.0/qrcode_plus.py
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 qrcode_plus-3.1.0/PKG-INFO
```

### Comparing `qrcode_plus-3.0.9/LICENSE` & `qrcode_plus-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qrcode_plus-3.0.9/README.rst` & `qrcode_plus-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `qrcode_plus-3.0.9/pyproject.toml` & `qrcode_plus-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "qrcode-plus"
 description = "Advance Artistic (Micro) QR Code plugin for Segno"
-version = "3.0.9"
+version = "3.1.0"
 readme = "README.rst"
 license = {file = "LICENSE"}
 authors = [{"name" = "Kyle Bradley", email = "kbradley53@gmail.com"}]
 requires-python = ">= 3.5"
 keywords = ["QR Code", "Micro QR Code", "ISO/IEC 18004", "ISO/IEC 18004:2006(E)",
     "ISO/IEC 18004:2015(E)", "qrcode", "QR", "barcode", "matrix", "2D",]
 classifiers = [
```

### Comparing `qrcode_plus-3.0.9/qrcode_plus.py` & `qrcode_plus-3.1.0/qrcode_plus.py`

 * *Files identical despite different names*

### Comparing `qrcode_plus-3.0.9/PKG-INFO` & `qrcode_plus-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrcode-plus
-Version: 3.0.9
+Version: 3.1.0
 Summary: Advance Artistic (Micro) QR Code plugin for Segno
 Keywords: QR Code,Micro QR Code,ISO/IEC 18004,ISO/IEC 18004:2006(E),ISO/IEC 18004:2015(E),qrcode,QR,barcode,matrix,2D
 Author-email: Kyle Bradley <kbradley53@gmail.com>
 Requires-Python: >= 3.5
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

