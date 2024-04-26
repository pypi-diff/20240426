# Comparing `tmp/lt-gee-py-0.0.1a2.tar.gz` & `tmp/lt_gee_py-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lt-gee-py-0.0.1a2.tar", last modified: Mon Mar 11 21:28:44 2024, max compression
+gzip compressed data, was "lt_gee_py-0.0.1a3.tar", last modified: Fri Apr 26 00:53:33 2024, max compression
```

## Comparing `lt-gee-py-0.0.1a2.tar` & `lt_gee_py-0.0.1a3.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:28:44.238308 lt-gee-py-0.0.1a2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:28:44.234308 lt-gee-py-0.0.1a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:28:44.238308 lt-gee-py-0.0.1a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19690 2024-03-11 21:28:44.238308 lt-gee-py-0.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:28:44.238308 lt-gee-py-0.0.1a2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    49520 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/examples/basic_examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 21:28:44.238308 lt-gee-py-0.0.1a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:28:44.234308 lt-gee-py-0.0.1a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:28:44.238308 lt-gee-py-0.0.1a2/src/lt_gee_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19690 2024-03-11 21:28:44.000000 lt-gee-py-0.0.1a2/src/lt_gee_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-11 21:28:44.000000 lt-gee-py-0.0.1a2/src/lt_gee_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 21:28:44.000000 lt-gee-py-0.0.1a2/src/lt_gee_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-11 21:28:44.000000 lt-gee-py-0.0.1a2/src/lt_gee_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:28:44.238308 lt-gee-py-0.0.1a2/src/ltgee/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/src/ltgee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/src/ltgee/gee_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43841 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/src/ltgee/landtrendr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:28:44.238308 lt-gee-py-0.0.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-03-11 21:28:39.000000 lt-gee-py-0.0.1a2/test/test_landtrendr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.108868 lt_gee_py-0.0.1a3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.104868 lt_gee_py-0.0.1a3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.104868 lt_gee_py-0.0.1a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-04-26 00:53:33.108868 lt_gee_py-0.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.104868 lt_gee_py-0.0.1a3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    33927 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/examples/basic_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 00:53:33.108868 lt_gee_py-0.0.1a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.104868 lt_gee_py-0.0.1a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.108868 lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-04-26 00:53:33.000000 lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-26 00:53:33.000000 lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 00:53:33.000000 lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 00:53:33.000000 lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.108868 lt_gee_py-0.0.1a3/src/ltgee/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/src/ltgee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/src/ltgee/gee_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44824 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/src/ltgee/landtrendr.py
```

### Comparing `lt-gee-py-0.0.1a2/.github/workflows/python-publish.yml` & `lt_gee_py-0.0.1a3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lt-gee-py-0.0.1a2/.gitignore` & `lt_gee_py-0.0.1a3/.gitignore`

 * *Files identical despite different names*

### Comparing `lt-gee-py-0.0.1a2/CONTRIBUTING.md` & `lt_gee_py-0.0.1a3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lt-gee-py-0.0.1a2/LICENSE` & `lt_gee_py-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `lt-gee-py-0.0.1a2/PKG-INFO` & `lt_gee_py-0.0.1a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lt-gee-py
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: Python interface to the Google Earth Engine implementation of the LandTrendr spectral-temporal segmentation algorithm.
 Author-email: Myscon Truong <myscontruong@gmail.com>, Robert Kennedy <robert.kennedy@oregonstate.edu>, Peter Clary <clarype@oregonstate.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,15 +224,15 @@
 # lt-gee-py
 Python interface to the Google Earth Engine implementation of the LandTrendr spectral-temporal segmentation algorithm.
 
 ## Introduction
 
 **LandTrendr** is set of spectral-temporal segmentation algorithms that are useful for change detection in a time series of moderate resolution satellite imagery (primarily Landsat) and for generating trajectory-based spectral time series data largely absent of inter-annual signal noise. LT was originally implemented in IDL (Interactive Data Language), but with the help of engineers at Google, it has been ported to the GEE platform.
 
-The **LandTrendr** class from **lt-gee-py** is a light wrapper around the Google Earth Engine API that includes convenience methods to generate images and collections in the format required for LandTrendr on GEE. 
+The **LandTrendr** class from **lt-gee-py** is a light wrapper around the Google Earth Engine API that includes convenience methods to generate images and collections in the format required for LandTrendr on GEE. Please be aware this package is in alpha and may change.
 
 ## Getting Started
 
 ### Download and Install packages and dependencies
 
 - Install the Python API for Google Earth Engine. This is the only dependency thus far.
 
@@ -260,22 +260,41 @@
 import ee
 from ltgee import LandTrendr
 
 # Initialize access to Google's EE servers
 ee.Initialize("my_project_name")
 
 # Initialize variables for LandTrendr algorithm
-lt_params = {
+composite_params = {
     "start_date": date(1985, 6,1),
     "end_date": date(2017, 9,1),
-    "index": 'NBR',
-    "ftv_list": ['TCB', 'TCG', 'TCW', 'NBR'],
+    "area_of_interest": ee.Geometry({
+        'type': 'Polygon',
+        'coordinates': [
+            [
+                [-122.37202331327023,44.62585686599272],
+                [-122.26765319608273,44.62585686599272],
+                [-122.26765319608273,44.696185837887384],
+                [-122.37202331327023,44.696185837887384],
+                [-122.37202331327023,44.62585686599272],
+                ]
+            ]
+    }),
     "mask_labels": ['cloud', 'shadow', 'snow', 'water'],
-
-    "area_of_interest": ee.Geometry.Point(-122.8848, 43.7929),
+    "debug": True
+}
+lt_collection_params = {
+        "sr_collection": LandsatComposite(**composite_params),
+        # "sr_collection": composite_params, # - you may also just pass in your own collection or the params directly. Note: in the former, some methods in the class may not work.
+        "index": 'NBR',
+        "ftv_list": ['TCB', 'TCG', 'TCW', 'NBR'],
+}
+lt_params = {
+    "lt_collection": LtCollection(**lt_collection_params),
+    # "lt_collection": lt_collection_params, # - you may also just pass in your own collection or the params directly. Note: in the former, some methods in the class may not work.
     "run_params": {
             "maxSegments": 6,
             "spikeThreshold": 0.9,
             "vertexCountOvershoot":  3,
             "preventOneYearRecovery":  True,
             "recoveryThreshold":  0.25,
             "pvalThreshold":  .05,
```

### Comparing `lt-gee-py-0.0.1a2/README.md` & `lt_gee_py-0.0.1a3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # lt-gee-py
 Python interface to the Google Earth Engine implementation of the LandTrendr spectral-temporal segmentation algorithm.
 
 ## Introduction
 
 **LandTrendr** is set of spectral-temporal segmentation algorithms that are useful for change detection in a time series of moderate resolution satellite imagery (primarily Landsat) and for generating trajectory-based spectral time series data largely absent of inter-annual signal noise. LT was originally implemented in IDL (Interactive Data Language), but with the help of engineers at Google, it has been ported to the GEE platform.
 
-The **LandTrendr** class from **lt-gee-py** is a light wrapper around the Google Earth Engine API that includes convenience methods to generate images and collections in the format required for LandTrendr on GEE. 
+The **LandTrendr** class from **lt-gee-py** is a light wrapper around the Google Earth Engine API that includes convenience methods to generate images and collections in the format required for LandTrendr on GEE. Please be aware this package is in alpha and may change.
 
 ## Getting Started
 
 ### Download and Install packages and dependencies
 
 - Install the Python API for Google Earth Engine. This is the only dependency thus far.
 
@@ -37,22 +37,41 @@
 import ee
 from ltgee import LandTrendr
 
 # Initialize access to Google's EE servers
 ee.Initialize("my_project_name")
 
 # Initialize variables for LandTrendr algorithm
