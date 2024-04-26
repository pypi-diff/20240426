# Comparing `tmp/pygmtsar-2024.4.17.tar.gz` & `tmp/pygmtsar-2024.4.17.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2024.4.17.tar", last modified: Mon Apr 22 06:47:48 2024, max compression
+gzip compressed data, was "pygmtsar-2024.4.17.post1.tar", last modified: Fri Apr 26 16:33:42 2024, max compression
```

## Comparing `pygmtsar-2024.4.17.tar` & `pygmtsar-2024.4.17.post1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-22 06:47:48.348651 pygmtsar-2024.4.17/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    13457 2024-04-22 06:47:48.348389 pygmtsar-2024.4.17/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-22 06:47:48.346999 pygmtsar-2024.4.17/pygmtsar/
--rw-r--r--   0 mbg        (501) staff       (20)    16155 2024-04-17 06:55:44.000000 pygmtsar-2024.4.17/pygmtsar/ASF.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17/pygmtsar/AWS.py
--rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17/pygmtsar/GMT.py
--rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17/pygmtsar/IO.py
--rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17/pygmtsar/NCubeVTK.py
--rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17/pygmtsar/PRM_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17/pygmtsar/S1.py
--rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.4.17/pygmtsar/Stack.py
--rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17/pygmtsar/Stack_align.py
--rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17/pygmtsar/Stack_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17/pygmtsar/Stack_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)    44173 2024-02-08 18:53:49.000000 pygmtsar-2024.4.17/pygmtsar/Stack_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17/pygmtsar/Stack_export.py
--rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17/pygmtsar/Stack_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17/pygmtsar/Stack_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17/pygmtsar/Stack_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17/pygmtsar/Stack_multilooking.py
--rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17/pygmtsar/Stack_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)    47295 2024-03-29 07:29:11.000000 pygmtsar-2024.4.17/pygmtsar/Stack_phasediff.py
--rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17/pygmtsar/Stack_prm.py
--rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17/pygmtsar/Stack_ps.py
--rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17/pygmtsar/Stack_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17/pygmtsar/Stack_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    46640 2024-04-11 04:05:10.000000 pygmtsar-2024.4.17/pygmtsar/Stack_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     8884 2024-01-01 15:32:51.000000 pygmtsar-2024.4.17/pygmtsar/Stack_stl.py
--rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17/pygmtsar/Stack_tidal.py
--rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17/pygmtsar/Stack_topo.py
--rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17/pygmtsar/Stack_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17/pygmtsar/Stack_trans_inv.py
--rw-r--r--   0 mbg        (501) staff       (20)    26654 2024-04-11 05:08:11.000000 pygmtsar-2024.4.17/pygmtsar/Stack_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17/pygmtsar/Stack_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17/pygmtsar/Tiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.4.17/pygmtsar/XYZTiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17/pygmtsar/_Stack_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)     1034 2024-04-17 08:18:17.000000 pygmtsar-2024.4.17/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17/pygmtsar/tqdm_joblib.py
--rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17/pygmtsar/utils.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-22 06:47:48.348097 pygmtsar-2024.4.17/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    13457 2024-04-22 06:47:48.000000 pygmtsar-2024.4.17/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-04-22 06:47:48.000000 pygmtsar-2024.4.17/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2024-04-22 06:47:48.000000 pygmtsar-2024.4.17/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      330 2024-04-22 06:47:48.000000 pygmtsar-2024.4.17/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2024-04-22 06:47:48.000000 pygmtsar-2024.4.17/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2024-04-22 06:47:48.348704 pygmtsar-2024.4.17/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.4.17/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-26 16:33:42.230689 pygmtsar-2024.4.17.post1/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17.post1/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-26 16:33:42.230375 pygmtsar-2024.4.17.post1/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17.post1/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-26 16:33:42.228724 pygmtsar-2024.4.17.post1/pygmtsar/
+-rw-r--r--   0 mbg        (501) staff       (20)    18153 2024-04-26 09:12:06.000000 pygmtsar-2024.4.17.post1/pygmtsar/ASF.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17.post1/pygmtsar/AWS.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17.post1/pygmtsar/GMT.py
+-rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17.post1/pygmtsar/IO.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17.post1/pygmtsar/NCubeVTK.py
+-rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17.post1/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17.post1/pygmtsar/PRM_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17.post1/pygmtsar/S1.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_align.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)    44173 2024-02-08 18:53:49.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_export.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_multilooking.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)    47295 2024-03-29 07:29:11.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_phasediff.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_prm.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_ps.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    46640 2024-04-11 04:05:10.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9103 2024-04-26 15:00:33.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_stl.py
+-rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_tidal.py
+-rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_topo.py
+-rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_trans_inv.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26654 2024-04-11 05:08:11.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17.post1/pygmtsar/Stack_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17.post1/pygmtsar/Tiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.4.17.post1/pygmtsar/XYZTiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17.post1/pygmtsar/_Stack_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1040 2024-04-26 15:55:09.000000 pygmtsar-2024.4.17.post1/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17.post1/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17.post1/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17.post1/pygmtsar/tqdm_joblib.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17.post1/pygmtsar/utils.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-26 16:33:42.230076 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-26 16:33:42.000000 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-04-26 16:33:42.000000 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2024-04-26 16:33:42.000000 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      330 2024-04-26 16:33:42.000000 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2024-04-26 16:33:42.000000 pygmtsar-2024.4.17.post1/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2024-04-26 16:33:42.230749 pygmtsar-2024.4.17.post1/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.4.17.post1/setup.py
```

### Comparing `pygmtsar-2024.4.17/LICENSE.txt` & `pygmtsar-2024.4.17.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/PKG-INFO` & `pygmtsar-2024.4.17.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17
+Version: 2024.4.17.post1
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.4.17/README.md` & `pygmtsar-2024.4.17.post1/README.md`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/ASF.py` & `pygmtsar-2024.4.17.post1/pygmtsar/ASF.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class ASF(tqdm_joblib):
     import pandas as pd
     from datetime import timedelta
 
     template_url = 'https://datapool.asf.alaska.edu/SLC/S{satellite}/{scene}.zip'
     template_safe = '*.SAFE/*/{mission}-iw{subswath}-slc-{polarization}-*'
     # check for downloaded scene files
-    template_scene = 'S1?_IW_SLC__1S??_{start}_*.SAFE/*/s1?-{subswath_lowercase}-slc-{polarization_lowercase}-{start_lowercase}-*'
+    template_scene = 'S1?_IW_SLC__1S??_{start}_*.SAFE/*/s1?-iw{subswath_lowercase}-slc-{polarization_lowercase}-{start_lowercase}-*'
     # URL of the HTML page
     # see https://asf.alaska.edu/data-sets/sar-data-sets/sentinel-1/sentinel-1-data-and-imagery/
     # https://s1qc.asf.alaska.edu
     poeorb_url = 'https://s1qc.asf.alaska.edu/aux_poeorb/'
     resorb_url = 'https://s1qc.asf.alaska.edu/aux_resorb/'
     # resorb - 69108
     # poeorb - 9811
@@ -52,30 +52,51 @@
         import numpy as np
         import asf_search
         import fnmatch
         import joblib
         from tqdm.auto import tqdm
         import os
         import re
+        import glob
         from datetime import datetime, timedelta
         import warnings
         # supress asf_search 'UserWarning: File already exists, skipping download'
         warnings.filterwarnings("ignore", category=UserWarning)
 
         # create the directory if needed
         os.makedirs(basedir, exist_ok=True)
 
         # collect all the existing files once
         files = os.listdir(basedir)
         #print ('files', len(files))
 
         # skip existing scenes
         if skip_exist:
-            # check scenes folders 
-            scenes_missed = np.unique([scene for scene in scenes if f'{scene}.SAFE' not in files])
+            # collect all the existing files once
+            files = glob.glob('**', root_dir=basedir, recursive=True)
+            #print ('files', len(files))
+            # check scenes folders only
+            #scenes_missed = np.unique([scene for scene in scenes if f'{scene}.SAFE' not in files])
+            scenes_missed = []
+            for scene in scenes:
+                scene_path = '/'.join([scene + '.SAFE'] + self.template_scene.split('/')[1:])
+                #print ('scene_path', scene_path)
+                for subswath in str(subswaths):
+                    pattern = scene_path.format(
+                                         subswath_lowercase = subswath.lower(),
+                                         polarization_lowercase = polarization.lower(),
+                                         start_lowercase = '*')
+                    #print ('pattern', pattern)
+                    matching = [filename for filename in files if fnmatch.fnmatch(filename, pattern)]
+                    exts = [os.path.splitext(fname)[1] for fname in matching]
+                    if '.tiff' in exts and '.xml'in exts:
+                        pass
+                    else:
+                        scenes_missed.append(scene)
+    
         else:
             # process all the defined scenes
             scenes_missed = scenes
         #print ('scenes_missed', len(scenes_missed))
 
         # do not use internet connection, work offline when all the scenes and orbits already available
         if len(scenes_missed) == 0:
@@ -113,17 +134,31 @@
                         #print (filename, filesize)
                         fullname = os.path.join(basedir, filename)
                         if os.path.exists(fullname) and os.path.getsize(fullname) == filesize:
                             #print (f'pass {fullname}')
                             pass
                         else:
                             #print (f'download {fullname}')
-                            #with open(fullname, 'wb') as file:
-                            #    file.write(remotezip.read(filename))
-                            remotezip.extract(filename, basedir)
+                            # create the directory if needed
+                            try:
+                                os.makedirs(os.path.dirname(fullname), exist_ok=True)
+                                if os.path.exists(fullname + '.tmp'):
+                                    os.remove(fullname + '.tmp')
+                                with open(fullname + '.tmp', 'wb') as file:
+                                    file.write(remotezip.read(filename))
+                                assert os.path.getsize(fullname + '.tmp') == filesize, \
+                                    f'ERROR: Downloaded incomplete scene content'
+                                os.rename(fullname + '.tmp', fullname)
+                            except Exception as e:
+                                print(e)
+                                raise
+                            finally:
+                                if os.path.exists(fullname + '.tmp'):
+                                    os.remove(fullname + '.tmp')
+                            #remotezip.extract(filename, basedir)
 
         # prepare authorized connection
         if session is None:
             session = self._get_asf_session()
 
         # download scenes
         with self.tqdm_joblib(tqdm(desc='ASF Downloading Sentinel-1 SLC:', total=len(scenes_missed))) as progress_bar:
```

