# Comparing `tmp/fisspy-1.0.6.tar.gz` & `tmp/fisspy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fisspy-1.0.6.tar", last modified: Thu Apr 25 11:55:19 2024, max compression
+gzip compressed data, was "fisspy-1.0.7.tar", last modified: Thu Apr 25 12:05:08 2024, max compression
```

## Comparing `fisspy-1.0.6.tar` & `fisspy-1.0.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.726634 fisspy-1.0.6/
--rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.6/LICENSE.txt
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-25 11:55:19.726441 fisspy-1.0.6/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.0.6/README.md
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.715932 fisspy-1.0.6/fisspy/
--rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-04-25 11:51:10.000000 fisspy-1.0.6/fisspy/__init__.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.717388 fisspy-1.0.6/fisspy/align/
--rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/align/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.0.6/fisspy/align/alignment.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.0.6/fisspy/align/base.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.719058 fisspy-1.0.6/fisspy/analysis/
--rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/analysis/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.0.6/fisspy/analysis/doppler.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/analysis/filter.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.0.6/fisspy/analysis/forecast.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/analysis/ofe.py
--rw-r--r--   0 jhkang     (501) staff       (20)    35498 2024-04-25 11:29:47.000000 fisspy-1.0.6/fisspy/analysis/tdmap.py
--rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.0.6/fisspy/analysis/wavelet.py
--rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.6/fisspy/cm.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.720080 fisspy-1.0.6/fisspy/correction/
--rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/correction/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/correction/correction.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/correction/get_inform.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.720992 fisspy-1.0.6/fisspy/data/
--rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.6/fisspy/data/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.6/fisspy/data/_sample.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.6/fisspy/data/download.py
--rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.6/fisspy/data/sample.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.721813 fisspy-1.0.6/fisspy/image/
--rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.0.6/fisspy/image/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    29769 2024-04-25 11:21:02.000000 fisspy-1.0.6/fisspy/image/interactive_image.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11423 2024-04-25 11:54:55.000000 fisspy-1.0.6/fisspy/image/raster_set.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.722037 fisspy-1.0.6/fisspy/inversion/
--rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/inversion/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/inversion/_mlsi.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.722493 fisspy-1.0.6/fisspy/io/
--rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.6/fisspy/io/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.6/fisspy/io/read.py
--rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/makevideo.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.724257 fisspy-1.0.6/fisspy/preprocess/
--rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/preprocess/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    52443 2024-04-25 11:18:41.000000 fisspy-1.0.6/fisspy/preprocess/proc_base.py
--rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/preprocess/proc_gui.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/preprocess/t_y_sh.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.726071 fisspy-1.0.6/fisspy/read/
--rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/read/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    49069 2024-04-25 11:24:21.000000 fisspy-1.0.6/fisspy/read/read_factory.py
--rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.0.6/fisspy/read/readbase.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.716693 fisspy-1.0.6/fisspy.egg-info/
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/SOURCES.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/dependency_links.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/not-zip-safe
--rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/requires.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/top_level.txt
--rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-25 11:55:19.726673 fisspy-1.0.6/setup.cfg
--rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-04-25 11:51:00.000000 fisspy-1.0.6/setup.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.288168 fisspy-1.0.7/
+-rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.7/LICENSE.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-25 12:05:08.287978 fisspy-1.0.7/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.0.7/README.md
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.276972 fisspy-1.0.7/fisspy/
+-rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-04-25 12:04:23.000000 fisspy-1.0.7/fisspy/__init__.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.278411 fisspy-1.0.7/fisspy/align/
+-rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/align/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.0.7/fisspy/align/alignment.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.0.7/fisspy/align/base.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.280809 fisspy-1.0.7/fisspy/analysis/
+-rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/analysis/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.0.7/fisspy/analysis/doppler.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/analysis/filter.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.0.7/fisspy/analysis/forecast.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/analysis/ofe.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    35498 2024-04-25 11:29:47.000000 fisspy-1.0.7/fisspy/analysis/tdmap.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.0.7/fisspy/analysis/wavelet.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.7/fisspy/cm.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.281818 fisspy-1.0.7/fisspy/correction/
+-rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/correction/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/correction/correction.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/correction/get_inform.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.282734 fisspy-1.0.7/fisspy/data/
+-rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.7/fisspy/data/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.7/fisspy/data/_sample.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.7/fisspy/data/download.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.7/fisspy/data/sample.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.283446 fisspy-1.0.7/fisspy/image/
+-rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.0.7/fisspy/image/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    29769 2024-04-25 11:21:02.000000 fisspy-1.0.7/fisspy/image/interactive_image.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11315 2024-04-25 12:04:09.000000 fisspy-1.0.7/fisspy/image/raster_set.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.283755 fisspy-1.0.7/fisspy/inversion/
+-rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/inversion/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/inversion/_mlsi.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.284182 fisspy-1.0.7/fisspy/io/
+-rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.7/fisspy/io/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.7/fisspy/io/read.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/makevideo.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.285837 fisspy-1.0.7/fisspy/preprocess/
+-rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/preprocess/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    52443 2024-04-25 11:18:41.000000 fisspy-1.0.7/fisspy/preprocess/proc_base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/preprocess/proc_gui.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/preprocess/t_y_sh.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.287580 fisspy-1.0.7/fisspy/read/
+-rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.7/fisspy/read/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    49069 2024-04-25 11:24:21.000000 fisspy-1.0.7/fisspy/read/read_factory.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.0.7/fisspy/read/readbase.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 12:05:08.277787 fisspy-1.0.7/fisspy.egg-info/
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/not-zip-safe
+-rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/requires.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-25 12:05:08.000000 fisspy-1.0.7/fisspy.egg-info/top_level.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-25 12:05:08.288209 fisspy-1.0.7/setup.cfg
+-rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-04-25 12:04:40.000000 fisspy-1.0.7/setup.py
```

### Comparing `fisspy-1.0.6/LICENSE.txt` & `fisspy-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/PKG-INFO` & `fisspy-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.0.6
+Version: 1.0.7
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.0.6/README.md` & `fisspy-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/align/alignment.py` & `fisspy-1.0.7/fisspy/align/alignment.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/align/base.py` & `fisspy-1.0.7/fisspy/align/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/analysis/doppler.py` & `fisspy-1.0.7/fisspy/analysis/doppler.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/analysis/filter.py` & `fisspy-1.0.7/fisspy/analysis/filter.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/analysis/forecast.py` & `fisspy-1.0.7/fisspy/analysis/forecast.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/analysis/ofe.py` & `fisspy-1.0.7/fisspy/analysis/ofe.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/analysis/tdmap.py` & `fisspy-1.0.7/fisspy/analysis/tdmap.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/analysis/wavelet.py` & `fisspy-1.0.7/fisspy/analysis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/cm.py` & `fisspy-1.0.7/fisspy/cm.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/correction/correction.py` & `fisspy-1.0.7/fisspy/correction/correction.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/correction/get_inform.py` & `fisspy-1.0.7/fisspy/correction/get_inform.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/data/_sample.py` & `fisspy-1.0.7/fisspy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/data/download.py` & `fisspy-1.0.7/fisspy/data/download.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/image/interactive_image.py` & `fisspy-1.0.7/fisspy/image/interactive_image.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/image/raster_set.py` & `fisspy-1.0.7/fisspy/image/raster_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import matplotlib.pyplot as plt
 from matplotlib.animation import FuncAnimation
 from .. import cm
 from ..preprocess.proc_base import fname2isot
 from ..read import FISS
 from astropy.time import Time
 from os.path import join, dirname, basename, isdir, isfile
