# Comparing `tmp/ncmlistdownloader-1.0.1.240425a1.tar.gz` & `tmp/ncmlistdownloader-1.0.1.240426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.1.240425a1.tar", last modified: Thu Apr 25 14:50:58 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.1.240426.tar", last modified: Fri Apr 26 07:15:44 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.1.240425a1.tar` & `ncmlistdownloader-1.0.1.240426.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.029814 ncmlistdownloader-1.0.1.240425a1/
--rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/LICENSE
--rw-rw-rw-   0        0        0     1399 2024-04-25 14:50:58.027834 ncmlistdownloader-1.0.1.240425a1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 14:50:57.977687 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1263 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:50:57.999958 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/
--rw-rw-rw-   0        0        0     1736 2024-04-25 10:28:31.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/__init__.py
--rw-rw-rw-   0        0        0      653 2024-04-25 14:23:37.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/common.py
--rw-rw-rw-   0        0        0     1661 2024-04-25 14:30:46.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/download.py
--rw-rw-rw-   0        0        0     2501 2024-04-22 14:56:53.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/find_from_id.py
--rw-rw-rw-   0        0        0     1664 2024-04-25 10:31:47.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/json_io.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.013215 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2866 2024-04-25 14:49:59.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2184 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.013215 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.013215 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.018180 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2323 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.020163 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     8355 2024-04-25 14:45:48.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:50:58.026830 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1399 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      777 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-25 14:50:57.000000 ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 14:50:58.029814 ncmlistdownloader-1.0.1.240425a1/setup.cfg
--rw-rw-rw-   0        0        0     1758 2024-04-25 14:50:26.000000 ncmlistdownloader-1.0.1.240425a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:15:44.869419 ncmlistdownloader-1.0.1.240426/
+-rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240426/LICENSE
+-rw-rw-rw-   0        0        0     1409 2024-04-26 07:15:44.869419 ncmlistdownloader-1.0.1.240426/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 07:15:44.837163 ncmlistdownloader-1.0.1.240426/cmd/
+-rw-rw-rw-   0        0        0     1736 2024-04-25 10:28:31.000000 ncmlistdownloader-1.0.1.240426/cmd/__init__.py
+-rw-rw-rw-   0        0        0      653 2024-04-25 14:23:37.000000 ncmlistdownloader-1.0.1.240426/cmd/common.py
+-rw-rw-rw-   0        0        0     1661 2024-04-25 14:30:46.000000 ncmlistdownloader-1.0.1.240426/cmd/download.py
+-rw-rw-rw-   0        0        0     2501 2024-04-22 14:56:53.000000 ncmlistdownloader-1.0.1.240426/cmd/find_from_id.py
+-rw-rw-rw-   0        0        0     1664 2024-04-25 10:31:47.000000 ncmlistdownloader-1.0.1.240426/cmd/json_io.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:15:44.838167 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1238 2024-04-26 07:13:33.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:15:44.857699 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2866 2024-04-26 07:14:57.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2184 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:15:44.858698 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:15:44.863898 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-26 07:14:43.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:15:44.866890 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2323 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:15:44.867886 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     8428 2024-04-26 07:14:17.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:15:44.869419 ncmlistdownloader-1.0.1.240426/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1409 2024-04-26 07:15:44.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      687 2024-04-26 07:15:44.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 07:15:44.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-26 07:15:44.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-26 07:15:44.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-26 07:15:44.000000 ncmlistdownloader-1.0.1.240426/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 07:15:44.875748 ncmlistdownloader-1.0.1.240426/setup.cfg
+-rw-rw-rw-   0        0        0     1756 2024-04-26 07:15:12.000000 ncmlistdownloader-1.0.1.240426/setup.py
```

### Comparing `ncmlistdownloader-1.0.1.240425a1/LICENSE` & `ncmlistdownloader-1.0.1.240426/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/PKG-INFO` & `ncmlistdownloader-1.0.1.240426/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.1.240425a1
+Version: 1.0.1.240426
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.1.240426/ncmlistdownloader/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 '''
 ncmlistdownloader/__init__.py
-Core.Ver.1.0.0.240414
+Core.Ver.1.0.2.240426
 Author: CooooldWind_
 '''
 from pathlib import Path
 from ncmlistdownloader.playlist import *
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.global_args import *
 
 def main():
     for i in CMD_START_WORDS:
         print(i)
-    print('[*]Core.Ver.1.0.0.240414')
+    print('[*]Core.Ver.1.0.2.240426')
     id = str(input("ID: "))
     p = Playlist(id)
     p.get_info()
-    p.get_detail_info()
     print("Playlist info-reading succeed.")
     d = str(input("Dir: "))
     if d == '':
         d = str(Path.home()) + '/Downloads/ncmld_downloads/'
     fnf = str(input("Filename format: "))
     if fnf == '':
         fnf = '$title$ - $artist$'
