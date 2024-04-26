# Comparing `tmp/moonss-0.95.tar.gz` & `tmp/moonss-0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonss-0.95.tar", last modified: Wed Apr  3 05:20:29 2024, max compression
+gzip compressed data, was "moonss-0.96.tar", last modified: Fri Apr 26 04:07:26 2024, max compression
```

## Comparing `moonss-0.95.tar` & `moonss-0.96.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:29.576264 moonss-0.95/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-03 05:20:20.000000 moonss-0.95/DownloadHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-03 05:20:29.576264 moonss-0.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 05:20:20.000000 moonss-0.95/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-03 05:20:20.000000 moonss-0.95/SourceDataHelper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:29.572264 moonss-0.95/moonss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-03 05:20:29.000000 moonss-0.95/moonss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 05:20:29.000000 moonss-0.95/moonss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:20:29.000000 moonss-0.95/moonss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 05:20:29.000000 moonss-0.95/moonss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 05:20:29.000000 moonss-0.95/moonss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-03 05:20:20.000000 moonss-0.95/moonss.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:20:29.576264 moonss-0.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-03 05:20:20.000000 moonss-0.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:07:26.695057 moonss-0.96/
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-26 04:07:18.000000 moonss-0.96/DownloadHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-26 04:07:26.695057 moonss-0.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 04:07:18.000000 moonss-0.96/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-26 04:07:18.000000 moonss-0.96/SourceDataHelper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:07:26.695057 moonss-0.96/moonss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-26 04:07:26.000000 moonss-0.96/moonss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 04:07:26.000000 moonss-0.96/moonss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:07:26.000000 moonss-0.96/moonss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 04:07:26.000000 moonss-0.96/moonss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 04:07:26.000000 moonss-0.96/moonss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-26 04:07:18.000000 moonss-0.96/moonss.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 04:07:26.695057 moonss-0.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-26 04:07:18.000000 moonss-0.96/setup.py
```

### Comparing `moonss-0.95/DownloadHelper.py` & `moonss-0.96/DownloadHelper.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,8 +58,14 @@
     return download_file(f"https://aweme.snssdk.com/aweme/v1/play/?video_id={video_id}&ratio=1080p&line=0",None, "mp4")
 def donwload_instagram_video(crawl_data_txt):
     crawl_data = json.loads(crawl_data_txt)
     if "video_url" in crawl_data:
         return download_file(crawl_data['video_url'],None, "mp4")
     else:
         return None
+def donwload_artlistio_video(crawl_data_txt):
+    crawl_data = json.loads(crawl_data_txt)
+    if "video_url" in crawl_data:
+        return download_file(crawl_data['video_url'],None, "mp4")
+    else:
+        return None
```

### Comparing `moonss-0.95/PKG-INFO` & `moonss-0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonss
-Version: 0.95
+Version: 0.96
 Summary: A Des of moonss
 Home-page: https://github.com/vtandroid/dokr
 Author: Thanh Hoa
 Author-email: thanhhoakhmt1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moonss-0.95/SourceDataHelper.py` & `moonss-0.96/SourceDataHelper.py`

 * *Files identical despite different names*

### Comparing `moonss-0.95/moonss.egg-info/PKG-INFO` & `moonss-0.96/moonss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonss
-Version: 0.95
+Version: 0.96
 Summary: A Des of moonss
 Home-page: https://github.com/vtandroid/dokr
 Author: Thanh Hoa
 Author-email: thanhhoakhmt1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moonss-0.95/moonss.py` & `moonss-0.96/moonss.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import time
-from DownloadHelper import download_ytdlp, download_tiktok_video, download_douyin_video, donwload_instagram_video
+from DownloadHelper import download_ytdlp, download_tiktok_video, download_douyin_video, donwload_instagram_video, donwload_artlistio_video
 from SourceDataHelper import process_video_sd
 import requests
 
 URL_HOME="https://moonseo.app"
 URL_GET_JOB=f"{URL_HOME}/api/source/data/crawl"
 URL_UPDATE_JOB=f"{URL_HOME}/api/source/data/update-by-id"
 headers={"platform":"autowin"}
@@ -20,14 +20,16 @@
             video_path = download_tiktok_video(obj['ori_link'])
         if obj['platform'] =='youtube' or obj['platform'] =='youtube-long':
             video_path = download_ytdlp(obj['ori_link'])
         if obj['platform'] =='douyin':
             video_path = download_douyin_video(obj['platform_id'])
         if obj['platform'] == 'instagram':
             video_path = donwload_instagram_video(obj['crawl_data'])
+        if obj['platform'] == 'artlistio':
+            video_path = donwload_artlistio_video(obj['crawl_data'])
         sc_new = process_video_sd(video_path)
         if not sc_new:
             sc_new={"id": obj['id']}
             if(obj['crawl_retries']<3):
                 sc_new['crawl_retries']=obj['crawl_retries']+1
                 sc_new['status'] = 1 #retries
             else:
```

### Comparing `moonss-0.95/setup.py` & `moonss-0.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='moonss',
-    version='0.95',
+    version='0.96',
     author="Thanh Hoa",
     author_email="thanhhoakhmt1@gmail.com",
     description="A Des of moonss",
     long_description="Des",
     long_description_content_type="text/markdown",
     url="https://github.com/vtandroid/dokr",
     packages=setuptools.find_packages(),
```

