# Comparing `tmp/ncmlistdownloader-1.0.1.240425.tar.gz` & `tmp/ncmlistdownloader-1.0.1.240425a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.1.240425.tar", last modified: Thu Apr 25 14:51:57 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.1.240425a1.tar", last modified: Thu Apr 25 14:50:58 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.1.240425.tar` & `ncmlistdownloader-1.0.1.240425a1.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 14:51:57.435033 ncmlistdownloader-1.0.1.240425/
--rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425/LICENSE
--rw-rw-rw-   0        0        0     1409 2024-04-25 14:51:57.433006 ncmlistdownloader-1.0.1.240425/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 14:51:57.406007 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1263 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:51:57.423646 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2866 2024-04-25 14:49:59.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2184 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:51:57.425634 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:51:57.427629 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:51:57.428852 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2323 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:51:57.428852 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     8355 2024-04-25 14:45:48.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:51:57.433006 ncmlistdownloader-1.0.1.240425/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1409 2024-04-25 14:51:57.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2024-04-25 14:51:57.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 14:51:57.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-25 14:51:57.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-25 14:51:57.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-25 14:51:57.000000 ncmlistdownloader-1.0.1.240425/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 14:51:57.435033 ncmlistdownloader-1.0.1.240425/setup.cfg
--rw-rw-rw-   0        0        0     1756 2024-04-25 14:51:30.000000 ncmlistdownloader-1.0.1.240425/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.029814 ncmlistdownloader-1.0.1.240425a1/
+-rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/LICENSE
+-rw-rw-rw-   0        0        0     1399 2024-04-25 14:50:58.027834 ncmlistdownloader-1.0.1.240425a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 14:50:57.977687 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1263 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:50:57.999958 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0     1736 2024-04-25 10:28:31.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/__init__.py
+-rw-rw-rw-   0        0        0      653 2024-04-25 14:23:37.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/common.py
+-rw-rw-rw-   0        0        0     1661 2024-04-25 14:30:46.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/download.py
+-rw-rw-rw-   0        0        0     2501 2024-04-22 14:56:53.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/find_from_id.py
+-rw-rw-rw-   0        0        0     1664 2024-04-25 10:31:47.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/json_io.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.013215 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2866 2024-04-25 14:49:59.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2184 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.013215 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.013215 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.018180 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2323 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.020163 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     8355 2024-04-25 14:45:48.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.026830 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1399 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 14:50:58.029814 ncmlistdownloader-1.0.1.240425a1/setup.cfg
+-rw-rw-rw-   0        0        0     1758 2024-04-25 14:50:26.000000 ncmlistdownloader-1.0.1.240425a1/setup.py
```

### Comparing `ncmlistdownloader-1.0.1.240425/LICENSE` & `ncmlistdownloader-1.0.1.240425a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425/PKG-INFO` & `ncmlistdownloader-1.0.1.240425a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.1.240425
+Version: 1.0.1.240425a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.1.240425/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/global_args.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/song/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.1.240425
+Version: 1.0.1.240425a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.1.240425/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 ncmlistdownloader/__init__.py
 ncmlistdownloader.egg-info/PKG-INFO
 ncmlistdownloader.egg-info/SOURCES.txt
 ncmlistdownloader.egg-info/dependency_links.txt
 ncmlistdownloader.egg-info/entry_points.txt
 ncmlistdownloader.egg-info/requires.txt
 ncmlistdownloader.egg-info/top_level.txt
+ncmlistdownloader/cmd/__init__.py
+ncmlistdownloader/cmd/common.py
+ncmlistdownloader/cmd/download.py
+ncmlistdownloader/cmd/find_from_id.py
+ncmlistdownloader/cmd/json_io.py
 ncmlistdownloader/common/__init__.py
 ncmlistdownloader/common/encode_sec_key.py
 ncmlistdownloader/common/global_args.py
 ncmlistdownloader/common/thread_test.py
 ncmlistdownloader/downloader/__init__.py
 ncmlistdownloader/editer/__init__.py
 ncmlistdownloader/playlist/__init__.py
```

### Comparing `ncmlistdownloader-1.0.1.240425/setup.py` & `ncmlistdownloader-1.0.1.240425a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 setup(
     classifiers = [
         # 发展时期
-        # 'Development Status :: 3 - Alpha',
+        'Development Status :: 3 - Alpha',
         # 'Development Status :: 4 - Beta',
-        'Development Status :: 5 - Production/Stable',
+        # 'Development Status :: 5 - Production/Stable',
         # 开发的目标用户
         'Intended Audience :: Customer Service',
         'Intended Audience :: Developers',
         'Intended Audience :: End Users/Desktop',
         # 属于什么类型
         'Topic :: Communications :: File Sharing',
         'Topic :: Internet',
@@ -26,15 +26,15 @@
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.1.240425",
+    version = "1.0.1.240425a1",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
     install_requires = ['pycryptodome','pillow','mutagen','requests',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