-from os import mkdir, getcwd, chdir
+from os import mkdir
 from shutil import move
 from glob import glob
 from zipfile import ZipFile
 
 __author__ = "Juhyung Kang"
 __all__ = ['makeRasterSet']
 
@@ -304,25 +304,22 @@
         h = A.header
         ifname = self.title.get_text().replace(':','_').replace('-','_')+'.png'
         self.saveImage(join(idir, ifname), i=self.nf//2)
 
         # make zip file
         zipname0 = h['target'].replace(' ', '')
         zipname = join(ddir, zipname0+'_01.zip')
-        zipname = ifname.replace('.png', '.zip')
         if isfile(zipname):
             lf = len(glob(join(ddir, zipname0+'*.zip')))
             zipname = zipname.replace("01.zip", f"{lf+1:02}.zip")
-        chdir(ddir)
         zp = ZipFile(zipname, 'w')
         for i in range(len(self.flistA)):
             zp.write(self.flistA[i])
             zp.write(self.flistB[i])
         zp.close()
-        chdir(getcwd())
 
         # input
         observer = h['observer']
         st = self.stT.isot[11:]
         ed = self.edT.isot[11:]
         obstime = f"{st} ~ {ed}"
         try:
```

### Comparing `fisspy-1.0.6/fisspy/io/read.py` & `fisspy-1.0.7/fisspy/io/read.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/makevideo.py` & `fisspy-1.0.7/fisspy/makevideo.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/preprocess/proc_base.py` & `fisspy-1.0.7/fisspy/preprocess/proc_base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/preprocess/proc_gui.py` & `fisspy-1.0.7/fisspy/preprocess/proc_gui.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/preprocess/t_y_sh.py` & `fisspy-1.0.7/fisspy/preprocess/t_y_sh.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/read/read_factory.py` & `fisspy-1.0.7/fisspy/read/read_factory.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy/read/readbase.py` & `fisspy-1.0.7/fisspy/read/readbase.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/fisspy.egg-info/PKG-INFO` & `fisspy-1.0.7/fisspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.0.6
+Version: 1.0.7
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.0.6/fisspy.egg-info/SOURCES.txt` & `fisspy-1.0.7/fisspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.6/setup.py` & `fisspy-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fisspy',
-    version='1.0.6',
+    version='1.0.7',
     description='fisspy: Python analysis tools for GST/FISS',
     url='http://fiss.snu.ac.kr',
     author='Juhyung Kang',
     author_email='jhkang@astro.snu.ac.kr',
     license='BSD-2',
     python_requires='>=3.6',
     packages=find_packages(exclude=['docs', 'logo']),
```

