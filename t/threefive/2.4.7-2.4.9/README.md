# Comparing `tmp/threefive-2.4.7.tar.gz` & `tmp/threefive-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threefive-2.4.7.tar", last modified: Thu Sep  7 03:45:40 2023, max compression
+gzip compressed data, was "threefive-2.4.9.tar", last modified: Thu Sep  7 03:49:45 2023, max compression
```

## Comparing `threefive-2.4.7.tar` & `threefive-2.4.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-09-07 03:45:40.568107 threefive-2.4.7/
--rw-r--r--   0 a         (1000) a         (1000)     1074 2023-09-07 03:43:42.000000 threefive-2.4.7/LICENSE
--rw-r--r--   0 a         (1000) a         (1000)    17981 2023-09-07 03:45:40.568107 threefive-2.4.7/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)    17411 2023-09-07 03:43:42.000000 threefive-2.4.7/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-09-07 03:45:40.564107 threefive-2.4.7/bin/
--rwxr-xr-x   0 a         (1000) a         (1000)      667 2023-09-07 03:43:42.000000 threefive-2.4.7/bin/threefive
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-09-07 03:45:40.568107 threefive-2.4.7/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1026 2023-09-07 03:43:42.000000 threefive-2.4.7/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-09-07 03:45:40.568107 threefive-2.4.7/threefive/
--rw-r--r--   0 a         (1000) a         (1000)      628 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/__init__.py
--rw-r--r--   0 a         (1000) a         (1000)     2873 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/base.py
--rw-r--r--   0 a         (1000) a         (1000)     4811 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/bitn.py
--rw-r--r--   0 a         (1000) a         (1000)    11730 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/commands.py
--rw-r--r--   0 a         (1000) a         (1000)      846 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/crc.py
--rw-r--r--   0 a         (1000) a         (1000)    10691 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/cue.py
--rw-r--r--   0 a         (1000) a         (1000)     1837 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/decode.py
--rw-r--r--   0 a         (1000) a         (1000)    13756 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/descriptors.py
--rw-r--r--   0 a         (1000) a         (1000)     2689 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/encode.py
--rw-r--r--   0 a         (1000) a         (1000)     1038 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/packetdata.py
--rw-r--r--   0 a         (1000) a         (1000)     5709 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/section.py
--rw-r--r--   0 a         (1000) a         (1000)     3477 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/segment.py
--rw-r--r--   0 a         (1000) a         (1000)     1970 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/segmentation.py
--rw-r--r--   0 a         (1000) a         (1000)     1660 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/smoketest.py
--rw-r--r--   0 a         (1000) a         (1000)    18353 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/stream.py
--rw-r--r--   0 a         (1000) a         (1000)      199 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/stuff.py
--rw-r--r--   0 a         (1000) a         (1000)     6595 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/upids.py
--rw-r--r--   0 a         (1000) a         (1000)       42 2023-09-07 03:43:42.000000 threefive-2.4.7/threefive/version.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-09-07 03:45:40.568107 threefive-2.4.7/threefive.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)    17981 2023-09-07 03:45:40.000000 threefive-2.4.7/threefive.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      577 2023-09-07 03:45:40.000000 threefive-2.4.7/threefive.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-09-07 03:45:40.000000 threefive-2.4.7/threefive.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       24 2023-09-07 03:45:40.000000 threefive-2.4.7/threefive.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)       10 2023-09-07 03:45:40.000000 threefive-2.4.7/threefive.egg-info/top_level.txt
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-09-07 03:49:45.600384 threefive-2.4.9/
+-rw-r--r--   0 a         (1000) a         (1000)     1074 2023-09-07 03:43:42.000000 threefive-2.4.9/LICENSE
+-rw-r--r--   0 a         (1000) a         (1000)    17981 2023-09-07 03:49:45.600384 threefive-2.4.9/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)    17411 2023-09-07 03:49:39.000000 threefive-2.4.9/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-09-07 03:49:45.596384 threefive-2.4.9/bin/
+-rwxr-xr-x   0 a         (1000) a         (1000)      667 2023-09-07 03:43:42.000000 threefive-2.4.9/bin/threefive
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-09-07 03:49:45.600384 threefive-2.4.9/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1026 2023-09-07 03:43:42.000000 threefive-2.4.9/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-09-07 03:49:45.596384 threefive-2.4.9/threefive/
+-rw-r--r--   0 a         (1000) a         (1000)      628 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/__init__.py
+-rw-r--r--   0 a         (1000) a         (1000)     2873 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/base.py
+-rw-r--r--   0 a         (1000) a         (1000)     4811 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/bitn.py
+-rw-r--r--   0 a         (1000) a         (1000)    11730 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/commands.py
+-rw-r--r--   0 a         (1000) a         (1000)      846 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/crc.py
+-rw-r--r--   0 a         (1000) a         (1000)    10691 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/cue.py
+-rw-r--r--   0 a         (1000) a         (1000)     1837 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/decode.py
+-rw-r--r--   0 a         (1000) a         (1000)    13756 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/descriptors.py
+-rw-r--r--   0 a         (1000) a         (1000)     2689 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/encode.py
+-rw-r--r--   0 a         (1000) a         (1000)     1038 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/packetdata.py
+-rw-r--r--   0 a         (1000) a         (1000)     5709 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/section.py
+-rw-r--r--   0 a         (1000) a         (1000)     3477 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/segment.py
+-rw-r--r--   0 a         (1000) a         (1000)     1970 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/segmentation.py
+-rw-r--r--   0 a         (1000) a         (1000)     1660 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/smoketest.py
+-rw-r--r--   0 a         (1000) a         (1000)    18354 2023-09-07 03:49:39.000000 threefive-2.4.9/threefive/stream.py
+-rw-r--r--   0 a         (1000) a         (1000)      199 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/stuff.py
+-rw-r--r--   0 a         (1000) a         (1000)     6595 2023-09-07 03:43:42.000000 threefive-2.4.9/threefive/upids.py
+-rw-r--r--   0 a         (1000) a         (1000)       42 2023-09-07 03:49:39.000000 threefive-2.4.9/threefive/version.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-09-07 03:49:45.600384 threefive-2.4.9/threefive.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)    17981 2023-09-07 03:49:45.000000 threefive-2.4.9/threefive.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      577 2023-09-07 03:49:45.000000 threefive-2.4.9/threefive.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-09-07 03:49:45.000000 threefive-2.4.9/threefive.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       24 2023-09-07 03:49:45.000000 threefive-2.4.9/threefive.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)       10 2023-09-07 03:49:45.000000 threefive-2.4.9/threefive.egg-info/top_level.txt
```

### Comparing `threefive-2.4.7/LICENSE` & `threefive-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/PKG-INFO` & `threefive-2.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threefive
-Version: 2.4.7
+Version: 2.4.9
 Summary: Pythonic SCTE35
 Home-page: https://github.com/futzu/threefive
 Author: Adrian and a Cast of Thousands.
 Author-email: spam@iodisco.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
