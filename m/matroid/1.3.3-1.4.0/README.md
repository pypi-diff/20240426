# Comparing `tmp/matroid-1.3.3.tar.gz` & `tmp/matroid-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matroid-1.3.3.tar", last modified: Fri Mar 15 00:29:50 2024, max compression
+gzip compressed data, was "matroid-1.4.0.tar", last modified: Fri Apr 26 00:41:24 2024, max compression
```

## Comparing `matroid-1.3.3.tar` & `matroid-1.4.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-15 00:29:50.721826 matroid-1.3.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2024-03-15 00:28:15.000000 matroid-1.3.3/LICENSE.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2024-03-15 00:29:50.721826 matroid-1.3.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8690 2024-03-15 00:28:15.000000 matroid-1.3.3/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-15 00:29:50.697826 matroid-1.3.3/matroid/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4259 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1217 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/error.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-15 00:29:50.705826 matroid-1.3.3/matroid/src/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2193 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/accounts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7816 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/collections.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10796 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/detectors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9921 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5243 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/labels.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/sse.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10239 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6339 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/temporal_task.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6964 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/video_summary.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3355 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/src/videos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-03-15 00:28:15.000000 matroid-1.3.3/matroid/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-15 00:29:50.697826 matroid-1.3.3/matroid.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2024-03-15 00:29:50.000000 matroid-1.3.3/matroid.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2024-03-15 00:29:50.000000 matroid-1.3.3/matroid.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-15 00:29:50.000000 matroid-1.3.3/matroid.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-03-15 00:29:50.000000 matroid-1.3.3/matroid.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2024-03-15 00:29:50.000000 matroid-1.3.3/matroid.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-15 00:29:50.721826 matroid-1.3.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      463 2024-03-15 00:28:15.000000 matroid-1.3.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-15 00:29:50.721826 matroid-1.3.3/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-15 00:28:15.000000 matroid-1.3.3/test/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      969 2024-03-15 00:28:15.000000 matroid-1.3.3/test/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      823 2024-03-15 00:28:15.000000 matroid-1.3.3/test/data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2024-03-15 00:28:15.000000 matroid-1.3.3/test/helper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2024-03-15 00:28:15.000000 matroid-1.3.3/test/test_accounts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5714 2024-03-15 00:28:15.000000 matroid-1.3.3/test/test_collections.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11943 2024-03-15 00:28:15.000000 matroid-1.3.3/test/test_detectors_labels.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2328 2024-03-15 00:28:15.000000 matroid-1.3.3/test/test_images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9925 2024-03-15 00:28:15.000000 matroid-1.3.3/test/test_streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7318 2024-03-15 00:28:15.000000 matroid-1.3.3/test/test_temporal_task.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9491 2024-03-15 00:28:15.000000 matroid-1.3.3/test/test_video_summary.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2024-03-15 00:28:15.000000 matroid-1.3.3/test/test_videos.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:41:24.548307 matroid-1.4.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2024-04-26 00:39:41.000000 matroid-1.4.0/LICENSE.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2024-04-26 00:41:24.548307 matroid-1.4.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8690 2024-04-26 00:39:41.000000 matroid-1.4.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:41:24.516306 matroid-1.4.0/matroid/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4259 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1217 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/error.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:41:24.528307 matroid-1.4.0/matroid/src/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2193 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/accounts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7816 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/collections.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10796 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/detectors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9921 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/images.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5243 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/labels.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/sse.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10239 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6407 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/temporal_task.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6964 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/video_summary.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3355 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/videos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:41:24.516306 matroid-1.4.0/matroid.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2024-04-26 00:41:24.000000 matroid-1.4.0/matroid.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2024-04-26 00:41:24.000000 matroid-1.4.0/matroid.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-26 00:41:24.000000 matroid-1.4.0/matroid.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-26 00:41:24.000000 matroid-1.4.0/matroid.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2024-04-26 00:41:24.000000 matroid-1.4.0/matroid.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-26 00:41:24.548307 matroid-1.4.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      463 2024-04-26 00:39:41.000000 matroid-1.4.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:41:24.548307 matroid-1.4.0/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:39:41.000000 matroid-1.4.0/test/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      969 2024-04-26 00:39:41.000000 matroid-1.4.0/test/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      849 2024-04-26 00:39:41.000000 matroid-1.4.0/test/data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2024-04-26 00:39:41.000000 matroid-1.4.0/test/helper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_accounts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5714 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_collections.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11943 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_detectors_labels.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2328 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_images.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9925 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7590 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_temporal_task.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9491 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_video_summary.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_videos.py
```

### Comparing `matroid-1.3.3/LICENSE.txt` & `matroid-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/README.md` & `matroid-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/client.py` & `matroid-1.4.0/matroid/client.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/error.py` & `matroid-1.4.0/matroid/error.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/src/accounts.py` & `matroid-1.4.0/matroid/src/accounts.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/src/collections.py` & `matroid-1.4.0/matroid/src/collections.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/src/detectors.py` & `matroid-1.4.0/matroid/src/detectors.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/src/helpers.py` & `matroid-1.4.0/matroid/src/helpers.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/src/images.py` & `matroid-1.4.0/matroid/src/images.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/src/labels.py` & `matroid-1.4.0/matroid/src/labels.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/src/sse.py` & `matroid-1.4.0/matroid/src/sse.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/src/streams.py` & `matroid-1.4.0/matroid/src/streams.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/src/temporal_task.py` & `matroid-1.4.0/matroid/src/temporal_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,27 +67,29 @@
     self,
     streamId,
     startTime,
     endTime,
     detectorId,
     labels=None,
     fps=None,
