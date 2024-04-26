# Comparing `tmp/VESIcal-1.2.8.tar.gz` & `tmp/VESIcal-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VESIcal-1.2.8.tar", last modified: Fri Mar 29 20:22:32 2024, max compression
+gzip compressed data, was "VESIcal-1.2.9.tar", last modified: Fri Apr 12 18:35:45 2024, max compression
```

## Comparing `VESIcal-1.2.8.tar` & `VESIcal-1.2.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-03-29 20:22:32.415330 VESIcal-1.2.8/
--rw-r--r--   0 kiacovin   (502) staff       (20)     1090 2022-04-20 22:21:41.000000 VESIcal-1.2.8/LICENSE
--rw-r--r--   0 kiacovin   (502) staff       (20)     6433 2024-03-29 20:22:32.414173 VESIcal-1.2.8/PKG-INFO
--rw-r--r--   0 kiacovin   (502) staff       (20)     5731 2022-04-20 22:21:41.000000 VESIcal-1.2.8/README.md
-drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-03-29 20:22:32.387038 VESIcal-1.2.8/VESIcal/
--rw-r--r--   0 kiacovin   (502) staff       (20)    24598 2024-03-29 20:19:20.000000 VESIcal-1.2.8/VESIcal/__init__.py
--rw-r--r--   0 kiacovin   (502) staff       (20)     1442 2021-05-06 19:25:00.000000 VESIcal-1.2.8/VESIcal/activity_models.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    31143 2024-03-29 18:54:57.000000 VESIcal-1.2.8/VESIcal/batchfile.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    42471 2024-03-29 18:54:51.000000 VESIcal-1.2.8/VESIcal/batchmodel.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    21321 2024-03-29 18:54:57.000000 VESIcal-1.2.8/VESIcal/calculate_classes.py
--rw-r--r--   0 kiacovin   (502) staff       (20)     8577 2024-03-29 18:54:57.000000 VESIcal-1.2.8/VESIcal/calibration_checks.py
--rw-r--r--   0 kiacovin   (502) staff       (20)   112200 2021-06-07 18:27:21.000000 VESIcal-1.2.8/VESIcal/calibrations.py
--rw-r--r--   0 kiacovin   (502) staff       (20)     6929 2024-03-29 18:24:20.000000 VESIcal-1.2.8/VESIcal/core.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    47788 2021-06-07 20:27:39.000000 VESIcal-1.2.8/VESIcal/fugacity_models.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    34920 2024-03-29 18:54:57.000000 VESIcal-1.2.8/VESIcal/model_classes.py
-drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-03-29 20:22:32.399882 VESIcal-1.2.8/VESIcal/models/
--rw-r--r--   0 kiacovin   (502) staff       (20)     2596 2021-06-07 18:27:21.000000 VESIcal-1.2.8/VESIcal/models/__init__.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    22246 2023-10-17 16:01:15.000000 VESIcal-1.2.8/VESIcal/models/allison.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    17079 2023-10-17 16:01:45.000000 VESIcal-1.2.8/VESIcal/models/dixon.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    25128 2023-10-17 15:55:02.000000 VESIcal-1.2.8/VESIcal/models/iaconomarziano.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    22398 2024-03-29 18:54:57.000000 VESIcal-1.2.8/VESIcal/models/liu.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    44547 2024-03-29 20:17:34.000000 VESIcal-1.2.8/VESIcal/models/magmasat.py
--rw-r--r--   0 kiacovin   (502) staff       (20)     7777 2023-10-17 16:02:13.000000 VESIcal-1.2.8/VESIcal/models/moore.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    14812 2022-12-28 19:30:10.000000 VESIcal-1.2.8/VESIcal/models/shishkina.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    30013 2024-03-29 18:54:57.000000 VESIcal-1.2.8/VESIcal/sample_class.py
-drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-03-29 20:22:32.401686 VESIcal-1.2.8/VESIcal/tasplot/
--rw-r--r--   0 kiacovin   (502) staff       (20)     4700 2021-04-12 14:13:54.000000 VESIcal-1.2.8/VESIcal/tasplot/__init__.py
--rw-r--r--   0 kiacovin   (502) staff       (20)      627 2021-04-12 14:13:54.000000 VESIcal-1.2.8/VESIcal/tasplot/setup.py
-drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-03-29 20:22:32.406819 VESIcal-1.2.8/VESIcal/thermo/
--rw-r--r--   0 kiacovin   (502) staff       (20)        0 2022-04-21 23:11:18.000000 VESIcal-1.2.8/VESIcal/thermo/__init__.py
--rw-r--r--   0 kiacovin   (502) staff       (20)     1294 2022-04-21 23:11:18.000000 VESIcal-1.2.8/VESIcal/thermo/densityx.py
--rw-r--r--   0 kiacovin   (502) staff       (20)     9579 2024-03-29 18:54:57.000000 VESIcal-1.2.8/VESIcal/thermo/giordano.py
--rw-r--r--   0 kiacovin   (502) staff       (20)     4338 2022-04-21 23:11:18.000000 VESIcal-1.2.8/VESIcal/thermo/thermo_calculate_classes.py
--rw-r--r--   0 kiacovin   (502) staff       (20)     2511 2022-04-21 23:11:18.000000 VESIcal-1.2.8/VESIcal/thermo/thermo_core.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    40464 2024-03-21 15:43:49.000000 VESIcal-1.2.8/VESIcal/vplot.py
-drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-03-29 20:22:32.412699 VESIcal-1.2.8/VESIcal.egg-info/
--rw-r--r--   0 kiacovin   (502) staff       (20)     6433 2024-03-29 20:22:32.000000 VESIcal-1.2.8/VESIcal.egg-info/PKG-INFO
--rw-r--r--   0 kiacovin   (502) staff       (20)      993 2024-03-29 20:22:32.000000 VESIcal-1.2.8/VESIcal.egg-info/SOURCES.txt
--rw-r--r--   0 kiacovin   (502) staff       (20)        1 2024-03-29 20:22:32.000000 VESIcal-1.2.8/VESIcal.egg-info/dependency_links.txt
--rw-r--r--   0 kiacovin   (502) staff       (20)       45 2024-03-29 20:22:32.000000 VESIcal-1.2.8/VESIcal.egg-info/requires.txt
--rw-r--r--   0 kiacovin   (502) staff       (20)       14 2024-03-29 20:22:32.000000 VESIcal-1.2.8/VESIcal.egg-info/top_level.txt
--rw-r--r--   0 kiacovin   (502) staff       (20)       38 2024-03-29 20:22:32.415584 VESIcal-1.2.8/setup.cfg
--rw-r--r--   0 kiacovin   (502) staff       (20)      964 2024-03-29 20:19:31.000000 VESIcal-1.2.8/setup.py
-drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-03-29 20:22:32.411551 VESIcal-1.2.8/tests/
--rw-r--r--   0 kiacovin   (502) staff       (20)        0 2022-04-20 22:21:41.000000 VESIcal-1.2.8/tests/__init__.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    41305 2024-03-29 20:17:34.000000 VESIcal-1.2.8/tests/test_calculate.py
--rw-r--r--   0 kiacovin   (502) staff       (20)     2395 2024-03-29 20:17:34.000000 VESIcal-1.2.8/tests/test_importfile.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    15635 2024-03-29 20:17:34.000000 VESIcal-1.2.8/tests/test_manuscript.py
--rw-r--r--   0 kiacovin   (502) staff       (20)    24372 2024-03-29 20:17:34.000000 VESIcal-1.2.8/tests/test_sample.py
+drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-04-12 18:35:45.970925 VESIcal-1.2.9/
+-rw-r--r--   0 kiacovin   (502) staff       (20)     1090 2022-04-20 22:21:41.000000 VESIcal-1.2.9/LICENSE
+-rw-r--r--   0 kiacovin   (502) staff       (20)     6433 2024-04-12 18:35:45.969892 VESIcal-1.2.9/PKG-INFO
+-rw-r--r--   0 kiacovin   (502) staff       (20)     5731 2022-04-20 22:21:41.000000 VESIcal-1.2.9/README.md
+drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-04-12 18:35:45.943655 VESIcal-1.2.9/VESIcal/
+-rw-r--r--   0 kiacovin   (502) staff       (20)    24598 2024-04-12 18:33:05.000000 VESIcal-1.2.9/VESIcal/__init__.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)     1442 2021-05-06 19:25:00.000000 VESIcal-1.2.9/VESIcal/activity_models.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    31143 2024-03-29 18:54:57.000000 VESIcal-1.2.9/VESIcal/batchfile.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    42471 2024-03-29 18:54:51.000000 VESIcal-1.2.9/VESIcal/batchmodel.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    21321 2024-03-29 18:54:57.000000 VESIcal-1.2.9/VESIcal/calculate_classes.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)     8577 2024-04-12 18:33:05.000000 VESIcal-1.2.9/VESIcal/calibration_checks.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)   112200 2021-06-07 18:27:21.000000 VESIcal-1.2.9/VESIcal/calibrations.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)     6929 2024-03-29 18:24:20.000000 VESIcal-1.2.9/VESIcal/core.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    47788 2021-06-07 20:27:39.000000 VESIcal-1.2.9/VESIcal/fugacity_models.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    34921 2024-04-12 18:33:05.000000 VESIcal-1.2.9/VESIcal/model_classes.py
+drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-04-12 18:35:45.956605 VESIcal-1.2.9/VESIcal/models/
+-rw-r--r--   0 kiacovin   (502) staff       (20)     2596 2021-06-07 18:27:21.000000 VESIcal-1.2.9/VESIcal/models/__init__.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    22246 2023-10-17 16:01:15.000000 VESIcal-1.2.9/VESIcal/models/allison.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    17079 2023-10-17 16:01:45.000000 VESIcal-1.2.9/VESIcal/models/dixon.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    25128 2023-10-17 15:55:02.000000 VESIcal-1.2.9/VESIcal/models/iaconomarziano.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    22398 2024-03-29 18:54:57.000000 VESIcal-1.2.9/VESIcal/models/liu.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    44649 2024-04-12 18:33:05.000000 VESIcal-1.2.9/VESIcal/models/magmasat.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)     7777 2023-10-17 16:02:13.000000 VESIcal-1.2.9/VESIcal/models/moore.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    14812 2022-12-28 19:30:10.000000 VESIcal-1.2.9/VESIcal/models/shishkina.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    30013 2024-03-29 18:54:57.000000 VESIcal-1.2.9/VESIcal/sample_class.py
+drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-04-12 18:35:45.958269 VESIcal-1.2.9/VESIcal/tasplot/
+-rw-r--r--   0 kiacovin   (502) staff       (20)     4700 2021-04-12 14:13:54.000000 VESIcal-1.2.9/VESIcal/tasplot/__init__.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)      627 2021-04-12 14:13:54.000000 VESIcal-1.2.9/VESIcal/tasplot/setup.py
+drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-04-12 18:35:45.962292 VESIcal-1.2.9/VESIcal/thermo/
+-rw-r--r--   0 kiacovin   (502) staff       (20)        0 2022-04-21 23:11:18.000000 VESIcal-1.2.9/VESIcal/thermo/__init__.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)     1294 2022-04-21 23:11:18.000000 VESIcal-1.2.9/VESIcal/thermo/densityx.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)     9579 2024-03-29 18:54:57.000000 VESIcal-1.2.9/VESIcal/thermo/giordano.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)     4338 2022-04-21 23:11:18.000000 VESIcal-1.2.9/VESIcal/thermo/thermo_calculate_classes.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)     2511 2022-04-21 23:11:18.000000 VESIcal-1.2.9/VESIcal/thermo/thermo_core.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    40474 2024-04-12 18:33:05.000000 VESIcal-1.2.9/VESIcal/vplot.py
+drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-04-12 18:35:45.968690 VESIcal-1.2.9/VESIcal.egg-info/
+-rw-r--r--   0 kiacovin   (502) staff       (20)     6433 2024-04-12 18:35:45.000000 VESIcal-1.2.9/VESIcal.egg-info/PKG-INFO
+-rw-r--r--   0 kiacovin   (502) staff       (20)      993 2024-04-12 18:35:45.000000 VESIcal-1.2.9/VESIcal.egg-info/SOURCES.txt
+-rw-r--r--   0 kiacovin   (502) staff       (20)        1 2024-04-12 18:35:45.000000 VESIcal-1.2.9/VESIcal.egg-info/dependency_links.txt
+-rw-r--r--   0 kiacovin   (502) staff       (20)       45 2024-04-12 18:35:45.000000 VESIcal-1.2.9/VESIcal.egg-info/requires.txt
+-rw-r--r--   0 kiacovin   (502) staff       (20)       14 2024-04-12 18:35:45.000000 VESIcal-1.2.9/VESIcal.egg-info/top_level.txt
+-rw-r--r--   0 kiacovin   (502) staff       (20)       38 2024-04-12 18:35:45.971128 VESIcal-1.2.9/setup.cfg
+-rw-r--r--   0 kiacovin   (502) staff       (20)      964 2024-04-12 18:33:05.000000 VESIcal-1.2.9/setup.py
+drwxr-xr-x   0 kiacovin   (502) staff       (20)        0 2024-04-12 18:35:45.967335 VESIcal-1.2.9/tests/
+-rw-r--r--   0 kiacovin   (502) staff       (20)        0 2022-04-20 22:21:41.000000 VESIcal-1.2.9/tests/__init__.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    41305 2024-03-29 20:17:34.000000 VESIcal-1.2.9/tests/test_calculate.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)     2395 2024-03-29 20:17:34.000000 VESIcal-1.2.9/tests/test_importfile.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    16071 2024-04-12 18:33:05.000000 VESIcal-1.2.9/tests/test_manuscript.py
+-rw-r--r--   0 kiacovin   (502) staff       (20)    24372 2024-03-29 20:17:34.000000 VESIcal-1.2.9/tests/test_sample.py
```

### Comparing `VESIcal-1.2.8/LICENSE` & `VESIcal-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/PKG-INFO` & `VESIcal-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VESIcal
-Version: 1.2.8
+Version: 1.2.9
 Summary: A generalized python library for calculating and plotting various things related to mixed volatile (H2O-CO2) solubility in silicate melts.
 Home-page: https://github.com/kaylai/VESIcal
 Author: Kayla Iacovino, Simon Matthews, Penny Wieser
 Author-email: kaylaiacovino@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `VESIcal-1.2.8/README.md` & `VESIcal-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/__init__.py` & `VESIcal-1.2.9/VESIcal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 VESIcal
 
 A generalized python library for calculating and plotting various things
 related to mixed volatile (H2O-CO2) solubility in silicate melts.
 """
 
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 __author__ = "Kayla Iacovino, Simon Matthews, and Penny Wieser"
 
 # ----------------- IMPORTS ----------------- #
 import warnings as w
 import pandas as pd
 
 import VESIcal.core
```