@@ -13,15 +13,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  🥇 threefive is the most advanced SCTE-35 tool, ever.
  <br><br> SCTE-35 Encoder and Decoder Python3 lib.
  --- 
-Latest Version is `2.4.7`
+Latest Version is `2.4.9`
 
 - [x] `Decodes` SCTE-35.
 - [x] `Encodes` SCTE-35.
 - [x] Parses SCTE-35 from `Base64`, `Bytes`, `Hex`, `Integers`, and `MPEGTS` Streams.
 - [x] Parses  `files`, `http(s)`, `Multicast`, `UDP` and even `stdin` _( you can pipe to it)_. 
 - [x] Parses SCTE-35 from streams converted to `bin data` ( _type 0x06_ ) by `ffmpeg`.
```

### Comparing `threefive-2.4.7/README.md` & `threefive-2.4.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
  🥇 threefive is the most advanced SCTE-35 tool, ever.
  <br><br> SCTE-35 Encoder and Decoder Python3 lib.
  --- 
-Latest Version is `2.4.7`
+Latest Version is `2.4.9`
 
 - [x] `Decodes` SCTE-35.
 - [x] `Encodes` SCTE-35.
 - [x] Parses SCTE-35 from `Base64`, `Bytes`, `Hex`, `Integers`, and `MPEGTS` Streams.
 - [x] Parses  `files`, `http(s)`, `Multicast`, `UDP` and even `stdin` _( you can pipe to it)_. 
 - [x] Parses SCTE-35 from streams converted to `bin data` ( _type 0x06_ ) by `ffmpeg`.
