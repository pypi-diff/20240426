# Comparing `tmp/reduct_py-1.9.0-py3-none-any.whl.zip` & `tmp/reduct_py-1.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 15219 bytes, number of entries: 12
--rw-r--r--  2.0 unx      423 b- defN 24-Mar-08 20:14 reduct/__init__.py
--rw-r--r--  2.0 unx    15097 b- defN 24-Mar-08 20:14 reduct/bucket.py
--rw-r--r--  2.0 unx    11155 b- defN 24-Mar-08 20:14 reduct/client.py
--rw-r--r--  2.0 unx      891 b- defN 24-Mar-08 20:14 reduct/error.py
--rw-r--r--  2.0 unx     5096 b- defN 24-Mar-08 20:14 reduct/http.py
--rw-r--r--  2.0 unx     6730 b- defN 24-Mar-08 20:14 reduct/record.py
--rw-r--r--  2.0 unx     1771 b- defN 24-Mar-08 20:14 reduct/time.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Mar-08 20:14 reduct_py-1.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5133 b- defN 24-Mar-08 20:14 reduct_py-1.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-08 20:14 reduct_py-1.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-08 20:14 reduct_py-1.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      903 b- defN 24-Mar-08 20:14 reduct_py-1.9.0.dist-info/RECORD
-12 files, 48367 bytes uncompressed, 13729 bytes compressed:  71.6%
+Zip file size: 15223 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      423 b- defN 24-Apr-26 10:07 reduct/__init__.py
+-rw-r--r--  2.0 unx    15097 b- defN 24-Apr-26 10:07 reduct/bucket.py
+-rw-r--r--  2.0 unx    11155 b- defN 24-Apr-26 10:07 reduct/client.py
+-rw-r--r--  2.0 unx      891 b- defN 24-Apr-26 10:07 reduct/error.py
+-rw-r--r--  2.0 unx     5096 b- defN 24-Apr-26 10:07 reduct/http.py
+-rw-r--r--  2.0 unx     6737 b- defN 24-Apr-26 10:07 reduct/record.py
+-rw-r--r--  2.0 unx     1771 b- defN 24-Apr-26 10:07 reduct/time.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-26 10:07 reduct_py-1.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5133 b- defN 24-Apr-26 10:07 reduct_py-1.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 10:07 reduct_py-1.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-26 10:07 reduct_py-1.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      903 b- defN 24-Apr-26 10:07 reduct_py-1.9.1.dist-info/RECORD
+12 files, 48374 bytes uncompressed, 13733 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: reduct/record.py
 Comment: 
 
 Filename: reduct/time.py
 Comment: 
 
-Filename: reduct_py-1.9.0.dist-info/LICENSE
+Filename: reduct_py-1.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: reduct_py-1.9.0.dist-info/METADATA
+Filename: reduct_py-1.9.1.dist-info/METADATA
 Comment: 
 
-Filename: reduct_py-1.9.0.dist-info/WHEEL
+Filename: reduct_py-1.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: reduct_py-1.9.0.dist-info/top_level.txt
+Filename: reduct_py-1.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: reduct_py-1.9.0.dist-info/RECORD
+Filename: reduct_py-1.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reduct/record.py

```diff
@@ -86,15 +86,15 @@
             content_type=content_type,
             labels=labels,
             read_all=read_all,
             read=read,
             last=False,
         )
 
-        self._records[timestamp] = record
+        self._records[record.timestamp] = record
 
     def items(self) -> List[Tuple[int, Record]]:
         """Get records as dict items"""
         return sorted(self._records.items())
 
 
 LABEL_PREFIX = "x-reduct-label-"
```

## Comparing `reduct_py-1.9.0.dist-info/LICENSE` & `reduct_py-1.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `reduct_py-1.9.0.dist-info/METADATA` & `reduct_py-1.9.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reduct-py
-Version: 1.9.0
+Version: 1.9.1
 Summary: ReductStore Client SDK for Python
 Author: Ciaran Moyne
 Author-email: Alexey Timin <atimin@gmail.com>, Anthony Cavin <anthony@reduct.store>
 Maintainer-email: Alexey Timin <atimin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alexey Timin
```

