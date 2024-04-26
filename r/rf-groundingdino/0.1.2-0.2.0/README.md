# Comparing `tmp/rf_groundingdino-0.1.2.tar.gz` & `tmp/rf_groundingdino-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rf_groundingdino-0.1.2.tar", last modified: Mon Jun  5 03:42:37 2023, max compression
+gzip compressed data, was "rf_groundingdino-0.2.0.tar", last modified: Fri Apr 26 19:17:13 2024, max compression
```

## Comparing `rf_groundingdino-0.1.2.tar` & `rf_groundingdino-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:42:37.684290 rf_groundingdino-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-06-05 03:42:37.684290 rf_groundingdino-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14972 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:42:37.672290 rf_groundingdino-0.1.2/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 03:42:37.000000 rf_groundingdino-0.1.2/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:42:37.676290 rf_groundingdino-0.1.2/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:42:37.676290 rf_groundingdino-0.1.2/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:42:37.676290 rf_groundingdino-0.1.2/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:42:37.676290 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:42:37.680290 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16691 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:42:37.684290 rf_groundingdino-0.1.2/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/groundingdino/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:42:37.684290 rf_groundingdino-0.1.2/rf_groundingdino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-06-05 03:42:37.000000 rf_groundingdino-0.1.2/rf_groundingdino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-05 03:42:37.000000 rf_groundingdino-0.1.2/rf_groundingdino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 03:42:37.000000 rf_groundingdino-0.1.2/rf_groundingdino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-05 03:42:37.000000 rf_groundingdino-0.1.2/rf_groundingdino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 03:42:37.000000 rf_groundingdino-0.1.2/rf_groundingdino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 03:42:37.684290 rf_groundingdino-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-06-05 03:40:11.000000 rf_groundingdino-0.1.2/setup.py
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 19:17:13.196615 rf_groundingdino-0.2.0/
+-rw-r--r--   0 lake       (502) staff       (20)    11355 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/LICENSE
+-rw-r--r--   0 lake       (502) staff       (20)      122 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/MANIFEST.in
+-rw-r--r--   0 lake       (502) staff       (20)    32268 2024-04-26 19:17:13.196510 rf_groundingdino-0.2.0/PKG-INFO
+-rw-r--r--   0 lake       (502) staff       (20)    18784 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/README.md
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 19:17:13.185907 rf_groundingdino-0.2.0/groundingdino/
+-rw-r--r--   0 lake       (502) staff       (20)       22 2024-04-26 19:17:13.000000 rf_groundingdino-0.2.0/groundingdino/__init__.py
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 19:17:13.186761 rf_groundingdino-0.2.0/groundingdino/config/
+-rw-r--r--   0 lake       (502) staff       (20)     1007 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 lake       (502) staff       (20)     1006 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 lake       (502) staff       (20)        0 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/config/__init__.py
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 19:17:13.187350 rf_groundingdino-0.2.0/groundingdino/datasets/
+-rw-r--r--   0 lake       (502) staff       (20)        0 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/datasets/__init__.py
+-rw-r--r--   0 lake       (502) staff       (20)     9398 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 lake       (502) staff       (20)     9711 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 19:17:13.187995 rf_groundingdino-0.2.0/groundingdino/models/
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 19:17:13.190700 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 lake       (502) staff       (20)      823 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 19:17:13.191933 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 lake       (502) staff       (20)       37 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 lake       (502) staff       (20)     7972 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 lake       (502) staff       (20)     6866 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 lake       (502) staff       (20)    29339 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 lake       (502) staff       (20)    12242 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 lake       (502) staff       (20)    11825 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 lake       (502) staff       (20)    17406 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 lake       (502) staff       (20)    13253 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 lake       (502) staff       (20)    36805 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 lake       (502) staff       (20)     4020 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 lake       (502) staff       (20)    10087 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 lake       (502) staff       (20)      754 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/__init__.py
+-rw-r--r--   0 lake       (502) staff       (20)     2143 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/models/registry.py
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 19:17:13.195196 rf_groundingdino-0.2.0/groundingdino/util/
+-rw-r--r--   0 lake       (502) staff       (20)       71 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/__init__.py
+-rw-r--r--   0 lake       (502) staff       (20)     3905 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/box_ops.py
+-rw-r--r--   0 lake       (502) staff       (20)     1345 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 lake       (502) staff       (20)     9243 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/inference.py
+-rw-r--r--   0 lake       (502) staff       (20)     3303 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/logger.py
+-rw-r--r--   0 lake       (502) staff       (20)    23348 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/misc.py
+-rw-r--r--   0 lake       (502) staff       (20)    14380 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/slconfig.py
+-rw-r--r--   0 lake       (502) staff       (20)     5377 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/slio.py
+-rw-r--r--   0 lake       (502) staff       (20)     1567 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/time_counter.py
+-rw-r--r--   0 lake       (502) staff       (20)    17828 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/utils.py
+-rw-r--r--   0 lake       (502) staff       (20)    12047 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/visualizer.py
+-rw-r--r--   0 lake       (502) staff       (20)     3489 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/groundingdino/util/vl_utils.py
+-rw-r--r--   0 lake       (502) staff       (20)       92 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/requirements.txt
+drwxr-xr-x   0 lake       (502) staff       (20)        0 2024-04-26 19:17:13.196102 rf_groundingdino-0.2.0/rf_groundingdino.egg-info/
+-rw-r--r--   0 lake       (502) staff       (20)    32268 2024-04-26 19:17:13.000000 rf_groundingdino-0.2.0/rf_groundingdino.egg-info/PKG-INFO
+-rw-r--r--   0 lake       (502) staff       (20)     1618 2024-04-26 19:17:13.000000 rf_groundingdino-0.2.0/rf_groundingdino.egg-info/SOURCES.txt
+-rw-r--r--   0 lake       (502) staff       (20)        1 2024-04-26 19:17:13.000000 rf_groundingdino-0.2.0/rf_groundingdino.egg-info/dependency_links.txt
+-rw-r--r--   0 lake       (502) staff       (20)       92 2024-04-26 19:17:13.000000 rf_groundingdino-0.2.0/rf_groundingdino.egg-info/requires.txt
+-rw-r--r--   0 lake       (502) staff       (20)       14 2024-04-26 19:17:13.000000 rf_groundingdino-0.2.0/rf_groundingdino.egg-info/top_level.txt
+-rw-r--r--   0 lake       (502) staff       (20)      396 2024-04-26 19:17:13.196931 rf_groundingdino-0.2.0/setup.cfg
+-rw-r--r--   0 lake       (502) staff       (20)     7804 2024-04-26 19:15:57.000000 rf_groundingdino-0.2.0/setup.py
```

### Comparing `rf_groundingdino-0.1.2/LICENSE` & `rf_groundingdino-0.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2020 - present, Facebook, Inc
+   Copyright 2023 - present, IDEA Research.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rf_groundingdino-0.1.2/PKG-INFO` & `rf_groundingdino-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rf_groundingdino
-Version: 0.1.2
+Version: 0.2.0
 Summary: open-set object detector
 Home-page: https://github.com/roboflow/GroundingDINO
 Author: International Digital Economy Academy, Shilong Liu
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -188,15 +188,15 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright 2020 - present, Facebook, Inc
+           Copyright 2023 - present, IDEA Research.
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
@@ -204,70 +204,101 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: transformers
+Requires-Dist: addict
+Requires-Dist: yapf
+Requires-Dist: timm
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: supervision
+Requires-Dist: pycocotools
+
+<div align="center">
+  <img src="./.asset/grounding_dino_logo.png" width="30%">
+</div>
 