### Comparing `VESIcal-1.2.8/VESIcal/activity_models.py` & `VESIcal-1.2.9/VESIcal/activity_models.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/batchfile.py` & `VESIcal-1.2.9/VESIcal/batchfile.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/batchmodel.py` & `VESIcal-1.2.9/VESIcal/batchmodel.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/calculate_classes.py` & `VESIcal-1.2.9/VESIcal/calculate_classes.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/calibration_checks.py` & `VESIcal-1.2.9/VESIcal/calibration_checks.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/calibrations.py` & `VESIcal-1.2.9/VESIcal/calibrations.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/core.py` & `VESIcal-1.2.9/VESIcal/core.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/fugacity_models.py` & `VESIcal-1.2.9/VESIcal/fugacity_models.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/model_classes.py` & `VESIcal-1.2.9/VESIcal/model_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             samplecopy = kwargs['sample'].change_composition(
                              {self.volatile_species[0]: result0},
                              inplace=False)
             kwargs['sample'] = samplecopy
             result1 = self.models[1].calculate_dissolved_volatiles(
                             pressure=pressure, X_fluid=X_fluid[1], **kwargs)
             result = (result0, result1)
-        elif(len(self.models) == 2 and
+        elif (len(self.models) == 2 and
              self.models[1].solubility_dependence is False and
              'sample' in kwargs):
             result1 = self.models[1].calculate_dissolved_volatiles(
                                pressure=pressure, X_fluid=X_fluid[1], **kwargs)
             samplecopy = kwargs['sample'].change_composition(
                             {self.volatile_species[1]: result1}, inplace=False)
             kwargs['sample'] = samplecopy
```

### Comparing `VESIcal-1.2.8/VESIcal/models/__init__.py` & `VESIcal-1.2.9/VESIcal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/models/allison.py` & `VESIcal-1.2.9/VESIcal/models/allison.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/models/dixon.py` & `VESIcal-1.2.9/VESIcal/models/dixon.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/models/iaconomarziano.py` & `VESIcal-1.2.9/VESIcal/models/iaconomarziano.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/models/liu.py` & `VESIcal-1.2.9/VESIcal/models/liu.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/models/magmasat.py` & `VESIcal-1.2.9/VESIcal/models/magmasat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1103,15 +1103,14 @@
             (status, temp, p, xmlout) = output[0]
             liq_comp = self.melts.get_composition_of_phase(xmlout, phase_name="Liquid")
             fl_comp = self.melts.get_composition_of_phase(xmlout, phase_name="Fluid",
                                                           mode="component")
             liq_mass = self.melts.get_mass_of_phase(xmlout, phase_name="Liquid")
             fl_mass = self.melts.get_mass_of_phase(xmlout, phase_name="Fluid")
             fl_wtper = 100 * fl_mass / (fl_mass + liq_mass)
-
             if fl_mass > 0:
                 press.append(p * 10.0)
                 try:
                     H2Oliq.append(liq_comp["H2O"])
                 except Exception:
                     H2Oliq.append(0)
                 try:
@@ -1134,14 +1133,17 @@
                                            (1.0 - fractionate_vapor))
                 except Exception:
                     _sample_dict["H2O"] = 0
                 try:
                     _sample_dict["CO2"] = (liq_comp["CO2"] +
                                            (_sample_dict["CO2"] - liq_comp["CO2"]) *
                                            (1.0 - fractionate_vapor))
