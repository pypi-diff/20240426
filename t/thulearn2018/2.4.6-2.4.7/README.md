# Comparing `tmp/thulearn2018-2.4.6.tar.gz` & `tmp/thulearn2018-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thulearn2018-2.4.6.tar", last modified: Tue Apr 16 11:21:37 2024, max compression
+gzip compressed data, was "thulearn2018-2.4.7.tar", last modified: Fri Apr 26 17:34:33 2024, max compression
```

## Comparing `thulearn2018-2.4.6.tar` & `thulearn2018-2.4.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-16 11:21:37.240623 thulearn2018-2.4.6/
--rw-r--r--   0 hyr       (1000) hyr       (1000)       75 2023-09-13 09:31:57.000000 thulearn2018-2.4.6/.gitignore
--rw-r--r--   0 hyr       (1000) hyr       (1000)     1074 2024-04-16 08:17:55.000000 thulearn2018-2.4.6/LICENSE
--rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-04-16 11:21:37.240623 thulearn2018-2.4.6/PKG-INFO
--rw-r-----   0 hyr       (1000) hyr       (1000)     5277 2024-04-07 05:13:15.000000 thulearn2018-2.4.6/README.md
--rw-r-----   0 hyr       (1000) hyr       (1000)       38 2024-04-16 11:21:37.240623 thulearn2018-2.4.6/setup.cfg
--rw-r-----   0 hyr       (1000) hyr       (1000)     2540 2024-04-16 11:20:48.000000 thulearn2018-2.4.6/setup.py
-drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-16 11:21:37.240623 thulearn2018-2.4.6/thulearn2018/
--rw-r--r--   0 hyr       (1000) hyr       (1000)       22 2023-09-13 09:31:57.000000 thulearn2018-2.4.6/thulearn2018/__init__.py
--rw-r-----   0 hyr       (1000) hyr       (1000)    10532 2024-04-16 09:59:06.000000 thulearn2018-2.4.6/thulearn2018/browser.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     5708 2024-04-07 05:13:21.000000 thulearn2018-2.4.6/thulearn2018/filemanager.py
--rw-r-----   0 hyr       (1000) hyr       (1000)      415 2024-04-07 05:12:59.000000 thulearn2018-2.4.6/thulearn2018/jsonhelper.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     3779 2024-04-16 09:56:44.000000 thulearn2018-2.4.6/thulearn2018/learn.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     3207 2024-04-07 05:13:14.000000 thulearn2018-2.4.6/thulearn2018/settings.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     3941 2024-04-07 05:13:20.000000 thulearn2018-2.4.6/thulearn2018/soup.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     1496 2024-04-16 11:17:32.000000 thulearn2018-2.4.6/thulearn2018/utils.py
-drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-16 11:21:37.240623 thulearn2018-2.4.6/thulearn2018.egg-info/
--rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-04-16 11:21:37.000000 thulearn2018-2.4.6/thulearn2018.egg-info/PKG-INFO
--rw-r--r--   0 hyr       (1000) hyr       (1000)      449 2024-04-16 11:21:37.000000 thulearn2018-2.4.6/thulearn2018.egg-info/SOURCES.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)        1 2024-04-16 11:21:37.000000 thulearn2018-2.4.6/thulearn2018.egg-info/dependency_links.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)       50 2024-04-16 11:21:37.000000 thulearn2018-2.4.6/thulearn2018.egg-info/entry_points.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)       79 2024-04-16 11:21:37.000000 thulearn2018-2.4.6/thulearn2018.egg-info/requires.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)       13 2024-04-16 11:21:37.000000 thulearn2018-2.4.6/thulearn2018.egg-info/top_level.txt
+drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-26 17:34:33.369778 thulearn2018-2.4.7/
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       75 2023-09-13 09:31:57.000000 thulearn2018-2.4.7/.gitignore
+-rw-r-----   0 hyr       (1000) hyr       (1000)     1074 2024-04-18 12:09:52.000000 thulearn2018-2.4.7/LICENSE
+-rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-04-26 17:34:33.369778 thulearn2018-2.4.7/PKG-INFO
+-rw-r-----   0 hyr       (1000) hyr       (1000)     5277 2024-04-07 05:13:15.000000 thulearn2018-2.4.7/README.md
+-rw-r-----   0 hyr       (1000) hyr       (1000)       38 2024-04-26 17:34:33.369778 thulearn2018-2.4.7/setup.cfg
+-rw-r-----   0 hyr       (1000) hyr       (1000)     2540 2024-04-26 17:27:44.000000 thulearn2018-2.4.7/setup.py
+drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-26 17:34:33.369778 thulearn2018-2.4.7/thulearn2018/
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       22 2023-09-13 09:31:57.000000 thulearn2018-2.4.7/thulearn2018/__init__.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)    10559 2024-04-25 13:35:26.000000 thulearn2018-2.4.7/thulearn2018/browser.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     5708 2024-04-07 05:13:21.000000 thulearn2018-2.4.7/thulearn2018/filemanager.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)      415 2024-04-07 05:12:59.000000 thulearn2018-2.4.7/thulearn2018/jsonhelper.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     3779 2024-04-26 17:20:40.000000 thulearn2018-2.4.7/thulearn2018/learn.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     3207 2024-04-07 05:13:14.000000 thulearn2018-2.4.7/thulearn2018/settings.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     3941 2024-04-07 05:13:20.000000 thulearn2018-2.4.7/thulearn2018/soup.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     1496 2024-04-16 11:17:32.000000 thulearn2018-2.4.7/thulearn2018/utils.py
+drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-26 17:34:33.369778 thulearn2018-2.4.7/thulearn2018.egg-info/
+-rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-04-26 17:34:33.000000 thulearn2018-2.4.7/thulearn2018.egg-info/PKG-INFO
+-rw-r-----   0 hyr       (1000) hyr       (1000)      449 2024-04-26 17:34:33.000000 thulearn2018-2.4.7/thulearn2018.egg-info/SOURCES.txt
+-rw-r-----   0 hyr       (1000) hyr       (1000)        1 2024-04-26 17:34:33.000000 thulearn2018-2.4.7/thulearn2018.egg-info/dependency_links.txt
+-rw-r-----   0 hyr       (1000) hyr       (1000)       50 2024-04-26 17:34:33.000000 thulearn2018-2.4.7/thulearn2018.egg-info/entry_points.txt
+-rw-r-----   0 hyr       (1000) hyr       (1000)       79 2024-04-26 17:34:33.000000 thulearn2018-2.4.7/thulearn2018.egg-info/requires.txt
+-rw-r-----   0 hyr       (1000) hyr       (1000)       13 2024-04-26 17:34:33.000000 thulearn2018-2.4.7/thulearn2018.egg-info/top_level.txt
```

### Comparing `thulearn2018-2.4.6/LICENSE` & `thulearn2018-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.6/PKG-INFO` & `thulearn2018-2.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thulearn2018
-Version: 2.4.6
+Version: 2.4.7
 Summary: Tools for Web Learning of Tsinghua University
 Home-page: https://github.com/euxcet/thulearn2018
 Author: Chengchi Zhou, Yingtian Liu, Yurui Hong
 Author-email: zcc16@mails.tsinghua.edu.cn, liu-yt16@mails.tsinghua.edu.cn,yuruihong02@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `thulearn2018-2.4.6/README.md` & `thulearn2018-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.6/setup.py` & `thulearn2018-2.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="thulearn2018",
-    version="2.4.6",
+    version="2.4.7",
     author="Chengchi Zhou, Yingtian Liu, Yurui Hong",
     author_email="zcc16@mails.tsinghua.edu.cn, liu-yt16@mails.tsinghua.edu.cn,"
                  "yuruihong02@outlook.com",
     description="Tools for Web Learning of Tsinghua University",
     long_description="Tools for Web Learning of Tsinghua University",
     long_description_content_type="text/markdown",
     url="https://github.com/euxcet/thulearn2018",
```