```

### Comparing `threefive-2.4.7/bin/threefive` & `threefive-2.4.9/bin/threefive`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/setup.py` & `threefive-2.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/__init__.py` & `threefive-2.4.9/threefive/__init__.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/base.py` & `threefive-2.4.9/threefive/base.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/bitn.py` & `threefive-2.4.9/threefive/bitn.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/commands.py` & `threefive-2.4.9/threefive/commands.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/crc.py` & `threefive-2.4.9/threefive/crc.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/cue.py` & `threefive-2.4.9/threefive/cue.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/decode.py` & `threefive-2.4.9/threefive/decode.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/descriptors.py` & `threefive-2.4.9/threefive/descriptors.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/encode.py` & `threefive-2.4.9/threefive/encode.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/packetdata.py` & `threefive-2.4.9/threefive/packetdata.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/section.py` & `threefive-2.4.9/threefive/section.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/segment.py` & `threefive-2.4.9/threefive/segment.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/segmentation.py` & `threefive-2.4.9/threefive/segmentation.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/smoketest.py` & `threefive-2.4.9/threefive/smoketest.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive/stream.py` & `threefive-2.4.9/threefive/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     0x0F: "AAC Audio",
     0x15: "ID3 Timed Meta Data",
     0x1B: "AVC Video",
     0x80 : "MPEG-1 Audio",
     0x81 : "MPEG-2 Audio",
     0x82: "AC3 Audio ",
     0x83 : "AAC Audio",
-    0x84 : "AAC HE v2 Audio"
+    0x84 : "AAC HE v2 Audio",
     0x86: "SCTE35 Data",
     0xC0: "Unknown",
     
 }
 
 
 def no_op(cue):
```

### Comparing `threefive-2.4.7/threefive/upids.py` & `threefive-2.4.9/threefive/upids.py`

 * *Files identical despite different names*

### Comparing `threefive-2.4.7/threefive.egg-info/PKG-INFO` & `threefive-2.4.9/threefive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threefive
-Version: 2.4.7
+Version: 2.4.9
 Summary: Pythonic SCTE35
 Home-page: https://github.com/futzu/threefive
 Author: Adrian and a Cast of Thousands.
 Author-email: spam@iodisco.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
@@ -13,15 +13,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  🥇 threefive is the most advanced SCTE-35 tool, ever.
  <br><br> SCTE-35 Encoder and Decoder Python3 lib.
  --- 
-Latest Version is `2.4.7`
+Latest Version is `2.4.9`
 
 - [x] `Decodes` SCTE-35.
 - [x] `Encodes` SCTE-35.
 - [x] Parses SCTE-35 from `Base64`, `Bytes`, `Hex`, `Integers`, and `MPEGTS` Streams.
 - [x] Parses  `files`, `http(s)`, `Multicast`, `UDP` and even `stdin` _( you can pipe to it)_. 
 - [x] Parses SCTE-35 from streams converted to `bin data` ( _type 0x06_ ) by `ffmpeg`.
```

### Comparing `threefive-2.4.7/threefive.egg-info/SOURCES.txt` & `threefive-2.4.9/threefive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

