# Comparing `tmp/fplab-0.0.2.4.tar.gz` & `tmp/fplab-0.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fplab-0.0.2.4.tar", last modified: Thu Apr 25 13:26:02 2024, max compression
+gzip compressed data, was "fplab-0.0.2.5.tar", last modified: Fri Apr 26 09:49:38 2024, max compression
```

## Comparing `fplab-0.0.2.4.tar` & `fplab-0.0.2.5.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:02.008452 fplab-0.0.2.4/
--rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0      523 2024-04-25 13:26:02.008452 fplab-0.0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.909229 fplab-0.0.2.4/fplab/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.925147 fplab-0.0.2.4/fplab/enhancement/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2.4/fplab/enhancement/__init__.py
--rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2.4/fplab/enhancement/frequency.py
--rw-rw-rw-   0        0        0     4907 2024-04-25 13:22:26.000000 fplab-0.0.2.4/fplab/enhancement/spatial.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.932763 fplab-0.0.2.4/fplab/generation/
--rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2.4/fplab/generation/__init__.py
--rw-rw-rw-   0        0        0     6948 2024-04-06 06:07:55.000000 fplab-0.0.2.4/fplab/generation/tps.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.933766 fplab-0.0.2.4/fplab/intrinsic/
--rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2.4/fplab/intrinsic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.949600 fplab-0.0.2.4/fplab/intrinsic/frequency/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/intrinsic/frequency/__init__.py
--rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2.4/fplab/intrinsic/frequency/projection.py
--rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2.4/fplab/intrinsic/frequency/tools.py
--rw-rw-rw-   0        0        0     3116 2024-04-07 04:59:12.000000 fplab-0.0.2.4/fplab/intrinsic/frequency/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.955455 fplab-0.0.2.4/fplab/intrinsic/mask/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/intrinsic/mask/__init__.py
--rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2.4/fplab/intrinsic/mask/mask.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.960742 fplab-0.0.2.4/fplab/intrinsic/multiple/
--rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2.4/fplab/intrinsic/multiple/__init__.py
--rw-rw-rw-   0        0        0     6990 2024-04-07 05:24:47.000000 fplab-0.0.2.4/fplab/intrinsic/multiple/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.972586 fplab-0.0.2.4/fplab/intrinsic/orientation/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/intrinsic/orientation/__init__.py
--rw-rw-rw-   0        0        0     6640 2024-04-06 09:18:53.000000 fplab-0.0.2.4/fplab/intrinsic/orientation/gradient.py
--rw-rw-rw-   0        0        0     6215 2024-04-07 04:39:10.000000 fplab-0.0.2.4/fplab/intrinsic/orientation/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.978589 fplab-0.0.2.4/fplab/intrinsic/skeleton/
--rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2.4/fplab/intrinsic/skeleton/__init__.py
--rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2.4/fplab/intrinsic/skeleton/skeleton.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.984213 fplab-0.0.2.4/fplab/matching/
--rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2.4/fplab/matching/__init__.py
--rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2.4/fplab/matching/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.986680 fplab-0.0.2.4/fplab/minutiae/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/minutiae/__init__.py
--rw-rw-rw-   0        0        0     6782 2024-04-14 14:52:02.000000 fplab-0.0.2.4/fplab/minutiae/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:02.006341 fplab-0.0.2.4/fplab/tools/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/tools/__init__.py
--rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2.4/fplab/tools/array.py
--rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2.4/fplab/tools/image.py
--rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2.4/fplab/tools/nbis.py
--rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2.4/fplab/tools/tensor.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.917947 fplab-0.0.2.4/fplab.egg-info/
--rw-rw-rw-   0        0        0      523 2024-04-25 13:26:01.000000 fplab-0.0.2.4/fplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2024-04-25 13:26:01.000000 fplab-0.0.2.4/fplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 13:26:01.000000 fplab-0.0.2.4/fplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-25 13:26:01.000000 fplab-0.0.2.4/fplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 13:26:02.008452 fplab-0.0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      801 2024-04-25 13:24:06.000000 fplab-0.0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.303383 fplab-0.0.2.5/
+-rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      523 2024-04-26 09:49:38.303383 fplab-0.0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.176627 fplab-0.0.2.5/fplab/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.5/fplab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.204567 fplab-0.0.2.5/fplab/enhancement/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2.5/fplab/enhancement/__init__.py
+-rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2.5/fplab/enhancement/frequency.py
+-rw-rw-rw-   0        0        0     4907 2024-04-25 13:22:26.000000 fplab-0.0.2.5/fplab/enhancement/spatial.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.220993 fplab-0.0.2.5/fplab/generation/
+-rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2.5/fplab/generation/__init__.py
+-rw-rw-rw-   0        0        0     1449 2024-04-26 02:12:49.000000 fplab-0.0.2.5/fplab/generation/tools.py
+-rw-rw-rw-   0        0        0     6948 2024-04-06 06:07:55.000000 fplab-0.0.2.5/fplab/generation/tps.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.220993 fplab-0.0.2.5/fplab/intrinsic/
+-rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2.5/fplab/intrinsic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.238412 fplab-0.0.2.5/fplab/intrinsic/frequency/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.5/fplab/intrinsic/frequency/__init__.py
+-rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2.5/fplab/intrinsic/frequency/projection.py
+-rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2.5/fplab/intrinsic/frequency/tools.py
+-rw-rw-rw-   0        0        0     3116 2024-04-07 04:59:12.000000 fplab-0.0.2.5/fplab/intrinsic/frequency/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.244852 fplab-0.0.2.5/fplab/intrinsic/mask/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.5/fplab/intrinsic/mask/__init__.py
+-rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2.5/fplab/intrinsic/mask/mask.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.251189 fplab-0.0.2.5/fplab/intrinsic/multiple/
+-rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2.5/fplab/intrinsic/multiple/__init__.py
+-rw-rw-rw-   0        0        0     6990 2024-04-07 05:24:47.000000 fplab-0.0.2.5/fplab/intrinsic/multiple/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.262136 fplab-0.0.2.5/fplab/intrinsic/orientation/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.5/fplab/intrinsic/orientation/__init__.py
+-rw-rw-rw-   0        0        0     6640 2024-04-06 09:18:53.000000 fplab-0.0.2.5/fplab/intrinsic/orientation/gradient.py
+-rw-rw-rw-   0        0        0     6215 2024-04-07 04:39:10.000000 fplab-0.0.2.5/fplab/intrinsic/orientation/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.267313 fplab-0.0.2.5/fplab/intrinsic/skeleton/
+-rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2.5/fplab/intrinsic/skeleton/__init__.py
+-rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2.5/fplab/intrinsic/skeleton/skeleton.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.273706 fplab-0.0.2.5/fplab/matching/
+-rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2.5/fplab/matching/__init__.py
+-rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2.5/fplab/matching/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.283219 fplab-0.0.2.5/fplab/minutiae/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.5/fplab/minutiae/__init__.py
+-rw-rw-rw-   0        0        0     6782 2024-04-14 14:52:02.000000 fplab-0.0.2.5/fplab/minutiae/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.303383 fplab-0.0.2.5/fplab/tools/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.5/fplab/tools/__init__.py
+-rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2.5/fplab/tools/array.py
+-rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2.5/fplab/tools/image.py
+-rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2.5/fplab/tools/nbis.py
+-rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2.5/fplab/tools/tensor.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:49:38.193974 fplab-0.0.2.5/fplab.egg-info/
+-rw-rw-rw-   0        0        0      523 2024-04-26 09:49:38.000000 fplab-0.0.2.5/fplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1051 2024-04-26 09:49:38.000000 fplab-0.0.2.5/fplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 09:49:38.000000 fplab-0.0.2.5/fplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 09:49:38.000000 fplab-0.0.2.5/fplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 09:49:38.303383 fplab-0.0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      801 2024-04-26 09:48:24.000000 fplab-0.0.2.5/setup.py
```

### Comparing `fplab-0.0.2.4/LICENSE.txt` & `fplab-0.0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/PKG-INFO` & `fplab-0.0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2.4
+Version: 0.0.2.5
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2.4/README.md` & `fplab-0.0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/enhancement/frequency.py` & `fplab-0.0.2.5/fplab/enhancement/frequency.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/enhancement/spatial.py` & `fplab-0.0.2.5/fplab/enhancement/spatial.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/generation/tps.py` & `fplab-0.0.2.5/fplab/generation/tps.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/intrinsic/frequency/projection.py` & `fplab-0.0.2.5/fplab/intrinsic/frequency/projection.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/intrinsic/frequency/tools.py` & `fplab-0.0.2.5/fplab/intrinsic/frequency/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/intrinsic/frequency/transform.py` & `fplab-0.0.2.5/fplab/intrinsic/frequency/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/intrinsic/mask/mask.py` & `fplab-0.0.2.5/fplab/intrinsic/mask/mask.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/intrinsic/multiple/transform.py` & `fplab-0.0.2.5/fplab/intrinsic/multiple/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/intrinsic/orientation/gradient.py` & `fplab-0.0.2.5/fplab/intrinsic/orientation/gradient.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/intrinsic/orientation/tools.py` & `fplab-0.0.2.5/fplab/intrinsic/orientation/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/intrinsic/skeleton/skeleton.py` & `fplab-0.0.2.5/fplab/intrinsic/skeleton/skeleton.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/matching/tools.py` & `fplab-0.0.2.5/fplab/matching/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/minutiae/tools.py` & `fplab-0.0.2.5/fplab/minutiae/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/tools/array.py` & `fplab-0.0.2.5/fplab/tools/array.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/tools/image.py` & `fplab-0.0.2.5/fplab/tools/image.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/tools/nbis.py` & `fplab-0.0.2.5/fplab/tools/nbis.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab/tools/tensor.py` & `fplab-0.0.2.5/fplab/tools/tensor.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.4/fplab.egg-info/PKG-INFO` & `fplab-0.0.2.5/fplab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2.4
+Version: 0.0.2.5
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2.4/fplab.egg-info/SOURCES.txt` & `fplab-0.0.2.5/fplab.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 fplab.egg-info/SOURCES.txt
 fplab.egg-info/dependency_links.txt
 fplab.egg-info/top_level.txt
 fplab/enhancement/__init__.py
 fplab/enhancement/frequency.py
 fplab/enhancement/spatial.py
 fplab/generation/__init__.py
+fplab/generation/tools.py
 fplab/generation/tps.py
 fplab/intrinsic/__init__.py
 fplab/intrinsic/frequency/__init__.py
 fplab/intrinsic/frequency/projection.py
 fplab/intrinsic/frequency/tools.py
 fplab/intrinsic/frequency/transform.py
 fplab/intrinsic/mask/__init__.py
```

### Comparing `fplab-0.0.2.4/setup.py` & `fplab-0.0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2.4'
+VERSION = '0.0.2.5'
 DESCRIPTION = 'Python3 Package for Fingerprint Processing'
 LONG_DESCRIPTION = ('This is a python3 package for fingerprint processing,'
                     ' which can be used for fingerprint enhancement.')
 
 setup(
     name="fplab",
     version=VERSION,
```

