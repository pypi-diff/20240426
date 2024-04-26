# Comparing `tmp/fastfuels-1.0.5.tar.gz` & `tmp/fastfuels-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfuels-1.0.5.tar", last modified: Mon Nov 27 00:21:43 2023, max compression
+gzip compressed data, was "fastfuels-1.0.6.tar", last modified: Fri Apr 26 02:26:07 2024, max compression
```

## Comparing `fastfuels-1.0.5.tar` & `fastfuels-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 00:21:43.045814 fastfuels-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    34502 2023-11-27 00:21:30.000000 fastfuels-1.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-11-27 00:21:43.045814 fastfuels-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2023-11-27 00:21:30.000000 fastfuels-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 00:21:43.045814 fastfuels-1.0.5/fastfuels/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-27 00:21:30.000000 fastfuels-1.0.5/fastfuels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35612 2023-11-27 00:21:30.000000 fastfuels-1.0.5/fastfuels/core.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5042 2023-11-27 00:21:30.000000 fastfuels-1.0.5/fastfuels/fastfuels_create_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 00:21:43.045814 fastfuels-1.0.5/fastfuels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-11-27 00:21:43.000000 fastfuels-1.0.5/fastfuels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-11-27 00:21:43.000000 fastfuels-1.0.5/fastfuels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 00:21:43.000000 fastfuels-1.0.5/fastfuels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-27 00:21:43.000000 fastfuels-1.0.5/fastfuels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-27 00:21:43.000000 fastfuels-1.0.5/fastfuels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-27 00:21:43.049814 fastfuels-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2023-11-27 00:21:30.000000 fastfuels-1.0.5/setup.py
+drwxr-xr-x   0 lucaswells   (501) staff       (20)        0 2024-04-26 02:26:07.660703 fastfuels-1.0.6/
+-rw-r--r--   0 lucaswells   (501) staff       (20)    34502 2024-04-26 02:21:14.000000 fastfuels-1.0.6/LICENSE.txt
+-rw-r--r--   0 lucaswells   (501) staff       (20)     3373 2024-04-26 02:26:07.660616 fastfuels-1.0.6/PKG-INFO
+-rw-r--r--   0 lucaswells   (501) staff       (20)     2377 2024-04-26 02:21:14.000000 fastfuels-1.0.6/README.md
+drwxr-xr-x   0 lucaswells   (501) staff       (20)        0 2024-04-26 02:26:07.659285 fastfuels-1.0.6/fastfuels/
+-rw-r--r--   0 lucaswells   (501) staff       (20)       23 2024-04-26 02:21:14.000000 fastfuels-1.0.6/fastfuels/__init__.py
+-rw-r--r--   0 lucaswells   (501) staff       (20)    35612 2024-04-26 02:21:14.000000 fastfuels-1.0.6/fastfuels/core.py
+-rwxr-xr-x   0 lucaswells   (501) staff       (20)     5042 2024-04-26 02:21:14.000000 fastfuels-1.0.6/fastfuels/fastfuels_create_index.py
+drwxr-xr-x   0 lucaswells   (501) staff       (20)        0 2024-04-26 02:26:07.660329 fastfuels-1.0.6/fastfuels.egg-info/
+-rw-r--r--   0 lucaswells   (501) staff       (20)     3373 2024-04-26 02:26:07.000000 fastfuels-1.0.6/fastfuels.egg-info/PKG-INFO
+-rw-r--r--   0 lucaswells   (501) staff       (20)      280 2024-04-26 02:26:07.000000 fastfuels-1.0.6/fastfuels.egg-info/SOURCES.txt
+-rw-r--r--   0 lucaswells   (501) staff       (20)        1 2024-04-26 02:26:07.000000 fastfuels-1.0.6/fastfuels.egg-info/dependency_links.txt
+-rw-r--r--   0 lucaswells   (501) staff       (20)      130 2024-04-26 02:26:07.000000 fastfuels-1.0.6/fastfuels.egg-info/requires.txt
+-rw-r--r--   0 lucaswells   (501) staff       (20)       10 2024-04-26 02:26:07.000000 fastfuels-1.0.6/fastfuels.egg-info/top_level.txt
+-rw-r--r--   0 lucaswells   (501) staff       (20)       79 2024-04-26 02:26:07.660947 fastfuels-1.0.6/setup.cfg
+-rw-r--r--   0 lucaswells   (501) staff       (20)     1766 2024-04-26 02:24:03.000000 fastfuels-1.0.6/setup.py
```

### Comparing `fastfuels-1.0.5/LICENSE.txt` & `fastfuels-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastfuels-1.0.5/PKG-INFO` & `fastfuels-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfuels
-Version: 1.0.5
+Version: 1.0.6
 Summary: 3D fuelscapes for the contiguous US
 Home-page: https://github.com/teamholtz/FastFuels-Python
 Author: Holtz Technology and Development Services LLC
 Author-email: lucas@holtztds.com
 License: GNU GPLv3
 Keywords: fire model,fuelscape,wildfire
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: colorcet==2.0.6
 Requires-Dist: fsspec==2021.11.0
 Requires-Dist: msgpack==1.0.2
 Requires-Dist: numpy==1.23.0
 Requires-Dist: pyvista==0.28.1
-Requires-Dist: s3fs==2021.11.0
+Requires-Dist: s3fs==2024.2.0
 Requires-Dist: scipy==1.11.4
 Requires-Dist: shapely<2
 Requires-Dist: zarr==2.8.3
 
 # FastFuels-Python 
 
 Python client library for the FastFuels API
```

### Comparing `fastfuels-1.0.5/README.md` & `fastfuels-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fastfuels-1.0.5/fastfuels/core.py` & `fastfuels-1.0.6/fastfuels/core.py`

 * *Files identical despite different names*

### Comparing `fastfuels-1.0.5/fastfuels/fastfuels_create_index.py` & `fastfuels-1.0.6/fastfuels/fastfuels_create_index.py`

 * *Files identical despite different names*

### Comparing `fastfuels-1.0.5/fastfuels.egg-info/PKG-INFO` & `fastfuels-1.0.6/fastfuels.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfuels
-Version: 1.0.5
+Version: 1.0.6
 Summary: 3D fuelscapes for the contiguous US
 Home-page: https://github.com/teamholtz/FastFuels-Python
 Author: Holtz Technology and Development Services LLC
 Author-email: lucas@holtztds.com
 License: GNU GPLv3
 Keywords: fire model,fuelscape,wildfire
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: colorcet==2.0.6
 Requires-Dist: fsspec==2021.11.0
 Requires-Dist: msgpack==1.0.2
 Requires-Dist: numpy==1.23.0
 Requires-Dist: pyvista==0.28.1
-Requires-Dist: s3fs==2021.11.0
+Requires-Dist: s3fs==2024.2.0
 Requires-Dist: scipy==1.11.4
 Requires-Dist: shapely<2
 Requires-Dist: zarr==2.8.3
 
 # FastFuels-Python 
 
 Python client library for the FastFuels API
```

### Comparing `fastfuels-1.0.5/setup.py` & `fastfuels-1.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         'colorcet==2.0.6',
         'fsspec==2021.11.0',
         # numcodecs no longer includes msgpack?
         'msgpack==1.0.2',
         # use numpy 1.23 to avoid TypeError: 'numpy._DTypeMeta' object is not subscriptable
         'numpy==1.23.0',
         'pyvista==0.28.1',
-        's3fs==2021.11.0',
+        's3fs==2024.2.0',
         # use newer scipy for numpy 1.23
         'scipy==1.11.4',
         'shapely<2',
         'zarr==2.8.3'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

