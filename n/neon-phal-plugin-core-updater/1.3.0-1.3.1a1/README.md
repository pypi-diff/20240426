# Comparing `tmp/neon-phal-plugin-core-updater-1.3.0.tar.gz` & `tmp/neon-phal-plugin-core-updater-1.3.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-core-updater-1.3.0.tar", last modified: Tue Sep  5 22:32:07 2023, max compression
+gzip compressed data, was "neon-phal-plugin-core-updater-1.3.1a1.tar", last modified: Fri Apr 26 00:44:21 2024, max compression
```

## Comparing `neon-phal-plugin-core-updater-1.3.0.tar` & `neon-phal-plugin-core-updater-1.3.1a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:32:07.160825 neon-phal-plugin-core-updater-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (999)     1634 2023-09-05 22:32:04.000000 neon-phal-plugin-core-updater-1.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (999)     2227 2023-09-05 22:32:07.160825 neon-phal-plugin-core-updater-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1910 2023-09-05 22:32:04.000000 neon-phal-plugin-core-updater-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:32:07.160825 neon-phal-plugin-core-updater-1.3.0/neon_phal_plugin_core_updater/
--rw-r--r--   0 runner    (1001) docker     (999)     9403 2023-09-05 22:32:04.000000 neon-phal-plugin-core-updater-1.3.0/neon_phal_plugin_core_updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:32:07.160825 neon-phal-plugin-core-updater-1.3.0/neon_phal_plugin_core_updater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2227 2023-09-05 22:32:07.000000 neon-phal-plugin-core-updater-1.3.0/neon_phal_plugin_core_updater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      391 2023-09-05 22:32:07.000000 neon-phal-plugin-core-updater-1.3.0/neon_phal_plugin_core_updater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-05 22:32:07.000000 neon-phal-plugin-core-updater-1.3.0/neon_phal_plugin_core_updater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       99 2023-09-05 22:32:07.000000 neon-phal-plugin-core-updater-1.3.0/neon_phal_plugin_core_updater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       95 2023-09-05 22:32:07.000000 neon-phal-plugin-core-updater-1.3.0/neon_phal_plugin_core_updater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       30 2023-09-05 22:32:07.000000 neon-phal-plugin-core-updater-1.3.0/neon_phal_plugin_core_updater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-05 22:32:07.160825 neon-phal-plugin-core-updater-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     3369 2023-09-05 22:32:04.000000 neon-phal-plugin-core-updater-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:44:21.523465 neon-phal-plugin-core-updater-1.3.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-26 00:44:14.000000 neon-phal-plugin-core-updater-1.3.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-26 00:44:21.523465 neon-phal-plugin-core-updater-1.3.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 00:44:14.000000 neon-phal-plugin-core-updater-1.3.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:44:21.523465 neon-phal-plugin-core-updater-1.3.1a1/neon_phal_plugin_core_updater/
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-04-26 00:44:14.000000 neon-phal-plugin-core-updater-1.3.1a1/neon_phal_plugin_core_updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:44:21.523465 neon-phal-plugin-core-updater-1.3.1a1/neon_phal_plugin_core_updater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-26 00:44:21.000000 neon-phal-plugin-core-updater-1.3.1a1/neon_phal_plugin_core_updater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-26 00:44:21.000000 neon-phal-plugin-core-updater-1.3.1a1/neon_phal_plugin_core_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 00:44:21.000000 neon-phal-plugin-core-updater-1.3.1a1/neon_phal_plugin_core_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-26 00:44:21.000000 neon-phal-plugin-core-updater-1.3.1a1/neon_phal_plugin_core_updater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-26 00:44:21.000000 neon-phal-plugin-core-updater-1.3.1a1/neon_phal_plugin_core_updater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 00:44:21.000000 neon-phal-plugin-core-updater-1.3.1a1/neon_phal_plugin_core_updater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 00:44:21.523465 neon-phal-plugin-core-updater-1.3.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-26 00:44:14.000000 neon-phal-plugin-core-updater-1.3.1a1/setup.py
```

### Comparing `neon-phal-plugin-core-updater-1.3.0/LICENSE.md` & `neon-phal-plugin-core-updater-1.3.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-core-updater-1.3.0/PKG-INFO` & `neon-phal-plugin-core-updater-1.3.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.3.0
+Version: 1.3.1a1
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-core-updater-1.3.0/README.md` & `neon-phal-plugin-core-updater-1.3.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-core-updater-1.3.0/neon_phal_plugin_core_updater/__init__.py` & `neon-phal-plugin-core-updater-1.3.1a1/neon_phal_plugin_core_updater/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-core-updater-1.3.0/neon_phal_plugin_core_updater.egg-info/PKG-INFO` & `neon-phal-plugin-core-updater-1.3.1a1/neon_phal_plugin_core_updater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.3.0
+Version: 1.3.1a1
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-core-updater-1.3.0/setup.py` & `neon-phal-plugin-core-updater-1.3.1a1/setup.py`

 * *Files identical despite different names*

