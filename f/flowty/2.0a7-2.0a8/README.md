# Comparing `tmp/flowty-2.0a7-cp39-cp39-win_amd64.whl.zip` & `tmp/flowty-2.0a8-cp39-cp39-manylinux_2_35_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1970144 bytes, number of entries: 7
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-22 12:25 flowty/__init__.py
--rw-r--r--  2.0 unx  4937728 b- defN 24-Apr-22 12:25 flowty/flowty.pyd
--rw-r--r--  2.0 unx     2754 b- defN 24-Apr-22 12:26 flowty-2.0a7.dist-info/LICENSE
--rw-r--r--  2.0 unx     4529 b- defN 24-Apr-22 12:26 flowty-2.0a7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 24-Apr-22 12:26 flowty-2.0a7.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-22 12:26 flowty-2.0a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      530 b- defN 24-Apr-22 12:26 flowty-2.0a7.dist-info/RECORD
-7 files, 4945669 bytes uncompressed, 1969212 bytes compressed:  60.2%
+Zip file size: 2621286 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-26 10:35 flowty/__init__.py
+-rw-r--r--  2.0 unx  6673832 b- defN 24-Apr-26 10:35 flowty/flowty.so
+-rw-r--r--  2.0 unx     2754 b- defN 24-Apr-26 10:36 flowty-2.0a8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4529 b- defN 24-Apr-26 10:36 flowty-2.0a8.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 24-Apr-26 10:36 flowty-2.0a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-26 10:36 flowty-2.0a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      530 b- defN 24-Apr-26 10:36 flowty-2.0a8.dist-info/RECORD
+7 files, 6681786 bytes uncompressed, 2620356 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: flowty/__init__.py
 Comment: 
 
-Filename: flowty/flowty.pyd
+Filename: flowty/flowty.so
 Comment: 
 
-Filename: flowty-2.0a7.dist-info/LICENSE
+Filename: flowty-2.0a8.dist-info/LICENSE
 Comment: 
 
-Filename: flowty-2.0a7.dist-info/METADATA
+Filename: flowty-2.0a8.dist-info/METADATA
 Comment: 
 
-Filename: flowty-2.0a7.dist-info/WHEEL
+Filename: flowty-2.0a8.dist-info/WHEEL
 Comment: 
 
-Filename: flowty-2.0a7.dist-info/top_level.txt
+Filename: flowty-2.0a8.dist-info/top_level.txt
 Comment: 
 
-Filename: flowty-2.0a7.dist-info/RECORD
+Filename: flowty-2.0a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `flowty-2.0a7.dist-info/LICENSE` & `flowty-2.0a8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flowty-2.0a7.dist-info/METADATA` & `flowty-2.0a8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowty
-Version: 2.0a7
+Version: 2.0a8
 Summary: Flowty Network Optimization Solver
 Author-email: Flowty <info@flowty.ai>
 License: Community License
         
         Copyright 2024 Flowty ApS
         All rights reserved.
```

