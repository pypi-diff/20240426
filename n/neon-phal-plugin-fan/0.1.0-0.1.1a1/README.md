# Comparing `tmp/neon-phal-plugin-fan-0.1.0.tar.gz` & `tmp/neon-phal-plugin-fan-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-fan-0.1.0.tar", last modified: Tue Sep  5 22:32:43 2023, max compression
+gzip compressed data, was "neon-phal-plugin-fan-0.1.1a1.tar", last modified: Fri Apr 26 00:42:19 2024, max compression
```

## Comparing `neon-phal-plugin-fan-0.1.0.tar` & `neon-phal-plugin-fan-0.1.1a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:32:43.508987 neon-phal-plugin-fan-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (999)     1634 2023-09-05 22:32:39.000000 neon-phal-plugin-fan-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (999)      546 2023-09-05 22:32:43.508987 neon-phal-plugin-fan-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      254 2023-09-05 22:32:39.000000 neon-phal-plugin-fan-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:32:43.508987 neon-phal-plugin-fan-0.1.0/neon_phal_plugin_fan/
--rw-r--r--   0 runner    (1001) docker     (999)     5283 2023-09-05 22:32:39.000000 neon-phal-plugin-fan-0.1.0/neon_phal_plugin_fan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:32:43.508987 neon-phal-plugin-fan-0.1.0/neon_phal_plugin_fan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      546 2023-09-05 22:32:43.000000 neon-phal-plugin-fan-0.1.0/neon_phal_plugin_fan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      328 2023-09-05 22:32:43.000000 neon-phal-plugin-fan-0.1.0/neon_phal_plugin_fan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-05 22:32:43.000000 neon-phal-plugin-fan-0.1.0/neon_phal_plugin_fan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       75 2023-09-05 22:32:43.000000 neon-phal-plugin-fan-0.1.0/neon_phal_plugin_fan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       70 2023-09-05 22:32:43.000000 neon-phal-plugin-fan-0.1.0/neon_phal_plugin_fan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       21 2023-09-05 22:32:43.000000 neon-phal-plugin-fan-0.1.0/neon_phal_plugin_fan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-05 22:32:43.508987 neon-phal-plugin-fan-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     3778 2023-09-05 22:32:39.000000 neon-phal-plugin-fan-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:42:19.566973 neon-phal-plugin-fan-0.1.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-26 00:42:16.000000 neon-phal-plugin-fan-0.1.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-26 00:42:19.566973 neon-phal-plugin-fan-0.1.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-26 00:42:16.000000 neon-phal-plugin-fan-0.1.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:42:19.566973 neon-phal-plugin-fan-0.1.1a1/neon_phal_plugin_fan/
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-26 00:42:16.000000 neon-phal-plugin-fan-0.1.1a1/neon_phal_plugin_fan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:42:19.566973 neon-phal-plugin-fan-0.1.1a1/neon_phal_plugin_fan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-26 00:42:19.000000 neon-phal-plugin-fan-0.1.1a1/neon_phal_plugin_fan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-26 00:42:19.000000 neon-phal-plugin-fan-0.1.1a1/neon_phal_plugin_fan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 00:42:19.000000 neon-phal-plugin-fan-0.1.1a1/neon_phal_plugin_fan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 00:42:19.000000 neon-phal-plugin-fan-0.1.1a1/neon_phal_plugin_fan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-26 00:42:19.000000 neon-phal-plugin-fan-0.1.1a1/neon_phal_plugin_fan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-26 00:42:19.000000 neon-phal-plugin-fan-0.1.1a1/neon_phal_plugin_fan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 00:42:19.566973 neon-phal-plugin-fan-0.1.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-26 00:42:16.000000 neon-phal-plugin-fan-0.1.1a1/setup.py
```

### Comparing `neon-phal-plugin-fan-0.1.0/LICENSE.md` & `neon-phal-plugin-fan-0.1.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-fan-0.1.0/PKG-INFO` & `neon-phal-plugin-fan-0.1.1a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-fan
-Version: 0.1.0
+Version: 0.1.1a1
 Summary: Fan Control Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-fan
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-fan-0.1.0/neon_phal_plugin_fan/__init__.py` & `neon-phal-plugin-fan-0.1.1a1/neon_phal_plugin_fan/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-fan-0.1.0/neon_phal_plugin_fan.egg-info/PKG-INFO` & `neon-phal-plugin-fan-0.1.1a1/neon_phal_plugin_fan.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-fan
-Version: 0.1.0
+Version: 0.1.1a1
 Summary: Fan Control Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-fan
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-fan-0.1.0/setup.py` & `neon-phal-plugin-fan-0.1.1a1/setup.py`

 * *Files identical despite different names*