### Comparing `thulearn2018-2.4.6/thulearn2018/browser.py` & `thulearn2018-2.4.7/thulearn2018/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         for i in range(len(lessons)):
             self.fm.mkdirl(os.path.join(self.path, lessons[i][4]))
         return lessons
 
     def get_files_id(self, lesson_id):
         form = {"wlkcid": lesson_id}
         files = self.jh.loads(self.get(settings.files_url, params=form))
-        files_id = [row["id"] for row in files["object"]["rows"]]
+        files_id = [row["id"] for row in files["object"]["rows"]] if files["object"] else []
 
         return files_id
 
     def file_id_exist(self, fid):
         return (fid in self.local)
 
     def save_file_id(self, fid, fpath):
```

### Comparing `thulearn2018-2.4.6/thulearn2018/filemanager.py` & `thulearn2018-2.4.7/thulearn2018/filemanager.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.6/thulearn2018/learn.py` & `thulearn2018-2.4.7/thulearn2018/learn.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.6/thulearn2018/settings.py` & `thulearn2018-2.4.7/thulearn2018/settings.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.6/thulearn2018/soup.py` & `thulearn2018-2.4.7/thulearn2018/soup.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.6/thulearn2018/utils.py` & `thulearn2018-2.4.7/thulearn2018/utils.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.6/thulearn2018.egg-info/PKG-INFO` & `thulearn2018-2.4.7/thulearn2018.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thulearn2018
-Version: 2.4.6
+Version: 2.4.7
 Summary: Tools for Web Learning of Tsinghua University
 Home-page: https://github.com/euxcet/thulearn2018
 Author: Chengchi Zhou, Yingtian Liu, Yurui Hong
 Author-email: zcc16@mails.tsinghua.edu.cn, liu-yt16@mails.tsinghua.edu.cn,yuruihong02@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

