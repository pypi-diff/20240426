# Comparing `tmp/nrstitcher_utils-0.1.0.dev5.tar.gz` & `tmp/nrstitcher_utils-0.1.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrstitcher_utils-0.1.0.dev5.tar", last modified: Thu Apr 25 08:36:13 2024, max compression
+gzip compressed data, was "nrstitcher_utils-0.1.0.dev6.tar", last modified: Fri Apr 26 12:45:00 2024, max compression
```

## Comparing `nrstitcher_utils-0.1.0.dev5.tar` & `nrstitcher_utils-0.1.0.dev6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 08:36:13.269266 nrstitcher_utils-0.1.0.dev5/
--rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-22 13:12:35.000000 nrstitcher_utils-0.1.0.dev5/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-25 08:36:13.269266 nrstitcher_utils-0.1.0.dev5/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      251 2024-04-25 06:33:30.000000 nrstitcher_utils-0.1.0.dev5/README.md
--rw-r--r--   0 payno     (1000) payno     (1000)     2131 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev5/pyproject.toml
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-25 08:36:13.269266 nrstitcher_utils-0.1.0.dev5/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev5/setup.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 08:36:13.265265 nrstitcher_utils-0.1.0.dev5/src/
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 08:36:13.269266 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-22 12:54:51.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 08:36:13.269266 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/app/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/app/__init__.py
--rwxr-xr-x   0 payno     (1000) payno     (1000)     8275 2024-04-25 08:34:58.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 08:36:13.269266 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/core/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/core/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3220 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/core/h5_settings.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8694 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/core/ht_vol.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3430 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/core/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 08:36:13.269266 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/resources/
--rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/resources/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 08:36:13.269266 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/resources/config_files/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-25 06:33:38.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/resources/config_files/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-04-25 08:35:05.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-25 08:36:13.269266 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-25 08:36:13.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      706 2024-04-25 08:36:13.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-25 08:36:13.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-04-25 08:36:13.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils.egg-info/entry_points.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-04-25 08:36:13.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-04-25 08:36:13.000000 nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      251 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/README.md
+-rw-r--r--   0 payno     (1000) payno     (1000)     2131 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/pyproject.toml
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/app/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/app/__init__.py
+-rwxr-xr-x   0 payno     (1000) payno     (1000)     8279 2024-04-26 12:43:55.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3220 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/h5_settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8694 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/ht_vol.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3430 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/resources/
+-rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/resources/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/resources/config_files/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/resources/config_files/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-04-26 12:44:49.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 12:45:00.709495 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      706 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/entry_points.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-04-26 12:45:00.000000 nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/top_level.txt
```

### Comparing `nrstitcher_utils-0.1.0.dev5/LICENSE` & `nrstitcher_utils-0.1.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev5/PKG-INFO` & `nrstitcher_utils-0.1.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev5
+Version: 0.1.0.dev6
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
```

### Comparing `nrstitcher_utils-0.1.0.dev5/pyproject.toml` & `nrstitcher_utils-0.1.0.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/app/nrs_config_id16a_ht.py` & `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/app/nrs_config_id16a_ht.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         Name of the h5 file as a string.
         """
 
         h5_filename = glob.glob(h5_folder + "*.h5")[0]
 
         return h5_filename
 
-    argv = sys.argv
+    argv = sys.argv[1:]
     argparser = argparse.ArgumentParser(
         description="Creates input file for nr_stitcher.py program from id16a holotomography scan settings."
     )
     argparser.add_argument(
         "--base_dir",
         type=str,
         help="Required. Base directory containing sub-directories for individual scans and reconstructed volumes.",
```

### Comparing `nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/core/h5_settings.py` & `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/h5_settings.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/core/ht_vol.py` & `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/ht_vol.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils/core/utils.py` & `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils/core/utils.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils.egg-info/PKG-INFO` & `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev5
+Version: 0.1.0.dev6
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
```

### Comparing `nrstitcher_utils-0.1.0.dev5/src/nrstitcher_utils.egg-info/SOURCES.txt` & `nrstitcher_utils-0.1.0.dev6/src/nrstitcher_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