+    thresholds=None,
 ):
     """Localize actions in a stream"""
     (endpoint, method) = self.endpoints["localize_stream_actions"]
     endpoint = endpoint.replace(":streamId", streamId)
 
     try:
         headers = {"Authorization": self.token.authorization_header()}
         data = {
             "startTime": startTime,
             "endTime": endTime,
             "detectorId": detectorId,
             "labels": labels,
             "fps": fps,
+            "detectionThresholds": thresholds,
         }
 
         return requests.request(method, endpoint, **{"headers": headers, "data": data})
     except Exception as e:
         raise error.APIConnectionError(message=e)
```

### Comparing `matroid-1.3.3/matroid/src/video_summary.py` & `matroid-1.4.0/matroid/src/video_summary.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid/src/videos.py` & `matroid-1.4.0/matroid/src/videos.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/matroid.egg-info/SOURCES.txt` & `matroid-1.4.0/matroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/test/conftest.py` & `matroid-1.4.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/test/data.py` & `matroid-1.4.0/test/data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 
 EVERYDAY_OBJECT_DETECTOR_ID = "598e23679fd1a805a5c09275"
 DETECTOR_LABELS = ["person", "boat"]
+DEFAULT_DETECTION_THRESHOLD = 0.5
 RANDOM_MONGO_ID = "5d0148512563ae5e748e9a66"
 
 TEST_IMAGE_URL = (
     "https://m-test-public.s3.amazonaws.com/test/python-client/tesla-cat.jpg"
 )
-TEST_IMAGE_URL_DOG = (
-    "https://m-test-public.s3.amazonaws.com/test/python-client/dog.jpg"
-)
+TEST_IMAGE_URL_DOG = "https://m-test-public.s3.amazonaws.com/test/python-client/dog.jpg"
 TEST_IMAGE_FILE = os.getcwd() + "/test/test_file/cat.png"
 TEST_IMAGE_FILE_DOG = os.getcwd() + "/test/test_file/dog.png"
 
 TEST_LOCAL_VIDEO_URL = os.getcwd() + "/test/test_file/construction.mp4"
 TEST_VIDEO_URL = "https://www.youtube.com/watch?v=nDvh3upNJmA"
 TEST_S3_VIDEO_URL = (
     "https://m-test-public.s3-us-west-2.amazonaws.com/videos/Multiple+cars+-+5s.mp4"
```

### Comparing `matroid-1.3.3/test/test_accounts.py` & `matroid-1.4.0/test/test_accounts.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/test/test_collections.py` & `matroid-1.4.0/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/test/test_detectors_labels.py` & `matroid-1.4.0/test/test_detectors_labels.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/test/test_images.py` & `matroid-1.4.0/test/test_images.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/test/test_streams.py` & `matroid-1.4.0/test/test_streams.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/test/test_temporal_task.py` & `matroid-1.4.0/test/test_temporal_task.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from test.data import (
     TEST_LOCAL_VIDEO_URL,
     TEST_S3_VIDEO_URL,
     TEST_VIDEO_URL,
     EVERYDAY_OBJECT_DETECTOR_ID,
     DETECTOR_LABELS,
+    DEFAULT_DETECTION_THRESHOLD,
 )
 from matroid.error import APIError
 from test.helper import print_test_pass
 
 
 class TestTemporalTask(object):
     def test_temporal_task(self, set_up_client):
@@ -164,34 +165,37 @@
         with pytest.raises(APIError) as e:
             self.api.localize_stream_actions(
                 streamId=streamId,
                 startTime="test",
                 endTime=endTime,
                 detectorId=EVERYDAY_OBJECT_DETECTOR_ID,
                 labels=DETECTOR_LABELS,
+                thresholds=[DEFAULT_DETECTION_THRESHOLD] * len(DETECTOR_LABELS),
             )
         assert "Invalid dates provided" in str(e)
         with pytest.raises(APIError) as e:
             self.api.localize_stream_actions(
                 detectorId=EVERYDAY_OBJECT_DETECTOR_ID,
                 labels=DETECTOR_LABELS,
                 streamId=streamId,
                 startTime=datetime.utcfromtimestamp(
                     int(time.time()) - (24 * 60 * 60 * 8)
                 ),
                 endTime=endTime,
+                thresholds=[DEFAULT_DETECTION_THRESHOLD] * len(DETECTOR_LABELS),
             )
         assert "Provided dates are not within your stream" in str(e)
 
         res = self.api.localize_stream_actions(
             streamId,
             startTime,
             endTime,
             detectorId=EVERYDAY_OBJECT_DETECTOR_ID,
             labels=DETECTOR_LABELS,
+            thresholds=[DEFAULT_DETECTION_THRESHOLD] * len(DETECTOR_LABELS),
         )
         assert res["temporal_task"]["feed"] == streamId
         assert (
             datetime.strptime(
                 res["temporal_task"]["startTime"], "%Y-%m-%dT%H:%M:%S.000Z"
             )
             == startTime
```

### Comparing `matroid-1.3.3/test/test_video_summary.py` & `matroid-1.4.0/test/test_video_summary.py`

 * *Files identical despite different names*

### Comparing `matroid-1.3.3/test/test_videos.py` & `matroid-1.4.0/test/test_videos.py`

 * *Files identical despite different names*

