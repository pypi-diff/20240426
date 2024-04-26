# Comparing `tmp/ncmlistdownloader-1.0.1.24042601.tar.gz` & `tmp/ncmlistdownloader-1.0.2.240426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.1.24042601.tar", last modified: Fri Apr 26 07:22:43 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.2.240426.tar", last modified: Fri Apr 26 07:24:08 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.1.24042601.tar` & `ncmlistdownloader-1.0.2.240426.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 07:22:43.093518 ncmlistdownloader-1.0.1.24042601/
--rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.24042601/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-04-26 07:22:43.085127 ncmlistdownloader-1.0.1.24042601/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-26 07:22:43.053135 ncmlistdownloader-1.0.1.24042601/cmd/
--rw-rw-rw-   0        0        0     1736 2024-04-25 10:28:31.000000 ncmlistdownloader-1.0.1.24042601/cmd/__init__.py
--rw-rw-rw-   0        0        0      653 2024-04-25 14:23:37.000000 ncmlistdownloader-1.0.1.24042601/cmd/common.py
--rw-rw-rw-   0        0        0     1661 2024-04-25 14:30:46.000000 ncmlistdownloader-1.0.1.24042601/cmd/download.py
--rw-rw-rw-   0        0        0     2501 2024-04-22 14:56:53.000000 ncmlistdownloader-1.0.1.24042601/cmd/find_from_id.py
--rw-rw-rw-   0        0        0     1664 2024-04-25 10:31:47.000000 ncmlistdownloader-1.0.1.24042601/cmd/json_io.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:22:43.053135 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1232 2024-04-26 07:19:53.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:22:43.081419 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2866 2024-04-26 07:14:57.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2258 2024-04-26 07:22:12.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:22:43.082419 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:22:43.084413 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-26 07:14:43.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:22:43.085127 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2323 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:22:43.085127 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     8428 2024-04-26 07:14:17.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:22:43.085127 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-04-26 07:22:43.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      687 2024-04-26 07:22:43.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 07:22:43.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-26 07:22:43.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-26 07:22:43.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-26 07:22:43.000000 ncmlistdownloader-1.0.1.24042601/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 07:22:43.093518 ncmlistdownloader-1.0.1.24042601/setup.cfg
--rw-rw-rw-   0        0        0     1758 2024-04-26 07:22:17.000000 ncmlistdownloader-1.0.1.24042601/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.812514 ncmlistdownloader-1.0.2.240426/
+-rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.2.240426/LICENSE
+-rw-rw-rw-   0        0        0     1409 2024-04-26 07:24:08.812514 ncmlistdownloader-1.0.2.240426/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.780915 ncmlistdownloader-1.0.2.240426/cmd/
+-rw-rw-rw-   0        0        0     1736 2024-04-25 10:28:31.000000 ncmlistdownloader-1.0.2.240426/cmd/__init__.py
+-rw-rw-rw-   0        0        0      653 2024-04-25 14:23:37.000000 ncmlistdownloader-1.0.2.240426/cmd/common.py
+-rw-rw-rw-   0        0        0     1661 2024-04-25 14:30:46.000000 ncmlistdownloader-1.0.2.240426/cmd/download.py
+-rw-rw-rw-   0        0        0     2501 2024-04-22 14:56:53.000000 ncmlistdownloader-1.0.2.240426/cmd/find_from_id.py
+-rw-rw-rw-   0        0        0     1664 2024-04-25 10:31:47.000000 ncmlistdownloader-1.0.2.240426/cmd/json_io.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.782515 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1232 2024-04-26 07:19:53.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.802026 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2866 2024-04-26 07:14:57.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2258 2024-04-26 07:22:12.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.803346 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.805342 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-26 07:14:43.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.806321 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2323 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.807339 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     8428 2024-04-26 07:14:17.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:24:08.810311 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1409 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      687 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-26 07:24:08.000000 ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 07:24:08.812514 ncmlistdownloader-1.0.2.240426/setup.cfg
+-rw-rw-rw-   0        0        0     1756 2024-04-26 07:23:52.000000 ncmlistdownloader-1.0.2.240426/setup.py
```

### Comparing `ncmlistdownloader-1.0.1.24042601/LICENSE` & `ncmlistdownloader-1.0.2.240426/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/PKG-INFO` & `ncmlistdownloader-1.0.2.240426/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.1.24042601
+Version: 1.0.2.240426
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.1.24042601/cmd/__init__.py` & `ncmlistdownloader-1.0.2.240426/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/cmd/common.py` & `ncmlistdownloader-1.0.2.240426/cmd/common.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/cmd/download.py` & `ncmlistdownloader-1.0.2.240426/cmd/download.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/cmd/find_from_id.py` & `ncmlistdownloader-1.0.2.240426/cmd/find_from_id.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/cmd/json_io.py` & `ncmlistdownloader-1.0.2.240426/cmd/json_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/global_args.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.2.240426/ncmlistdownloader/song/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.1.24042601
+Version: 1.0.2.240426
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.1.24042601/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.2.240426/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.24042601/setup.py` & `ncmlistdownloader-1.0.2.240426/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.1.24042601",
+    version = "1.0.2.240426",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
     install_requires = ['pycryptodome','pillow','mutagen','requests',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

