# Comparing `tmp/tinymovr-2.0.0a1.tar.gz` & `tmp/tinymovr-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinymovr-2.0.0a1.tar", last modified: Mon Apr 22 10:51:18 2024, max compression
+gzip compressed data, was "tinymovr-2.0.0a2.tar", last modified: Fri Apr 26 11:46:17 2024, max compression
```

## Comparing `tinymovr-2.0.0a1.tar` & `tinymovr-2.0.0a2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-22 10:51:18.146318 tinymovr-2.0.0a1/
--rw-r--r--   0 yanconst   (501) staff       (20)      638 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/MANIFEST.in
--rw-r--r--   0 yanconst   (501) staff       (20)     2146 2024-04-22 10:51:18.146153 tinymovr-2.0.0a1/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)     1689 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/README.md
--rw-r--r--   0 yanconst   (501) staff       (20)       38 2024-04-22 10:51:18.146371 tinymovr-2.0.0a1/setup.cfg
--rw-r--r--   0 yanconst   (501) staff       (20)     2387 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/setup.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-22 10:51:18.139713 tinymovr-2.0.0a1/tinymovr/
--rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-2.0.0a1/tinymovr/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     4167 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/channel.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3164 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/cli.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-22 10:51:18.141097 tinymovr-2.0.0a1/tinymovr/codec/
--rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-2.0.0a1/tinymovr/codec/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3281 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/codec/codec.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-22 10:51:18.141469 tinymovr-2.0.0a1/tinymovr/config/
--rw-r--r--   0 yanconst   (501) staff       (20)      148 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/config/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     5338 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/config/config.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1079 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/constants.py
--rw-r--r--   0 yanconst   (501) staff       (20)     7313 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/dfu.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3256 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/discovery.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-22 10:51:18.142668 tinymovr-2.0.0a1/tinymovr/gui/
--rw-r--r--   0 yanconst   (501) staff       (20)      665 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/gui/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2204 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/gui/gui.py
--rw-r--r--   0 yanconst   (501) staff       (20)    14412 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/gui/helpers.py
--rw-r--r--   0 yanconst   (501) staff       (20)    19455 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/gui/widgets.py
--rw-r--r--   0 yanconst   (501) staff       (20)    14125 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/gui/window.py
--rw-r--r--   0 yanconst   (501) staff       (20)     5620 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/gui/worker.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-22 10:51:18.137557 tinymovr-2.0.0a1/tinymovr/resources/
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-22 10:51:18.144354 tinymovr-2.0.0a1/tinymovr/resources/icons/
--rw-r--r--   0 yanconst   (501) staff       (20)     3184 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/resources/icons/call.png
--rw-r--r--   0 yanconst   (501) staff       (20)     3184 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/resources/icons/call@2x.png
--rw-r--r--   0 yanconst   (501) staff       (20)    22790 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/resources/icons/call_dark.png
--rw-r--r--   0 yanconst   (501) staff       (20)    22672 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/resources/icons/call_dark@2x.png
--rw-r--r--   0 yanconst   (501) staff       (20)    26604 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/resources/icons/empty.png
--rw-r--r--   0 yanconst   (501) staff       (20)    44831 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/resources/icons/empty@2x.png
--rw-r--r--   0 yanconst   (501) staff       (20)    30381 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/resources/icons/empty_dark.png
--rw-r--r--   0 yanconst   (501) staff       (20)    51206 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/resources/icons/empty_dark@2x.png
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-22 10:51:18.145832 tinymovr-2.0.0a1/tinymovr/specs/
--rw-r--r--   0 yanconst   (501) staff       (20)     1820 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/specs/dfu_1_0_x.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)     2148 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/specs/dfu_1_1_x.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)    15484 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/specs/tinymovr_1_3_x.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)    16329 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/specs/tinymovr_1_4_x.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)    18659 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/specs/tinymovr_1_5_x.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)    18824 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/specs/tinymovr_1_6_x.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)     3555 2024-04-21 22:08:50.000000 tinymovr-2.0.0a1/tinymovr/tee.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-22 10:51:18.140684 tinymovr-2.0.0a1/tinymovr.egg-info/
--rw-r--r--   0 yanconst   (501) staff       (20)     2146 2024-04-22 10:51:18.000000 tinymovr-2.0.0a1/tinymovr.egg-info/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)     1109 2024-04-22 10:51:18.000000 tinymovr-2.0.0a1/tinymovr.egg-info/SOURCES.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        1 2024-04-22 10:51:18.000000 tinymovr-2.0.0a1/tinymovr.egg-info/dependency_links.txt
--rw-r--r--   0 yanconst   (501) staff       (20)      116 2024-04-22 10:51:18.000000 tinymovr-2.0.0a1/tinymovr.egg-info/entry_points.txt
--rw-r--r--   0 yanconst   (501) staff       (20)      173 2024-04-22 10:51:18.000000 tinymovr-2.0.0a1/tinymovr.egg-info/requires.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        9 2024-04-22 10:51:18.000000 tinymovr-2.0.0a1/tinymovr.egg-info/top_level.txt
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-26 11:46:17.005914 tinymovr-2.0.0a2/
+-rw-r--r--   0 yanconst   (501) staff       (20)      681 2024-04-26 11:45:39.000000 tinymovr-2.0.0a2/MANIFEST.in
+-rw-r--r--   0 yanconst   (501) staff       (20)     2146 2024-04-26 11:46:17.005731 tinymovr-2.0.0a2/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     1689 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/README.md
+-rw-r--r--   0 yanconst   (501) staff       (20)       38 2024-04-26 11:46:17.005962 tinymovr-2.0.0a2/setup.cfg
+-rw-r--r--   0 yanconst   (501) staff       (20)     2387 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/setup.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-26 11:46:16.998266 tinymovr-2.0.0a2/tinymovr/
+-rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-2.0.0a2/tinymovr/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     4167 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/channel.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3164 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/cli.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-26 11:46:16.999693 tinymovr-2.0.0a2/tinymovr/codec/
+-rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-2.0.0a2/tinymovr/codec/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3281 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/codec/codec.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-26 11:46:17.000018 tinymovr-2.0.0a2/tinymovr/config/
+-rw-r--r--   0 yanconst   (501) staff       (20)      148 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/config/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     5338 2024-04-26 11:39:11.000000 tinymovr-2.0.0a2/tinymovr/config/config.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1079 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/constants.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     7313 2024-04-26 11:39:11.000000 tinymovr-2.0.0a2/tinymovr/dfu.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3256 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/discovery.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-26 11:46:17.001277 tinymovr-2.0.0a2/tinymovr/gui/
+-rw-r--r--   0 yanconst   (501) staff       (20)      665 2024-04-26 11:39:11.000000 tinymovr-2.0.0a2/tinymovr/gui/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2204 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/gui/gui.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    14412 2024-04-26 11:39:11.000000 tinymovr-2.0.0a2/tinymovr/gui/helpers.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    19455 2024-04-26 11:39:11.000000 tinymovr-2.0.0a2/tinymovr/gui/widgets.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    14125 2024-04-26 11:39:11.000000 tinymovr-2.0.0a2/tinymovr/gui/window.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     5620 2024-04-26 11:39:11.000000 tinymovr-2.0.0a2/tinymovr/gui/worker.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-26 11:46:16.996403 tinymovr-2.0.0a2/tinymovr/resources/
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-26 11:46:17.003707 tinymovr-2.0.0a2/tinymovr/resources/icons/
+-rw-r--r--   0 yanconst   (501) staff       (20)     3184 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/resources/icons/call.png
+-rw-r--r--   0 yanconst   (501) staff       (20)     3184 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/resources/icons/call@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    22790 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/resources/icons/call_dark.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    22672 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/resources/icons/call_dark@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    26604 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/resources/icons/empty.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    44831 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/resources/icons/empty@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    30381 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/resources/icons/empty_dark.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    51206 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/resources/icons/empty_dark@2x.png
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-26 11:46:17.005278 tinymovr-2.0.0a2/tinymovr/specs/
+-rw-r--r--   0 yanconst   (501) staff       (20)     1820 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/specs/dfu_1_0_x.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)     2148 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/specs/dfu_1_1_x.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)    15484 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/specs/tinymovr_1_3_x.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)    16329 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/specs/tinymovr_1_4_x.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)    18659 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/specs/tinymovr_1_5_x.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)    18824 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/specs/tinymovr_1_6_x.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)    24079 2024-04-26 11:39:11.000000 tinymovr-2.0.0a2/tinymovr/specs/tinymovr_2_0_x.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)     3555 2024-04-21 22:08:50.000000 tinymovr-2.0.0a2/tinymovr/tee.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2024-04-26 11:46:16.999346 tinymovr-2.0.0a2/tinymovr.egg-info/
+-rw-r--r--   0 yanconst   (501) staff       (20)     2146 2024-04-26 11:46:16.000000 tinymovr-2.0.0a2/tinymovr.egg-info/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     1144 2024-04-26 11:46:16.000000 tinymovr-2.0.0a2/tinymovr.egg-info/SOURCES.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        1 2024-04-26 11:46:16.000000 tinymovr-2.0.0a2/tinymovr.egg-info/dependency_links.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)      116 2024-04-26 11:46:16.000000 tinymovr-2.0.0a2/tinymovr.egg-info/entry_points.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)      173 2024-04-26 11:46:16.000000 tinymovr-2.0.0a2/tinymovr.egg-info/requires.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        9 2024-04-26 11:46:16.000000 tinymovr-2.0.0a2/tinymovr.egg-info/top_level.txt
```

### Comparing `tinymovr-2.0.0a1/MANIFEST.in` & `tinymovr-2.0.0a2/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -7,9 +7,10 @@
 include tinymovr/resources/icons/empty@2x.png
 include tinymovr/resources/icons/empty_dark.png
 include tinymovr/resources/icons/empty_dark@2x.png
 include tinymovr/specs/tinymovr_1_3_x.yaml
 include tinymovr/specs/tinymovr_1_4_x.yaml
 include tinymovr/specs/tinymovr_1_5_x.yaml
 include tinymovr/specs/tinymovr_1_6_x.yaml
