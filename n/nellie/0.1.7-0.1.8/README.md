# Comparing `tmp/nellie-0.1.7.tar.gz` & `tmp/nellie-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nellie-0.1.7.tar", last modified: Fri Apr  5 16:10:11 2024, max compression
+gzip compressed data, was "nellie-0.1.8.tar", last modified: Fri Apr 26 16:18:29 2024, max compression
```

## Comparing `nellie-0.1.7.tar` & `nellie-0.1.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:10:11.655045 nellie-0.1.7/
--rw-r--r--   0 austin     (501) staff       (20)    18826 2024-03-19 19:14:37.000000 nellie-0.1.7/LICENSE
--rw-r--r--   0 austin     (501) staff       (20)    11217 2024-04-05 16:10:11.654920 nellie-0.1.7/PKG-INFO
--rw-r--r--   0 austin     (501) staff       (20)    10555 2024-03-23 00:41:03.000000 nellie-0.1.7/README.md
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:10:11.643768 nellie-0.1.7/nellie/
--rw-r--r--   0 austin     (501) staff       (20)     1421 2024-03-15 22:18:53.000000 nellie-0.1.7/nellie/__init__.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:10:11.644844 nellie-0.1.7/nellie/feature_extraction/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.7/nellie/feature_extraction/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    54414 2024-04-01 21:48:11.000000 nellie-0.1.7/nellie/feature_extraction/hierarchical.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:10:11.645717 nellie-0.1.7/nellie/im_info/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.7/nellie/im_info/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    16203 2024-04-01 22:05:10.000000 nellie-0.1.7/nellie/im_info/im_info.py
--rw-r--r--   0 austin     (501) staff       (20)     1774 2024-04-01 22:21:40.000000 nellie-0.1.7/nellie/run.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:10:11.646893 nellie-0.1.7/nellie/segmentation/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.7/nellie/segmentation/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    11578 2024-03-15 22:18:53.000000 nellie-0.1.7/nellie/segmentation/filtering.py
--rw-r--r--   0 austin     (501) staff       (20)     6487 2024-03-15 22:18:53.000000 nellie-0.1.7/nellie/segmentation/labelling.py
--rw-r--r--   0 austin     (501) staff       (20)     9769 2024-04-01 17:29:51.000000 nellie-0.1.7/nellie/segmentation/mocap_marking.py
--rw-r--r--   0 austin     (501) staff       (20)    16823 2024-03-15 22:18:53.000000 nellie-0.1.7/nellie/segmentation/networking.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:10:11.648315 nellie-0.1.7/nellie/tracking/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.7/nellie/tracking/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)     4743 2024-03-23 00:41:03.000000 nellie-0.1.7/nellie/tracking/all_tracks_for_label.py
--rw-r--r--   0 austin     (501) staff       (20)    11441 2024-04-01 16:16:45.000000 nellie-0.1.7/nellie/tracking/flow_interpolation.py
--rw-r--r--   0 austin     (501) staff       (20)    17974 2024-04-01 16:16:45.000000 nellie-0.1.7/nellie/tracking/hu_tracking.py
--rw-r--r--   0 austin     (501) staff       (20)    19639 2024-04-01 16:16:45.000000 nellie-0.1.7/nellie/tracking/voxel_reassignment.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:10:11.649562 nellie-0.1.7/nellie/utils/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.7/nellie/utils/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)      275 2024-03-15 22:13:16.000000 nellie-0.1.7/nellie/utils/base_logger.py
--rw-r--r--   0 austin     (501) staff       (20)     1572 2024-04-01 21:26:56.000000 nellie-0.1.7/nellie/utils/general.py
--rw-r--r--   0 austin     (501) staff       (20)     2594 2024-03-15 22:18:53.000000 nellie-0.1.7/nellie/utils/gpu_functions.py
--rw-r--r--   0 austin     (501) staff       (20)     5892 2024-03-15 22:13:16.000000 nellie-0.1.7/nellie/utils/torch_xp.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:10:11.654572 nellie-0.1.7/nellie.egg-info/
--rw-r--r--   0 austin     (501) staff       (20)    11217 2024-04-05 16:10:11.000000 nellie-0.1.7/nellie.egg-info/PKG-INFO
--rw-r--r--   0 austin     (501) staff       (20)     1253 2024-04-05 16:10:11.000000 nellie-0.1.7/nellie.egg-info/SOURCES.txt
--rw-r--r--   0 austin     (501) staff       (20)        1 2024-04-05 16:10:11.000000 nellie-0.1.7/nellie.egg-info/dependency_links.txt
--rw-r--r--   0 austin     (501) staff       (20)       53 2024-04-05 16:10:11.000000 nellie-0.1.7/nellie.egg-info/entry_points.txt
--rw-r--r--   0 austin     (501) staff       (20)      127 2024-04-05 16:10:11.000000 nellie-0.1.7/nellie.egg-info/requires.txt
--rw-r--r--   0 austin     (501) staff       (20)       27 2024-04-05 16:10:11.000000 nellie-0.1.7/nellie.egg-info/top_level.txt
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:10:11.653066 nellie-0.1.7/nellie_napari/
--rw-r--r--   0 austin     (501) staff       (20)      112 2024-03-18 21:13:24.000000 nellie-0.1.7/nellie_napari/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)     8386 2024-03-19 15:37:36.000000 nellie-0.1.7/nellie_napari/batch_mode.py
--rw-r--r--   0 austin     (501) staff       (20)     3595 2024-03-23 00:44:38.000000 nellie-0.1.7/nellie_napari/home.py
--rw-r--r--   0 austin     (501) staff       (20)    89016 2024-03-19 16:27:20.000000 nellie-0.1.7/nellie_napari/logo.png
--rw-r--r--   0 austin     (501) staff       (20)      218 2024-03-15 22:32:30.000000 nellie-0.1.7/nellie_napari/napari.yaml
--rw-r--r--   0 austin     (501) staff       (20)    20913 2024-03-19 21:11:06.000000 nellie-0.1.7/nellie_napari/nellie_analysis.py
--rw-r--r--   0 austin     (501) staff       (20)    16190 2024-03-19 18:53:00.000000 nellie-0.1.7/nellie_napari/nellie_fileselect.py
--rw-r--r--   0 austin     (501) staff       (20)     2719 2024-03-19 01:57:46.000000 nellie-0.1.7/nellie_napari/nellie_loader.py
--rw-r--r--   0 austin     (501) staff       (20)    15621 2024-04-01 16:16:45.000000 nellie-0.1.7/nellie_napari/nellie_processor.py
--rw-r--r--   0 austin     (501) staff       (20)    12833 2024-03-19 16:50:50.000000 nellie-0.1.7/nellie_napari/visualizer.py
--rw-r--r--   0 austin     (501) staff       (20)       90 2024-01-23 18:46:05.000000 nellie-0.1.7/pyproject.toml
--rw-r--r--   0 austin     (501) staff       (20)      822 2024-04-05 16:10:11.655369 nellie-0.1.7/setup.cfg
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:10:11.653397 nellie-0.1.7/tests/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.7/tests/__init__.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:10:11.653893 nellie-0.1.7/tests/unit/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.7/tests/unit/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)        6 2024-03-15 22:13:16.000000 nellie-0.1.7/tests/unit/test_frangi_filter.py
--rw-r--r--   0 austin     (501) staff       (20)     3310 2024-03-15 22:18:53.000000 nellie-0.1.7/tests/unit/test_im_info.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.351884 nellie-0.1.8/
+-rw-r--r--   0 austin     (501) staff       (20)    18826 2024-03-19 19:14:37.000000 nellie-0.1.8/LICENSE
+-rw-r--r--   0 austin     (501) staff       (20)    11217 2024-04-26 16:18:29.351703 nellie-0.1.8/PKG-INFO
+-rw-r--r--   0 austin     (501) staff       (20)    10555 2024-03-23 00:41:03.000000 nellie-0.1.8/README.md
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.340877 nellie-0.1.8/nellie/
+-rw-r--r--   0 austin     (501) staff       (20)     1421 2024-03-15 22:18:53.000000 nellie-0.1.8/nellie/__init__.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.341939 nellie-0.1.8/nellie/feature_extraction/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/feature_extraction/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    54414 2024-04-01 21:48:11.000000 nellie-0.1.8/nellie/feature_extraction/hierarchical.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.342222 nellie-0.1.8/nellie/im_info/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/im_info/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    16203 2024-04-01 22:05:10.000000 nellie-0.1.8/nellie/im_info/im_info.py
+-rw-r--r--   0 austin     (501) staff       (20)     1774 2024-04-26 16:15:57.000000 nellie-0.1.8/nellie/run.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.343223 nellie-0.1.8/nellie/segmentation/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/segmentation/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    11578 2024-04-26 16:12:16.000000 nellie-0.1.8/nellie/segmentation/filtering.py
+-rw-r--r--   0 austin     (501) staff       (20)     6525 2024-04-26 16:17:35.000000 nellie-0.1.8/nellie/segmentation/labelling.py
+-rw-r--r--   0 austin     (501) staff       (20)     9769 2024-04-01 17:29:51.000000 nellie-0.1.8/nellie/segmentation/mocap_marking.py
+-rw-r--r--   0 austin     (501) staff       (20)    16823 2024-03-15 22:18:53.000000 nellie-0.1.8/nellie/segmentation/networking.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.344311 nellie-0.1.8/nellie/tracking/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/tracking/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)     4743 2024-04-12 20:45:28.000000 nellie-0.1.8/nellie/tracking/all_tracks_for_label.py
+-rw-r--r--   0 austin     (501) staff       (20)    11441 2024-04-26 16:12:16.000000 nellie-0.1.8/nellie/tracking/flow_interpolation.py
+-rw-r--r--   0 austin     (501) staff       (20)    17974 2024-04-26 16:12:16.000000 nellie-0.1.8/nellie/tracking/hu_tracking.py
+-rw-r--r--   0 austin     (501) staff       (20)    19639 2024-04-26 16:12:16.000000 nellie-0.1.8/nellie/tracking/voxel_reassignment.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.345369 nellie-0.1.8/nellie/utils/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/utils/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)      275 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/utils/base_logger.py
+-rw-r--r--   0 austin     (501) staff       (20)     1572 2024-04-01 21:26:56.000000 nellie-0.1.8/nellie/utils/general.py
+-rw-r--r--   0 austin     (501) staff       (20)     2594 2024-03-15 22:18:53.000000 nellie-0.1.8/nellie/utils/gpu_functions.py
+-rw-r--r--   0 austin     (501) staff       (20)     5892 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/utils/torch_xp.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.351389 nellie-0.1.8/nellie.egg-info/
+-rw-r--r--   0 austin     (501) staff       (20)    11217 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/PKG-INFO
+-rw-r--r--   0 austin     (501) staff       (20)     1253 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/SOURCES.txt
+-rw-r--r--   0 austin     (501) staff       (20)        1 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/dependency_links.txt
+-rw-r--r--   0 austin     (501) staff       (20)       53 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/entry_points.txt
+-rw-r--r--   0 austin     (501) staff       (20)      127 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/requires.txt
+-rw-r--r--   0 austin     (501) staff       (20)       27 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/top_level.txt
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.348394 nellie-0.1.8/nellie_napari/
+-rw-r--r--   0 austin     (501) staff       (20)      112 2024-03-18 21:13:24.000000 nellie-0.1.8/nellie_napari/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)     8386 2024-03-19 15:37:36.000000 nellie-0.1.8/nellie_napari/batch_mode.py
+-rw-r--r--   0 austin     (501) staff       (20)     3595 2024-03-23 00:44:38.000000 nellie-0.1.8/nellie_napari/home.py
+-rw-r--r--   0 austin     (501) staff       (20)    89016 2024-03-19 16:27:20.000000 nellie-0.1.8/nellie_napari/logo.png
+-rw-r--r--   0 austin     (501) staff       (20)      218 2024-03-15 22:32:30.000000 nellie-0.1.8/nellie_napari/napari.yaml
+-rw-r--r--   0 austin     (501) staff       (20)    20913 2024-03-19 21:11:06.000000 nellie-0.1.8/nellie_napari/nellie_analysis.py
+-rw-r--r--   0 austin     (501) staff       (20)    16190 2024-03-19 18:53:00.000000 nellie-0.1.8/nellie_napari/nellie_fileselect.py
+-rw-r--r--   0 austin     (501) staff       (20)     2719 2024-03-19 01:57:46.000000 nellie-0.1.8/nellie_napari/nellie_loader.py
+-rw-r--r--   0 austin     (501) staff       (20)    15621 2024-04-01 16:16:45.000000 nellie-0.1.8/nellie_napari/nellie_processor.py
+-rw-r--r--   0 austin     (501) staff       (20)    12833 2024-03-19 16:50:50.000000 nellie-0.1.8/nellie_napari/visualizer.py
+-rw-r--r--   0 austin     (501) staff       (20)       90 2024-01-23 18:46:05.000000 nellie-0.1.8/pyproject.toml
+-rw-r--r--   0 austin     (501) staff       (20)      822 2024-04-26 16:18:29.352696 nellie-0.1.8/setup.cfg
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.348703 nellie-0.1.8/tests/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/tests/__init__.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.349336 nellie-0.1.8/tests/unit/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/tests/unit/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)        6 2024-03-15 22:13:16.000000 nellie-0.1.8/tests/unit/test_frangi_filter.py
+-rw-r--r--   0 austin     (501) staff       (20)     3310 2024-03-15 22:18:53.000000 nellie-0.1.8/tests/unit/test_im_info.py
```

### Comparing `nellie-0.1.7/LICENSE` & `nellie-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/PKG-INFO` & `nellie-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nellie
-Version: 0.1.7
+Version: 0.1.8
 Summary: Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 Home-page: https://github.com/aelefebv/nellie
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre+nellie@gmail.com
 Classifier: Framework :: napari
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `nellie-0.1.7/README.md` & `nellie-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/__init__.py` & `nellie-0.1.8/nellie/__init__.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/feature_extraction/hierarchical.py` & `nellie-0.1.8/nellie/feature_extraction/hierarchical.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/im_info/im_info.py` & `nellie-0.1.8/nellie/im_info/im_info.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/run.py` & `nellie-0.1.8/nellie/run.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/segmentation/filtering.py` & `nellie-0.1.8/nellie/segmentation/filtering.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/segmentation/labelling.py` & `nellie-0.1.8/nellie/segmentation/labelling.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         self.snr_cleaning = snr_cleaning
 
         self.im_memmap = None
         self.frangi_memmap = None
 
         self.max_label_num = 0
 
-        self.min_z_radius_um = min(self.im_info.dim_sizes['Z'], 0.2)
+        if not self.im_info.no_z:
+            self.min_z_radius_um = min(self.im_info.dim_sizes['Z'], 0.2)
 
         self.semantic_mask_memmap = None
         self.instance_label_memmap = None
         self.shape = ()
 
         self.debug = {}
```

