# Comparing `tmp/pms-onpremise-encoder-0.0.8.tar.gz` & `tmp/pms-onpremise-encoder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pms-onpremise-encoder-0.0.8.tar", last modified: Fri Apr 26 07:56:33 2024, max compression
+gzip compressed data, was "pms-onpremise-encoder-0.0.9.tar", last modified: Fri Apr 26 08:15:35 2024, max compression
```

## Comparing `pms-onpremise-encoder-0.0.8.tar` & `pms-onpremise-encoder-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 07:56:33.434213 pms-onpremise-encoder-0.0.8/
--rw-r--r--   0 furiosa   (1000) furiosa   (1000)      517 2024-04-26 07:56:33.430213 pms-onpremise-encoder-0.0.8/PKG-INFO
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 07:56:33.430213 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       21 2024-04-26 07:56:31.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/__init__.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 07:56:33.430213 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/common/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-18 08:06:38.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/common/__init__.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1132 2024-04-26 07:56:05.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/common/_mysql_client.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      430 2024-04-22 04:28:43.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/common/_redis_client.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      264 2024-04-19 06:20:36.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/common/data_struct.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 07:56:33.430213 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       83 2024-04-22 05:41:52.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/__init__.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      328 2024-04-19 02:13:11.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/_image_encoder.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     3984 2024-04-26 05:59:21.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/_video_encoder.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 07:56:33.430213 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/processor/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-19 08:51:59.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/processor/__init__.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     7186 2024-04-26 06:57:24.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/processor/_video_processor.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 07:56:33.430213 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/redis/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 07:08:26.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/redis/__init__.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      266 2024-04-22 04:34:34.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/redis/_progress.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 07:56:33.430213 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/repository/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-24 01:37:21.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/repository/__init__.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1042 2024-04-26 05:57:05.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/repository/_file_status_repo.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1625 2024-04-24 04:33:18.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/repository/_video_meta_repo.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 07:56:33.430213 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/utils/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-19 02:29:29.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/utils/__init__.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      446 2024-04-22 07:14:07.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/utils/_calculate_progress.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      950 2024-04-26 03:39:29.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/utils/_delete_file_util.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     4571 2024-04-22 07:32:04.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/utils/_queue_object_generator.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      521 2024-04-26 03:17:00.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/utils/_sub_output_util.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)    10615 2024-04-26 03:11:48.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1075 2024-04-22 05:41:39.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/onpremise_encoder.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 07:56:33.430213 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder.egg-info/
--rw-r--r--   0 furiosa   (1000) furiosa   (1000)      517 2024-04-26 07:56:33.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder.egg-info/PKG-INFO
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1403 2024-04-26 07:56:33.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder.egg-info/SOURCES.txt
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        1 2024-04-26 07:56:33.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder.egg-info/dependency_links.txt
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        1 2024-04-26 07:09:22.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder.egg-info/not-zip-safe
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       76 2024-04-26 07:56:33.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder.egg-info/requires.txt
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       22 2024-04-26 07:56:33.000000 pms-onpremise-encoder-0.0.8/pms_onpremise_encoder.egg-info/top_level.txt
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       38 2024-04-26 07:56:33.434213 pms-onpremise-encoder-0.0.8/setup.cfg
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      650 2024-04-26 07:56:28.000000 pms-onpremise-encoder-0.0.8/setup.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 08:15:35.843801 pms-onpremise-encoder-0.0.9/
+-rw-r--r--   0 furiosa   (1000) furiosa   (1000)      517 2024-04-26 08:15:35.843801 pms-onpremise-encoder-0.0.9/PKG-INFO
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 08:15:35.839801 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       21 2024-04-26 08:15:34.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/__init__.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 08:15:35.843801 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/common/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-18 08:06:38.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/common/__init__.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1148 2024-04-26 08:08:20.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/common/_mysql_client.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      430 2024-04-22 04:28:43.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/common/_redis_client.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      264 2024-04-19 06:20:36.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/common/data_struct.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 08:15:35.843801 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       83 2024-04-22 05:41:52.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/__init__.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      328 2024-04-19 02:13:11.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/_image_encoder.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     3984 2024-04-26 05:59:21.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/_video_encoder.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 08:15:35.843801 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/processor/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-19 08:51:59.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/processor/__init__.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     7186 2024-04-26 06:57:24.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/processor/_video_processor.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 08:15:35.843801 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/redis/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 07:08:26.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/redis/__init__.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      266 2024-04-22 04:34:34.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/redis/_progress.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 08:15:35.843801 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/repository/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-24 01:37:21.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/repository/__init__.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1108 2024-04-26 08:14:42.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/repository/_file_status_repo.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1642 2024-04-26 08:14:49.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/repository/_video_meta_repo.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 08:15:35.843801 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/utils/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-19 02:29:29.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/utils/__init__.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      446 2024-04-22 07:14:07.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/utils/_calculate_progress.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      950 2024-04-26 03:39:29.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/utils/_delete_file_util.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     4571 2024-04-22 07:32:04.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/utils/_queue_object_generator.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      521 2024-04-26 03:17:00.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/utils/_sub_output_util.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)    10615 2024-04-26 03:11:48.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1075 2024-04-22 05:41:39.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/onpremise_encoder.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 08:15:35.843801 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder.egg-info/
+-rw-r--r--   0 furiosa   (1000) furiosa   (1000)      517 2024-04-26 08:15:35.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder.egg-info/PKG-INFO
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1403 2024-04-26 08:15:35.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        1 2024-04-26 08:15:35.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        1 2024-04-26 07:09:22.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder.egg-info/not-zip-safe
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       76 2024-04-26 08:15:35.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder.egg-info/requires.txt
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       22 2024-04-26 08:15:35.000000 pms-onpremise-encoder-0.0.9/pms_onpremise_encoder.egg-info/top_level.txt
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       38 2024-04-26 08:15:35.843801 pms-onpremise-encoder-0.0.9/setup.cfg
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      650 2024-04-26 08:15:03.000000 pms-onpremise-encoder-0.0.9/setup.py
```

### Comparing `pms-onpremise-encoder-0.0.8/PKG-INFO` & `pms-onpremise-encoder-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pms-onpremise-encoder
-Version: 0.0.8
+Version: 0.0.9
 Home-page: 
 Author: Heeyong Kwon
 Author-email: heeyong.kwon@4by4inc.com
 Keywords: pms-encoder
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/common/_mysql_client.py` & `pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/common/_mysql_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,24 +17,24 @@
     def _close(self):
         if self.cursor:
             self.cursor.close()
         if self.conn:
             self.conn.close()
     
     def execute(self, sql, params=None):
