# Comparing `tmp/ld_msgs-0.1.tar.gz` & `tmp/ld_msgs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ld_msgs-0.1.tar", last modified: Fri Apr 26 15:19:39 2024, max compression
+gzip compressed data, was "ld_msgs-0.1.1.tar", last modified: Fri Apr 26 15:42:15 2024, max compression
```

## Comparing `ld_msgs-0.1.tar` & `ld_msgs-0.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 15:19:39.905000 ld_msgs-0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2024-04-26 15:19:39.899000 ld_msgs-0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1067 2024-04-26 15:18:23.000000 ld_msgs-0.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 15:19:39.202000 ld_msgs-0.1/ld_msgs.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2024-04-26 15:19:38.000000 ld_msgs-0.1/ld_msgs.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2024-04-26 15:19:38.000000 ld_msgs-0.1/ld_msgs.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-26 15:19:38.000000 ld_msgs-0.1/ld_msgs.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2024-04-26 15:19:38.000000 ld_msgs-0.1/ld_msgs.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-04-26 15:19:38.000000 ld_msgs-0.1/ld_msgs.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 15:19:39.879000 ld_msgs-0.1/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1071 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22329 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_image_tagging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10493 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_2d_bbox.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14195 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_2d_bbox_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16461 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_2d_instance_segmentation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4835 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_2d_polyline.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_2d_polyline_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26612 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_2dobject.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29664 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_2dobject_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36941 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_annotation_comment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21483 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_annotation_comment_item.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39518 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_annotation_comment_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_can.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_can2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27850 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_data_msg.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16722 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_ego_motion.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24385 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_face.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10533 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_gps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9283 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_image.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15051 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_imu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17608 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_imu_gps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22494 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_imugps_can.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    49544 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_mesh.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48580 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_mesh_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33434 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_mobileye_lane.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11909 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_mobileye_traffic_sign.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48881 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_object.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    51330 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_object_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4123 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_packet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9033 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_road_feature_facility.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14093 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_road_feature_feature.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7894 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_road_feature_lane.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29628 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_road_feature_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6998 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_rt_matrix.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7047 2024-04-26 12:08:33.000000 ld_msgs-0.1/msg/_ld_sensor_location.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-26 15:19:39.909000 ld_msgs-0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      809 2024-04-26 15:17:47.000000 ld_msgs-0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 15:42:15.321000 ld_msgs-0.1.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      623 2024-04-26 15:42:15.316000 ld_msgs-0.1.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       95 2024-04-26 15:33:23.000000 ld_msgs-0.1.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 15:42:14.613000 ld_msgs-0.1.1/ld_msgs.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      623 2024-04-26 15:42:14.000000 ld_msgs-0.1.1/ld_msgs.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2024-04-26 15:42:14.000000 ld_msgs-0.1.1/ld_msgs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-26 15:42:14.000000 ld_msgs-0.1.1/ld_msgs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2024-04-26 15:42:14.000000 ld_msgs-0.1.1/ld_msgs.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-04-26 15:42:14.000000 ld_msgs-0.1.1/ld_msgs.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 15:42:15.296000 ld_msgs-0.1.1/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1071 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22329 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_image_tagging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10493 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_2d_bbox.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14195 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_2d_bbox_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16461 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_2d_instance_segmentation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4835 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_2d_polyline.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_2d_polyline_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26612 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_2dobject.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29664 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_2dobject_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36941 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_annotation_comment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21483 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_annotation_comment_item.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39518 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_annotation_comment_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_can.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_can2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27850 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_data_msg.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16722 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_ego_motion.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24385 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_face.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10533 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_gps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9283 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_image.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15051 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_imu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17608 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_imu_gps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22494 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_imugps_can.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    49544 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_mesh.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48580 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_mesh_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33434 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_mobileye_lane.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11909 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_mobileye_traffic_sign.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48881 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_object.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    51330 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_object_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4123 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_packet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9033 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_road_feature_facility.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14093 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_road_feature_feature.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7894 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_road_feature_lane.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29628 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_road_feature_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6998 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_rt_matrix.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7047 2024-04-26 12:08:33.000000 ld_msgs-0.1.1/msg/_ld_sensor_location.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-26 15:42:15.328000 ld_msgs-0.1.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2024-04-26 15:40:57.000000 ld_msgs-0.1.1/setup.py
```

### Comparing `ld_msgs-0.1/ld_msgs.egg-info/SOURCES.txt` & `ld_msgs-0.1.1/ld_msgs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/__init__.py` & `ld_msgs-0.1.1/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_image_tagging.py` & `ld_msgs-0.1.1/msg/_image_tagging.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_2d_bbox.py` & `ld_msgs-0.1.1/msg/_ld_2d_bbox.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_2d_bbox_list.py` & `ld_msgs-0.1.1/msg/_ld_2d_bbox_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_2d_instance_segmentation.py` & `ld_msgs-0.1.1/msg/_ld_2d_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_2d_polyline.py` & `ld_msgs-0.1.1/msg/_ld_2d_polyline.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_2d_polyline_list.py` & `ld_msgs-0.1.1/msg/_ld_2d_polyline_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_2dobject.py` & `ld_msgs-0.1.1/msg/_ld_2dobject.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_2dobject_list.py` & `ld_msgs-0.1.1/msg/_ld_2dobject_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_annotation_comment.py` & `ld_msgs-0.1.1/msg/_ld_annotation_comment.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_annotation_comment_item.py` & `ld_msgs-0.1.1/msg/_ld_annotation_comment_item.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_annotation_comment_list.py` & `ld_msgs-0.1.1/msg/_ld_annotation_comment_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_can.py` & `ld_msgs-0.1.1/msg/_ld_can.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_can2.py` & `ld_msgs-0.1.1/msg/_ld_can2.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_data_msg.py` & `ld_msgs-0.1.1/msg/_ld_data_msg.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_ego_motion.py` & `ld_msgs-0.1.1/msg/_ld_ego_motion.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_face.py` & `ld_msgs-0.1.1/msg/_ld_face.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_gps.py` & `ld_msgs-0.1.1/msg/_ld_gps.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_image.py` & `ld_msgs-0.1.1/msg/_ld_image.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_imu.py` & `ld_msgs-0.1.1/msg/_ld_imu.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_imu_gps.py` & `ld_msgs-0.1.1/msg/_ld_imu_gps.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_imugps_can.py` & `ld_msgs-0.1.1/msg/_ld_imugps_can.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_mesh.py` & `ld_msgs-0.1.1/msg/_ld_mesh.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_mesh_list.py` & `ld_msgs-0.1.1/msg/_ld_mesh_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_mobileye_lane.py` & `ld_msgs-0.1.1/msg/_ld_mobileye_lane.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_mobileye_traffic_sign.py` & `ld_msgs-0.1.1/msg/_ld_mobileye_traffic_sign.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_object.py` & `ld_msgs-0.1.1/msg/_ld_object.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_object_list.py` & `ld_msgs-0.1.1/msg/_ld_object_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_packet.py` & `ld_msgs-0.1.1/msg/_ld_packet.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_road_feature_facility.py` & `ld_msgs-0.1.1/msg/_ld_road_feature_facility.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_road_feature_feature.py` & `ld_msgs-0.1.1/msg/_ld_road_feature_feature.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_road_feature_lane.py` & `ld_msgs-0.1.1/msg/_ld_road_feature_lane.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_road_feature_list.py` & `ld_msgs-0.1.1/msg/_ld_road_feature_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_rt_matrix.py` & `ld_msgs-0.1.1/msg/_ld_rt_matrix.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/msg/_ld_sensor_location.py` & `ld_msgs-0.1.1/msg/_ld_sensor_location.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.1/setup.py` & `ld_msgs-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ld_msgs',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     description='ld_msg lib for python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='shuo shen',
     author_email='shuo.shen@liangdao.de',
     url='',
```

