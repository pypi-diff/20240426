# Comparing `tmp/nrstitcher_utils-0.1.0.dev6.tar.gz` & `tmp/nrstitcher_utils-0.1.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrstitcher_utils-0.1.0.dev6.tar", last modified: Fri Apr 26 12:45:00 2024, max compression
+gzip compressed data, was "nrstitcher_utils-0.1.0.dev7.tar", last modified: Fri Apr 26 12:54:09 2024, max compression
```

## Comparing `nrstitcher_utils-0.1.0.dev6.tar` & `nrstitcher_utils-0.1.0.dev7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/
--rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      251 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/README.md
--rw-r--r--   0 payno     (1000) payno     (1000)     2131 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/pyproject.toml
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/setup.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/app/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/app/__init__.py
--rwxr-xr-x   0 payno     (1000) payno     (1000)     8279 2024-04-26 12:43:55.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3220 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/h5_settings.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8694 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/ht_vol.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3430 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/resources/
--rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/resources/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/resources/config_files/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/resources/config_files/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-04-26 12:44:49.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      706 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/entry_points.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:54:09.157080 nrstitcher_utils-0.1.0.dev7/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev7/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-26 12:54:09.157080 nrstitcher_utils-0.1.0.dev7/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      251 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev7/README.md
+-rw-r--r--   0 payno     (1000) payno     (1000)     2131 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev7/pyproject.toml
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-26 12:54:09.157080 nrstitcher_utils-0.1.0.dev7/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev7/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:54:09.157080 nrstitcher_utils-0.1.0.dev7/src/
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:54:09.157080 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:54:09.157080 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/app/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/app/__init__.py
+-rwxr-xr-x   0 payno     (1000) payno     (1000)     8278 2024-04-26 12:51:15.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:54:09.157080 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/core/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/core/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3140 2024-04-26 12:51:59.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/core/h5_settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8708 2024-04-26 12:52:37.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/core/ht_vol.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3460 2024-04-26 12:52:46.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/core/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:54:09.157080 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/resources/
+-rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/resources/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:54:09.157080 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/resources/config_files/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/resources/config_files/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-04-26 12:53:25.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:54:09.157080 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-26 12:54:09.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      706 2024-04-26 12:54:09.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-26 12:54:09.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-04-26 12:54:09.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils.egg-info/entry_points.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-04-26 12:54:09.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-04-26 12:54:09.000000 nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils.egg-info/top_level.txt
```

### Comparing `nrstitcher_utils-0.1.0.dev6/LICENSE` & `nrstitcher_utils-0.1.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev6/PKG-INFO` & `nrstitcher_utils-0.1.0.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev6
+Version: 0.1.0.dev7
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
```

### Comparing `nrstitcher_utils-0.1.0.dev6/pyproject.toml` & `nrstitcher_utils-0.1.0.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/app/nrs_config_id16a_ht.py` & `nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/app/nrs_config_id16a_ht.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
 stitch_settings_from_ID16a_ht.py:
 
-This script is dedicated to holotomographic data acquired on the beamline ID16A at the ESRF, and is used to generate a stitch settings file to be used as input to nr_stitcher.py. 
+This script is dedicated to holotomographic data acquired on the beamline ID16A at the ESRF, and is used to generate a stitch settings file to be used as input to nr_stitcher.py.
 The stitch settings file is generated based on the template default_stitch_settings.py provided with nr_stitcher, with parameters mofdified based on user-selected options.
 After adding the NRStitcher directory to the path, this script should be run from the directory where the generated stitch settings file is to be saved.
 
 """
 
 import argparse
 import glob
@@ -118,15 +118,15 @@
         "--debug",
         type=bool,
         default=False,
         help='Optional. Name of stitch_settings file. Default is "stitch_settings.txt". Will be saved in the current working directory.',
     )
 
     args = argparser.parse_args(argv)
-    if args.distances == None:
+    if args.distances is None:
         args.distances = [1, 2, 3, 4]
     args.distances.sort()
     log_level = logging.DEBUG if args.debug else logging.INFO
     logging.basicConfig(level=log_level)
 
     # Get volumes from command line input
     if len(args.volumes) > 1:
```

### Comparing `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/h5_settings.py` & `nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/core/h5_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,30 +8,27 @@
 class H5Settings:
 
     def __init__(self, h5_filename, volume_name, scan_suffix):
         self.filename = h5_filename
         self.file = h5py.File(self.filename, "r")
         self.keys = list(self.file.keys())
 
-        first_dist = args.distances[0]
-        scan_suffix = f"_{first_dist}_"
-
         mask = [x.endswith(scan_suffix) for x in self.keys]
         entry_list = list(compress(self.keys, mask))
 
         found = False
 
         for entry in entry_list:
             prefix = entry.split(" ")[-1].replace(scan_suffix, "")
             if prefix in volume_name:
                 self.root = self.file[entry]
                 _logger.info("will treat volume", volume_name)
                 found = True
 
-        if found == False:
+        if found is False:
             for entry in entry_list:
                 tmp = entry.split(" ")[-1]
                 prefix = "".join(tmp.rsplit(scan_suffix, 1))
 
                 if prefix in volume_name:
                     self.root = self.file[entry]
                     _logger.info("will treat volume", volume_name)
```

### Comparing `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/ht_vol.py` & `nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/core/ht_vol.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,28 +30,28 @@
         self.vmin = float(self.info["ValMin"])
         self.vmax = float(self.info["ValMax"])
         self.byteorder = self.info["BYTEORDER"].strip()
 
         self.dimensions = [self.cols, self.rows, self.slices]
 
         self.fromType = "float32"
-        if args.bitdepth == None:
+        if args.bitdepth is None:
             args.bitdepth = self.fromType
 
         self.toType = dt[args.bitdepth]
 
         if args.vrange is not None:
             self.tomin = args.vrange[0]
             self.tomax = args.vrange[1]
         else:
             self.tomin = self.vmin
             self.tomax = self.vmax
 
         self.rescaleTo = args.voxelsize
-        if self.rescaleTo != None:
+        if self.rescaleTo is not None:
             self.zoom = self.voxelSize / (float(self.rescaleTo) / 1000.0)
         else:
             self.zoom = 1
 
         strbits = args.bitdepth
 
         self.modified = False
@@ -81,15 +81,15 @@
 
         info = {}
         with open(infoFile) as f:
             for line in f.readlines():
                 try:
                     key, value = line.replace(" ", "").replace("\n", "").split("=")
                     info[key] = value
-                except:
+                except Exception:
                     continue
 
         return info
 
     def check_raw(self):
         """
         Check if a processed image corresponding to selected options already exists or not.
```

### Comparing `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/utils.py` & `nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """generic utils function"""
 
+import numpy as np
+
 
 def get_sax_say(su, sv):
     """
     Calculate the sax and say values from the su and sv positions.
 
     Arguments:
     su: Position of motor su, read from experiment .h5 file
@@ -114,11 +116,11 @@
 
     info = {}
     with open(infoFile) as f:
         for line in f.readlines():
             try:
                 key, value = line.replace(" ", "").split("=")
                 info[key] = value
-            except:
+            except Exception:
                 continue
 
     return info
```

### Comparing `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/PKG-INFO` & `nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev6
+Version: 0.1.0.dev7
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
```

### Comparing `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/SOURCES.txt` & `nrstitcher_utils-0.1.0.dev7/src/nrstitcher_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