-lt_params = {
+composite_params = {
     "start_date": date(1985, 6,1),
     "end_date": date(2017, 9,1),
-    "index": 'NBR',
-    "ftv_list": ['TCB', 'TCG', 'TCW', 'NBR'],
+    "area_of_interest": ee.Geometry({
+        'type': 'Polygon',
+        'coordinates': [
+            [
+                [-122.37202331327023,44.62585686599272],
+                [-122.26765319608273,44.62585686599272],
+                [-122.26765319608273,44.696185837887384],
+                [-122.37202331327023,44.696185837887384],
+                [-122.37202331327023,44.62585686599272],
+                ]
+            ]
+    }),
     "mask_labels": ['cloud', 'shadow', 'snow', 'water'],
-
-    "area_of_interest": ee.Geometry.Point(-122.8848, 43.7929),
+    "debug": True
+}
+lt_collection_params = {
+        "sr_collection": LandsatComposite(**composite_params),
+        # "sr_collection": composite_params, # - you may also just pass in your own collection or the params directly. Note: in the former, some methods in the class may not work.
+        "index": 'NBR',
+        "ftv_list": ['TCB', 'TCG', 'TCW', 'NBR'],
+}
+lt_params = {
+    "lt_collection": LtCollection(**lt_collection_params),
+    # "lt_collection": lt_collection_params, # - you may also just pass in your own collection or the params directly. Note: in the former, some methods in the class may not work.
     "run_params": {
             "maxSegments": 6,
             "spikeThreshold": 0.9,
             "vertexCountOvershoot":  3,
             "preventOneYearRecovery":  True,
             "recoveryThreshold":  0.25,
             "pvalThreshold":  .05,
```

### Comparing `lt-gee-py-0.0.1a2/pyproject.toml` & `lt_gee_py-0.0.1a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lt-gee-py-0.0.1a2/src/lt_gee_py.egg-info/PKG-INFO` & `lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lt-gee-py
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: Python interface to the Google Earth Engine implementation of the LandTrendr spectral-temporal segmentation algorithm.
 Author-email: Myscon Truong <myscontruong@gmail.com>, Robert Kennedy <robert.kennedy@oregonstate.edu>, Peter Clary <clarype@oregonstate.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,15 +224,15 @@
 # lt-gee-py
 Python interface to the Google Earth Engine implementation of the LandTrendr spectral-temporal segmentation algorithm.
 
 ## Introduction
 
 **LandTrendr** is set of spectral-temporal segmentation algorithms that are useful for change detection in a time series of moderate resolution satellite imagery (primarily Landsat) and for generating trajectory-based spectral time series data largely absent of inter-annual signal noise. LT was originally implemented in IDL (Interactive Data Language), but with the help of engineers at Google, it has been ported to the GEE platform.
 
-The **LandTrendr** class from **lt-gee-py** is a light wrapper around the Google Earth Engine API that includes convenience methods to generate images and collections in the format required for LandTrendr on GEE. 
+The **LandTrendr** class from **lt-gee-py** is a light wrapper around the Google Earth Engine API that includes convenience methods to generate images and collections in the format required for LandTrendr on GEE. Please be aware this package is in alpha and may change.
 
 ## Getting Started
 
 ### Download and Install packages and dependencies
 
 - Install the Python API for Google Earth Engine. This is the only dependency thus far.
 
@@ -260,22 +260,41 @@
 import ee
 from ltgee import LandTrendr
 
 # Initialize access to Google's EE servers
 ee.Initialize("my_project_name")
 
 # Initialize variables for LandTrendr algorithm
-lt_params = {
+composite_params = {
     "start_date": date(1985, 6,1),
     "end_date": date(2017, 9,1),
-    "index": 'NBR',
-    "ftv_list": ['TCB', 'TCG', 'TCW', 'NBR'],
+    "area_of_interest": ee.Geometry({
+        'type': 'Polygon',
+        'coordinates': [
+            [
+                [-122.37202331327023,44.62585686599272],
+                [-122.26765319608273,44.62585686599272],
+                [-122.26765319608273,44.696185837887384],
+                [-122.37202331327023,44.696185837887384],
+                [-122.37202331327023,44.62585686599272],
+                ]
+            ]
+    }),
     "mask_labels": ['cloud', 'shadow', 'snow', 'water'],
-
-    "area_of_interest": ee.Geometry.Point(-122.8848, 43.7929),
+    "debug": True
+}
+lt_collection_params = {
+        "sr_collection": LandsatComposite(**composite_params),
+        # "sr_collection": composite_params, # - you may also just pass in your own collection or the params directly. Note: in the former, some methods in the class may not work.
+        "index": 'NBR',
+        "ftv_list": ['TCB', 'TCG', 'TCW', 'NBR'],
+}
+lt_params = {
+    "lt_collection": LtCollection(**lt_collection_params),
+    # "lt_collection": lt_collection_params, # - you may also just pass in your own collection or the params directly. Note: in the former, some methods in the class may not work.
     "run_params": {
             "maxSegments": 6,
             "spikeThreshold": 0.9,
             "vertexCountOvershoot":  3,
             "preventOneYearRecovery":  True,
             "recoveryThreshold":  0.25,
             "pvalThreshold":  .05,
```

### Comparing `lt-gee-py-0.0.1a2/src/ltgee/gee_utils.py` & `lt_gee_py-0.0.1a3/src/ltgee/gee_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 import ee
 import math
 
 
-def calculate_median_diff(img, median):
+def count_clear_view_pixels(collection: ee.ImageCollection) -> ee.Image:
+    """
+    Counts the number of clear view pixels for the given collection.
+
+    Args:
+        collection (ee.ImageCollection): The image collection.
+
+    Returns:
+        ee.Image: The image containing the number of clear view pixels.
+    """
+    binary = collection.map(lambda image: image.select(
+        0).multiply(0).add(1).unmask(0))
+    return binary.sum()
+
+
+def calculate_median_diff(img: ee.Image, median: ee.Image) -> ee.Image:
     """
     Calculates the difference between an image and a given median value.
 
     Parameters:
         img (ee.Image): The input image.
         median (ee.Image): The median image.
 
     Returns:
         ee.Image: The difference image with an additional band representing the input image.
     """
     diff = img.subtract(median).pow(ee.Image.constant(2))
     return diff.reduce('sum').addBands(img)
 
 
-def forest_mask(aoi):
+def forest_mask(aoi: ee.Geometry) -> ee.Image:
     """
     Generate a forest mask for a given area of interest (AOI).
 
     Parameters:
     aoi (ee.Geometry): The area of interest for which the forest mask is generated.
 
     Returns:
@@ -34,15 +49,15 @@
         'Band >= 0 ? 1 : 0', {
             'Band': forest_image
         }
     )
     return selected_forests.clip(aoi)
 
 
-def water_mask(aoi):
+def water_mask(aoi: ee.Geometry) -> ee.Image:
     """
     Generate a water mask to the given area of interest (aoi).
 
     Parameters:
     aoi (ee.Geometry): The area of interest to apply the water mask to.
 
     Returns:
@@ -53,15 +68,15 @@
         'band > 99 ? 0 : 1', {
             'band': mapped_water.select('recurrence')
         }
     )
     return mapped_water_binary.clip(aoi)
 
 
-def standardize_collection(collection):
+def standardize_collection(collection: ee.ImageCollection) -> ee.ImageCollection:
     """
     Standardizes the given collection by subtracting the mean and dividing by the standard deviation.
 
     Args:
         collection (ee.ImageCollection): The image collection to be standardized.
 
     Returns:
@@ -70,15 +85,16 @@
     mean = collection.reduce(ee.Reducer.mean())
     std_dev = collection.reduce(ee.Reducer.stdDev())
     mean_adj = collection.map(lambda img: img.subtract(mean)
                               .set('system:time_start', img.get('system:time_start')))
     return mean_adj.map(lambda img: img.divide(std_dev).set('system:time_start', img.get('system:time_start')))
 
 
-def tc_transform(img, color_bands=['B1', 'B2', 'B3', 'B4', 'B5', 'B7']):
+def tc_transform(img: ee.Image,
+                 color_bands: list[str] = ['B1', 'B2', 'B3', 'B4', 'B5', 'B7']) -> ee.Image:
     b = ee.Image(img).select(color_bands)
 
     brt_coeffs = ee.Image.constant(
         [0.2043, 0.4158, 0.5524, 0.5741, 0.3124, 0.2303])
     grn_coeffs = ee.Image.constant(
         [-0.1603, -0.2819, -0.4934, 0.7940, -0.0002, -0.1446])
     wet_coeffs = ee.Image.constant(
@@ -94,22 +110,22 @@
     return brightness.addBands(greenness) \
         .addBands(wetness) \
         .addBands(angle) \
         .select([0, 1, 2, 3], ['TCB', 'TCG', 'TCW', 'TCA'])\
         .set('system:time_start', img.get('system:time_start'))
 
 
-def nbr_transform(img):
+def nbr_transform(img: ee.Image) -> ee.Image:
     return img.normalizedDifference(['B4', 'B7']) \
         .multiply(1000) \
         .select([0], ['NBR']) \
         .set('system:time_start', img.get('system:time_start'))
 
 
-def ndfi_transform(img):
+def ndfi_transform(img: ee.Image) -> ee.Image:
     params = {
         'cfThreshold': 0.01,
         'soil': [2000, 3000, 3400, 5800, 6000, 5800],
         'gv': [500, 900, 400, 6100, 3000, 1000],
         'npv': [1400, 1700, 2200, 3000, 5500, 3000],
         'shade': [0, 0, 0, 0, 0, 0],
         'cloud': [9000, 9600, 8000, 7800, 7200, 6500]
@@ -146,39 +162,48 @@
         .select(['band_0', 'band_1', 'band_2', 'band_3', 'NDFI', 'NDVI', 'EVI', 'B1', 'B2', 'B3', 'B4', 'B5']) \
         .rename(['GV', 'Shade', 'NPV', 'Soil', 'NDFI', 'NDVI', 'EVI', 'Blue', 'Green', 'Red', 'NIR', 'SWIR1'])
 
     return to_exp.select(['NDFI']).multiply(1000).set(
         'system:time_start', img.get('system:time_start'))
 
 
-def ndvi_transform(img, nir_band_name='B4', red_band_name='B5'):
+def ndvi_transform(img: ee.Image,
+                   nir_band_name: str = 'B4',
+                   red_band_name: str = 'B5') -> ee.Image:
     ndvi = img.normalizedDifference([nir_band_name, red_band_name]) \
         .multiply(1000) \
         .select([0], ['NDVI']) \
         .set('system:time_start', img.get('system:time_start'))
     return ndvi
 
 
-def ndsi_transform(img, swir_band_name='B5', green_band_name='B2'):
+def ndsi_transform(img: ee.Image,
+                   swir_band_name: str = 'B5',
+                   green_band_name: str = 'B2') -> ee.Image:
     ndsi = img.normalizedDifference([green_band_name, swir_band_name]) \
         .multiply(1000) \
         .select([0], ['NDSI']) \
         .set('system:time_start', img.get('system:time_start'))
     return ndsi
 
 
-def ndmi_transform(img, nir_band_name='B4', swir_band_name='B5'):
+def ndmi_transform(img: ee.Image,
+                   nir_band_name: str = 'B4',
+                   swir_band_name: str = 'B5') -> ee.Image:
     ndmi = img.normalizedDifference([nir_band_name, swir_band_name]) \
         .multiply(1000) \
         .select([0], ['NDMI']) \
         .set('system:time_start', img.get('system:time_start'))
     return ndmi
 
 
-def evi_transform(img, nir_band_name='B4', red_band_name='B3', blue_band_name='B1'):
+def evi_transform(img: ee.Image,
+                  nir_band_name: str = 'B4',
+                  red_band_name: str = 'B3',
+                  blue_band_name: str = 'B1') -> ee.Image:
     evi = img.expression(
         '2.5 * ((NIR - RED) / (NIR + 6 * RED - 7.5 * BLUE + 1))', {
             'NIR': img.select(nir_band_name),
             'RED': img.select(red_band_name),
             'BLUE': img.select(blue_band_name)
         }) \
         .multiply(1000) \
```

### Comparing `lt-gee-py-0.0.1a2/src/ltgee/landtrendr.py` & `lt_gee_py-0.0.1a3/src/ltgee/landtrendr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,239 +1,259 @@
 import ee
-from .gee_utils import water_mask, forest_mask, calculate_median_diff, tc_transform, ndvi_transform, ndmi_transform, ndsi_transform, nbr_transform, evi_transform, ndfi_transform, standardize_collection
 
+from datetime import datetime
+from typing import Optional
 
-class LandTrendr:
+from .gee_utils import (count_clear_view_pixels,
+                        water_mask,
+                        forest_mask,
+                        calculate_median_diff,
+                        tc_transform,
+                        ndvi_transform,
+                        ndmi_transform,
+                        ndsi_transform,
+                        nbr_transform,
+                        evi_transform,
+                        ndfi_transform,
+                        standardize_collection)
+
+
+class LandsatComposite(ee.ImageCollection):
     """
-    ### Landtrendr class for performing landtrendr analysis using Google Earth Engine.
+    ### LandsatComposite class for building a Landsat surface reflectance composite for use in LandTrendr.
 
     #### Args:
-    start_date (datetime):          The start date of the analysis.
-    end_date (datetime):            The end date of the analysis.
-    area_of_interest (ee.Geometry):              The area of interest for the analysis.
-    index (str):                    The index to be used for the analysis.
-    ftv_list (list, optional):      List of additional feature variables. Defaults to [].
-    mask_labels (list, optional):   List of mask labels. Defaults to ['cloud', 'shadow', 'snow'].
-    exclude (dict, optional):       Dictionary of image ids to be excluded. Defaults to {}.
-    debug (bool, optional):         Whether to run in debug mode. Defaults to False.
-    run (bool, optional):           Whether to run the run method immediately. Defaults to True.
-    run_params (:obj:, optional):    Dictionary of run parameters (See below).
-        {
-            maxSegments (int, optional):                Maximum number of segments. Defaults to 6.
-            spikeThreshold (float, optional):           Spike threshold. Defaults to 0.9.
-            vertexCountOvershoot (int, optional):       Vertex count overshoot. Defaults to 3.
-            preventOneYearRecovery (bool, optional):    Prevent one year recovery. Defaults to True.
-            recoveryThreshold (float, optional):        Recovery threshold. Defaults to 0.25.
-            pvalThreshold (float, optional):            P-value threshold. Defaults to 0.25.
-            bestModelProportion (float, optional):      Best model proportion. Defaults to 0.75.
-            minObservationsNeeded (int, optional):      Minimum number of observations needed. Defaults to 6.
-        }
+        collection (ee.ImageCollection, optional):  An ee.ImageCollection of Landsat surface reflectance images. Defaults to None.
+        start_date (datetime, optional): The start date of the annual composites. Defaults to None.
+        end_date (datetime, optional): The end date of the annual composites. Defaults to None.
+        area_of_interest (ee.Geometry, optional): The area of interest for the composite. Defaults to None.
+        mask_labels (list, optional): A list of mask labels to apply to the composite. Defaults to ['cloud', 'shadow', 'snow'].
+        exclude (dict, optional): A dictionary of exclude criteria. Defaults to {}.
+        debug (bool, optional): Whether to calculate the number of clear view pixels. Defaults to False.
     """
-
+    _band_names = ['B1', 'B2', 'B3', 'B4', 'B5', 'B7']
     _mask_options = ['cloud', 'shadow', 'snow',
                      'water', 'waterplus', 'nonforest']
-    _valid_indices = ['B1', 'B2', 'B3', 'B4', 'B5', 'B7', 'NBR',
-                      'NDMI', 'NDVI', 'NDSI', 'EVI', 'NDFI', 'TCB', 'TCG', 'TCW', 'TCA']
-    _valid_indices_alt = ['TCC', 'TCM', 'TCS', 'ENC', 'ENM', 'ENS', 'ENC1',
-                          'ENM1', 'ENS1', 'B5z', 'B7z', 'TCWz', 'TCAz', 'NDMIz', 'NBRz']
-    _default_run_params = {
-        "maxSegments": 6,
-        "spikeThreshold": 0.9,
-        "vertexCountOvershoot":  3,
-        "preventOneYearRecovery":  False,
-        "recoveryThreshold":  0.25,
-        "pvalThreshold":  0.1,
-        "bestModelProportion":  1.25,
-        "minObservationsNeeded": 6,
-    }
-    _needs_index_flip = ['NBR', 'NDVI', 'NDSI', 'NDMI',
-                         'EVI', 'TCG', 'TCW', 'TCA', 'B4', 'NDFI',]
-    _band_names = ['B1', 'B2', 'B3', 'B4', 'B5', 'B7']
 
-    def __init__(self, start_date, end_date, area_of_interest, index='NBR', ftv_list=[], mask_labels=['cloud', 'shadow', 'snow'], exclude={}, debug=False, run=True, run_params={}) -> None:
-        self.start_date = start_date
-        self.end_date = end_date
-        self.area_of_interest = area_of_interest
-        self.index = index
-        self.ftv_list = ftv_list
-        self.mask_labels = mask_labels
-        self.exclude = exclude
-        self.run_params = run_params
-        if run:
-            self.run(debug)
+    def __init__(self,
+                 collection: Optional[ee.ImageCollection] = None,
+                 start_date: Optional[datetime] = None,
+                 end_date: Optional[datetime] = None,
+                 area_of_interest: Optional[ee.Geometry] = None,
+                 mask_labels: list[str] = ['cloud', 'shadow', 'snow'],
+                 exclude: dict = {},
+                 debug: bool = False):
+        if collection:
+            super().__init__(collection)
+        else:
+            assert start_date, "start_date is required"
+            assert end_date, "end_date is required"
+            assert area_of_interest, "area_of_interest is required"
+            self.start_date = start_date
+            self.end_date = end_date
+            self.area_of_interest = area_of_interest
+            self.mask_labels = mask_labels
+            self.exclude = exclude
+            super().__init__(self._build_sr_collection(debug))
 
     @property
-    def start_date(self):
-        return self._start_date
+    def mask_labels(self):
+        return self._mask_labels
 
-    @start_date.setter
-    def start_date(self, start_date):
-        self._start_date = start_date
-        self._needs_rebuild = True
+    @mask_labels.setter
+    def mask_labels(self, mask_labels: list):
+        assert all([_ in self._mask_options for _ in mask_labels]
+                   ), f"mask_labels must be a subset of {self._mask_options}"
+        self._mask_labels = mask_labels
 
-    @property
-    def end_date(self):
-        return self._end_date
+    def _build_sr_collection(self, debug: Optional[bool] = False):
+        """
+        Builds a medoid composite of Landsat surface reflectance TM-equivalent bands 1,2,3,4,5,7. 
+        This collection can be useful outside of use by LandTrendr, but is also the base for creating the input collection for LandTrendr.
 
-    @end_date.setter
-    def end_date(self, end_date):
-        self._end_date = end_date
-        self._needs_rebuild = True
+        Returns:
+            ee.ImageCollection: A collection where each image represents the medoid of observations per TM-equivalent surface reflectance bands 1-5 and 7, for a given year. There will be as many images as there are years in the range inclusive of the start year and end year.
+        """
+        dummy_collection = ee.ImageCollection(
+            [ee.Image([0, 0, 0, 0, 0, 0]).mask(ee.Image(0))])
+        return ee.ImageCollection(
+            [self._build_medoid_mosaic(year, dummy_collection, debug) for year in range(self.start_date.year, self.end_date.year + 1)])
 
-    @property
-    def area_of_interest(self):
-        return self._area_of_interest
+    def _build_medoid_mosaic(self,
+                             year: int,
+                             dummy_collection: ee.ImageCollection,
+                             debug: Optional[bool] = False):
+        collection = self._get_combined_sr_collection(year)
+        image_count = collection.size()
+        final_collection = ee.ImageCollection(ee.Algorithms.If(
+            image_count.gt(0), collection, dummy_collection))
+        if debug:
+            not_mask_count = ee.ImageCollection(
+                [count_clear_view_pixels(final_collection)])
+            if getattr(self, 'clear_pixel_count_collection', None) is not None:
+                self.clear_pixel_count_collection = self.clear_pixel_count_collection.merge(
+                    not_mask_count)
+            else:
+                self.clear_pixel_count_collection = not_mask_count
+        median = final_collection.median()
+        med_diff_collection = final_collection.map(
+            lambda image: calculate_median_diff(image, median))
+        return med_diff_collection\
+            .reduce(ee.Reducer.min(7))\
+            .select([1, 2, 3, 4, 5, 6], self._band_names)\
+            .set('system:time_start', ee.Date.fromYMD(year, self.start_date.month, self.start_date.day).millis())\
+            .toUint16()
 
-    @area_of_interest.setter
-    def area_of_interest(self, area_of_interest):
-        self._area_of_interest = area_of_interest
-        self._needs_rebuild = True
+    def _get_combined_sr_collection(self, year: int):
+        lt5 = self._get_sr_collection(year, 'LT05')
+        le7 = self._get_sr_collection(year, 'LE07')
+        lc8 = self._get_sr_collection(year, 'LC08')
+        lc9 = self._get_sr_collection(year, 'LC09')
+        return lt5.merge(le7).merge(lc8).merge(lc9)
 
-    @property
-    def index(self):
-        return self._index
+    def _get_sr_collection(self, year: int, sensor: str):
+        if self.start_date.month > self.end_date.month:
+            start_date = ee.Date.fromYMD(
+                year - 1, self.start_date.month, self.start_date.day)
+            end_date = ee.Date.fromYMD(
+                year, self.end_date.month, self.end_date.day)
+        else:
+            start_date = ee.Date.fromYMD(
+                year, self.start_date.month, self.start_date.day)
+            end_date = ee.Date.fromYMD(
+                year, self.end_date.month, self.end_date.day)
+        sr_collection = ee.ImageCollection('LANDSAT/' + sensor + '/C02/T1_L2')\
+            .filterBounds(self.area_of_interest)\
+            .filterDate(start_date, end_date)\
+            .map(lambda image: self._preprocess_image(image, sensor))\
+            .set("system:time_start", start_date.millis())
+        return self._remove_images(sr_collection)
 
-    @index.setter
-    def index(self, index):
-        assert index in self._valid_indices or index in self._valid_indices_alt, f"Index must be one of {self._valid_indices} or {self._valid_indices_alt}"
-        self._index = index
-        self._needs_rebuild = True
+    def _preprocess_image(self, image: int, sensor: str):
+        # Accounting for band shift between landsat difference landsat images
+        if sensor == 'LC08' or sensor == 'LC09':
+            dat = image.select(['SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B6', 'SR_B7'],
+                               self._band_names)
+        else:
+            dat = image.select(['SR_B1', 'SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B7'],
+                               self._band_names)
+        dat = self._scale_unmask_image(dat)
+        if len(self.mask_labels) > 0:
+            dat = self._apply_masks(image.select('QA_PIXEL'), dat)
+        return dat
 
-    @property
-    def ftv_list(self):
-        return self._ftv_list
+    def _scale_unmask_image(self, image: ee.Image):
+        return image.multiply(0.0000275).add(-0.2).multiply(10000).toUint16().unmask()
 
-    @ftv_list.setter
-    def ftv_list(self, ftv_list):
-        assert all([_ in self._valid_indices for _ in ftv_list]
-                   ), f"ftv_list must be a subset of {self._valid_indices}"
-        self._ftv_list = ftv_list
-        self._needs_rebuild = True
+    def _apply_masks(self, qa: ee.Image, dat: ee.Image):
+        mask = ee.Image(1)
+        # TODO: Refactor to allow dynamically allow new masks
+        for mask_label in self.mask_labels:
+            match mask_label:
+                case 'water':
+                    mask = qa.bitwiseAnd(1 << 7).eq(0).multiply(mask)
+                case 'shadow':
+                    mask = qa.bitwiseAnd(1 << 4).eq(0).multiply(mask)
+                case 'snow':
+                    mask = qa.bitwiseAnd(1 << 5).eq(0).multiply(mask)
+                case 'cloud':
+                    mask = qa.bitwiseAnd(1 << 3).eq(0).multiply(mask)
+                case 'waterplus':
+                    mask = mask.mask(water_mask(self.area_of_interest))
+                case 'nonforest':
+                    mask = mask.mask(forest_mask(self.area_of_interest))
+        return dat.mask(mask)
 
-    @property
-    def mask_labels(self):
-        return self._mask_labels
+    def _remove_images(self, collection: ee.ImageCollection):
+        """
+        Removes images from a collection based on the given exclude criteria.
 
-    @mask_labels.setter
-    def mask_labels(self, mask_labels):
-        assert all([_ in self._mask_options for _ in mask_labels]
-                   ), f"mask_labels must be a subset of {self._mask_options}"
-        self._mask_labels = mask_labels
-        self._needs_rebuild = True
+        Args:
+            collection (ee.ImageCollection): The image collection to remove images from.
 
-    @property
-    def run_params(self):
-        return self._run_params
+        Returns:
+            ee.ImageCollection: The updated image collection with images removed.
+        """
+        if 'imageIds' in self.exclude:
+            exclude_list = self.exclude['imageIds']
+            for image_id in exclude_list:
+                collection = collection.filter(ee.Filter.neq(
+                    'system:index', image_id.split('/')[-1]))
 
-    @run_params.setter
-    def run_params(self, run_params):
-        assert all([_ in self._default_run_params.keys()
-                    for _ in run_params.keys()]), f"run_params must be a subset of {self._default_run_params.keys()}"
-        if hasattr(self, '_data'):
-            self._run_params |= run_params
-        else:
-            self._run_params = self._default_run_params | run_params
-            self._data = None
+        if 'slcOff' in self.exclude:
+            if self.exclude['slcOff'] is True:
+                collection = collection.filter(ee.Filter.And(
+                    ee.Filter.eq('SPACECRAFT_ID', 'LANDSAT_7'),
+                    ee.Filter.gt('SCENE_CENTER_TIME', '2003-06-01T00:00')
+                ).Not())
+        return collection
 
-    @property
-    def data(self):
-        if self._data:
-            return self._data
-        else:
-            print(
-                f"No LandTrendr data. Please run the LandTrendr algorithm using LandTrendr.run().")
 
-    @data.setter
-    def data(self, data):
-        self._data = data
+class LtCollection(ee.ImageCollection):
+    """
 
-    @property
-    def sr_collection(self):
-        if self._sr_collection:
-            return self._sr_collection
-        else:
-            print(
-                f"No SR Collection data. Please run the LandTrendr algorithm using LandTrendr.run(debug=True).")
+    ### LtCollection class for building a LandTrendr collection for use in LandTrendr.
 
-    @sr_collection.setter
-    def sr_collection(self, collection):
-        self._sr_collection = collection
+    #### Args:
+    sr_collection (ee.ImageCollection, optional):  An ee.ImageCollection of Landsat surface reflectance images. Defaults to None.
+    composite_params (dict, optional):  A dictionary of parameters to build a new LandsatComposite. Defaults to None.
+    index (str, optional): The spectral index to base temporal segmentation on. Defaults to 'NBR'.
+    ftv_list (list, optional): A list of spectral indices to fit to the segmentation structure of the segmentation index. Defaults to [].
 
-    @property
-    def lt_collection(self):
-        if self._lt_collection:
-            return self._lt_collection
-        else:
-            print(
-                f"No LT collection data. Please run the LandTrendr algorithm using LandTrendr.run(debug=True).")
+    """
+    _index_flip = ['NBR', 'NDVI', 'NDSI', 'NDMI',
+                   'EVI', 'TCG', 'TCW', 'TCA', 'B4', 'NDFI']
+    _valid_indices = ['B1', 'B2', 'B3', 'B4', 'B5', 'B7', 'NBR',
+                      'NDMI', 'NDVI', 'NDSI', 'EVI', 'NDFI', 'TCB', 'TCG', 'TCW', 'TCA']
+    _valid_indices_alt = ['TCC', 'TCM', 'TCS', 'ENC', 'ENM', 'ENS', 'ENC1',
+                          'ENM1', 'ENS1', 'B5z', 'B7z', 'TCWz', 'TCAz', 'NDMIz', 'NBRz']
 
-    @lt_collection.setter
-    def lt_collection(self, collection):
-        self._lt_collection = collection
+    def __init__(self,
+                 sr_collection: LandsatComposite | ee.ImageCollection | dict,
+                 index: str = 'NBR',
+                 ftv_list: Optional[list[str]] = []):
+        self.index = index
+        self.ftv_list = ftv_list
+        if isinstance(sr_collection, dict):
+            self.sr_collection = LandsatComposite(**sr_collection)
+        else:
+            self.sr_collection = sr_collection
+        assert self.sr_collection, "sr_collection must be provided or composite_params must be provided to build a new collection."
+        self.needs_index_flip = self.index in self._index_flip
+        super().__init__(self._build_lt_collection(self.sr_collection))
 
     @property
-    def clear_pixel_count_collection(self):
-        if self._clear_pixel_count_collection:
-            return self._clear_pixel_count_collection
-        elif self._data:
-            print(
-                f"No Clear Pixel Count Collection data. Please run the LandTrendr algorithm using LandTrendr.run(debug=True).")
-
-    @clear_pixel_count_collection.setter
-    def clear_pixel_count_collection(self, collection):
-        self._clear_pixel_count_collection = collection
+    def index(self):
+        return self._index
 
-    def run(self, debug=False, clear_debug=False):
-        """
-        Initiates the LandTrendr algorithm on Google's servers using the specified run_params and generates an image. This is a wrapper around build_sr_collection and build_lt_collection functions. The array image result is saved to LandTrendr.data as an ee.Image.
-        """
-        if debug:
-            self.data = None
-            self.clear_pixel_count_collection = None
-            self.sr_collection = self.build_sr_collection(debug)
-            self.lt_collection = self.build_lt_collection(self.sr_collection)
-            self._needs_rebuild = False
-        else:
-            if self._needs_rebuild:
-                annual_sr_collection = self.build_sr_collection(debug)
-                annual_lt_collection = self.build_lt_collection(
-                    annual_sr_collection)
-                self.data = ee.Algorithms.TemporalSegmentation.LandTrendr(
-                    timeSeries=annual_lt_collection, **self.run_params)
-            else:
-                self.data = ee.Algorithms.TemporalSegmentation.LandTrendr(
-                    timeSeries=self.lt_collection, **self.run_params)
-            if clear_debug:
-                self.clear_pixel_count_collection = None
-                self.sr_collection = None
-                self.lt_collection = None
+    @index.setter
+    def index(self, index: str):
+        assert index in self._valid_indices or index in self._valid_indices_alt, f"Index must be one of {self._valid_indices} or {self._valid_indices_alt}"
+        self._index = index
 
-    def build_sr_collection(self, debug=False):
-        """
-        Builds an annual cloud and cloud shadow masked medoid composite of Landsat surface reflectance TM-equivalent bands 1,2,3,4,5,7. 
-        This collection can be useful outside of use by LandTrendr, but is also the base for creating the input collection for LandTrendr.
+    @property
+    def ftv_list(self):
+        return self._ftv_list
 
-        Returns:
-            ee.ImageCollection: A collection where each image represents the medoid of observations per TM-equivalent surface reflectance bands 1-5 and 7, for a given year. There will be as many images as there are years in the range inclusive of the start year and end year. If a given year does not exist for the range, then a masked band will act as a filler. Similarly, if all observations of a given pixel within a year are masked because of inclusion in the maskThese list, the pixel will be masked.
-        """
-        dummy_collection = ee.ImageCollection(
-            [ee.Image([0, 0, 0, 0, 0, 0]).mask(ee.Image(0))])
-        return ee.ImageCollection(
-            [self._build_medoid_mosaic(year, dummy_collection, debug) for year in range(self.start_date.year, self.end_date.year + 1)])
+    @ftv_list.setter
+    def ftv_list(self, ftv_list: list):
+        assert all([_ in self._valid_indices for _ in ftv_list]
+                   ), f"ftv_list must be a subset of {self._valid_indices}"
+        self._ftv_list = ftv_list
 
-    def build_lt_collection(self, collection):
+    def _build_lt_collection(self,
+                             collection: ee.ImageCollection) -> ee.ImageCollection:
         """
         Builds a collection as input to LandTrendr. It will prepare a collection where the first band is the spectral index to base temporal segmentation on, and the subsequent bands will be fitted to segmentation structure of the segmentation index.
 
         Args:
             collection (ee.ImageCollection): The input annual image collection.
 
         Returns:
-            ee.ImageCollection: The annual LandTrendr collection where each image represents an assemblage of bands or indices to be segmented and fitted by LandTrendr. There will be as many images as there are years in the range inclusive of the start year and end year. If a given year does not exist for the range, then a masked band will act as a filler. Similarly, if all observations of a given pixel within a year are masked because of cloud, cloud shadow, or snow, the pixel will be masked. The first band per image will be whatever spectral representation is defined by the index parameter - it will be oriented so that vegetation loss results in a positive spectral delta. Any following bands will be defined by the indices provided in the ftvList parameter, in the same order, and unmodified with regard to spectral delta orientation.
-
+            ee.ImageCollection
         """
 
         match self.index:
             case 'TCC':
                 return self._make_tc_composite(collection, 'mean')
             case 'TCM':
                 return self._make_tc_composite(collection, 'max')
@@ -260,17 +280,346 @@
             case 'TCAz':
                 return self._standardize_index(collection, 'TCA')
             case 'NDMIz':
                 return self._standardize_index(collection, 'NDMI')
             case 'NBRz':
                 return self._standardize_index(collection, 'NBR')
             case _:
-                return self.transform_sr_collection(collection, self.ftv_list, "ftv")
+                return self._transform_sr_collection(collection, self.ftv_list, "ftv")
+
+    def _transform_sr_collection(self,
+                                 collection: ee.ImageCollection,
+                                 band_list: list[str],
+                                 prefix: str = None) -> ee.ImageCollection:
+        """
+        Transforms the images within an annual surface reflectance collection built by buildSRcollection to a list of provided indices or bands.
+
+        Args:
+            collection (ee.ImageCollection): The surface reflectance collection to transform.
+            band_list (list): The list of bands to transform the collection to.
+
+        Returns:
+            ee.ImageCollection: The transformed surface reflectance collection that includes one image per year based on an image collection built by buildSRcollection function transformed to the indices provided in the bandList parameter..
+        """
+        return collection.map(lambda image: self._make_default_composite(image, band_list, prefix))
+
+    def _make_default_composite(self,
+                                image: ee.Image,
+                                band_list: list[str],
+                                prefix: str = None) -> ee.Image:
+        """
+        Generates a default feature composite for the given image.
+
+        Args:
+            image (ee.Image): The input image.
+            band_list (list[str]): The list of bands to include in the composite.
+            prefix (str): The prefix to add to the band names.
+
+        Returns:
+            ee.Image: The feature composite image.
+        """
+        all_stack = self._calculate_index(image, self.index)
+        for band in band_list:
+            band_image = self._calculate_index(image, band, False)
+            if prefix:
+                band_image = band_image.select(
+                    [band], [prefix + '_' + band.lower()])
+            all_stack = all_stack.addBands(band_image).set(
+                'system:time_start', image.get('system:time_start'))
+        return all_stack
+
+    def _standardize_index(self,
+                           collection: ee.ImageCollection,
+                           index: str) -> ee.ImageCollection:
+        """
+        Standardizes the images in a collection based on a given index.
+
+        Args:
+            collection (ee.ImageCollection): The image collection.
+            index (str): The index to standardize.
+
+        Returns:
+            ee.ImageCollection: The standardized image collection.
+        """
+        z_collection = collection.map(
+            lambda image: self._calculate_index(image, index))
+        return standardize_collection(z_collection).map(lambda image: image.multiply(1000).set('system:time_start', image.get('system:time_start')))
+
+    def _calculate_index(self,
+                         image: ee.Image,
+                         index: str,
+                         flip: bool = True) -> ee.Image:
+        index = index.upper()
+        match index:
+            case 'B1' | 'B2' | 'B3' | 'B5' | 'B4' | 'B7':
+                index_image = image.select(index).toFloat()
+            case 'NBR':
+                index_image = nbr_transform(image)
+            case 'NDMI':
+                index_image = ndmi_transform(image)
+            case 'NDVI':
+                index_image = ndvi_transform(image)
+            case 'NDSI':
+                index_image = ndsi_transform(image)
+            case 'EVI':
+                index_image = evi_transform(image)
+            case 'TCB' | 'TCG' | 'TCW' | 'TCA':
+                index_image = tc_transform(image).select([index])
+            case 'NDFI':
+                index_image = ndfi_transform(image)
+            case _:
+                raise ValueError('The index you provided is not supported')
+        if flip and self.needs_index_flip:
+            index_image = index_image.multiply(-1)
+        return index_image.set('system:time_start', image.get('system:time_start'))
 
-    def get_change_map(self, change_params):
+    def _reducer(image_collection: ee.ImageCollection,
+                 reducer: str) -> ee.Image:
+        match reducer:
+            case 'mean':
+                return image_collection.mean()
+            case 'max':
+                return image_collection.max()
+            case 'sum':
+                return image_collection.sum()
+            case _:
+                raise ValueError('The reducer you provided is not supported')
+
+    def _make_tc_composite(self,
+                           collection: ee.ImageCollection,
+                           reducer: str) -> ee.ImageCollection:
+        """
+        Creates a tasseled-cap (brightness, greenness, and wetness) composite for the given collection using the specified reducer.
+
+        Args:
+            collection (ee.ImageCollection): The image collection to create the composite from.
+            reducer (str): The reducer to use for compositing.
+
+        Returns:
+            ee.ImageCollection: The tasseled-cap composite.
+        """
+        tc_composite = collection.map(self._tc_composite)
+        tcb = tc_composite.select('TCB')
+        tcg = tc_composite.select('TCG')
+        tcw = tc_composite.select('TCW')
+
+        tcb_standard = standardize_collection(tcb)
+        tcg_standard = standardize_collection(tcg)
+        tcw_standard = standardize_collection(tcw)
+        tc_standard = tcb_standard.combine(tcg_standard).combine(tcw_standard)
+
+        return tc_standard.map(lambda image: self._tc_reducer(image, reducer))
+
+    def _tc_composite(self,
+                      image: ee.Image) -> ee.Image:
+        tcb = self._calculate_index(image, 'TCB')
+        tcg = self._calculate_index(image, 'TCG')
+        tcw = self._calculate_index(image, 'TCW')
+        return tcb.addBands(tcg).addBands(tcw).set('system:time_start', image.get('system:time_start'))
+
+    def _tc_reducer(self,
+                    image: ee.Image,
+                    reducer: str) -> ee.Image:
+        image_collection = ee.ImageCollection.fromImages(
+            [image.select(['TCB'], ['Z']),
+             image.select(['TCG'], ['Z']),
+             image.select(['TCW'], ['Z'])]
+        )
+        reduced_image = self._reducer(image_collection, reducer)
+        return reduced_image.multiply(1000).set('system:time_start', image.get('system:time_start'))
+
+    def _make_ensemble_composite(self,
+                                 collection: ee.ImageCollection,
+                                 reducer: str) -> ee.Image:
+        """
+        Creates an ensemble (see bands below) composite for the given collection using the specified reducer.
+
+        Args:
+            collection (ee.ImageCollection): The input image collection.
+            reducer (str): The reducer to apply when combining the bands.
+
+        Returns:
+            ee.Image: The ensemble composite image.
+        """
+
+        stack = collection.map(self._ensemble_composite)
+
+        b5 = stack.select('B5')
+        b7 = stack.select('B7')
+        tcw = stack.select('TCW')
+        tca = stack.select('TCA')
+        ndmi = stack.select('NDMI')
+        nbr = stack.select('NBR')
+
+        b5_standard = standardize_collection(b5)
+        b7_standard = standardize_collection(b7)
+        tcw_standard = standardize_collection(tcw)
+        tca_standard = standardize_collection(tca)
+        ndmi_standard = standardize_collection(ndmi)
+        nbr_standard = standardize_collection(nbr)
+        ensemble = b5_standard.combine(b7_standard)\
+            .combine(tcw_standard)\
+            .combine(tca_standard)\
+            .combine(ndmi_standard)\
+            .combine(nbr_standard)
+
+        return ensemble.map(lambda image: self._ensemble_reducer(image, reducer))
+
+    def _ensemble_composite(self,
+                            image: ee.Image) -> ee.Image:
+        b5 = self._calculate_index(image, 'B5')
+        b7 = self._calculate_index(image, 'B7')
+        tcw = self._calculate_index(image, 'TCW')
+        tca = self._calculate_index(image, 'TCA')
+        ndmi = self._calculate_index(image, 'NDMI')
+        nbr = self._calculate_index(image, 'NBR')
+
+        return b5.addBands(b7)\
+            .addBands(tcw)\
+            .addBands(tca)\
+            .addBands(ndmi)\
+            .addBands(nbr)\
+            .set('system:time_start', image.get('system:time_start'))
+
+    def _ensemble_reducer(self,
+                          image: ee.Image,
+                          reducer: str) -> ee.Image:
+        image_collection = ee.ImageCollection.fromImages(
+            [image.select(['B5'], ['Z']),
+             image.select(['B7'], ['Z']),
+             image.select(['TCW'], ['Z']),
+             image.select(['TCA'], ['Z']),
+             image.select(['NDMI'], ['Z']),
+             image.select(['NBR'], ['Z'])]
+        )
+        reduced_image = self._reducer(image_collection, reducer)
+        return reduced_image.multiply(1000).set('system:time_start', image.get('system:time_start'))
+
+    def _make_ensemble_composite_alt(self,
+                                     collection: ee.ImageCollection,
+                                     reducer: str) -> ee.ImageCollection:
+        """
+        Creates an ensemble (see bands below) composite for the given collection using the specified reducer.
+
+        Args:
+            collection (ee.ImageCollection): The input image collection.
+            reducer (str): The reducer to apply on the ensemble composite.
+
+        Returns:
+            ee.Image: The ensemble composite image.
+        """
+        e_composite = collection.map(self._ensemble_composite_alt)
+        b5 = e_composite.select('B5')
+        tcb = e_composite.select('TCB')
+        tcg = e_composite.select('TCG')
+        nbr = e_composite.select('NBR')
+
+        b5_standard = standardize_collection(b5)
+        tcb_standard = standardize_collection(tcb)
+        tcg_standard = standardize_collection(tcg)
+        nbr_standard = standardize_collection(nbr)
+        ensemble_alt = b5_standard.combine(tcb_standard)\
+            .combine(tcg_standard)\
+            .combine(nbr_standard)
+
+        return ensemble_alt.map(lambda image: self._ensemble_reducer_alt(image, reducer))
+
+    def _ensemble_composite_alt(self,
+                                image: ee.Image) -> ee.Image:
+        b5 = self._calculate_index(image, 'B5')
+        tcb = self._calculate_index(image, 'TCB')
+        tcg = self._calculate_index(image, 'TCG')
+        nbr = self._calculate_index(image, 'NBR')
+
+        return b5.addBands(tcb)\
+            .addBands(tcg)\
+            .addBands(nbr)\
+            .set('system:time_start', image.get('system:time_start'))
+
+    def _ensemble_reducer_alt(self,
+                              image: ee.Image,
+                              reducer: str) -> ee.Image:
+        image_collection = ee.ImageCollection.fromImages(
+            [image.select(['B5'], ['Z']),
+             image.select(['TCB'], ['Z']),
+             image.select(['TCG'], ['Z']),
+             image.select(['NBR'], ['Z'])]
+        )
+        reduced_image = self._reducer(image_collection, reducer)
+        return reduced_image.multiply(1000).set('system:time_start', image.get('system:time_start'))
+
+
+class LandTrendr:
+    """
+    ### Landtrendr class for performing landtrendr analysis using Google Earth Engine.
+
+    #### Args:
+    lt_collection (:obj:, optional):         LandTrendr collection. Defaults to None.
+    lt_collection_params (:obj:, optional):  Dictionary of parameters to build a new LandTrendr collection (See class definition above).
+    run_params (:obj:, optional):            Dictionary of run parameters (See below).
+        {
+            maxSegments (int, optional):                Maximum number of segments. Defaults to 6.
+            spikeThreshold (float, optional):           Spike threshold. Defaults to 0.9.
+            vertexCountOvershoot (int, optional):       Vertex count overshoot. Defaults to 3.
+            preventOneYearRecovery (bool, optional):    Prevent one year recovery. Defaults to True.
+            recoveryThreshold (float, optional):        Recovery threshold. Defaults to 0.25.
+            pvalThreshold (float, optional):            P-value threshold. Defaults to 0.25.
+            bestModelProportion (float, optional):      Best model proportion. Defaults to 0.75.
+            minObservationsNeeded (int, optional):      Minimum number of observations needed. Defaults to 6.
+        }
+    run (bool, optional):                               Whether to run the run method immediately. Defaults to True.
+    """
+
+    _default_run_params = {
+        "maxSegments": 6,
+        "spikeThreshold": 0.9,
+        "vertexCountOvershoot":  3,
+        "preventOneYearRecovery":  False,
+        "recoveryThreshold":  0.25,
+        "pvalThreshold":  0.1,
+        "bestModelProportion":  1.25,
+        "minObservationsNeeded": 6,
+    }
+
+    def __init__(self,
+                 lt_collection: LtCollection | ee.ImageCollection,
+                 run_params: dict = _default_run_params,
+                 run: bool = True):
+        self.run_params = run_params
+        if isinstance(lt_collection, dict):
+            self.lt_collection = LtCollection(**lt_collection)
+        else:
+            self.lt_collection = lt_collection
+
+        if run:
+            self.run()
+
+    @property
+    def run_params(self):
+        return self._run_params
+
+    @run_params.setter
+    def run_params(self, run_params: dict):
+        assert all([_ in self._default_run_params.keys()
+                    for _ in run_params.keys()]), f"run_params must be a subset of {self._default_run_params.keys()}"
+        if hasattr(self, '_data'):
+            self._run_params |= run_params
+        else:
+            self._run_params = self._default_run_params | run_params
+            self._data = None
+
+    def run(self):
+        """
+        Initiates the LandTrendr algorithm on Google's servers using the specified run_params and generates an image.
+        """
+        self.data = ee.Algorithms.TemporalSegmentation.LandTrendr(
+            timeSeries=self.lt_collection, **self.run_params)
+
+    def get_change_map(self,
+                       change_params: dict) -> ee.Image:
         """
         Generates a set of map layers describing either vegetation loss or gain events with attributes including: year of change detection, spectral delta, duration of change event, pre-change event spectral value, and the rate of spectral change. Each attribute is a band of an ee.Image.
 
         Args:
             change_params (dict): A dictionary containing the parameters for change detection.
                 {
                     'delta':                'loss' | 'gain' | 'all',
@@ -285,26 +634,26 @@
         Returns:
             ee.Image: An image with bands for attributes of change events meeting filtering criteria including:
                 Year of change event detection: 'yod' (year)
                 Magnitude of change event: 'mag' (absolute value of change event spectral delta)
                 Duration of change event: 'dur' (years)
                 Pre-change event spectral value: 'preval' (spectral value)
                 Rate of spectral change for event 'rate' (mag/dur)
-                DSNR 'dsnr' (mag/fit rmse) multipled by 100 to retain two decimal precision with Int16 data.
+                DSNR 'dsnr' (mag/fit rmse) multiplied by 100 to retain two decimal precision with Int16 data.
         """
         # Backward compatibility for dsnr
         if 'dsnr' not in change_params['mag']:
             change_params['mag']['dsnr'] = False
 
         # Get the segment info
         assert change_params['delta'] in \
             ['loss', 'gain', 'all'], \
             "delta must be one of 'loss', 'gain', or 'all'"
         seg_info = self.get_segment_data(
-            self.index, change_params['delta'])
+            change_params['delta'], self.lt_collection.needs_index_flip)
         change_mask = seg_info.arraySlice(0, 4, 5).gt(0)
         seg_info = seg_info.arrayMask(change_mask)
 
         # Filter by year
         if 'years' in change_params:
             yod_arr = seg_info.arraySlice(0, 0, 1).add(1)
             year_mask = yod_arr.gte(ee.Number(change_params['years']['start'])).And(
@@ -404,15 +753,18 @@
             assert change_params['mmu']['value'] >= 1, "mmu value must be greater than 1"
             mmu_lyr = change_image.select('yod')
             mmu_mask = self._apply_mmu(mmu_lyr, change_params['mmu']['value'])
             change_image = change_image.updateMask(mmu_mask)
 
         return change_image
 
-    def get_segment_data(self, index, delta, options=None):
+    def get_segment_data(self,
+                         delta: int,
+                         index_flip: bool,
+                         options: Optional[dict] = None) -> ee.Image:
         """
         Generates an array of information about spectral-temporal segments from the breakpoint vertices identified by LandTrendr. Returns either all spectral-temporal segments, or just vegetation loss segments, or just vegetation growth segments.
 
         Args:
             index (int): The index of the segment.
             delta (str): The type of delta to calculate. Can be 'all', 'gain', or 'loss'.
             options (bool, optional): Additional options for the segment data retrieval. Defaults to None.
@@ -461,15 +813,15 @@
         dsnr = mag.divide(rmse)  # make mag relative to fit rmse
 
         # Whether to return all segments or either dist or grow
         match delta:
             case 'all':
                 # If the data should be set to the correct orientation, adjust it
                 if _options['right']:
-                    if index in self._needs_index_flip:
+                    if index_flip:
                         start_val = start_val.multiply(-1)
                         end_val = end_val.multiply(-1)
                         mag = mag.multiply(-1)
                         rate = rate.multiply(-1)
                         dsnr = dsnr.multiply(-1)
 
                 # Now just get out - return the result
@@ -480,461 +832,127 @@
             case 'gain' | 'loss':
                 match delta:
                     case 'gain':
                         change_type_mask = mag.lt(0)
                     case 'loss':
                         change_type_mask = mag.gt(0)
 
-                flip = -1 if index in self._needs_index_flip else 1
+                flip = -1 if index_flip else 1
                 return ee.Image.cat([
                     start_year.arrayMask(change_type_mask),
                     end_year.arrayMask(change_type_mask),
                     start_val.arrayMask(change_type_mask).multiply(flip),
                     end_val.arrayMask(change_type_mask).multiply(flip),
                     mag.arrayMask(change_type_mask).abs(),
                     dur.arrayMask(change_type_mask),
                     rate.arrayMask(change_type_mask).abs(),
                     dsnr.arrayMask(change_type_mask).abs(),
                 ]) \
                     .unmask(ee.Image(ee.Array([[-9999]]))) \
                     .toArray(0)
 
-    def get_segment_count(segment_data):
+    @staticmethod
+    def get_segment_count(segment_data: ee.Image) -> ee.Image:
         """
         Given a segment data array produced by the getSegmentData function, this function returns the number of segments identified by LandTrendr as an ee.Image.
 
         Args:
             segment_data (ee.Image): an image array returned from the get_segment_data function
 
         Returns:
             ee.Image: A single-band ee.Image describing the number of segments per pixel time series identified by LandTrendr.
         """
         return segment_data.arrayLength(1).select([0], ['segCount']).toByte()
 
-    def get_fitted_data(self, index):
+    def get_fitted_data(self,
+                        index: str,
+                        start_date: datetime,
+                        end_date: datetime) -> ee.Image:
         """
         Generates an annual band stack for a given index provided as ftvList indices to either buildLTcollection or runLT. It flattens the FTV array format to a band per year for a given FTV index.
 
         Args:
             index (str): The index for which to retrieve the fitted data.
+            start_date (datetime): The start date of the time series.
+            end_date (datetime): The end date of the time series.
 
         Returns:
             ee.Image: An image representing fitted-to-vertex annual spectral data for whatever index was provided as the index parameter. There will be as many bands as there are years in the range inclusive of the start year and end year.
         """
         search = 'ftv_' + index.lower() + '_fit'
-        return self.data.select(search).arrayFlatten([[str(_) for _ in range(self.start_date.year, self.end_date.year + 1)]])
+        return self.data.select(search).arrayFlatten([[str(_) for _ in range(start_date.year, end_date.year + 1)]])
 
-    def collection_to_band_stack(self, collection, mask_fill=0):
+    def collection_to_band_stack(self,
+                                 collection: ee.ImageCollection,
+                                 start_date: datetime,
+                                 end_date: datetime,
+                                 mask_fill: int = 0) -> ee.Image:
         """
         Transforms an image collection into an image stack where each band of each image in the collection is concatenated as a band into a single image. Useful for mapping a function over a collection, like transforming surface reflectance to NDVI, and then transforming the resulting collection into a band sequential time series image stack.
 
         Args:
             collection (ee.ImageCollection): The Earth Engine image collection to convert.
+            start_date (datetime): The start date of the time series.
+            end_date (datetime): The end date of the time series.
             mask_fill (int, optional): The value to fill masked pixels with. Default is 0.
 
         Returns:
             ee.Image: The band stack image representing a band sequential time series of image bands from each image in the given collection between the start year and end year. Note that masked values in the image collection will be filled with 0
 
         """
         unmasked_collection = collection.map(
             lambda image: image.unmask(mask_fill))
         collection_array = unmasked_collection.toArrayPerBand()
         bands = unmasked_collection.first().bandNames().getInfo()
         all_stack = ee.Image()
 
         for band in bands:
             band_ts = collection_array.select(band).arrayFlatten(
-                [[str(_) for _ in range(self.start_date.year, self.end_date.year + 1)]])
+                [[str(_) for _ in range(start_date.year, end_date.year + 1)]])
             all_stack = ee.Image.cat([all_stack, band_ts])
 
         return all_stack.slice(1, None).toUint16()
 
-    def transform_sr_collection(self, collection, band_list, prefix=None):
-        """
-        Transforms the images within an annual surface reflectance collection built by buildSRcollection to a list of provided indices or bands.
-
-        Args:
-            collection (ee.ImageCollection): The surface reflectance collection to transform.
-            band_list (list): The list of bands to transform the collection to.
-
-        Returns:
-            ee.ImageCollection: The transformed surface reflectance collection that includes one image per year based on an image collection built by buildSRcollection function transformed to the indices provided in the bandList parameter..
-        """
-        return collection.map(lambda image: self._make_default_composite(image, band_list, prefix))
-
-    def get_fitted_rgb_col(self, bands, vis_params):
+    def get_fitted_rgb_col(self,
+                           bands: list[str],
+                           vis_params: dict,
+                           start_date: datetime,
+                           end_date: datetime) -> ee.ImageCollection:
         """
         Creates a collection of RGB visualization images from three FTV bands resulting from a call to LandTrendr segmentation. This is useful for creating thumbnails, filmstrips, and GIFs.
 
         Args:
             lt (LandTrendr): The LandTrendr object.
             bands (list): A list of band names.
             vis_params (dict): Visualization parameters for the RGB image.
 
         Returns:
             ee.ImageCollection: An image collection with an RGB image for each year between and including the start year and end year.
         """
 
-        r = self.get_fitted_data(bands[0])
-        g = self.get_fitted_data(bands[1])
-        b = self.get_fitted_data(bands[2])
+        r = self.get_fitted_data(
+            bands[0], start_date=start_date, end_date=end_date)
+        g = self.get_fitted_data(
+            bands[1], start_date=start_date, end_date=end_date)
+        b = self.get_fitted_data(
+            bands[2], start_date=start_date, end_date=end_date)
         rgb_list = []
-        for year in range(self.start_date.year, self.end_date.year + 1):
+        for year in range(start_date.year, end_date.year + 1):
             year_str = str(year)
             rgb_list.append(r.select(year_str)
                             .addBands(g.select(year_str))
                             .addBands(b.select(year_str))
                             .rename(['R', 'G', 'B']))
         rgb_col = ee.ImageCollection(rgb_list)\
             .map(lambda image: image.visualize(**vis_params))\
             .map(lambda image:
-                 image.set({'system:time_start': ee.Date.fromYMD(self.start_date.year, self.start_date.month, self.start_date.day).millis(), 'composite_year': self.start_date.year}))
+                 image.set({'system:time_start': ee.Date.fromYMD(start_date.year, start_date.month, start_date.day).millis(), 'composite_year': start_date.year}))
 
         return rgb_col
 
-    def _standardize_index(self, collection, index):
-        """
-        Standardizes the images in a collection based on a given index.
-
-        Args:
-            collection (ee.ImageCollection): The image collection.
-            index (str): The index to standardize.
-
-        Returns:
-            ee.ImageCollection: The standardized image collection.
-        """
-        z_collection = collection.map(
-            lambda image: self._calculate_index(image, index))
-        return standardize_collection(z_collection).map(lambda image: image.multiply(1000).set('system:time_start', image.get('system:time_start')))
-
-    def _make_default_composite(self, image, band_list, prefix):
-        """
-        Generates a default feature composite for the given image.
-
-        Args:
-            image (ee.Image): The input image.
-
-        Returns:
-            ee.Image: The feature composite image.
-        """
-        all_stack = self._calculate_index(image, self.index)
-        for band in band_list:
-            band_image = self._calculate_index(image, band, False)
-            if prefix:
-                band_image = band_image.select(
-                    [band], [prefix + '_' + band.lower()])
-            all_stack = all_stack.addBands(band_image).set(
-                'system:time_start', image.get('system:time_start'))
-        return all_stack
-
-    def _count_clear_view_pixels(self, collection):
-        """
-        Counts the number of clear view pixels for the given collection.
-
-        Args:
-            collection (ee.ImageCollection): The image collection.
-
-        Returns:
-            ee.Image: The image containing the number of clear view pixels.
-        """
-        binary = collection.map(lambda image: image.select(
-            0).multiply(0).add(1).unmask(0))
-        return binary.sum()
-
-    def _build_medoid_mosaic(self, year, dummy_collection, debug=False):
-        collection = self._get_combined_sr_collection(year)
-        image_count = collection.size()
-        final_collection = ee.ImageCollection(ee.Algorithms.If(
-            image_count.gt(0), collection, dummy_collection))
-        if debug:
-            not_mask_count = ee.ImageCollection(
-                [self._count_clear_view_pixels(final_collection)])
-            if self.clear_pixel_count_collection:
-                self.clear_pixel_count_collection = self.clear_pixel_count_collection.merge(
-                    not_mask_count)
-            else:
-                self.clear_pixel_count_collection = not_mask_count
-        median = final_collection.median()
-        med_diff_collection = final_collection.map(
-            lambda image: calculate_median_diff(image, median))
-        return med_diff_collection\
-            .reduce(ee.Reducer.min(7))\
-            .select([1, 2, 3, 4, 5, 6], self._band_names)\
-            .set('system:time_start', ee.Date.fromYMD(year, self.start_date.month, self.start_date.day).millis())\
-            .toUint16()
-
-    def _get_combined_sr_collection(self, year):
-        lt5 = self._get_sr_collection(year, 'LT05')
-        le7 = self._get_sr_collection(year, 'LE07')
-        lc8 = self._get_sr_collection(year, 'LC08')
-        lc9 = self._get_sr_collection(year, 'LC09')
-        return lt5.merge(le7).merge(lc8).merge(lc9)
-
-    def _get_sr_collection(self, year, sensor):
-        if self.start_date.month > self.end_date.month:
-            start_date = ee.Date.fromYMD(
-                year - 1, self.start_date.month, self.start_date.day)
-            end_date = ee.Date.fromYMD(
-                year, self.end_date.month, self.end_date.day)
-        else:
-            start_date = ee.Date.fromYMD(
-                year, self.start_date.month, self.start_date.day)
-            end_date = ee.Date.fromYMD(
-                year, self.end_date.month, self.end_date.day)
-        sr_collection = ee.ImageCollection('LANDSAT/' + sensor + '/C02/T1_L2')\
-            .filterBounds(self.area_of_interest)\
-            .filterDate(start_date, end_date)\
-            .map(lambda image: self._preprocess_image(image, sensor))\
-            .set("system:time_start", start_date.millis())
-        return self._remove_images(sr_collection)
-
-    def _preprocess_image(self, image, sensor):
-        # Accounting for band shift between landsat difference landsat images
-        if sensor == 'LC08' or sensor == 'LC09':
-            dat = image.select(['SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B6', 'SR_B7'],
-                               self._band_names)
-        else:
-            dat = image.select(['SR_B1', 'SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B7'],
-                               self._band_names)
-        dat = self._scale_unmask_image(dat)
-        if len(self.mask_labels) > 0:
-            dat = self._apply_masks(image.select('QA_PIXEL'), dat)
-        return dat
-
-    def _scale_unmask_image(self, image):
-        return image.multiply(0.0000275).add(-0.2).multiply(10000).toUint16().unmask()
-
-    def _apply_masks(self, qa, dat):
-        mask = ee.Image(1)
-        # TODO: Refactor to allow dynamically allow new masks
-        for mask_label in self.mask_labels:
-            match mask_label:
-                case 'water':
-                    mask = qa.bitwiseAnd(1 << 7).eq(0).multiply(mask)
-                case 'shadow':
-                    mask = qa.bitwiseAnd(1 << 4).eq(0).multiply(mask)
-                case 'snow':
-                    mask = qa.bitwiseAnd(1 << 5).eq(0).multiply(mask)
-                case 'cloud':
-                    mask = qa.bitwiseAnd(1 << 3).eq(0).multiply(mask)
-                case 'waterplus':
-                    mask = mask.mask(water_mask(self.area_of_interest))
-                case 'nonforest':
-                    mask = mask.mask(forest_mask(self.area_of_interest))
-        return dat.mask(mask)
-
-    def _apply_mmu(self, image, mmu_value):
+    def _apply_mmu(self, image: ee.Image, mmu_value: int) -> ee.Image:
         mmu_image = image.select([0])\
             .gte(ee.Number(1))\
             .selfMask()\
             .connectedPixelCount()
         min_area = mmu_image.gte(ee.Number(mmu_value)).selfMask()
         return min_area.reproject(image.projection().atScale(30)).unmask()
-
-    def _calculate_index(self, image, index, flip=True):
-        index = index.upper()
-        match index:
-            case 'B1' | 'B2' | 'B3' | 'B5' | 'B4' | 'B7':
-                index_image = image.select(index).toFloat()
-            case 'NBR':
-                index_image = nbr_transform(image)
-            case 'NDMI':
-                index_image = ndmi_transform(image)
-            case 'NDVI':
-                index_image = ndvi_transform(image)
-            case 'NDSI':
-                index_image = ndsi_transform(image)
-            case 'EVI':
-                index_image = evi_transform(image)
-            case 'TCB' | 'TCG' | 'TCW' | 'TCA':
-                index_image = tc_transform(image).select([index])
-            case 'NDFI':
-                index_image = ndfi_transform(image)
-            case _:
-                raise ValueError('The index you provided is not supported')
-        if flip and index in self._needs_index_flip:
-            index_image = index_image.multiply(-1)
-        return index_image.set('system:time_start', image.get('system:time_start'))
-
-    def _reducer(image_collection, reducer):
-        match reducer:
-            case 'mean':
-                return image_collection.mean()
-            case 'max':
-                return image_collection.max()
-            case 'sum':
-                return image_collection.sum()
-            case _:
-                raise ValueError('The reducer you provided is not supported')
-
-    def _make_tc_composite(self, collection, reducer):
-        """
-        Creates a tasseled-cap (brightness, greenness, and wetness) composite for the given collection using the specified reducer.
-
-        Args:
-            collection (ee.ImageCollection): The image collection to create the composite from.
-            reducer (ee.Reducer): The reducer to use for compositing.
-
-        Returns:
-            ee.ImageCollection: The tasseled-cap composite.
-        """
-        tc_composite = collection.map(self._tc_composite)
-        tcb = tc_composite.select('TCB')
-        tcg = tc_composite.select('TCG')
-        tcw = tc_composite.select('TCW')
-
-        tcb_standard = standardize_collection(tcb)
-        tcg_standard = standardize_collection(tcg)
-        tcw_standard = standardize_collection(tcw)
-        tc_standard = tcb_standard.combine(tcg_standard).combine(tcw_standard)
-
-        return tc_standard.map(lambda image: self._tc_reducer(image, reducer))
-
-    def _tc_composite(self, image):
-        tcb = self._calculate_index(image, 'TCB')
-        tcg = self._calculate_index(image, 'TCG')
-        tcw = self._calculate_index(image, 'TCW')
-        return tcb.addBands(tcg).addBands(tcw).set('system:time_start', image.get('system:time_start'))
-
-    def _tc_reducer(self, image, reducer):
-        image_collection = ee.ImageCollection.fromImages(
-            [image.select(['TCB'], ['Z']),
-             image.select(['TCG'], ['Z']),
-             image.select(['TCW'], ['Z'])]
-        )
-        reduced_image = self._reducer(image_collection, reducer)
-        return reduced_image.multiply(1000).set('system:time_start', image.get('system:time_start'))
-
-    def _make_ensemble_composite(self, collection, reducer):
-        """
-        Creates an ensemble (see bands below) composite for the given collection using the specified reducer.
-
-        Args:
-            collection (ee.ImageCollection): The input image collection.
-            reducer (ee.Reducer): The reducer to apply when combining the bands.
-
-        Returns:
-            ee.Image: The ensemble composite image.
-        """
-
-        stack = collection.map(self._ensemble_composite)
-
-        b5 = stack.select('B5')
-        b7 = stack.select('B7')
-        tcw = stack.select('TCW')
-        tca = stack.select('TCA')
-        ndmi = stack.select('NDMI')
-        nbr = stack.select('NBR')
-
-        b5_standard = standardize_collection(b5)
-        b7_standard = standardize_collection(b7)
-        tcw_standard = standardize_collection(tcw)
-        tca_standard = standardize_collection(tca)
-        ndmi_standard = standardize_collection(ndmi)
-        nbr_standard = standardize_collection(nbr)
-        ensemble = b5_standard.combine(b7_standard)\
-            .combine(tcw_standard)\
-            .combine(tca_standard)\
-            .combine(ndmi_standard)\
-            .combine(nbr_standard)
-
-        return ensemble.map(lambda image: self._ensemble_reducer(image, reducer))
-
-    def _ensemble_composite(self, image):
-        b5 = self._calculate_index(image, 'B5')
-        b7 = self._calculate_index(image, 'B7')
-        tcw = self._calculate_index(image, 'TCW')
-        tca = self._calculate_index(image, 'TCA')
-        ndmi = self._calculate_index(image, 'NDMI')
-        nbr = self._calculate_index(image, 'NBR')
-
-        return b5.addBands(b7)\
-            .addBands(tcw)\
-            .addBands(tca)\
-            .addBands(ndmi)\
-            .addBands(nbr)\
-            .set('system:time_start', image.get('system:time_start'))
-
-    def _ensemble_reducer(self, image, reducer):
-        image_collection = ee.ImageCollection.fromImages(
-            [image.select(['B5'], ['Z']),
-             image.select(['B7'], ['Z']),
-             image.select(['TCW'], ['Z']),
-             image.select(['TCA'], ['Z']),
-             image.select(['NDMI'], ['Z']),
-             image.select(['NBR'], ['Z'])]
-        )
-        reduced_image = self._reducer(image_collection, reducer)
-        return reduced_image.multiply(1000).set('system:time_start', image.get('system:time_start'))
-
-    def _make_ensemble_composite_alt(self, collection, reducer):
-        """
-        Creates an ensemble (see bands below) composite for the given collection using the specified reducer.
-
-        Args:
-            collection (ee.ImageCollection): The input image collection.
-            reducer (ee.Reducer): The reducer to apply on the ensemble composite.
-
-        Returns:
-            ee.Image: The ensemble composite image.
-        """
-        e_composite = collection.map(self._ensemble_composite_alt)
-        b5 = e_composite.select('B5')
-        tcb = e_composite.select('TCB')
-        tcg = e_composite.select('TCG')
-        nbr = e_composite.select('NBR')
-
-        b5_standard = standardize_collection(b5)
-        tcb_standard = standardize_collection(tcb)
-        tcg_standard = standardize_collection(tcg)
-        nbr_standard = standardize_collection(nbr)
-        ensemble_alt = b5_standard.combine(tcb_standard)\
-            .combine(tcg_standard)\
-            .combine(nbr_standard)
-
-        return ensemble_alt.map(lambda image: self._ensemble_reducer_alt(image, reducer))
-
-    def _ensemble_composite_alt(self, image):
-        b5 = self._calculate_index(image, 'B5')
-        tcb = self._calculate_index(image, 'TCB')
-        tcg = self._calculate_index(image, 'TCG')
-        nbr = self._calculate_index(image, 'NBR')
-
-        return b5.addBands(tcb)\
-            .addBands(tcg)\
-            .addBands(nbr)\
-            .set('system:time_start', image.get('system:time_start'))
-
-    def _ensemble_reducer_alt(self, image, reducer):
-        image_collection = ee.ImageCollection.fromImages(
-            [image.select(['B5'], ['Z']),
-             image.select(['TCB'], ['Z']),
-             image.select(['TCG'], ['Z']),
-             image.select(['NBR'], ['Z'])]
-        )
-        reduced_image = self._reducer(image_collection, reducer)
-        return reduced_image.multiply(1000).set('system:time_start', image.get('system:time_start'))
-
-    def _remove_images(self, collection):
-        """
-        Removes images from a collection based on the given exclude criteria.
-
-        Args:
-            collection (ee.ImageCollection): The image collection to remove images from.
-            exclude (dict): A dictionary containing the exclude criteria.
-
-        Returns:
-            ee.ImageCollection: The updated image collection with images removed.
-        """
-        if 'imageIds' in self.exclude:
-            exclude_list = self.exclude['imageIds']
-            for image_id in exclude_list:
-                collection = collection.filter(ee.Filter.neq(
-                    'system:index', image_id.split('/')[-1]))
-
-        if 'slcOff' in self.exclude:
-            if self.exclude['slcOff'] is True:
-                collection = collection.filter(ee.Filter.And(
-                    ee.Filter.eq('SPACECRAFT_ID', 'LANDSAT_7'),
-                    ee.Filter.gt('SCENE_CENTER_TIME', '2003-06-01T00:00')
-                ).Not())
-        return collection
```

