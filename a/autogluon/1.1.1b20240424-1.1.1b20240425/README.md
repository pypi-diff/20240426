# Comparing `tmp/autogluon-1.1.1b20240424.tar.gz` & `tmp/autogluon-1.1.1b20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.1.1b20240424.tar", last modified: Wed Apr 24 09:05:30 2024, max compression
+gzip compressed data, was "autogluon-1.1.1b20240425.tar", last modified: Thu Apr 25 09:05:47 2024, max compression
```

## Comparing `autogluon-1.1.1b20240424.tar` & `autogluon-1.1.1b20240425.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:05:30.706704 autogluon-1.1.1b20240424/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-24 09:05:30.706704 autogluon-1.1.1b20240424/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:05:30.706704 autogluon-1.1.1b20240424/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-24 09:03:44.000000 autogluon-1.1.1b20240424/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:05:30.702704 autogluon-1.1.1b20240424/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:05:30.702704 autogluon-1.1.1b20240424/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:05:30.702704 autogluon-1.1.1b20240424/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:03:44.000000 autogluon-1.1.1b20240424/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:05:30.702704 autogluon-1.1.1b20240424/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:05:30.000000 autogluon-1.1.1b20240424/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:05:47.065579 autogluon-1.1.1b20240425/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-25 09:05:47.065579 autogluon-1.1.1b20240425/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:05:47.065579 autogluon-1.1.1b20240425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-25 09:03:58.000000 autogluon-1.1.1b20240425/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:05:47.061579 autogluon-1.1.1b20240425/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:05:47.061579 autogluon-1.1.1b20240425/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:05:47.061579 autogluon-1.1.1b20240425/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:03:58.000000 autogluon-1.1.1b20240425/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:05:47.061579 autogluon-1.1.1b20240425/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-25 09:05:47.000000 autogluon-1.1.1b20240425/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-25 09:05:47.000000 autogluon-1.1.1b20240425/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:05:47.000000 autogluon-1.1.1b20240425/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 09:05:47.000000 autogluon-1.1.1b20240425/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-25 09:05:47.000000 autogluon-1.1.1b20240425/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 09:05:47.000000 autogluon-1.1.1b20240425/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:05:47.000000 autogluon-1.1.1b20240425/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.1.1b20240424/PKG-INFO` & `autogluon-1.1.1b20240425/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240424
+Version: 1.1.1b20240425
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-1.1.1b20240424/setup.py` & `autogluon-1.1.1b20240425/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.1.1b20240424/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.1.1b20240425/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240424
+Version: 1.1.1b20240425
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

