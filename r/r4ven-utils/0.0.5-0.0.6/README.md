# Comparing `tmp/r4ven_utils-0.0.5.tar.gz` & `tmp/r4ven_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r4ven_utils-0.0.5.tar", last modified: Fri Apr 26 14:32:19 2024, max compression
+gzip compressed data, was "r4ven_utils-0.0.6.tar", last modified: Fri Apr 26 15:06:08 2024, max compression
```

## Comparing `r4ven_utils-0.0.5.tar` & `r4ven_utils-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 14:32:19.103107 r4ven_utils-0.0.5/
--rw-rw-r--   0 victor    (1000) victor    (1000)    35149 2022-11-07 06:44:00.000000 r4ven_utils-0.0.5/LICENSE
--rw-r--r--   0 victor    (1000) victor    (1000)     3209 2024-04-26 14:32:19.103107 r4ven_utils-0.0.5/PKG-INFO
--rw-rw-r--   0 victor    (1000) victor    (1000)     2380 2024-04-26 14:24:30.000000 r4ven_utils-0.0.5/README.md
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 14:32:19.103107 r4ven_utils-0.0.5/r4ven_utils/
--rw-rw-r--   0 victor    (1000) victor    (1000)        0 2022-11-07 06:44:00.000000 r4ven_utils-0.0.5/r4ven_utils/__init__.py
--rw-rw-r--   0 victor    (1000) victor    (1000)      691 2022-11-24 11:06:45.000000 r4ven_utils-0.0.5/r4ven_utils/exceptions.py
--rw-rw-r--   0 victor    (1000) victor    (1000)     4373 2024-04-26 13:48:19.000000 r4ven_utils-0.0.5/r4ven_utils/log4me.py
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 14:32:19.103107 r4ven_utils-0.0.5/r4ven_utils.egg-info/
--rw-r--r--   0 victor    (1000) victor    (1000)     3209 2024-04-26 14:32:19.000000 r4ven_utils-0.0.5/r4ven_utils.egg-info/PKG-INFO
--rw-rw-r--   0 victor    (1000) victor    (1000)      269 2024-04-26 14:32:19.000000 r4ven_utils-0.0.5/r4ven_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 victor    (1000) victor    (1000)        1 2024-04-26 14:32:19.000000 r4ven_utils-0.0.5/r4ven_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 victor    (1000) victor    (1000)       12 2024-04-26 14:32:19.000000 r4ven_utils-0.0.5/r4ven_utils.egg-info/top_level.txt
--rw-rw-r--   0 victor    (1000) victor    (1000)      350 2024-04-26 14:32:19.107107 r4ven_utils-0.0.5/setup.cfg
--rw-rw-r--   0 victor    (1000) victor    (1000)     1454 2024-04-26 14:30:48.000000 r4ven_utils-0.0.5/setup.py
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 14:32:19.103107 r4ven_utils-0.0.5/tests/
--rw-rw-r--   0 victor    (1000) victor    (1000)     5162 2024-04-26 13:42:22.000000 r4ven_utils-0.0.5/tests/test_log4me.py
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 15:06:08.921448 r4ven_utils-0.0.6/
+-rw-rw-r--   0 victor    (1000) victor    (1000)    35149 2024-04-26 14:53:09.000000 r4ven_utils-0.0.6/LICENSE
+-rw-r--r--   0 victor    (1000) victor    (1000)     3411 2024-04-26 15:06:08.921448 r4ven_utils-0.0.6/PKG-INFO
+-rw-rw-r--   0 victor    (1000) victor    (1000)     2582 2024-04-26 14:53:09.000000 r4ven_utils-0.0.6/README.md
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 15:06:08.917448 r4ven_utils-0.0.6/r4ven_utils/
+-rw-rw-r--   0 victor    (1000) victor    (1000)        0 2024-04-26 14:53:09.000000 r4ven_utils-0.0.6/r4ven_utils/__init__.py
+-rw-rw-r--   0 victor    (1000) victor    (1000)     4373 2024-04-26 14:53:09.000000 r4ven_utils-0.0.6/r4ven_utils/log4me.py
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 15:06:08.917448 r4ven_utils-0.0.6/r4ven_utils.egg-info/
+-rw-r--r--   0 victor    (1000) victor    (1000)     3411 2024-04-26 15:06:08.000000 r4ven_utils-0.0.6/r4ven_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 victor    (1000) victor    (1000)      222 2024-04-26 15:06:08.000000 r4ven_utils-0.0.6/r4ven_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)        1 2024-04-26 15:06:08.000000 r4ven_utils-0.0.6/r4ven_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)       12 2024-04-26 15:06:08.000000 r4ven_utils-0.0.6/r4ven_utils.egg-info/top_level.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)      350 2024-04-26 15:06:08.921448 r4ven_utils-0.0.6/setup.cfg
+-rw-rw-r--   0 victor    (1000) victor    (1000)     1454 2024-04-26 14:54:38.000000 r4ven_utils-0.0.6/setup.py
```

### Comparing `r4ven_utils-0.0.5/LICENSE` & `r4ven_utils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `r4ven_utils-0.0.5/PKG-INFO` & `r4ven_utils-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: r4ven_utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: The companion that holds your grab-bag of utility functions and objects
 Home-page: https://github.com/VictorFantucci/r4ven_utils_dev
-Download-URL: https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.5.tar.gz
+Download-URL: https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.6.tar.gz
 Author: Victor Vinci Fantucci
 Author-email: victor.v.fantucci@gmail.com
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/VictorFantucci/r4ven_utils_dev/issues
 Keywords: r4ven_utils,utils,logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-  <img src="imgs/r4ven_logo.png"><br>
+  <img src="https://substackcdn.com/image/fetch/w_176,h_176,c_fill,f_webp,q_auto:good,fl_progressive:steep,g_auto/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2Ffe99049e-8950-4c81-9b70-4ab5fd15c84a_500x500.png"><br>
 </div>
 
 -----------------
 
 # r4ven: The companion that holds your grab-bag of utility functions and objects
 
 > Reimplementing utilities folder across multiple Python projects... Nevermore!
```