-# :sauropod: Grounding DINO
+# :sauropod: Grounding DINO 
 
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/zero-shot-object-detection-on-mscoco)](https://paperswithcode.com/sota/zero-shot-object-detection-on-mscoco?p=grounding-dino-marrying-dino-with-grounded) [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/zero-shot-object-detection-on-odinw)](https://paperswithcode.com/sota/zero-shot-object-detection-on-odinw?p=grounding-dino-marrying-dino-with-grounded) \
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/object-detection-on-coco-minival)](https://paperswithcode.com/sota/object-detection-on-coco-minival?p=grounding-dino-marrying-dino-with-grounded) [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/object-detection-on-coco)](https://paperswithcode.com/sota/object-detection-on-coco?p=grounding-dino-marrying-dino-with-grounded)
-[![image](https://img.shields.io/pypi/v/rf_groundingdino.svg)](https://pypi.python.org/pypi/rf_groundingdino)
 
-Official PyTorch implementation of ["Grounding DINO: Marrying DINO with Grounded Pre-Training for Open-Set Object Detection"](https://arxiv.org/abs/2303.05499): the SoTA open-set object detector.
+
+**[IDEA-CVR, IDEA-Research](https://github.com/IDEA-Research)** 
+
+[Shilong Liu](http://www.lsl.zone/), [Zhaoyang Zeng](https://scholar.google.com/citations?user=U_cvvUwAAAAJ&hl=zh-CN&oi=ao), [Tianhe Ren](https://rentainhe.github.io/), [Feng Li](https://scholar.google.com/citations?user=ybRe9GcAAAAJ&hl=zh-CN), [Hao Zhang](https://scholar.google.com/citations?user=B8hPxMQAAAAJ&hl=zh-CN), [Jie Yang](https://github.com/yangjie-cv), [Chunyuan Li](https://scholar.google.com/citations?user=Zd7WmXUAAAAJ&hl=zh-CN&oi=ao), [Jianwei Yang](https://jwyang.github.io/), [Hang Su](https://scholar.google.com/citations?hl=en&user=dxN1_X0AAAAJ&view_op=list_works&sortby=pubdate), [Jun Zhu](https://scholar.google.com/citations?hl=en&user=axsP38wAAAAJ), [Lei Zhang](https://www.leizhang.org/)<sup>:email:</sup>.
+
+
+[[`Paper`](https://arxiv.org/abs/2303.05499)] [[`Demo`](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo)] [[`BibTex`](#black_nib-citation)]
+
+
+PyTorch implementation and pretrained models for Grounding DINO. For details, see the paper **[Grounding DINO: Marrying DINO with Grounded Pre-Training for Open-Set Object Detection](https://arxiv.org/abs/2303.05499)**.
 
 ## :sun_with_face: Helpful Tutorial
 
 - :grapes: [[Read our arXiv Paper](https://arxiv.org/abs/2303.05499)]
-- :apple: [[Watch our simple introduction video on YouTube](https://youtu.be/wxWDt5UiwY8)]
-- :rose: &nbsp;[[Try the Colab Demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb)]
+- :apple:  [[Watch our simple introduction video on YouTube](https://youtu.be/wxWDt5UiwY8)]
+- :blossom:   &nbsp;[[Try the Colab Demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb)]
 - :sunflower: [[Try our Official Huggingface Demo](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo)]
 - :maple_leaf: [[Watch the Step by Step Tutorial about GroundingDINO by Roboflow AI](https://youtu.be/cMa77r3YrDk)]
 - :mushroom: [[GroundingDINO: Automated Dataset Annotation and Evaluation by Roboflow AI](https://youtu.be/C4NqaRBz_Kw)]
 - :hibiscus: [[Accelerate Image Annotation with SAM and GroundingDINO by Roboflow AI](https://youtu.be/oEQYStnF2l8)]
+- :white_flower: [[Autodistill: Train YOLOv8 with ZERO Annotations based on Grounding-DINO and Grounded-SAM by Roboflow AI](https://github.com/autodistill/autodistill)]
 
-<!-- Grounding DINO Methods |
-[![arXiv](https://img.shields.io/badge/arXiv-2303.05499-b31b1b.svg)](https://arxiv.org/abs/2303.05499)
+<!-- Grounding DINO Methods | 
+[![arXiv](https://img.shields.io/badge/arXiv-2303.05499-b31b1b.svg)](https://arxiv.org/abs/2303.05499) 
 [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/wxWDt5UiwY8) -->
 
 <!-- Grounding DINO Demos |
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb) -->
 <!-- [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/cMa77r3YrDk)
 [![HuggingFace space](https://img.shields.io/badge/🤗-HuggingFace%20Space-cyan.svg)](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo)
 [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/oEQYStnF2l8)
 [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/C4NqaRBz_Kw) -->
 
 ## :sparkles: Highlight Projects
 
+- [Semantic-SAM: a universal image segmentation model to enable segment and recognize anything at any desired granularity.](https://github.com/UX-Decoder/Semantic-SAM), 
 - [DetGPT: Detect What You Need via Reasoning](https://github.com/OptimalScale/DetGPT)
 - [Grounded-SAM: Marrying Grounding DINO with Segment Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything)
 - [Grounding DINO with Stable Diffusion](demo/image_editing_with_groundingdino_stablediffusion.ipynb)
 - [Grounding DINO with GLIGEN for Controllable Image Editing](demo/image_editing_with_groundingdino_gligen.ipynb)
 - [OpenSeeD: A Simple and Strong Openset Segmentation Model](https://github.com/IDEA-Research/OpenSeeD)
 - [SEEM: Segment Everything Everywhere All at Once](https://github.com/UX-Decoder/Segment-Everything-Everywhere-All-At-Once)
 - [X-GPT: Conversational Visual Agent supported by X-Decoder](https://github.com/microsoft/X-Decoder/tree/xgpt)
 - [GLIGEN: Open-Set Grounded Text-to-Image Generation](https://github.com/gligen/GLIGEN)
 - [LLaVA: Large Language and Vision Assistant](https://github.com/haotian-liu/LLaVA)
 
 <!-- Extensions | [Grounding DINO with Segment Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything); [Grounding DINO with Stable Diffusion](demo/image_editing_with_groundingdino_stablediffusion.ipynb); [Grounding DINO with GLIGEN](demo/image_editing_with_groundingdino_gligen.ipynb)  -->
 
+
+
 <!-- Official PyTorch implementation of [Grounding DINO](https://arxiv.org/abs/2303.05499), a stronger open-set object detector. Code is available now! -->
 
+
 ## :bulb: Highlight
 
 - **Open-Set Detection.** Detect **everything** with language!
 - **High Performancce.** COCO zero-shot **52.5 AP** (training without COCO data!). COCO fine-tune **63.0 AP**.
 - **Flexible.** Collaboration with Stable Diffusion for Image Editting.
 
-## :fire: News
 
+
+
+## :fire: News
+- **`2023/07/18`**: We release [Semantic-SAM](https://github.com/UX-Decoder/Semantic-SAM), a universal image segmentation model to enable segment and recognize anything at any desired granularity. **Code** and **checkpoint** are available!
+- **`2023/06/17`**: We provide an example to evaluate Grounding DINO on COCO zero-shot performance.
 - **`2023/04/15`**: Refer to [CV in the Wild Readings](https://github.com/Computer-Vision-in-the-Wild/CVinW_Readings) for those who are interested in open-set recognition!
-- **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN) for more controllable image editings.
+- **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN)  for more controllable image editings.
 - **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_stablediffusion.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) for image editings.
 - **`2023/04/06`**: We build a new demo by marrying GroundingDINO with [Segment-Anything](https://github.com/facebookresearch/segment-anything) named **[Grounded-Segment-Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything)** aims to support segmentation in GroundingDINO.
 - **`2023/03/28`**: A YouTube [video](https://youtu.be/cMa77r3YrDk) about Grounding DINO and basic object detection prompt engineering. [[SkalskiP](https://github.com/SkalskiP)]
 - **`2023/03/28`**: Add a [demo](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo) on Hugging Face Space!
 - **`2023/03/27`**: Support CPU-only mode. Now the model can run on machines without GPUs.
 - **`2023/03/25`**: A [demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb) for Grounding DINO is available at Colab. [[SkalskiP](https://github.com/SkalskiP)]
 - **`2023/03/22`**: Code is available Now!
@@ -279,96 +310,134 @@
  <a href="https://arxiv.org/abs/2303.05499">Paper</a> introduction.
 <img src=".asset/hero_figure.png" alt="ODinW" width="100%">
 Marrying <a href="https://github.com/IDEA-Research/GroundingDINO">Grounding DINO</a> and <a href="https://github.com/gligen/GLIGEN">GLIGEN</a>
 <img src="https://huggingface.co/ShilongLiu/GroundingDINO/resolve/main/GD_GLIGEN.png" alt="gd_gligen" width="100%">
 </details>
 
 ## :star: Explanations/Tips for Grounding DINO Inputs and Outputs
-
 - Grounding DINO accepts an `(image, text)` pair as inputs.
 - It outputs `900` (by default) object boxes. Each box has similarity scores across all input words. (as shown in Figures below.)
 - We defaultly choose the boxes whose highest similarities are higher than a `box_threshold`.
 - We extract the words whose similarities are higher than the `text_threshold` as predicted labels.
-- If you want to obtain objects of specific phrases, like the `dogs` in the sentence `two dogs with a stick.`, you can select the boxes with highest text similarities with `dogs` as final outputs.
+- If you want to obtain objects of specific phrases, like the `dogs` in the sentence `two dogs with a stick.`, you can select the boxes with highest text similarities with `dogs` as final outputs. 
 - Note that each word can be split to **more than one** tokens with different tokenlizers. The number of words in a sentence may not equal to the number of text tokens.
 - We suggest separating different category names with `.` for Grounding DINO.
-  ![model_explain1](.asset/model_explan1.PNG)
-  ![model_explain2](.asset/model_explan2.PNG)
+![model_explain1](.asset/model_explan1.PNG)
+![model_explain2](.asset/model_explan2.PNG)
 
-## :label: TODO
+## :label: TODO 
 
 - [x] Release inference code and demo.
 - [x] Release checkpoints.
 - [x] Grounding DINO with Stable Diffusion and GLIGEN demos.
 - [ ] Release training codes.
 
-## :hammer_and_wrench: Install
+## :hammer_and_wrench: Install 
 
 **Note:**
 
-If you have a CUDA environment, please make sure the environment variable `CUDA_HOME` is set. It will be compiled under CPU-only mode if no CUDA available.
+0. If you have a CUDA environment, please make sure the environment variable `CUDA_HOME` is set. It will be compiled under CPU-only mode if no CUDA available.
 
-**Installation:**
+Please make sure following the installation steps strictly, otherwise the program may produce: 
+```bash
+NameError: name '_C' is not defined
+```
 
-Clone the GroundingDINO repository from GitHub.
+If this happened, please reinstalled the groundingDINO by reclone the git and do all the installation steps again.
+ 
+#### how to check cuda:
+```bash
+echo $CUDA_HOME
+```
+If it print nothing, then it means you haven't set up the path/
 
+Run this so the environment variable will be set under current shell. 
 ```bash
-git clone https://github.com/IDEA-Research/GroundingDINO.git
+export CUDA_HOME=/path/to/cuda-11.3
 ```
 
-Change the current directory to the GroundingDINO folder.
+Notice the version of cuda should be aligned with your CUDA runtime, for there might exists multiple cuda at the same time. 
+
+If you want to set the CUDA_HOME permanently, store it using:
 
 ```bash
-cd GroundingDINO/
+echo 'export CUDA_HOME=/path/to/cuda' >> ~/.bashrc
+```
+after that, source the bashrc file and check CUDA_HOME:
+```bash
+source ~/.bashrc
+echo $CUDA_HOME
 ```
 
-Install the required dependencies in the current directory.
+In this example, /path/to/cuda-11.3 should be replaced with the path where your CUDA toolkit is installed. You can find this by typing **which nvcc** in your terminal:
 
+For instance, 
+if the output is /usr/local/cuda/bin/nvcc, then:
 ```bash
-pip3 install -q -e .
+export CUDA_HOME=/usr/local/cuda
 ```
+**Installation:**
 
-Create a new directory called "weights" to store the model weights.
+1.Clone the GroundingDINO repository from GitHub.
 
 ```bash
-mkdir weights
+git clone https://github.com/IDEA-Research/GroundingDINO.git
 ```
 
-Change the current directory to the "weights" folder.
+2. Change the current directory to the GroundingDINO folder.
 
 ```bash
-cd weights
+cd GroundingDINO/
 ```
 
-Download the model weights file.
+3. Install the required dependencies in the current directory.
 
 ```bash
+pip install -e .
+```
+
+4. Download pre-trained model weights.
+
+```bash
+mkdir weights
+cd weights
 wget -q https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth
+cd ..
 ```
 
 ## :arrow_forward: Demo
-
 Check your GPU ID (only if you're using a GPU)
 
 ```bash
 nvidia-smi
 ```
-
 Replace `{GPU ID}`, `image_you_want_to_detect.jpg`, and `"dir you want to save the output"` with appropriate values in the following command
-
 ```bash
 CUDA_VISIBLE_DEVICES={GPU ID} python demo/inference_on_a_image.py \
--c /GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py \
--p /GroundingDINO/weights/groundingdino_swint_ogc.pth \
+-c groundingdino/config/GroundingDINO_SwinT_OGC.py \
+-p weights/groundingdino_swint_ogc.pth \
 -i image_you_want_to_detect.jpg \
 -o "dir you want to save the output" \
 -t "chair"
  [--cpu-only] # open it for cpu mode
 ```
 
+If you would like to specify the phrases to detect, here is a demo:
+```bash
+CUDA_VISIBLE_DEVICES={GPU ID} python demo/inference_on_a_image.py \
+-c groundingdino/config/GroundingDINO_SwinT_OGC.py \
+-p ./groundingdino_swint_ogc.pth \
+-i .asset/cat_dog.jpeg \
+-o logs/1111 \
+-t "There is a cat and a dog in the image ." \
+--token_spans "[[[9, 10], [11, 14]], [[19, 20], [21, 24]]]"
+ [--cpu-only] # open it for cpu mode
+```
+The token_spans specify the start and end positions of a phrases. For example, the first phrase is `[[9, 10], [11, 14]]`. `"There is a cat and a dog in the image ."[9:10] = 'a'`, `"There is a cat and a dog in the image ."[11:14] = 'cat'`. Hence it refers to the phrase `a cat` . Similarly, the `[[19, 20], [21, 24]]` refers to the phrase `a dog`.
+
 See the `demo/inference_on_a_image.py` for more details.
 
 **Running with Python:**
 
 ```python
 from groundingdino.util.inference import load_model, load_image, predict, annotate
 import cv2
@@ -388,24 +457,37 @@
     box_threshold=BOX_TRESHOLD,
     text_threshold=TEXT_TRESHOLD
 )
 
 annotated_frame = annotate(image_source=image_source, boxes=boxes, logits=logits, phrases=phrases)
 cv2.imwrite("annotated_image.jpg", annotated_frame)
 ```
-
 **Web UI**
 
 We also provide a demo code to integrate Grounding DINO with Gradio Web UI. See the file `demo/gradio_app.py` for more details.
 
 **Notebooks**
 
-- We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN) for more controllable image editings.
+- We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN)  for more controllable image editings.
 - We release [demos](demo/image_editing_with_groundingdino_stablediffusion.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) for image editings.
 
+## COCO Zero-shot Evaluations
+
+We provide an example to evaluate Grounding DINO zero-shot performance on COCO. The results should be **48.5**.
+
+```bash
+CUDA_VISIBLE_DEVICES=0 \
+python demo/test_ap_on_coco.py \
+ -c groundingdino/config/GroundingDINO_SwinT_OGC.py \
+ -p weights/groundingdino_swint_ogc.pth \
+ --anno_path /path/to/annoataions/ie/instances_val2017.json \
+ --image_dir /path/to/imagedir/ie/val2017
+```
+
+
 ## :luggage: Checkpoints
 
 <!-- insert a table -->
 <table>
   <thead>
     <tr style="text-align: right;">
       <th></th>
@@ -430,15 +512,15 @@
     <tr>
       <th>2</th>
       <td>GroundingDINO-B</td>
       <td>Swin-B</td>
       <td>COCO,O365,GoldG,Cap4M,OpenImage,ODinW-35,RefCOCO</td>
       <td>56.7 </td>
       <td><a href="https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha2/groundingdino_swinb_cogcoor.pth">GitHub link</a>  | <a href="https://huggingface.co/ShilongLiu/GroundingDINO/resolve/main/groundingdino_swinb_cogcoor.pth">HF link</a> 
-      <td><a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/groundingdino/config/GroundingDINO_SwinB.cfg.py">link</a></td>
+      <td><a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/groundingdino/config/GroundingDINO_SwinB_cfg.py">link</a></td>
     </tr>
   </tbody>
 </table>
 
 ## :medal_military: Results
 
 <details open>
@@ -459,41 +541,48 @@
 <summary><font size="4">
 Marrying Grounding DINO with <a href="https://github.com/Stability-AI/StableDiffusion">Stable Diffusion</a> for Image Editing
 </font></summary>
 See our example <a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/demo/image_editing_with_groundingdino_stablediffusion.ipynb">notebook</a> for more details.
 <img src=".asset/GD_SD.png" alt="GD_SD" width="100%">
 </details>
 
+
 <details open>
 <summary><font size="4">
 Marrying Grounding DINO with <a href="https://github.com/gligen/GLIGEN">GLIGEN</a> for more Detailed Image Editing.
 </font></summary>
 See our example <a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/demo/image_editing_with_groundingdino_gligen.ipynb">notebook</a> for more details.
 <img src=".asset/GD_GLIGEN.png" alt="GD_GLIGEN" width="100%">
 </details>
 
 ## :sauropod: Model: Grounding DINO
 
 Includes: a text backbone, an image backbone, a feature enhancer, a language-guided query selection, and a cross-modality decoder.
 
 ![arch](.asset/arch.png)
 
+
 ## :hearts: Acknowledgement
 
 Our model is related to [DINO](https://github.com/IDEA-Research/DINO) and [GLIP](https://github.com/microsoft/GLIP). Thanks for their great work!
 
 We also thank great previous work including DETR, Deformable DETR, SMCA, Conditional DETR, Anchor DETR, Dynamic DETR, DAB-DETR, DN-DETR, etc. More related work are available at [Awesome Detection Transformer](https://github.com/IDEACVR/awesome-detection-transformer). A new toolbox [detrex](https://github.com/IDEA-Research/detrex) is available as well.
 
 Thanks [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) and [GLIGEN](https://github.com/gligen/GLIGEN) for their awesome models.
 
+
 ## :black_nib: Citation
 
-If you find our work helpful for your research, please consider citing the following BibTeX entry.
+If you find our work helpful for your research, please consider citing the following BibTeX entry.   
 
 ```bibtex
 @article{liu2023grounding,
   title={Grounding dino: Marrying dino with grounded pre-training for open-set object detection},
   author={Liu, Shilong and Zeng, Zhaoyang and Ren, Tianhe and Li, Feng and Zhang, Hao and Yang, Jie and Li, Chunyuan and Yang, Jianwei and Su, Hang and Zhu, Jun and others},
   journal={arXiv preprint arXiv:2303.05499},
   year={2023}
 }
 ```
+
+
+
+
```

### Comparing `rf_groundingdino-0.1.2/README.md` & `rf_groundingdino-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,83 @@
-# :sauropod: Grounding DINO
+<div align="center">
+  <img src="./.asset/grounding_dino_logo.png" width="30%">
+</div>
+
+# :sauropod: Grounding DINO 
 
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/zero-shot-object-detection-on-mscoco)](https://paperswithcode.com/sota/zero-shot-object-detection-on-mscoco?p=grounding-dino-marrying-dino-with-grounded) [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/zero-shot-object-detection-on-odinw)](https://paperswithcode.com/sota/zero-shot-object-detection-on-odinw?p=grounding-dino-marrying-dino-with-grounded) \
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/object-detection-on-coco-minival)](https://paperswithcode.com/sota/object-detection-on-coco-minival?p=grounding-dino-marrying-dino-with-grounded) [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/object-detection-on-coco)](https://paperswithcode.com/sota/object-detection-on-coco?p=grounding-dino-marrying-dino-with-grounded)
-[![image](https://img.shields.io/pypi/v/rf_groundingdino.svg)](https://pypi.python.org/pypi/rf_groundingdino)
 
-Official PyTorch implementation of ["Grounding DINO: Marrying DINO with Grounded Pre-Training for Open-Set Object Detection"](https://arxiv.org/abs/2303.05499): the SoTA open-set object detector.
+
+**[IDEA-CVR, IDEA-Research](https://github.com/IDEA-Research)** 
+
+[Shilong Liu](http://www.lsl.zone/), [Zhaoyang Zeng](https://scholar.google.com/citations?user=U_cvvUwAAAAJ&hl=zh-CN&oi=ao), [Tianhe Ren](https://rentainhe.github.io/), [Feng Li](https://scholar.google.com/citations?user=ybRe9GcAAAAJ&hl=zh-CN), [Hao Zhang](https://scholar.google.com/citations?user=B8hPxMQAAAAJ&hl=zh-CN), [Jie Yang](https://github.com/yangjie-cv), [Chunyuan Li](https://scholar.google.com/citations?user=Zd7WmXUAAAAJ&hl=zh-CN&oi=ao), [Jianwei Yang](https://jwyang.github.io/), [Hang Su](https://scholar.google.com/citations?hl=en&user=dxN1_X0AAAAJ&view_op=list_works&sortby=pubdate), [Jun Zhu](https://scholar.google.com/citations?hl=en&user=axsP38wAAAAJ), [Lei Zhang](https://www.leizhang.org/)<sup>:email:</sup>.
+
+
+[[`Paper`](https://arxiv.org/abs/2303.05499)] [[`Demo`](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo)] [[`BibTex`](#black_nib-citation)]
+
+
+PyTorch implementation and pretrained models for Grounding DINO. For details, see the paper **[Grounding DINO: Marrying DINO with Grounded Pre-Training for Open-Set Object Detection](https://arxiv.org/abs/2303.05499)**.
 
 ## :sun_with_face: Helpful Tutorial
 
 - :grapes: [[Read our arXiv Paper](https://arxiv.org/abs/2303.05499)]
-- :apple: [[Watch our simple introduction video on YouTube](https://youtu.be/wxWDt5UiwY8)]
-- :rose: &nbsp;[[Try the Colab Demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb)]
+- :apple:  [[Watch our simple introduction video on YouTube](https://youtu.be/wxWDt5UiwY8)]
+- :blossom:   &nbsp;[[Try the Colab Demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb)]
 - :sunflower: [[Try our Official Huggingface Demo](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo)]
 - :maple_leaf: [[Watch the Step by Step Tutorial about GroundingDINO by Roboflow AI](https://youtu.be/cMa77r3YrDk)]
 - :mushroom: [[GroundingDINO: Automated Dataset Annotation and Evaluation by Roboflow AI](https://youtu.be/C4NqaRBz_Kw)]
 - :hibiscus: [[Accelerate Image Annotation with SAM and GroundingDINO by Roboflow AI](https://youtu.be/oEQYStnF2l8)]
+- :white_flower: [[Autodistill: Train YOLOv8 with ZERO Annotations based on Grounding-DINO and Grounded-SAM by Roboflow AI](https://github.com/autodistill/autodistill)]
 
-<!-- Grounding DINO Methods |
-[![arXiv](https://img.shields.io/badge/arXiv-2303.05499-b31b1b.svg)](https://arxiv.org/abs/2303.05499)
+<!-- Grounding DINO Methods | 
+[![arXiv](https://img.shields.io/badge/arXiv-2303.05499-b31b1b.svg)](https://arxiv.org/abs/2303.05499) 
 [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/wxWDt5UiwY8) -->
 
 <!-- Grounding DINO Demos |
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb) -->
 <!-- [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/cMa77r3YrDk)
 [![HuggingFace space](https://img.shields.io/badge/🤗-HuggingFace%20Space-cyan.svg)](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo)
 [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/oEQYStnF2l8)
 [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/C4NqaRBz_Kw) -->
 
 ## :sparkles: Highlight Projects
 
+- [Semantic-SAM: a universal image segmentation model to enable segment and recognize anything at any desired granularity.](https://github.com/UX-Decoder/Semantic-SAM), 
 - [DetGPT: Detect What You Need via Reasoning](https://github.com/OptimalScale/DetGPT)
 - [Grounded-SAM: Marrying Grounding DINO with Segment Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything)
 - [Grounding DINO with Stable Diffusion](demo/image_editing_with_groundingdino_stablediffusion.ipynb)
 - [Grounding DINO with GLIGEN for Controllable Image Editing](demo/image_editing_with_groundingdino_gligen.ipynb)
 - [OpenSeeD: A Simple and Strong Openset Segmentation Model](https://github.com/IDEA-Research/OpenSeeD)
 - [SEEM: Segment Everything Everywhere All at Once](https://github.com/UX-Decoder/Segment-Everything-Everywhere-All-At-Once)
 - [X-GPT: Conversational Visual Agent supported by X-Decoder](https://github.com/microsoft/X-Decoder/tree/xgpt)
 - [GLIGEN: Open-Set Grounded Text-to-Image Generation](https://github.com/gligen/GLIGEN)
 - [LLaVA: Large Language and Vision Assistant](https://github.com/haotian-liu/LLaVA)
 
 <!-- Extensions | [Grounding DINO with Segment Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything); [Grounding DINO with Stable Diffusion](demo/image_editing_with_groundingdino_stablediffusion.ipynb); [Grounding DINO with GLIGEN](demo/image_editing_with_groundingdino_gligen.ipynb)  -->
 
+
+
 <!-- Official PyTorch implementation of [Grounding DINO](https://arxiv.org/abs/2303.05499), a stronger open-set object detector. Code is available now! -->
 
+
 ## :bulb: Highlight
 
 - **Open-Set Detection.** Detect **everything** with language!
 - **High Performancce.** COCO zero-shot **52.5 AP** (training without COCO data!). COCO fine-tune **63.0 AP**.
 - **Flexible.** Collaboration with Stable Diffusion for Image Editting.
 
-## :fire: News
 
+
+
+## :fire: News
+- **`2023/07/18`**: We release [Semantic-SAM](https://github.com/UX-Decoder/Semantic-SAM), a universal image segmentation model to enable segment and recognize anything at any desired granularity. **Code** and **checkpoint** are available!
+- **`2023/06/17`**: We provide an example to evaluate Grounding DINO on COCO zero-shot performance.
 - **`2023/04/15`**: Refer to [CV in the Wild Readings](https://github.com/Computer-Vision-in-the-Wild/CVinW_Readings) for those who are interested in open-set recognition!
-- **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN) for more controllable image editings.
+- **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN)  for more controllable image editings.
 - **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_stablediffusion.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) for image editings.
 - **`2023/04/06`**: We build a new demo by marrying GroundingDINO with [Segment-Anything](https://github.com/facebookresearch/segment-anything) named **[Grounded-Segment-Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything)** aims to support segmentation in GroundingDINO.
 - **`2023/03/28`**: A YouTube [video](https://youtu.be/cMa77r3YrDk) about Grounding DINO and basic object detection prompt engineering. [[SkalskiP](https://github.com/SkalskiP)]
 - **`2023/03/28`**: Add a [demo](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo) on Hugging Face Space!
 - **`2023/03/27`**: Support CPU-only mode. Now the model can run on machines without GPUs.
 - **`2023/03/25`**: A [demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb) for Grounding DINO is available at Colab. [[SkalskiP](https://github.com/SkalskiP)]
 - **`2023/03/22`**: Code is available Now!
@@ -68,96 +89,134 @@
  <a href="https://arxiv.org/abs/2303.05499">Paper</a> introduction.
 <img src=".asset/hero_figure.png" alt="ODinW" width="100%">
 Marrying <a href="https://github.com/IDEA-Research/GroundingDINO">Grounding DINO</a> and <a href="https://github.com/gligen/GLIGEN">GLIGEN</a>
 <img src="https://huggingface.co/ShilongLiu/GroundingDINO/resolve/main/GD_GLIGEN.png" alt="gd_gligen" width="100%">
 </details>
 
 ## :star: Explanations/Tips for Grounding DINO Inputs and Outputs
-
 - Grounding DINO accepts an `(image, text)` pair as inputs.
 - It outputs `900` (by default) object boxes. Each box has similarity scores across all input words. (as shown in Figures below.)
 - We defaultly choose the boxes whose highest similarities are higher than a `box_threshold`.
 - We extract the words whose similarities are higher than the `text_threshold` as predicted labels.
-- If you want to obtain objects of specific phrases, like the `dogs` in the sentence `two dogs with a stick.`, you can select the boxes with highest text similarities with `dogs` as final outputs.
+- If you want to obtain objects of specific phrases, like the `dogs` in the sentence `two dogs with a stick.`, you can select the boxes with highest text similarities with `dogs` as final outputs. 
 - Note that each word can be split to **more than one** tokens with different tokenlizers. The number of words in a sentence may not equal to the number of text tokens.
 - We suggest separating different category names with `.` for Grounding DINO.
-  ![model_explain1](.asset/model_explan1.PNG)
-  ![model_explain2](.asset/model_explan2.PNG)
+![model_explain1](.asset/model_explan1.PNG)
+![model_explain2](.asset/model_explan2.PNG)
 
-## :label: TODO
+## :label: TODO 
 
 - [x] Release inference code and demo.
 - [x] Release checkpoints.
 - [x] Grounding DINO with Stable Diffusion and GLIGEN demos.
 - [ ] Release training codes.
 
-## :hammer_and_wrench: Install
+## :hammer_and_wrench: Install 
 
 **Note:**
 
-If you have a CUDA environment, please make sure the environment variable `CUDA_HOME` is set. It will be compiled under CPU-only mode if no CUDA available.
+0. If you have a CUDA environment, please make sure the environment variable `CUDA_HOME` is set. It will be compiled under CPU-only mode if no CUDA available.
 
-**Installation:**
+Please make sure following the installation steps strictly, otherwise the program may produce: 
+```bash
+NameError: name '_C' is not defined
+```
 
-Clone the GroundingDINO repository from GitHub.
+If this happened, please reinstalled the groundingDINO by reclone the git and do all the installation steps again.
+ 
+#### how to check cuda:
+```bash
+echo $CUDA_HOME
+```
+If it print nothing, then it means you haven't set up the path/
 
+Run this so the environment variable will be set under current shell. 
 ```bash
-git clone https://github.com/IDEA-Research/GroundingDINO.git
+export CUDA_HOME=/path/to/cuda-11.3
 ```
 
-Change the current directory to the GroundingDINO folder.
+Notice the version of cuda should be aligned with your CUDA runtime, for there might exists multiple cuda at the same time. 
+
+If you want to set the CUDA_HOME permanently, store it using:
 
 ```bash
-cd GroundingDINO/
+echo 'export CUDA_HOME=/path/to/cuda' >> ~/.bashrc
+```
+after that, source the bashrc file and check CUDA_HOME:
+```bash
+source ~/.bashrc
+echo $CUDA_HOME
 ```
 
-Install the required dependencies in the current directory.
+In this example, /path/to/cuda-11.3 should be replaced with the path where your CUDA toolkit is installed. You can find this by typing **which nvcc** in your terminal:
 
+For instance, 
+if the output is /usr/local/cuda/bin/nvcc, then:
 ```bash
-pip3 install -q -e .
+export CUDA_HOME=/usr/local/cuda
 ```
+**Installation:**
 
-Create a new directory called "weights" to store the model weights.
+1.Clone the GroundingDINO repository from GitHub.
 
 ```bash
-mkdir weights
+git clone https://github.com/IDEA-Research/GroundingDINO.git
 ```
 
-Change the current directory to the "weights" folder.
+2. Change the current directory to the GroundingDINO folder.
 
 ```bash
-cd weights
+cd GroundingDINO/
+```
+
+3. Install the required dependencies in the current directory.
+
+```bash
+pip install -e .
 ```
 
-Download the model weights file.
+4. Download pre-trained model weights.
 
 ```bash
+mkdir weights
+cd weights
 wget -q https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth
+cd ..
 ```
 
 ## :arrow_forward: Demo
-
 Check your GPU ID (only if you're using a GPU)
 
 ```bash
 nvidia-smi
 ```
-
 Replace `{GPU ID}`, `image_you_want_to_detect.jpg`, and `"dir you want to save the output"` with appropriate values in the following command
-
 ```bash
 CUDA_VISIBLE_DEVICES={GPU ID} python demo/inference_on_a_image.py \
--c /GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py \
--p /GroundingDINO/weights/groundingdino_swint_ogc.pth \
+-c groundingdino/config/GroundingDINO_SwinT_OGC.py \
+-p weights/groundingdino_swint_ogc.pth \
 -i image_you_want_to_detect.jpg \
 -o "dir you want to save the output" \
 -t "chair"
  [--cpu-only] # open it for cpu mode
 ```
 
+If you would like to specify the phrases to detect, here is a demo:
+```bash
+CUDA_VISIBLE_DEVICES={GPU ID} python demo/inference_on_a_image.py \
+-c groundingdino/config/GroundingDINO_SwinT_OGC.py \
+-p ./groundingdino_swint_ogc.pth \
+-i .asset/cat_dog.jpeg \
+-o logs/1111 \
+-t "There is a cat and a dog in the image ." \
+--token_spans "[[[9, 10], [11, 14]], [[19, 20], [21, 24]]]"
+ [--cpu-only] # open it for cpu mode
+```
+The token_spans specify the start and end positions of a phrases. For example, the first phrase is `[[9, 10], [11, 14]]`. `"There is a cat and a dog in the image ."[9:10] = 'a'`, `"There is a cat and a dog in the image ."[11:14] = 'cat'`. Hence it refers to the phrase `a cat` . Similarly, the `[[19, 20], [21, 24]]` refers to the phrase `a dog`.
+
 See the `demo/inference_on_a_image.py` for more details.
 
 **Running with Python:**
 
 ```python
 from groundingdino.util.inference import load_model, load_image, predict, annotate
 import cv2
@@ -177,24 +236,37 @@
     box_threshold=BOX_TRESHOLD,
     text_threshold=TEXT_TRESHOLD
 )
 
 annotated_frame = annotate(image_source=image_source, boxes=boxes, logits=logits, phrases=phrases)
 cv2.imwrite("annotated_image.jpg", annotated_frame)
 ```
-
 **Web UI**
 
 We also provide a demo code to integrate Grounding DINO with Gradio Web UI. See the file `demo/gradio_app.py` for more details.
 
 **Notebooks**
 
-- We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN) for more controllable image editings.
+- We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN)  for more controllable image editings.
 - We release [demos](demo/image_editing_with_groundingdino_stablediffusion.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) for image editings.
 
+## COCO Zero-shot Evaluations
+
+We provide an example to evaluate Grounding DINO zero-shot performance on COCO. The results should be **48.5**.
+
+```bash
+CUDA_VISIBLE_DEVICES=0 \
+python demo/test_ap_on_coco.py \
+ -c groundingdino/config/GroundingDINO_SwinT_OGC.py \
+ -p weights/groundingdino_swint_ogc.pth \
+ --anno_path /path/to/annoataions/ie/instances_val2017.json \
+ --image_dir /path/to/imagedir/ie/val2017
+```
+
+
 ## :luggage: Checkpoints
 
 <!-- insert a table -->
 <table>
   <thead>
     <tr style="text-align: right;">
       <th></th>
@@ -219,15 +291,15 @@
     <tr>
       <th>2</th>
       <td>GroundingDINO-B</td>
       <td>Swin-B</td>
       <td>COCO,O365,GoldG,Cap4M,OpenImage,ODinW-35,RefCOCO</td>
       <td>56.7 </td>
       <td><a href="https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha2/groundingdino_swinb_cogcoor.pth">GitHub link</a>  | <a href="https://huggingface.co/ShilongLiu/GroundingDINO/resolve/main/groundingdino_swinb_cogcoor.pth">HF link</a> 
-      <td><a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/groundingdino/config/GroundingDINO_SwinB.cfg.py">link</a></td>
+      <td><a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/groundingdino/config/GroundingDINO_SwinB_cfg.py">link</a></td>
     </tr>
   </tbody>
 </table>
 
 ## :medal_military: Results
 
 <details open>
@@ -248,41 +320,48 @@
 <summary><font size="4">
 Marrying Grounding DINO with <a href="https://github.com/Stability-AI/StableDiffusion">Stable Diffusion</a> for Image Editing
 </font></summary>
 See our example <a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/demo/image_editing_with_groundingdino_stablediffusion.ipynb">notebook</a> for more details.
 <img src=".asset/GD_SD.png" alt="GD_SD" width="100%">
 </details>
 
+
 <details open>
 <summary><font size="4">
 Marrying Grounding DINO with <a href="https://github.com/gligen/GLIGEN">GLIGEN</a> for more Detailed Image Editing.
 </font></summary>
 See our example <a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/demo/image_editing_with_groundingdino_gligen.ipynb">notebook</a> for more details.
 <img src=".asset/GD_GLIGEN.png" alt="GD_GLIGEN" width="100%">
 </details>
 
 ## :sauropod: Model: Grounding DINO
 
 Includes: a text backbone, an image backbone, a feature enhancer, a language-guided query selection, and a cross-modality decoder.
 
 ![arch](.asset/arch.png)
 
+
 ## :hearts: Acknowledgement
 
 Our model is related to [DINO](https://github.com/IDEA-Research/DINO) and [GLIP](https://github.com/microsoft/GLIP). Thanks for their great work!
 
 We also thank great previous work including DETR, Deformable DETR, SMCA, Conditional DETR, Anchor DETR, Dynamic DETR, DAB-DETR, DN-DETR, etc. More related work are available at [Awesome Detection Transformer](https://github.com/IDEACVR/awesome-detection-transformer). A new toolbox [detrex](https://github.com/IDEA-Research/detrex) is available as well.
 
 Thanks [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) and [GLIGEN](https://github.com/gligen/GLIGEN) for their awesome models.
 
+
 ## :black_nib: Citation
 
-If you find our work helpful for your research, please consider citing the following BibTeX entry.
+If you find our work helpful for your research, please consider citing the following BibTeX entry.   
 
 ```bibtex
 @article{liu2023grounding,
   title={Grounding dino: Marrying dino with grounded pre-training for open-set object detection},
   author={Liu, Shilong and Zeng, Zhaoyang and Ren, Tianhe and Li, Feng and Zhang, Hao and Yang, Jie and Li, Chunyuan and Yang, Jianwei and Su, Hang and Zhu, Jun and others},
   journal={arXiv preprint arXiv:2303.05499},
   year={2023}
 }
 ```
+
+
+
+
```

### Comparing `rf_groundingdino-0.1.2/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `rf_groundingdino-0.2.0/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `rf_groundingdino-0.2.0/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/datasets/transforms.py` & `rf_groundingdino-0.2.0/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/__init__.py` & `rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/backbone/backbone.py` & `rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/bertwarper.py` & `rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/fuse_modules.py` & `rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/groundingdino.py` & `rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files 10% similar despite different names*

```diff
@@ -202,14 +202,29 @@
 
     def _reset_parameters(self):
         # init input_proj
         for proj in self.input_proj:
             nn.init.xavier_uniform_(proj[0].weight, gain=1)
             nn.init.constant_(proj[0].bias, 0)
 
+    def set_image_tensor(self, samples: NestedTensor):
+        if isinstance(samples, (list, torch.Tensor)):
+            samples = nested_tensor_from_tensor_list(samples)
+        self.features, self.poss = self.backbone(samples)
+
+    def unset_image_tensor(self):
+        if hasattr(self, 'features'):
+            del self.features
+        if hasattr(self,'poss'):
+            del self.poss 
+
+    def set_image_features(self, features , poss):
+        self.features = features
+        self.poss = poss
+
     def init_ref_points(self, use_num_queries):
         self.refpoint_embed = nn.Embedding(use_num_queries, self.query_dim)
 
     def forward(self, samples: NestedTensor, targets: List = None, **kw):
         """The forward expects a NestedTensor, which consists of:
            - samples.tensor: batched images, of shape [batch_size x 3 x H x W]
            - samples.mask: a binary mask of shape [batch_size x H x W], containing 1 on padded pixels
@@ -224,15 +239,14 @@
            - "aux_outputs": Optional, only returned when auxilary losses are activated. It is a list of
                             dictionnaries containing the two above keys for each decoder layer.
         """
         if targets is None:
             captions = kw["captions"]
         else:
             captions = [t["caption"] for t in targets]
-        len(captions)
 
         # encoder texts
         tokenized = self.tokenizer(captions, padding="longest", return_tensors="pt").to(
             samples.device
         )
         (
             text_self_attention_masks,
@@ -279,43 +293,43 @@
             "encoded_text": encoded_text,  # bs, 195, d_model
             "text_token_mask": text_token_mask,  # bs, 195
             "position_ids": position_ids,  # bs, 195
             "text_self_attention_masks": text_self_attention_masks,  # bs, 195,195
         }
 
         # import ipdb; ipdb.set_trace()
-
         if isinstance(samples, (list, torch.Tensor)):
             samples = nested_tensor_from_tensor_list(samples)
-        features, poss = self.backbone(samples)
+        if not hasattr(self, 'features') or not hasattr(self, 'poss'):
+            self.set_image_tensor(samples)
 
         srcs = []
         masks = []
-        for l, feat in enumerate(features):
+        for l, feat in enumerate(self.features):
             src, mask = feat.decompose()
             srcs.append(self.input_proj[l](src))
             masks.append(mask)
             assert mask is not None
         if self.num_feature_levels > len(srcs):
             _len_srcs = len(srcs)
             for l in range(_len_srcs, self.num_feature_levels):
                 if l == _len_srcs:
-                    src = self.input_proj[l](features[-1].tensors)
+                    src = self.input_proj[l](self.features[-1].tensors)
                 else:
                     src = self.input_proj[l](srcs[-1])
                 m = samples.mask
                 mask = F.interpolate(m[None].float(), size=src.shape[-2:]).to(torch.bool)[0]
                 pos_l = self.backbone[1](NestedTensor(src, mask)).to(src.dtype)
                 srcs.append(src)
                 masks.append(mask)
-                poss.append(pos_l)
+                self.poss.append(pos_l)
 
         input_query_bbox = input_query_label = attn_mask = dn_meta = None
         hs, reference, hs_enc, ref_enc, init_box_proposal = self.transformer(
-            srcs, masks, input_query_bbox, poss, input_query_label, attn_mask, text_dict
+            srcs, masks, input_query_bbox, self.poss, input_query_label, attn_mask, text_dict
         )
 
         # deformable-detr-like anchor update
         outputs_coord_list = []
         for dec_lid, (layer_ref_sig, layer_bbox_embed, layer_hs) in enumerate(
             zip(reference[:-1], self.bbox_embed, hs)
         ):
@@ -341,15 +355,17 @@
         # # for encoder output
         # if hs_enc is not None:
         #     # prepare intermediate outputs
         #     interm_coord = ref_enc[-1]
         #     interm_class = self.transformer.enc_out_class_embed(hs_enc[-1], text_dict)
         #     out['interm_outputs'] = {'pred_logits': interm_class, 'pred_boxes': interm_coord}
         #     out['interm_outputs_for_matching_pre'] = {'pred_logits': interm_class, 'pred_boxes': init_box_proposal}
-
+        unset_image_tensor = kw.get('unset_image_tensor', True)
+        if unset_image_tensor:
+            self.unset_image_tensor() ## If necessary
         return out
 
     @torch.jit.unused
     def _set_aux_loss(self, outputs_class, outputs_coord):
         # this is a workaround to make torchscript happy, as torchscript
         # doesn't support dictionary with non-homogeneous values, such
         # as a dict having both a Tensor and a list.
@@ -389,7 +405,8 @@
         dn_labelbook_size=dn_labelbook_size,
         text_encoder_type=args.text_encoder_type,
         sub_sentence_present=sub_sentence_present,
         max_text_len=args.max_text_len,
     )
 
     return model
+
```

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.autograd import Function
 from torch.autograd.function import once_differentiable
 from torch.nn.init import constant_, xavier_uniform_
 
+
 # helpers
 def _is_power_of_2(n):
     if (not isinstance(n, int)) or (n < 0):
         raise ValueError("invalid input for _is_power_of_2: {} (type: {})".format(n, type(n)))
     return (n & (n - 1) == 0) and n != 0
 
 
@@ -264,15 +265,15 @@
             )
         else:
             raise ValueError(
                 "Last dim of reference_points must be 2 or 4, but get {} instead.".format(
                     reference_points.shape[-1]
                 )
             )
-        
+
         output = multi_scale_deformable_attn_pytorch(
             value, spatial_shapes, sampling_locations, attention_weights
         )
 
         output = self.output_proj(output)
 
         if not self.batch_first:
```

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/transformer.py` & `rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/GroundingDINO/utils.py` & `rf_groundingdino-0.2.0/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/__init__.py` & `rf_groundingdino-0.2.0/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/models/registry.py` & `rf_groundingdino-0.2.0/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/util/box_ops.py` & `rf_groundingdino-0.2.0/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/util/get_tokenlizer.py` & `rf_groundingdino-0.2.0/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/util/inference.py` & `rf_groundingdino-0.2.0/groundingdino/util/inference.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import cv2
 import numpy as np
 import supervision as sv
 import torch
 from PIL import Image
 from torchvision.ops import box_convert
+import bisect
 
 import groundingdino.datasets.transforms as T
 from groundingdino.models import build_model
 from groundingdino.util.misc import clean_state_dict
 from groundingdino.util.slconfig import SLConfig
 from groundingdino.util.utils import get_phrases_from_posmap
 
@@ -51,15 +52,16 @@
 
 def predict(
         model,
         image: torch.Tensor,
         caption: str,
         box_threshold: float,
         text_threshold: float,
-        device: str = "cuda"
+        device: str = "cuda",
+        remove_combined: bool = False
 ) -> Tuple[torch.Tensor, torch.Tensor, List[str]]:
     caption = preprocess_caption(caption=caption)
 
     model = model.to(device)
     image = image.to(device)
 
     with torch.no_grad():
@@ -71,24 +73,47 @@
     mask = prediction_logits.max(dim=1)[0] > box_threshold
     logits = prediction_logits[mask]  # logits.shape = (n, 256)
     boxes = prediction_boxes[mask]  # boxes.shape = (n, 4)
 
     tokenizer = model.tokenizer
     tokenized = tokenizer(caption)
 
-    phrases = [
-        get_phrases_from_posmap(logit > text_threshold, tokenized, tokenizer).replace('.', '')
-        for logit
-        in logits
-    ]
+    if remove_combined:
+        sep_idx = [i for i in range(len(tokenized['input_ids'])) if tokenized['input_ids'][i] in [101, 102, 1012]]
+
+        phrases = []
+        for logit in logits:
+            max_idx = logit.argmax()
+            insert_idx = bisect.bisect_left(sep_idx, max_idx)
+            right_idx = sep_idx[insert_idx]
+            left_idx = sep_idx[insert_idx - 1]
+            phrases.append(get_phrases_from_posmap(logit > text_threshold, tokenized, tokenizer, left_idx, right_idx).replace('.', ''))
+    else:
+        phrases = [
+            get_phrases_from_posmap(logit > text_threshold, tokenized, tokenizer).replace('.', '')
+            for logit
+            in logits
+        ]
 
     return boxes, logits.max(dim=1)[0], phrases
 
 
 def annotate(image_source: np.ndarray, boxes: torch.Tensor, logits: torch.Tensor, phrases: List[str]) -> np.ndarray:
+    """
+    This function annotates an image with bounding boxes and labels.
+
+    Parameters:
+    image_source (np.ndarray): The source image to be annotated.
+    boxes (torch.Tensor): A tensor containing bounding box coordinates.
+    logits (torch.Tensor): A tensor containing confidence scores for each bounding box.
+    phrases (List[str]): A list of labels for each bounding box.
+
+    Returns:
+    np.ndarray: The annotated image.
+    """
     h, w, _ = image_source.shape
     boxes = boxes * torch.Tensor([w, h, w, h])
     xyxy = box_convert(boxes=boxes, in_fmt="cxcywh", out_fmt="xyxy").numpy()
     detections = sv.Detections(xyxy=xyxy)
 
     labels = [
         f"{phrase} {logit:.2f}"
@@ -149,16 +174,17 @@
         """
         processed_image = Model.preprocess_image(image_bgr=image).to(self.device)
         boxes, logits, phrases = predict(
             model=self.model,
             image=processed_image,
             caption=caption,
             box_threshold=box_threshold,
-            text_threshold=text_threshold, 
-            device=self.device)
+            text_threshold=text_threshold,
+            device=self.device,
+            remove_combined=True)
         source_h, source_w, _ = image.shape
         detections = Model.post_process_result(
             source_h=source_h,
             source_w=source_w,
             boxes=boxes,
             logits=logits)
         return detections, phrases
@@ -193,15 +219,16 @@
         processed_image = Model.preprocess_image(image_bgr=image).to(self.device)
         boxes, logits, phrases = predict(
             model=self.model,
             image=processed_image,
             caption=caption,
             box_threshold=box_threshold,
             text_threshold=text_threshold,
-            device=self.device)
+            device=self.device,
+            remove_combined=True)
         source_h, source_w, _ = image.shape
         detections = Model.post_process_result(
             source_h=source_h,
             source_w=source_w,
             boxes=boxes,
             logits=logits)
         class_id = Model.phrases2classes(phrases=phrases, classes=classes)
@@ -233,12 +260,14 @@
         confidence = logits.numpy()
         return sv.Detections(xyxy=xyxy, confidence=confidence)
 
     @staticmethod
     def phrases2classes(phrases: List[str], classes: List[str]) -> np.ndarray:
         class_ids = []
         for phrase in phrases:
-            try:
-                class_ids.append(classes.index(phrase))
-            except ValueError:
+            for class_ in classes:
+                if class_ in phrase:
+                    class_ids.append(classes.index(class_))
+                    break
+            else:
                 class_ids.append(None)
         return np.array(class_ids)
```

### Comparing `rf_groundingdino-0.1.2/groundingdino/util/logger.py` & `rf_groundingdino-0.2.0/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/util/misc.py` & `rf_groundingdino-0.2.0/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/util/slconfig.py` & `rf_groundingdino-0.2.0/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/util/slio.py` & `rf_groundingdino-0.2.0/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/util/time_counter.py` & `rf_groundingdino-0.2.0/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/util/utils.py` & `rf_groundingdino-0.2.0/groundingdino/util/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -593,16 +593,18 @@
     ]
     return [
         {k: v.to(device) if k not in excluded_keys else v for k, v in t.items()} for t in targets
     ]
 
 
 def get_phrases_from_posmap(
-    posmap: torch.BoolTensor, tokenized: Dict, tokenizer: AutoTokenizer
+    posmap: torch.BoolTensor, tokenized: Dict, tokenizer: AutoTokenizer, left_idx: int = 0, right_idx: int = 255
 ):
     assert isinstance(posmap, torch.Tensor), "posmap must be torch.Tensor"
     if posmap.dim() == 1:
+        posmap[0: left_idx + 1] = False
+        posmap[right_idx:] = False
         non_zero_idx = posmap.nonzero(as_tuple=True)[0].tolist()
         token_ids = [tokenized["input_ids"][i] for i in non_zero_idx]
         return tokenizer.decode(token_ids)
     else:
         raise NotImplementedError("posmap must be 1-dim")
```

### Comparing `rf_groundingdino-0.1.2/groundingdino/util/visualizer.py` & `rf_groundingdino-0.2.0/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/groundingdino/util/vl_utils.py` & `rf_groundingdino-0.2.0/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `rf_groundingdino-0.1.2/rf_groundingdino.egg-info/PKG-INFO` & `rf_groundingdino-0.2.0/rf_groundingdino.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rf-groundingdino
-Version: 0.1.2
+Version: 0.2.0
 Summary: open-set object detector
 Home-page: https://github.com/roboflow/GroundingDINO
 Author: International Digital Economy Academy, Shilong Liu
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -188,15 +188,15 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright 2020 - present, Facebook, Inc
+           Copyright 2023 - present, IDEA Research.
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
@@ -204,70 +204,101 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: transformers
+Requires-Dist: addict
+Requires-Dist: yapf
+Requires-Dist: timm
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: supervision
+Requires-Dist: pycocotools
+
+<div align="center">
+  <img src="./.asset/grounding_dino_logo.png" width="30%">
+</div>
 
-# :sauropod: Grounding DINO
+# :sauropod: Grounding DINO 
 
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/zero-shot-object-detection-on-mscoco)](https://paperswithcode.com/sota/zero-shot-object-detection-on-mscoco?p=grounding-dino-marrying-dino-with-grounded) [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/zero-shot-object-detection-on-odinw)](https://paperswithcode.com/sota/zero-shot-object-detection-on-odinw?p=grounding-dino-marrying-dino-with-grounded) \
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/object-detection-on-coco-minival)](https://paperswithcode.com/sota/object-detection-on-coco-minival?p=grounding-dino-marrying-dino-with-grounded) [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/object-detection-on-coco)](https://paperswithcode.com/sota/object-detection-on-coco?p=grounding-dino-marrying-dino-with-grounded)
-[![image](https://img.shields.io/pypi/v/rf_groundingdino.svg)](https://pypi.python.org/pypi/rf_groundingdino)
 
-Official PyTorch implementation of ["Grounding DINO: Marrying DINO with Grounded Pre-Training for Open-Set Object Detection"](https://arxiv.org/abs/2303.05499): the SoTA open-set object detector.
+
+**[IDEA-CVR, IDEA-Research](https://github.com/IDEA-Research)** 
+
+[Shilong Liu](http://www.lsl.zone/), [Zhaoyang Zeng](https://scholar.google.com/citations?user=U_cvvUwAAAAJ&hl=zh-CN&oi=ao), [Tianhe Ren](https://rentainhe.github.io/), [Feng Li](https://scholar.google.com/citations?user=ybRe9GcAAAAJ&hl=zh-CN), [Hao Zhang](https://scholar.google.com/citations?user=B8hPxMQAAAAJ&hl=zh-CN), [Jie Yang](https://github.com/yangjie-cv), [Chunyuan Li](https://scholar.google.com/citations?user=Zd7WmXUAAAAJ&hl=zh-CN&oi=ao), [Jianwei Yang](https://jwyang.github.io/), [Hang Su](https://scholar.google.com/citations?hl=en&user=dxN1_X0AAAAJ&view_op=list_works&sortby=pubdate), [Jun Zhu](https://scholar.google.com/citations?hl=en&user=axsP38wAAAAJ), [Lei Zhang](https://www.leizhang.org/)<sup>:email:</sup>.
+
+
+[[`Paper`](https://arxiv.org/abs/2303.05499)] [[`Demo`](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo)] [[`BibTex`](#black_nib-citation)]
+
+
+PyTorch implementation and pretrained models for Grounding DINO. For details, see the paper **[Grounding DINO: Marrying DINO with Grounded Pre-Training for Open-Set Object Detection](https://arxiv.org/abs/2303.05499)**.
 
 ## :sun_with_face: Helpful Tutorial
 
 - :grapes: [[Read our arXiv Paper](https://arxiv.org/abs/2303.05499)]
-- :apple: [[Watch our simple introduction video on YouTube](https://youtu.be/wxWDt5UiwY8)]
-- :rose: &nbsp;[[Try the Colab Demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb)]
+- :apple:  [[Watch our simple introduction video on YouTube](https://youtu.be/wxWDt5UiwY8)]
+- :blossom:   &nbsp;[[Try the Colab Demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb)]
 - :sunflower: [[Try our Official Huggingface Demo](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo)]
 - :maple_leaf: [[Watch the Step by Step Tutorial about GroundingDINO by Roboflow AI](https://youtu.be/cMa77r3YrDk)]
 - :mushroom: [[GroundingDINO: Automated Dataset Annotation and Evaluation by Roboflow AI](https://youtu.be/C4NqaRBz_Kw)]
 - :hibiscus: [[Accelerate Image Annotation with SAM and GroundingDINO by Roboflow AI](https://youtu.be/oEQYStnF2l8)]
+- :white_flower: [[Autodistill: Train YOLOv8 with ZERO Annotations based on Grounding-DINO and Grounded-SAM by Roboflow AI](https://github.com/autodistill/autodistill)]
 
-<!-- Grounding DINO Methods |
-[![arXiv](https://img.shields.io/badge/arXiv-2303.05499-b31b1b.svg)](https://arxiv.org/abs/2303.05499)
+<!-- Grounding DINO Methods | 
+[![arXiv](https://img.shields.io/badge/arXiv-2303.05499-b31b1b.svg)](https://arxiv.org/abs/2303.05499) 
 [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/wxWDt5UiwY8) -->
 
 <!-- Grounding DINO Demos |
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb) -->
 <!-- [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/cMa77r3YrDk)
 [![HuggingFace space](https://img.shields.io/badge/🤗-HuggingFace%20Space-cyan.svg)](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo)
 [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/oEQYStnF2l8)
 [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/C4NqaRBz_Kw) -->
 
 ## :sparkles: Highlight Projects
 
+- [Semantic-SAM: a universal image segmentation model to enable segment and recognize anything at any desired granularity.](https://github.com/UX-Decoder/Semantic-SAM), 
 - [DetGPT: Detect What You Need via Reasoning](https://github.com/OptimalScale/DetGPT)
 - [Grounded-SAM: Marrying Grounding DINO with Segment Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything)
 - [Grounding DINO with Stable Diffusion](demo/image_editing_with_groundingdino_stablediffusion.ipynb)
 - [Grounding DINO with GLIGEN for Controllable Image Editing](demo/image_editing_with_groundingdino_gligen.ipynb)
 - [OpenSeeD: A Simple and Strong Openset Segmentation Model](https://github.com/IDEA-Research/OpenSeeD)
 - [SEEM: Segment Everything Everywhere All at Once](https://github.com/UX-Decoder/Segment-Everything-Everywhere-All-At-Once)
 - [X-GPT: Conversational Visual Agent supported by X-Decoder](https://github.com/microsoft/X-Decoder/tree/xgpt)
 - [GLIGEN: Open-Set Grounded Text-to-Image Generation](https://github.com/gligen/GLIGEN)
 - [LLaVA: Large Language and Vision Assistant](https://github.com/haotian-liu/LLaVA)
 
 <!-- Extensions | [Grounding DINO with Segment Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything); [Grounding DINO with Stable Diffusion](demo/image_editing_with_groundingdino_stablediffusion.ipynb); [Grounding DINO with GLIGEN](demo/image_editing_with_groundingdino_gligen.ipynb)  -->
 
+
+
 <!-- Official PyTorch implementation of [Grounding DINO](https://arxiv.org/abs/2303.05499), a stronger open-set object detector. Code is available now! -->
 
+
 ## :bulb: Highlight
 
 - **Open-Set Detection.** Detect **everything** with language!
 - **High Performancce.** COCO zero-shot **52.5 AP** (training without COCO data!). COCO fine-tune **63.0 AP**.
 - **Flexible.** Collaboration with Stable Diffusion for Image Editting.
 
-## :fire: News
 
+
+
+## :fire: News
+- **`2023/07/18`**: We release [Semantic-SAM](https://github.com/UX-Decoder/Semantic-SAM), a universal image segmentation model to enable segment and recognize anything at any desired granularity. **Code** and **checkpoint** are available!
+- **`2023/06/17`**: We provide an example to evaluate Grounding DINO on COCO zero-shot performance.
 - **`2023/04/15`**: Refer to [CV in the Wild Readings](https://github.com/Computer-Vision-in-the-Wild/CVinW_Readings) for those who are interested in open-set recognition!
-- **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN) for more controllable image editings.
+- **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN)  for more controllable image editings.
 - **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_stablediffusion.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) for image editings.
 - **`2023/04/06`**: We build a new demo by marrying GroundingDINO with [Segment-Anything](https://github.com/facebookresearch/segment-anything) named **[Grounded-Segment-Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything)** aims to support segmentation in GroundingDINO.
 - **`2023/03/28`**: A YouTube [video](https://youtu.be/cMa77r3YrDk) about Grounding DINO and basic object detection prompt engineering. [[SkalskiP](https://github.com/SkalskiP)]
 - **`2023/03/28`**: Add a [demo](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo) on Hugging Face Space!
 - **`2023/03/27`**: Support CPU-only mode. Now the model can run on machines without GPUs.
 - **`2023/03/25`**: A [demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb) for Grounding DINO is available at Colab. [[SkalskiP](https://github.com/SkalskiP)]
 - **`2023/03/22`**: Code is available Now!
@@ -279,96 +310,134 @@
  <a href="https://arxiv.org/abs/2303.05499">Paper</a> introduction.
 <img src=".asset/hero_figure.png" alt="ODinW" width="100%">
 Marrying <a href="https://github.com/IDEA-Research/GroundingDINO">Grounding DINO</a> and <a href="https://github.com/gligen/GLIGEN">GLIGEN</a>
 <img src="https://huggingface.co/ShilongLiu/GroundingDINO/resolve/main/GD_GLIGEN.png" alt="gd_gligen" width="100%">
 </details>
 
 ## :star: Explanations/Tips for Grounding DINO Inputs and Outputs
-
 - Grounding DINO accepts an `(image, text)` pair as inputs.
 - It outputs `900` (by default) object boxes. Each box has similarity scores across all input words. (as shown in Figures below.)
 - We defaultly choose the boxes whose highest similarities are higher than a `box_threshold`.
 - We extract the words whose similarities are higher than the `text_threshold` as predicted labels.
-- If you want to obtain objects of specific phrases, like the `dogs` in the sentence `two dogs with a stick.`, you can select the boxes with highest text similarities with `dogs` as final outputs.
+- If you want to obtain objects of specific phrases, like the `dogs` in the sentence `two dogs with a stick.`, you can select the boxes with highest text similarities with `dogs` as final outputs. 
 - Note that each word can be split to **more than one** tokens with different tokenlizers. The number of words in a sentence may not equal to the number of text tokens.
 - We suggest separating different category names with `.` for Grounding DINO.
-  ![model_explain1](.asset/model_explan1.PNG)
-  ![model_explain2](.asset/model_explan2.PNG)
+![model_explain1](.asset/model_explan1.PNG)
+![model_explain2](.asset/model_explan2.PNG)
 
-## :label: TODO
+## :label: TODO 
 
 - [x] Release inference code and demo.
 - [x] Release checkpoints.
 - [x] Grounding DINO with Stable Diffusion and GLIGEN demos.
 - [ ] Release training codes.
 
-## :hammer_and_wrench: Install
+## :hammer_and_wrench: Install 
 
 **Note:**
 
-If you have a CUDA environment, please make sure the environment variable `CUDA_HOME` is set. It will be compiled under CPU-only mode if no CUDA available.
+0. If you have a CUDA environment, please make sure the environment variable `CUDA_HOME` is set. It will be compiled under CPU-only mode if no CUDA available.
 
-**Installation:**
+Please make sure following the installation steps strictly, otherwise the program may produce: 
+```bash
+NameError: name '_C' is not defined
+```
 
-Clone the GroundingDINO repository from GitHub.
+If this happened, please reinstalled the groundingDINO by reclone the git and do all the installation steps again.
+ 
+#### how to check cuda:
+```bash
+echo $CUDA_HOME
+```
+If it print nothing, then it means you haven't set up the path/
 
+Run this so the environment variable will be set under current shell. 
 ```bash
-git clone https://github.com/IDEA-Research/GroundingDINO.git
+export CUDA_HOME=/path/to/cuda-11.3
 ```
 
-Change the current directory to the GroundingDINO folder.
+Notice the version of cuda should be aligned with your CUDA runtime, for there might exists multiple cuda at the same time. 
+
+If you want to set the CUDA_HOME permanently, store it using:
 
 ```bash
-cd GroundingDINO/
+echo 'export CUDA_HOME=/path/to/cuda' >> ~/.bashrc
+```
+after that, source the bashrc file and check CUDA_HOME:
+```bash
+source ~/.bashrc
+echo $CUDA_HOME
 ```
 
-Install the required dependencies in the current directory.
+In this example, /path/to/cuda-11.3 should be replaced with the path where your CUDA toolkit is installed. You can find this by typing **which nvcc** in your terminal:
 
+For instance, 
+if the output is /usr/local/cuda/bin/nvcc, then:
 ```bash
-pip3 install -q -e .
+export CUDA_HOME=/usr/local/cuda
 ```
+**Installation:**
 
-Create a new directory called "weights" to store the model weights.
+1.Clone the GroundingDINO repository from GitHub.
 
 ```bash
-mkdir weights
+git clone https://github.com/IDEA-Research/GroundingDINO.git
 ```
 
-Change the current directory to the "weights" folder.
+2. Change the current directory to the GroundingDINO folder.
 
 ```bash
-cd weights
+cd GroundingDINO/
 ```
 
-Download the model weights file.
+3. Install the required dependencies in the current directory.
 
 ```bash
+pip install -e .
+```
+
+4. Download pre-trained model weights.
+
+```bash
+mkdir weights
+cd weights
 wget -q https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth
+cd ..
 ```
 
 ## :arrow_forward: Demo
-
 Check your GPU ID (only if you're using a GPU)
 
 ```bash
 nvidia-smi
 ```
-
 Replace `{GPU ID}`, `image_you_want_to_detect.jpg`, and `"dir you want to save the output"` with appropriate values in the following command
-
 ```bash
 CUDA_VISIBLE_DEVICES={GPU ID} python demo/inference_on_a_image.py \
--c /GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py \
--p /GroundingDINO/weights/groundingdino_swint_ogc.pth \
+-c groundingdino/config/GroundingDINO_SwinT_OGC.py \
+-p weights/groundingdino_swint_ogc.pth \
 -i image_you_want_to_detect.jpg \
 -o "dir you want to save the output" \
 -t "chair"
  [--cpu-only] # open it for cpu mode
 ```
 
+If you would like to specify the phrases to detect, here is a demo:
+```bash
+CUDA_VISIBLE_DEVICES={GPU ID} python demo/inference_on_a_image.py \
+-c groundingdino/config/GroundingDINO_SwinT_OGC.py \
+-p ./groundingdino_swint_ogc.pth \
+-i .asset/cat_dog.jpeg \
+-o logs/1111 \
+-t "There is a cat and a dog in the image ." \
+--token_spans "[[[9, 10], [11, 14]], [[19, 20], [21, 24]]]"
+ [--cpu-only] # open it for cpu mode
+```
+The token_spans specify the start and end positions of a phrases. For example, the first phrase is `[[9, 10], [11, 14]]`. `"There is a cat and a dog in the image ."[9:10] = 'a'`, `"There is a cat and a dog in the image ."[11:14] = 'cat'`. Hence it refers to the phrase `a cat` . Similarly, the `[[19, 20], [21, 24]]` refers to the phrase `a dog`.
+
 See the `demo/inference_on_a_image.py` for more details.
 
 **Running with Python:**
 
 ```python
 from groundingdino.util.inference import load_model, load_image, predict, annotate
 import cv2
@@ -388,24 +457,37 @@
     box_threshold=BOX_TRESHOLD,
     text_threshold=TEXT_TRESHOLD
 )
 
 annotated_frame = annotate(image_source=image_source, boxes=boxes, logits=logits, phrases=phrases)
 cv2.imwrite("annotated_image.jpg", annotated_frame)
 ```
-
 **Web UI**
 
 We also provide a demo code to integrate Grounding DINO with Gradio Web UI. See the file `demo/gradio_app.py` for more details.
 
 **Notebooks**
 
-- We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN) for more controllable image editings.
+- We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN)  for more controllable image editings.
 - We release [demos](demo/image_editing_with_groundingdino_stablediffusion.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) for image editings.
 
+## COCO Zero-shot Evaluations
+
+We provide an example to evaluate Grounding DINO zero-shot performance on COCO. The results should be **48.5**.
+
+```bash
+CUDA_VISIBLE_DEVICES=0 \
+python demo/test_ap_on_coco.py \
+ -c groundingdino/config/GroundingDINO_SwinT_OGC.py \
+ -p weights/groundingdino_swint_ogc.pth \
+ --anno_path /path/to/annoataions/ie/instances_val2017.json \
+ --image_dir /path/to/imagedir/ie/val2017
+```
+
+
 ## :luggage: Checkpoints
 
 <!-- insert a table -->
 <table>
   <thead>
     <tr style="text-align: right;">
       <th></th>
@@ -430,15 +512,15 @@
     <tr>
       <th>2</th>
       <td>GroundingDINO-B</td>
       <td>Swin-B</td>
       <td>COCO,O365,GoldG,Cap4M,OpenImage,ODinW-35,RefCOCO</td>
       <td>56.7 </td>
       <td><a href="https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha2/groundingdino_swinb_cogcoor.pth">GitHub link</a>  | <a href="https://huggingface.co/ShilongLiu/GroundingDINO/resolve/main/groundingdino_swinb_cogcoor.pth">HF link</a> 
-      <td><a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/groundingdino/config/GroundingDINO_SwinB.cfg.py">link</a></td>
+      <td><a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/groundingdino/config/GroundingDINO_SwinB_cfg.py">link</a></td>
     </tr>
   </tbody>
 </table>
 
 ## :medal_military: Results
 
 <details open>
@@ -459,41 +541,48 @@
 <summary><font size="4">
 Marrying Grounding DINO with <a href="https://github.com/Stability-AI/StableDiffusion">Stable Diffusion</a> for Image Editing
 </font></summary>
 See our example <a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/demo/image_editing_with_groundingdino_stablediffusion.ipynb">notebook</a> for more details.
 <img src=".asset/GD_SD.png" alt="GD_SD" width="100%">
 </details>
 
+
 <details open>
 <summary><font size="4">
 Marrying Grounding DINO with <a href="https://github.com/gligen/GLIGEN">GLIGEN</a> for more Detailed Image Editing.
 </font></summary>
 See our example <a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/demo/image_editing_with_groundingdino_gligen.ipynb">notebook</a> for more details.
 <img src=".asset/GD_GLIGEN.png" alt="GD_GLIGEN" width="100%">
 </details>
 
 ## :sauropod: Model: Grounding DINO
 
 Includes: a text backbone, an image backbone, a feature enhancer, a language-guided query selection, and a cross-modality decoder.
 
 ![arch](.asset/arch.png)
 
+
 ## :hearts: Acknowledgement
 
 Our model is related to [DINO](https://github.com/IDEA-Research/DINO) and [GLIP](https://github.com/microsoft/GLIP). Thanks for their great work!
 
 We also thank great previous work including DETR, Deformable DETR, SMCA, Conditional DETR, Anchor DETR, Dynamic DETR, DAB-DETR, DN-DETR, etc. More related work are available at [Awesome Detection Transformer](https://github.com/IDEACVR/awesome-detection-transformer). A new toolbox [detrex](https://github.com/IDEA-Research/detrex) is available as well.
 
 Thanks [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) and [GLIGEN](https://github.com/gligen/GLIGEN) for their awesome models.
 
+
 ## :black_nib: Citation
 
-If you find our work helpful for your research, please consider citing the following BibTeX entry.
+If you find our work helpful for your research, please consider citing the following BibTeX entry.   
 
 ```bibtex
 @article{liu2023grounding,
   title={Grounding dino: Marrying dino with grounded pre-training for open-set object detection},
   author={Liu, Shilong and Zeng, Zhaoyang and Ren, Tianhe and Li, Feng and Zhang, Hao and Yang, Jie and Li, Chunyuan and Yang, Jianwei and Su, Hang and Zhu, Jun and others},
   journal={arXiv preprint arXiv:2303.05499},
   year={2023}
 }
 ```
+
+
+
+
```

### Comparing `rf_groundingdino-0.1.2/rf_groundingdino.egg-info/SOURCES.txt` & `rf_groundingdino-0.2.0/rf_groundingdino.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 groundingdino/__init__.py
-groundingdino/version.py
 groundingdino/config/GroundingDINO_SwinB_cfg.py
 groundingdino/config/GroundingDINO_SwinT_OGC.py
 groundingdino/config/__init__.py
 groundingdino/datasets/__init__.py
+groundingdino/datasets/cocogrounding_eval.py
 groundingdino/datasets/transforms.py
 groundingdino/models/__init__.py
 groundingdino/models/registry.py
 groundingdino/models/GroundingDINO/__init__.py
 groundingdino/models/GroundingDINO/bertwarper.py
 groundingdino/models/GroundingDINO/fuse_modules.py
 groundingdino/models/GroundingDINO/groundingdino.py
```

### Comparing `rf_groundingdino-0.1.2/setup.py` & `rf_groundingdino-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,27 @@
 # https://github.com/Oneflow-Inc/libai/blob/main/setup.py
 # ------------------------------------------------------------------------------------------------
 
 import glob
 import os
 import subprocess
 
-# import torch
+import subprocess
+import sys
+
+def install_torch():
+    try:
+        import torch
+    except ImportError:
+        subprocess.check_call([sys.executable, "-m", "pip", "install", "torch"])
+
+# Call the function to ensure torch is installed
+install_torch()
+
+import torch
 from setuptools import find_packages, setup
 # from torch.utils.cpp_extension import CUDA_HOME, CppExtension, CUDAExtension
 
 # groundingdino version info
 with open('groundingdino/__init__.py') as f:
     lines = f.readlines()
 
@@ -195,15 +207,15 @@
     with open("LICENSE", "r", encoding="utf-8") as f:
         license = f.read()
 
     write_version_file()
 
     setup(
         name="rf_groundingdino",
-        version='0.1.2',
+        version='0.2.0',
         author="International Digital Economy Academy, Shilong Liu",
         url="https://github.com/roboflow/GroundingDINO",
         description="open-set object detector",
         license=license,
         install_requires=parse_requirements("requirements.txt"),
         packages=find_packages(
             exclude=(
```