+                    if _sample_dict["CO2"] < 1e-10:
+                        _sample_dict["CO2"] = 0.0
+
                 except Exception:
                     _sample_dict["CO2"] = 0
             _sample = sample_class.Sample(_sample_dict)
             _sample_dict = _sample.get_composition(normalization="standard", units="wtpt_oxides")
 
         self.melts.set_bulk_composition(self.bulk_comp_orig)  # this needs to be reset always!
         open_degassing_df = pd.DataFrame(list(zip(press, H2Oliq, CO2liq, H2Ofl, CO2fl,
```

### Comparing `VESIcal-1.2.8/VESIcal/models/moore.py` & `VESIcal-1.2.9/VESIcal/models/moore.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/models/shishkina.py` & `VESIcal-1.2.9/VESIcal/models/shishkina.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/sample_class.py` & `VESIcal-1.2.9/VESIcal/sample_class.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/tasplot/__init__.py` & `VESIcal-1.2.9/VESIcal/tasplot/__init__.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/tasplot/setup.py` & `VESIcal-1.2.9/VESIcal/tasplot/setup.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/thermo/densityx.py` & `VESIcal-1.2.9/VESIcal/thermo/densityx.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/thermo/giordano.py` & `VESIcal-1.2.9/VESIcal/thermo/giordano.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/thermo/thermo_calculate_classes.py` & `VESIcal-1.2.9/VESIcal/thermo/thermo_calculate_classes.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/thermo/thermo_core.py` & `VESIcal-1.2.9/VESIcal/thermo/thermo_core.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/VESIcal/vplot.py` & `VESIcal-1.2.9/VESIcal/vplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     # Define color cycler based on plot style set here
     # get style formatting set by plt.style.use():
     the_rc = plt.style.library[style]
     # list of colors by hex code:
     color_list = the_rc['axes.prop_cycle'].by_key()['color'] * 10
     color_cyler = the_rc['axes.prop_cycle']  # get the cycler
 
-except:
+except Exception:
     style = "seaborn-v0_8-colorblind"  # new style name as of 3.6.0
     plt.style.use(style)
 
     # Define color cycler based on plot style set here
     # get style formatting set by plt.style.use():
     the_rc = plt.style.library[style]
     # list of colors by hex code:
```

### Comparing `VESIcal-1.2.8/VESIcal.egg-info/PKG-INFO` & `VESIcal-1.2.9/VESIcal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VESIcal
-Version: 1.2.8
+Version: 1.2.9
 Summary: A generalized python library for calculating and plotting various things related to mixed volatile (H2O-CO2) solubility in silicate melts.
 Home-page: https://github.com/kaylai/VESIcal
 Author: Kayla Iacovino, Simon Matthews, Penny Wieser
 Author-email: kaylaiacovino@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `VESIcal-1.2.8/VESIcal.egg-info/SOURCES.txt` & `VESIcal-1.2.9/VESIcal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/setup.py` & `VESIcal-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="VESIcal",
-    version="1.2.8",
+    version="1.2.9",
     author="Kayla Iacovino, Simon Matthews, Penny Wieser",
     author_email="kaylaiacovino@gmail.com",
     description=("A generalized python library for calculating and plotting various things "
                  "related to mixed volatile (H2O-CO2) solubility in silicate melts."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kaylai/VESIcal",
```

### Comparing `VESIcal-1.2.8/tests/test_calculate.py` & `VESIcal-1.2.9/tests/test_calculate.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/tests/test_importfile.py` & `VESIcal-1.2.9/tests/test_importfile.py`

 * *Files identical despite different names*

### Comparing `VESIcal-1.2.8/tests/test_manuscript.py` & `VESIcal-1.2.9/tests/test_manuscript.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,15 +58,16 @@
 class TestManuscriptCalculations(unittest.TestCase):
     """
     Some of the "correct" values hard coded here are not exactly the same as those in the
     manuscript. However, they are very very close and likely are different because of changes
     to normalization routines made after publication. I've noted original values in commented
     text below where they differ from currently accepted values.
 
-    Current values last updated March 2024 by Kayla Iacovino.
+    Current values last updated March 2024 by Kayla Iacovino. 
+    Some degassing paths updated March 2024 by Simon Matthews (see comments below).
     """
     def setUp(self):
         # import any pickled objects
         with open(PICKLE_DISSOLVED, "rb") as f:
             self.pickle_dissolved = pickle.load(f)
 
         with open(PICKLE_EQFLUID, "rb") as f:
@@ -93,15 +94,15 @@
         with open(PICKLE_ISOPLETHS, "rb") as f:
             self.pickle_isopleths = pickle.load(f)
         
         with open(PICKLE_CLOSED_DF, "rb") as f:
             self.pickle_closed_df = pickle.load(f)
         
         with open(PICKLE_OPEN_DF, "rb") as f:
-            self.pickle_open_df = pickle.load(f)
+            self.pickle_open_df = pickle.load(f) # Updated following bug fix. SM.
         
         with open(PICKLE_HALF_DF, "rb") as f:
             self.pickle_half_df = pickle.load(f)
         
         with open(PICKLE_EXSOLVED_DF, "rb") as f:
             self.pickle_exsolved_df = pickle.load(f)
         
@@ -205,44 +206,46 @@
          'H2O': 0.994713385706339}
         """
     
     def test_degassing_paths(self):
         print_msg_box("TestManuscript \ndegassing_paths")
         """Calculate open, closed, and closed + 2 wt% initial vapor"""
         closed_df = v.calculate_degassing_path(sample=self.sample_10star, temperature=1200).result
-        assert_frame_equal(closed_df, self.pickle_closed_df)
+        assert_frame_equal(closed_df, self.pickle_closed_df, atol=1e-4)
 
         open_df = v.calculate_degassing_path(sample=self.sample_10star, temperature=1200,
                                              fractionate_vapor=1.0).result
-        assert_frame_equal(open_df, self.pickle_open_df)
+        assert_frame_equal(open_df, self.pickle_open_df, atol=1e-4)
 
         half_df = v.calculate_degassing_path(sample=self.sample_10star, temperature=1200,
                                              fractionate_vapor=0.5).result
-        assert_frame_equal(half_df, self.pickle_half_df)
+        assert_frame_equal(half_df, self.pickle_half_df, atol=5e-4)
 
         exsolved_df = v.calculate_degassing_path(sample=self.sample_10star, temperature=1200,
                                                  init_vapor=2.0).result
-        assert_frame_equal(exsolved_df, self.pickle_exsolved_df)
+        assert_frame_equal(exsolved_df, self.pickle_exsolved_df, atol=1e-4)
 
         """Calculate closed-system degassing starting from a pressure of 2000 bars"""
         start2000_df = v.calculate_degassing_path(sample=self.sample_10star, temperature=1200,
                                                   pressure=2000.0).result
-        assert_frame_equal(start2000_df, self.pickle_start2000_df)
+        assert_frame_equal(start2000_df, self.pickle_start2000_df, atol=1e-4)
     
     def test_dissolved_batch(self):
         print_msg_box("TestManuscript \ndissolved_batch")
         result = self.myfile.calculate_dissolved_volatiles(temperature=900.0, pressure=2000.0,
                                                            X_fluid=1, print_status=True)
         assert_frame_equal(result, self.pickle_dissolved)
     
     def test_dissolved_volatiles_sample_10star(self):
         print_msg_box("TestManuscript \ndissolved_volatiles_sample_10star")
         result = v.calculate_dissolved_volatiles(sample=self.sample_10star, temperature=900.0,
                                                  pressure=2000.0, X_fluid=0.5, verbose=True).result
-        self.assertDictEqual(result, self.tenstar_verbose_diss_vol)
+        params = list(result.keys())
+        for param in params:
+            self.assertAlmostEqual(result[param], self.tenstar_verbose_diss_vol[param])
     
     def test_eqfluid_batch(self):
         print_msg_box("TestManuscript \neqfluid_batch")
         result = self.myfile.calculate_equilibrium_fluid_comp(temperature=900.0, pressure=1000.0)
         assert_frame_equal(result, self.pickle_eqfluid)
     
     def test_eqfluid_batch_wTemps(self):
@@ -260,15 +263,16 @@
         result = v.fluid_wt_to_molfrac(self.pickle_eqfluid_wt)
         assert_frame_equal(result, self.pickle_eqfluid_mol)
     
     def test_equilibrium_fluid_sample_10star(self):
         print_msg_box("TestManuscript \nequilibrium_fluid_sample_10star")
         result = v.calculate_equilibrium_fluid_comp(sample=self.sample_10star, temperature=900.0,
                                                     pressure=100.0).result
-        self.assertDictEqual(result, self.tenstar_eqfluid)
+        self.assertAlmostEqual(result['H2O'], self.tenstar_eqfluid['H2O'])
+        self.assertAlmostEqual(result['CO2'], self.tenstar_eqfluid['CO2'])
     
     def test_isobars_and_isopleths(self):
         print_msg_box("TestManuscript \nisobars_and_isopleths")
         result_isobars, result_isopleths = v.calculate_isobars_and_isopleths(
                                             sample=self.sample_10star, 
                                             temperature=1200.0,
                                             pressure_list=[1000.0, 2000.0, 3000.0],
@@ -311,8 +315,10 @@
         result = self.myfile.calculate_saturation_pressure(temperature="Temp")
         assert_frame_equal(result, self.pickle_satPs_wTemps)
     
     def test_saturation_pressure_mysample(self):
         print_msg_box("TestManuscript \nsaturation_pressure_mysample")
         result = v.calculate_saturation_pressure(sample=self.mysample, temperature=925.0,
                                                  verbose=True).result
-        self.assertDictEqual(result, self.mysample_satP)
+        params = list(result.keys())
+        for param in params:
+            self.assertAlmostEqual(result[param], self.mysample_satP[param])
```

### Comparing `VESIcal-1.2.8/tests/test_sample.py` & `VESIcal-1.2.9/tests/test_sample.py`

 * *Files identical despite different names*

