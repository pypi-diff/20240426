# Comparing `tmp/neon-tts-plugin-coqui-0.8.0.tar.gz` & `tmp/neon-tts-plugin-coqui-0.8.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-tts-plugin-coqui-0.8.0.tar", last modified: Fri Feb 23 18:59:14 2024, max compression
+gzip compressed data, was "neon-tts-plugin-coqui-0.8.1a1.tar", last modified: Fri Apr 26 01:10:15 2024, max compression
```

## Comparing `neon-tts-plugin-coqui-0.8.0.tar` & `neon-tts-plugin-coqui-0.8.1a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:59:14.911822 neon-tts-plugin-coqui-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-23 18:59:08.000000 neon-tts-plugin-coqui-0.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-02-23 18:59:14.911822 neon-tts-plugin-coqui-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-02-23 18:59:08.000000 neon-tts-plugin-coqui-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:59:14.911822 neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui/
--rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-02-23 18:59:08.000000 neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-02-23 18:59:08.000000 neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:59:14.911822 neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-02-23 18:59:14.000000 neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-23 18:59:14.000000 neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 18:59:14.000000 neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-23 18:59:14.000000 neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-23 18:59:14.000000 neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-23 18:59:14.000000 neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 18:59:14.000000 neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 18:59:14.911822 neon-tts-plugin-coqui-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-02-23 18:59:08.000000 neon-tts-plugin-coqui-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:10:15.646724 neon-tts-plugin-coqui-0.8.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-26 01:10:07.000000 neon-tts-plugin-coqui-0.8.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-26 01:10:15.646724 neon-tts-plugin-coqui-0.8.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-26 01:10:07.000000 neon-tts-plugin-coqui-0.8.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:10:15.646724 neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui/
+-rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-04-26 01:10:07.000000 neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-04-26 01:10:07.000000 neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:10:15.646724 neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-26 01:10:15.000000 neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-26 01:10:15.000000 neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:10:15.000000 neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-26 01:10:15.000000 neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-26 01:10:15.000000 neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 01:10:15.000000 neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:10:15.000000 neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 01:10:15.646724 neon-tts-plugin-coqui-0.8.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-26 01:10:07.000000 neon-tts-plugin-coqui-0.8.1a1/setup.py
```

### Comparing `neon-tts-plugin-coqui-0.8.0/LICENSE.md` & `neon-tts-plugin-coqui-0.8.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-0.8.0/PKG-INFO` & `neon-tts-plugin-coqui-0.8.1a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui
-Version: 0.8.0
+Version: 0.8.1a1
 Summary: A Coqui AI TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin tts
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-tts-plugin-coqui-0.8.0/README.md` & `neon-tts-plugin-coqui-0.8.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui/__init__.py` & `neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui/configs.py` & `neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui/configs.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-0.8.0/neon_tts_plugin_coqui.egg-info/PKG-INFO` & `neon-tts-plugin-coqui-0.8.1a1/neon_tts_plugin_coqui.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui
-Version: 0.8.0
+Version: 0.8.1a1
 Summary: A Coqui AI TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin tts
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-tts-plugin-coqui-0.8.0/setup.py` & `neon-tts-plugin-coqui-0.8.1a1/setup.py`

 * *Files identical despite different names*