### Comparing `pygmtsar-2024.4.17/pygmtsar/AWS.py` & `pygmtsar-2024.4.17.post1/pygmtsar/AWS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/GMT.py` & `pygmtsar-2024.4.17.post1/pygmtsar/GMT.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/IO.py` & `pygmtsar-2024.4.17.post1/pygmtsar/IO.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/NCubeVTK.py` & `pygmtsar-2024.4.17.post1/pygmtsar/NCubeVTK.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/PRM.py` & `pygmtsar-2024.4.17.post1/pygmtsar/PRM.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2024.4.17.post1/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/S1.py` & `pygmtsar-2024.4.17.post1/pygmtsar/S1.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_align.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_align.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_base.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_base.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_dem.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_detrend.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_detrend.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_export.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_export.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_geocode.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_geocode.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_incidence.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_landmask.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_landmask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_multilooking.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_multilooking.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_orbits.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_phasediff.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_phasediff.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_prm.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_prm.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_ps.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_ps.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_reframe.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_reframe.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_reframe_gmtsar.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_sbas.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_sbas.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_stl.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_stl.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 # Licensed under the BSD 3-Clause License (see LICENSE for details)
 # ----------------------------------------------------------------------------
 from .Stack_tidal import Stack_tidal
 from .tqdm_dask import tqdm_dask
 
 class Stack_stl(Stack_tidal):
 