+include tinymovr/specs/tinymovr_2_0_x.yaml
 include tinymovr/specs/dfu_1_0_x.yaml
 include tinymovr/specs/dfu_1_1_x.yaml
```

### Comparing `tinymovr-2.0.0a1/PKG-INFO` & `tinymovr-2.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-2.0.0a1/README.md` & `tinymovr-2.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/setup.py` & `tinymovr-2.0.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/channel.py` & `tinymovr-2.0.0a2/tinymovr/channel.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/cli.py` & `tinymovr-2.0.0a2/tinymovr/cli.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/codec/codec.py` & `tinymovr-2.0.0a2/tinymovr/codec/codec.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/config/config.py` & `tinymovr-2.0.0a2/tinymovr/config/config.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/constants.py` & `tinymovr-2.0.0a2/tinymovr/constants.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/dfu.py` & `tinymovr-2.0.0a2/tinymovr/dfu.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/discovery.py` & `tinymovr-2.0.0a2/tinymovr/discovery.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/gui/__init__.py` & `tinymovr-2.0.0a2/tinymovr/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/gui/gui.py` & `tinymovr-2.0.0a2/tinymovr/gui/gui.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/gui/helpers.py` & `tinymovr-2.0.0a2/tinymovr/gui/helpers.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/gui/widgets.py` & `tinymovr-2.0.0a2/tinymovr/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/gui/window.py` & `tinymovr-2.0.0a2/tinymovr/gui/window.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/gui/worker.py` & `tinymovr-2.0.0a2/tinymovr/gui/worker.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/resources/icons/call.png` & `tinymovr-2.0.0a2/tinymovr/resources/icons/call.png`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/resources/icons/call@2x.png` & `tinymovr-2.0.0a2/tinymovr/resources/icons/call@2x.png`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/resources/icons/call_dark.png` & `tinymovr-2.0.0a2/tinymovr/resources/icons/call_dark.png`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/resources/icons/call_dark@2x.png` & `tinymovr-2.0.0a2/tinymovr/resources/icons/call_dark@2x.png`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/resources/icons/empty.png` & `tinymovr-2.0.0a2/tinymovr/resources/icons/empty.png`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/resources/icons/empty@2x.png` & `tinymovr-2.0.0a2/tinymovr/resources/icons/empty@2x.png`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/resources/icons/empty_dark.png` & `tinymovr-2.0.0a2/tinymovr/resources/icons/empty_dark.png`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/resources/icons/empty_dark@2x.png` & `tinymovr-2.0.0a2/tinymovr/resources/icons/empty_dark@2x.png`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/specs/dfu_1_0_x.yaml` & `tinymovr-2.0.0a2/tinymovr/specs/dfu_1_0_x.yaml`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/specs/dfu_1_1_x.yaml` & `tinymovr-2.0.0a2/tinymovr/specs/dfu_1_1_x.yaml`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/specs/tinymovr_1_3_x.yaml` & `tinymovr-2.0.0a2/tinymovr/specs/tinymovr_1_3_x.yaml`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/specs/tinymovr_1_4_x.yaml` & `tinymovr-2.0.0a2/tinymovr/specs/tinymovr_1_4_x.yaml`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/specs/tinymovr_1_5_x.yaml` & `tinymovr-2.0.0a2/tinymovr/specs/tinymovr_1_5_x.yaml`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/specs/tinymovr_1_6_x.yaml` & `tinymovr-2.0.0a2/tinymovr/specs/tinymovr_1_6_x.yaml`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr/tee.py` & `tinymovr-2.0.0a2/tinymovr/tee.py`

 * *Files identical despite different names*

### Comparing `tinymovr-2.0.0a1/tinymovr.egg-info/PKG-INFO` & `tinymovr-2.0.0a2/tinymovr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-2.0.0a1/tinymovr.egg-info/SOURCES.txt` & `tinymovr-2.0.0a2/tinymovr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,8 +33,9 @@
 tinymovr/resources/icons/empty_dark.png
 tinymovr/resources/icons/empty_dark@2x.png
 tinymovr/specs/dfu_1_0_x.yaml
 tinymovr/specs/dfu_1_1_x.yaml
 tinymovr/specs/tinymovr_1_3_x.yaml
 tinymovr/specs/tinymovr_1_4_x.yaml
 tinymovr/specs/tinymovr_1_5_x.yaml
-tinymovr/specs/tinymovr_1_6_x.yaml
+tinymovr/specs/tinymovr_1_6_x.yaml
+tinymovr/specs/tinymovr_2_0_x.yaml
```