### Comparing `nellie-0.1.7/nellie/segmentation/mocap_marking.py` & `nellie-0.1.8/nellie/segmentation/mocap_marking.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/segmentation/networking.py` & `nellie-0.1.8/nellie/segmentation/networking.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/tracking/all_tracks_for_label.py` & `nellie-0.1.8/nellie/tracking/all_tracks_for_label.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/tracking/flow_interpolation.py` & `nellie-0.1.8/nellie/tracking/flow_interpolation.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/tracking/hu_tracking.py` & `nellie-0.1.8/nellie/tracking/hu_tracking.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/tracking/voxel_reassignment.py` & `nellie-0.1.8/nellie/tracking/voxel_reassignment.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/utils/general.py` & `nellie-0.1.8/nellie/utils/general.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/utils/gpu_functions.py` & `nellie-0.1.8/nellie/utils/gpu_functions.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie/utils/torch_xp.py` & `nellie-0.1.8/nellie/utils/torch_xp.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie.egg-info/PKG-INFO` & `nellie-0.1.8/nellie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nellie
-Version: 0.1.7
+Version: 0.1.8
 Summary: Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 Home-page: https://github.com/aelefebv/nellie
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre+nellie@gmail.com
 Classifier: Framework :: napari
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `nellie-0.1.7/nellie.egg-info/SOURCES.txt` & `nellie-0.1.8/nellie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie_napari/batch_mode.py` & `nellie-0.1.8/nellie_napari/batch_mode.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie_napari/home.py` & `nellie-0.1.8/nellie_napari/home.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie_napari/logo.png` & `nellie-0.1.8/nellie_napari/logo.png`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie_napari/nellie_analysis.py` & `nellie-0.1.8/nellie_napari/nellie_analysis.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie_napari/nellie_fileselect.py` & `nellie-0.1.8/nellie_napari/nellie_fileselect.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie_napari/nellie_loader.py` & `nellie-0.1.8/nellie_napari/nellie_loader.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie_napari/nellie_processor.py` & `nellie-0.1.8/nellie_napari/nellie_processor.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/nellie_napari/visualizer.py` & `nellie-0.1.8/nellie_napari/visualizer.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.7/setup.cfg` & `nellie-0.1.8/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nellie
-version = 0.1.7
+version = 0.1.8
 description = Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Austin E. Y. T. Lefebvre
 author_email = austin.e.lefebvre+nellie@gmail.com
 url = https://github.com/aelefebv/nellie
 classifiers =
```

### Comparing `nellie-0.1.7/tests/unit/test_im_info.py` & `nellie-0.1.8/tests/unit/test_im_info.py`

 * *Files identical despite different names*

