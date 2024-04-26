# Comparing `tmp/HeraData-0.1.2.tar.gz` & `tmp/HeraData-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HeraData-0.1.2.tar", last modified: Tue Apr 23 06:41:00 2024, max compression
+gzip compressed data, was "HeraData-0.1.3.tar", last modified: Fri Apr 26 11:53:40 2024, max compression
```

## Comparing `HeraData-0.1.2.tar` & `HeraData-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 06:41:00.407394 HeraData-0.1.2/
--rw-rw-r--   0 mark      (1000) mark      (1000)      129 2024-04-23 01:24:54.000000 HeraData-0.1.2/.gitignore
--rw-rw-r--   0 mark      (1000) mark      (1000)      104 2024-04-22 07:50:16.000000 HeraData-0.1.2/.gitmodules
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 06:41:00.407394 HeraData-0.1.2/HeraData.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)      155 2024-04-23 06:41:00.000000 HeraData-0.1.2/HeraData.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      317 2024-04-23 06:41:00.000000 HeraData-0.1.2/HeraData.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 06:41:00.000000 HeraData-0.1.2/HeraData.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       14 2024-04-23 06:41:00.000000 HeraData-0.1.2/HeraData.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-23 06:41:00.000000 HeraData-0.1.2/HeraData.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)      155 2024-04-23 06:41:00.407394 HeraData-0.1.2/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)       35 2024-04-22 09:32:31.000000 HeraData-0.1.2/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 06:41:00.407394 HeraData-0.1.2/hera/
--rw-rw-r--   0 mark      (1000) mark      (1000)      311 2024-04-23 06:10:33.000000 HeraData-0.1.2/hera/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1876 2024-04-23 06:35:10.000000 HeraData-0.1.2/hera/_data_storage.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       21 2024-04-23 02:00:27.000000 HeraData-0.1.2/requirements.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       79 2024-04-23 06:41:00.407394 HeraData-0.1.2/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      377 2024-04-23 06:40:52.000000 HeraData-0.1.2/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 06:41:00.407394 HeraData-0.1.2/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)      811 2024-04-23 06:10:33.000000 HeraData-0.1.2/tests/test___init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1167 2024-04-23 06:11:38.000000 HeraData-0.1.2/tests/test__data_storage.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 11:53:40.014208 HeraData-0.1.3/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      129 2024-04-23 01:24:54.000000 HeraData-0.1.3/.gitignore
+-rw-rw-r--   0 mark      (1000) mark      (1000)      104 2024-04-22 07:50:16.000000 HeraData-0.1.3/.gitmodules
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 11:53:40.014208 HeraData-0.1.3/HeraData.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      155 2024-04-26 11:53:39.000000 HeraData-0.1.3/HeraData.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      295 2024-04-26 11:53:39.000000 HeraData-0.1.3/HeraData.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-26 11:53:39.000000 HeraData-0.1.3/HeraData.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       14 2024-04-26 11:53:39.000000 HeraData-0.1.3/HeraData.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-26 11:53:39.000000 HeraData-0.1.3/HeraData.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)      155 2024-04-26 11:53:40.014208 HeraData-0.1.3/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)       35 2024-04-22 09:32:31.000000 HeraData-0.1.3/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 11:53:40.014208 HeraData-0.1.3/hera/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      629 2024-04-26 11:51:12.000000 HeraData-0.1.3/hera/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       21 2024-04-23 02:00:27.000000 HeraData-0.1.3/requirements.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       79 2024-04-26 11:53:40.014208 HeraData-0.1.3/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      377 2024-04-26 11:51:12.000000 HeraData-0.1.3/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 11:53:40.014208 HeraData-0.1.3/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      811 2024-04-23 06:10:33.000000 HeraData-0.1.3/tests/test___init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1167 2024-04-23 06:11:38.000000 HeraData-0.1.3/tests/test__data_storage.py
```

### Comparing `HeraData-0.1.2/tests/test___init__.py` & `HeraData-0.1.3/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `HeraData-0.1.2/tests/test__data_storage.py` & `HeraData-0.1.3/tests/test__data_storage.py`

 * *Files identical despite different names*