### Comparing `r4ven_utils-0.0.5/README.md` & `r4ven_utils-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center">
-  <img src="imgs/r4ven_logo.png"><br>
+  <img src="https://substackcdn.com/image/fetch/w_176,h_176,c_fill,f_webp,q_auto:good,fl_progressive:steep,g_auto/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2Ffe99049e-8950-4c81-9b70-4ab5fd15c84a_500x500.png"><br>
 </div>
 
 -----------------
 
 # r4ven: The companion that holds your grab-bag of utility functions and objects
 
 > Reimplementing utilities folder across multiple Python projects... Nevermore!
```

### Comparing `r4ven_utils-0.0.5/r4ven_utils/log4me.py` & `r4ven_utils-0.0.6/r4ven_utils/log4me.py`

 * *Files identical despite different names*

### Comparing `r4ven_utils-0.0.5/r4ven_utils.egg-info/PKG-INFO` & `r4ven_utils-0.0.6/r4ven_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: r4ven_utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: The companion that holds your grab-bag of utility functions and objects
 Home-page: https://github.com/VictorFantucci/r4ven_utils_dev
-Download-URL: https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.5.tar.gz
+Download-URL: https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.6.tar.gz
 Author: Victor Vinci Fantucci
 Author-email: victor.v.fantucci@gmail.com
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/VictorFantucci/r4ven_utils_dev/issues
 Keywords: r4ven_utils,utils,logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-  <img src="imgs/r4ven_logo.png"><br>
+  <img src="https://substackcdn.com/image/fetch/w_176,h_176,c_fill,f_webp,q_auto:good,fl_progressive:steep,g_auto/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2Ffe99049e-8950-4c81-9b70-4ab5fd15c84a_500x500.png"><br>
 </div>
 
 -----------------
 
 # r4ven: The companion that holds your grab-bag of utility functions and objects
 
 > Reimplementing utilities folder across multiple Python projects... Nevermore!
```

### Comparing `r4ven_utils-0.0.5/setup.py` & `r4ven_utils-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # Package Information:
     name='r4ven_utils',
     packages=['r4ven_utils'], # Should match the package folder.
-    version='0.0.5',
+    version='0.0.6',
     license='GPLv3',
 
     # Description Information:
     description='The companion that holds your grab-bag of utility functions and objects',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
@@ -39,9 +39,9 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Documentation',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3',
     ],
 
-    download_url="https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.5.tar.gz",
+    download_url="https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.6.tar.gz",
 )
```