-        self._connect()
+        self._connect(self)
         self.cursor.execute(sql, params)
         self.conn.commit()
-        self._close()
+        self._close(self)
         
     def fetchone(self, sql, params=None):
-        self._connect()
+        self._connect(self)
         self.cursor.execute(sql, params)
         result = self.cursor.fetchone()
-        self._close()
+        self._close(self)
         return result
         
     def fetchall(self, sql, params=None):
         self._connect()
         self.cursor.execute(sql, params)
         result = self.cursor.fetchall()
         self.close()
```

### Comparing `pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/_video_encoder.py` & `pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/_video_encoder.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/processor/_video_processor.py` & `pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/processor/_video_processor.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/repository/_video_meta_repo.py` & `pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/repository/_video_meta_repo.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,9 +38,9 @@
         format_data["bit_rate"],
         frame_rate,
         original_data["nb_frames"],
         data["audio"],
         now, 'encoder', now, 'encoder'
     )
     
-    
-    MySQLClient.execute(sql, val)
+    client = MySQLClient()
+    client.execute(sql, val)
```

### Comparing `pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/utils/_delete_file_util.py` & `pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/utils/_delete_file_util.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/utils/_queue_object_generator.py` & `pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/utils/_queue_object_generator.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/utils/_sub_output_util.py` & `pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/utils/_sub_output_util.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py` & `pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.8/pms_onpremise_encoder/onpremise_encoder.py` & `pms-onpremise-encoder-0.0.9/pms_onpremise_encoder/onpremise_encoder.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.8/pms_onpremise_encoder.egg-info/PKG-INFO` & `pms-onpremise-encoder-0.0.9/pms_onpremise_encoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pms-onpremise-encoder
-Version: 0.0.8
+Version: 0.0.9
 Home-page: 
 Author: Heeyong Kwon
 Author-email: heeyong.kwon@4by4inc.com
 Keywords: pms-encoder
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `pms-onpremise-encoder-0.0.8/pms_onpremise_encoder.egg-info/SOURCES.txt` & `pms-onpremise-encoder-0.0.9/pms_onpremise_encoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.8/setup.py` & `pms-onpremise-encoder-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pms-onpremise-encoder',
-    version='0.0.8',
+    version='0.0.9',
     description='',
     author='Heeyong Kwon',
     author_email='heeyong.kwon@4by4inc.com',
     url='',
     install_requires=['ffmpeg-python', 'pms-inference-engine', 'loguru', 'numpy', 'python-dotenv', 'redis', 'PyMySQL', ],
     packages=find_packages(exclude=[]),
     keywords=['pms-encoder'],
```