```

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/__init__.py` & `ncmlistdownloader-1.0.1.240426/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/common.py` & `ncmlistdownloader-1.0.1.240426/cmd/common.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/download.py` & `ncmlistdownloader-1.0.1.240426/cmd/download.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/find_from_id.py` & `ncmlistdownloader-1.0.1.240426/cmd/find_from_id.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/cmd/json_io.py` & `ncmlistdownloader-1.0.1.240426/cmd/json_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.1.240426/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.1.240426/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.1.240426/ncmlistdownloader/common/global_args.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.1.240426/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.1.240426/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.1.240426/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.1.240426/ncmlistdownloader/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.1.240426/ncmlistdownloader/song/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/song/__init__.py
-Core.Ver.1.0.0.240425a1
+Core.Ver.1.0.0.240426
 Author: CooooldWind_
 '''
 
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.thread_test import best_thread
 from ncmlistdownloader.downloader import *
@@ -59,23 +59,19 @@
         ----------
         无参数。
         如果直接`print`这个类就是调用这个函数了。
         '''
         return str(self.processed_info)
     
     def get_formated_filename(self, suffix):
-        format_info = self.processed_info
-        format_info.update({
-            'filename': self.filename_format,
-            'artist': self.artist_str,
-            'album': self.album,
-            'id': self.id,
-            'title': self.title,
-            })
-        formated = format(**format_info)
+        formated = format(filename = self.filename_format,
+                          artist = self.artist_str,
+                          album = self.album,
+                          id = self.id,
+                          title = self.title)
         if formated.rfind('/') != -1:
             formated = formated[:formated.rfind('/') + 1] + clean(formated[formated.rfind('/') + 1:])
         else:
             formated = clean(formated)
         formated += ('.' + suffix)
         return formated
 
@@ -99,19 +95,19 @@
             'artist': self.artist,
             'id': self.id,
         }
         self.url_info.update({
             'album_pic': self.raw_info['al']['picUrl'],
             'song_file': SONG_FILE_API + self.id,
         })
-        self.filename_info.update({
+        self.filename_info = {
             'song': self.get_formated_filename('mp3'),
             'pic': self.get_formated_filename('jpg'),
             'lyric': self.get_formated_filename('lrc'),
-        })
+        }
         self.is_get = True
         return self.raw_info
     
     def multi_get_info(self):
         '''
         获取歌曲信息（多线程用）
         ----------
@@ -158,35 +154,38 @@
         enhanced_info = NeteaseParams(
             encode_data = enhance_encode_data,
             url = SONG_FILE_API_2
         ).get_resource(cookies = cookies)
         return enhanced_info
 
     def song_download(self):
-        filename = self.get_formated_filename('mp3')
+        # filename = self.get_formated_filename('mp3')
+        filename = self.filename_info['song']
         file_origin = OriginFile(self.url_info['song_file'])
         if file_origin.total_size <= 0:
             return -1
         file_origin.single_thread_start(filename = filename)
         return filename
 
     def cover_download(self):
-        filename = self.get_formated_filename('jpg')
+        filename = self.filename_info['pic']
+        # filename = self.get_formated_filename('jpg')
         file_origin = OriginFile(self.url_info['album_pic'])
         if file_origin.total_size == -1:
             return -1
         file_origin.auto_start(filename = filename)
         return filename
 
     def lyric_get(self):
         self.lyric = NeteaseParams(
             url = LYRIC_API,
             encode_data = self.lyric_encode_data
         ).get_resource()['lrc']['lyric'].replace("\n", '\n')
-        filename = self.get_formated_filename('lrc')
+        # filename = self.get_formated_filename('lrc')
+        filename = self.filename_info['lyric']
         with open(file = filename, mode = 'w+', encoding = 'UTF-8') as file:
             file.write(self.lyric)
         return filename
 
     def attribute_write(self, filename = 'No filename'):
         '''
         往文件里面写入歌曲信息
```

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.1.240426/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.1.240425a1
+Version: 1.0.1.240426
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.1.240425a1/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.1.240426/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 LICENSE
 setup.py
+cmd/__init__.py
+cmd/common.py
+cmd/download.py
+cmd/find_from_id.py
+cmd/json_io.py
 ncmlistdownloader/__init__.py
 ncmlistdownloader.egg-info/PKG-INFO
 ncmlistdownloader.egg-info/SOURCES.txt
 ncmlistdownloader.egg-info/dependency_links.txt
 ncmlistdownloader.egg-info/entry_points.txt
 ncmlistdownloader.egg-info/requires.txt
 ncmlistdownloader.egg-info/top_level.txt
-ncmlistdownloader/cmd/__init__.py
-ncmlistdownloader/cmd/common.py
-ncmlistdownloader/cmd/download.py
-ncmlistdownloader/cmd/find_from_id.py
-ncmlistdownloader/cmd/json_io.py
 ncmlistdownloader/common/__init__.py
 ncmlistdownloader/common/encode_sec_key.py
 ncmlistdownloader/common/global_args.py
 ncmlistdownloader/common/thread_test.py
 ncmlistdownloader/downloader/__init__.py
 ncmlistdownloader/editer/__init__.py
 ncmlistdownloader/playlist/__init__.py
```

### Comparing `ncmlistdownloader-1.0.1.240425a1/setup.py` & `ncmlistdownloader-1.0.1.240426/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 setup(
     classifiers = [
         # 发展时期
-        'Development Status :: 3 - Alpha',
+        # 'Development Status :: 3 - Alpha',
         # 'Development Status :: 4 - Beta',
-        # 'Development Status :: 5 - Production/Stable',
+        'Development Status :: 5 - Production/Stable',
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
-    version = "1.0.1.240425a1",
+    version = "1.0.1.240426",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
     install_requires = ['pycryptodome','pillow','mutagen','requests',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

