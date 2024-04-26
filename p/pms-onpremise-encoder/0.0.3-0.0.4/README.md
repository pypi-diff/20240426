# Comparing `tmp/pms-onpremise-encoder-0.0.3.tar.gz` & `tmp/pms-onpremise-encoder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pms-onpremise-encoder-0.0.3.tar", last modified: Fri Apr 26 06:51:14 2024, max compression
+gzip compressed data, was "pms-onpremise-encoder-0.0.4.tar", last modified: Fri Apr 26 06:53:58 2024, max compression
```

## Comparing `pms-onpremise-encoder-0.0.3.tar` & `pms-onpremise-encoder-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:51:14.500207 pms-onpremise-encoder-0.0.3/
--rw-r--r--   0 furiosa   (1000) furiosa   (1000)      517 2024-04-26 06:51:14.500207 pms-onpremise-encoder-0.0.3/PKG-INFO
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:51:14.496207 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       21 2024-04-26 06:51:02.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/__init__.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:51:14.496207 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/common/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-18 08:06:38.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/common/__init__.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1127 2024-04-22 05:31:02.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/common/_mysql_client.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      430 2024-04-22 04:28:43.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/common/_redis_client.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      264 2024-04-19 06:20:36.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/common/data_struct.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:51:14.496207 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       83 2024-04-22 05:41:52.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/__init__.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      328 2024-04-19 02:13:11.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/_image_encoder.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     3984 2024-04-26 05:59:21.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/_video_encoder.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:51:14.496207 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/processor/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-19 08:51:59.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/processor/__init__.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     7184 2024-04-26 04:35:51.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/processor/_video_processor.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:51:14.500207 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/repository/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-24 01:37:21.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/repository/__init__.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1042 2024-04-26 05:57:05.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/repository/_file_status_repo.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1625 2024-04-24 04:33:18.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/repository/_video_meta_repo.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:51:14.500207 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/utils/
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-19 02:29:29.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/utils/__init__.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      446 2024-04-22 07:14:07.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/utils/_calculate_progress.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      950 2024-04-26 03:39:29.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/utils/_delete_file_util.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     4571 2024-04-22 07:32:04.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/utils/_queue_object_generator.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      521 2024-04-26 03:17:00.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/utils/_sub_output_util.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)    10615 2024-04-26 03:11:48.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1075 2024-04-22 05:41:39.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/onpremise_encoder.py
-drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:51:14.496207 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder.egg-info/
--rw-r--r--   0 furiosa   (1000) furiosa   (1000)      517 2024-04-26 06:51:14.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder.egg-info/PKG-INFO
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1306 2024-04-26 06:51:14.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder.egg-info/SOURCES.txt
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        1 2024-04-26 06:51:14.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder.egg-info/dependency_links.txt
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        1 2024-04-26 06:51:14.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder.egg-info/not-zip-safe
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       76 2024-04-26 06:51:14.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder.egg-info/requires.txt
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       22 2024-04-26 06:51:14.000000 pms-onpremise-encoder-0.0.3/pms_onpremise_encoder.egg-info/top_level.txt
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       38 2024-04-26 06:51:14.500207 pms-onpremise-encoder-0.0.3/setup.cfg
--rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      650 2024-04-26 06:51:06.000000 pms-onpremise-encoder-0.0.3/setup.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:53:58.413656 pms-onpremise-encoder-0.0.4/
+-rw-r--r--   0 furiosa   (1000) furiosa   (1000)      517 2024-04-26 06:53:58.413656 pms-onpremise-encoder-0.0.4/PKG-INFO
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:53:58.409656 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       21 2024-04-26 06:53:07.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/__init__.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:53:58.409656 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/common/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-18 08:06:38.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/common/__init__.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1127 2024-04-22 05:31:02.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/common/_mysql_client.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      430 2024-04-22 04:28:43.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/common/_redis_client.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      264 2024-04-19 06:20:36.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/common/data_struct.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:53:58.409656 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       83 2024-04-22 05:41:52.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/__init__.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      328 2024-04-19 02:13:11.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/_image_encoder.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     3984 2024-04-26 05:59:21.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/_video_encoder.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:53:58.409656 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/processor/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-19 08:51:59.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/processor/__init__.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     7186 2024-04-26 06:52:24.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/processor/_video_processor.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:53:58.413656 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/repository/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-24 01:37:21.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/repository/__init__.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1042 2024-04-26 05:57:05.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/repository/_file_status_repo.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1625 2024-04-24 04:33:18.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/repository/_video_meta_repo.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:53:58.413656 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/utils/
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        0 2024-04-19 02:29:29.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/utils/__init__.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      446 2024-04-22 07:14:07.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/utils/_calculate_progress.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      950 2024-04-26 03:39:29.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/utils/_delete_file_util.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     4571 2024-04-22 07:32:04.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/utils/_queue_object_generator.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      521 2024-04-26 03:17:00.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/utils/_sub_output_util.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)    10615 2024-04-26 03:11:48.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1075 2024-04-22 05:41:39.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/onpremise_encoder.py
+drwxrwxr-x   0 furiosa   (1000) furiosa   (1000)        0 2024-04-26 06:53:58.409656 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder.egg-info/
+-rw-r--r--   0 furiosa   (1000) furiosa   (1000)      517 2024-04-26 06:53:58.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder.egg-info/PKG-INFO
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)     1306 2024-04-26 06:53:58.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        1 2024-04-26 06:53:58.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)        1 2024-04-26 06:53:58.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder.egg-info/not-zip-safe
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       76 2024-04-26 06:53:58.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder.egg-info/requires.txt
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       22 2024-04-26 06:53:58.000000 pms-onpremise-encoder-0.0.4/pms_onpremise_encoder.egg-info/top_level.txt
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)       38 2024-04-26 06:53:58.413656 pms-onpremise-encoder-0.0.4/setup.cfg
+-rw-rw-r--   0 furiosa   (1000) furiosa   (1000)      650 2024-04-26 06:53:19.000000 pms-onpremise-encoder-0.0.4/setup.py
```

### Comparing `pms-onpremise-encoder-0.0.3/PKG-INFO` & `pms-onpremise-encoder-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pms-onpremise-encoder
-Version: 0.0.3
+Version: 0.0.4
 Home-page: 
 Author: Heeyong Kwon
 Author-email: heeyong.kwon@4by4inc.com
 Keywords: pms-encoder
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/common/_mysql_client.py` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/common/_mysql_client.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/_video_encoder.py` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/_video_encoder.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/processor/_video_processor.py` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/processor/_video_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,16 +168,16 @@
     inferenced_data = next(s for s in probe["streams"] if s["codec_type"] == "video")
     format_data = probe.get("format", {})
     inferenced_size = os.path.getsize("/app/tmp/{}.{}".format(redis_data["fileKey"], redis_data["format"].lower()))
     
     insert_inferenced_file_meta(
         redis_data=redis_data,
         original_data=meta_data,
-        inferenced_data=inferenced_data
-        format_data=format_data
+        inferenced_data=inferenced_data,
+        format_data=format_data,
         file_size=inferenced_size,
         audio=audio,
     )
     logger.info("COMPLETE || save_inferenced_meta")
     
 
 def downscale_sub_output(
```

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/repository/_file_status_repo.py` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/repository/_file_status_repo.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/repository/_video_meta_repo.py` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/repository/_video_meta_repo.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/utils/_delete_file_util.py` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/utils/_delete_file_util.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/utils/_queue_object_generator.py` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/utils/_queue_object_generator.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/utils/_sub_output_util.py` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/utils/_sub_output_util.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/encoder/utils/_video_ffmpeg_cmd_generator.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder/onpremise_encoder.py` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder/onpremise_encoder.py`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder.egg-info/PKG-INFO` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pms-onpremise-encoder
-Version: 0.0.3
+Version: 0.0.4
 Home-page: 
 Author: Heeyong Kwon
 Author-email: heeyong.kwon@4by4inc.com
 Keywords: pms-encoder
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `pms-onpremise-encoder-0.0.3/pms_onpremise_encoder.egg-info/SOURCES.txt` & `pms-onpremise-encoder-0.0.4/pms_onpremise_encoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pms-onpremise-encoder-0.0.3/setup.py` & `pms-onpremise-encoder-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pms-onpremise-encoder',
-    version='0.0.3',
+    version='0.0.4',
     description='',
     author='Heeyong Kwon',
     author_email='heeyong.kwon@4by4inc.com',
     url='',
     install_requires=['ffmpeg-python', 'pms-inference-engine', 'loguru', 'numpy', 'python-dotenv', 'redis', 'PyMySQL', ],
     packages=find_packages(exclude=[]),
     keywords=['pms-encoder'],
```