+    def velocity(self, data):
+        years = ((data.date.max() - data.date.min()).dt.days/365.25).item()
+        #print ('years', np.round(years, 3))
+        velocity = data.mean('date')/years
+        return velocity
+
     def trend(self, data, deg=1):
         import xarray as xr
 
         trend = xr.polyval(data.date, data.polyfit('date', deg).polyfit_coefficients)
         return trend
     
     @staticmethod
```

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_tidal.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_tidal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_topo.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_topo.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_trans.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_trans_inv.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_trans_inv.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_unwrap.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_unwrap.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Stack_unwrap_snaphu.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Stack_unwrap_snaphu.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/Tiles.py` & `pygmtsar-2024.4.17.post1/pygmtsar/Tiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/XYZTiles.py` & `pygmtsar-2024.4.17.post1/pygmtsar/XYZTiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/_Stack_merge.py` & `pygmtsar-2024.4.17.post1/pygmtsar/_Stack_merge.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/__init__.py` & `pygmtsar-2024.4.17.post1/pygmtsar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 
 # This file is part of the PyGMTSAR project: https://github.com/mobigroup/gmtsar
 # 
 # Copyright (c) 2023, Alexey Pechnikov
 # 
 # Licensed under the BSD 3-Clause License (see LICENSE for details)
 # ----------------------------------------------------------------------------
-__version__ = '2024.4.17'
+__version__ = '2024.4.17.post1'
 
 # unified progress indicators
 from .tqdm_joblib import tqdm_joblib
 from .tqdm_dask import tqdm_dask
 # base NetCDF operations and parameters on NetCDF grid
 from .datagrid import datagrid
 # top level module classes
```

### Comparing `pygmtsar-2024.4.17/pygmtsar/datagrid.py` & `pygmtsar-2024.4.17.post1/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/tqdm_dask.py` & `pygmtsar-2024.4.17.post1/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/tqdm_joblib.py` & `pygmtsar-2024.4.17.post1/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar/utils.py` & `pygmtsar-2024.4.17.post1/pygmtsar/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2024.4.17.post1/pygmtsar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17
+Version: 2024.4.17.post1
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.4.17/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2024.4.17.post1/pygmtsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17/setup.py` & `pygmtsar-2024.4.17.post1/setup.py`

 * *Files identical despite different names*

