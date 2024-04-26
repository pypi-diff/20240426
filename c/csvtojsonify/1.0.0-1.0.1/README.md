# Comparing `tmp/csvtojsonify-1.0.0.tar.gz` & `tmp/csvtojsonify-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvtojsonify-1.0.0.tar", last modified: Thu Apr 25 03:53:40 2024, max compression
+gzip compressed data, was "csvtojsonify-1.0.1.tar", last modified: Thu Apr 25 13:45:56 2024, max compression
```

## Comparing `csvtojsonify-1.0.0.tar` & `csvtojsonify-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-25 03:53:40.890680 csvtojsonify-1.0.0/
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)       38 2024-04-25 03:53:17.000000 csvtojsonify-1.0.0/MANIFEST.in
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      225 2024-04-25 03:53:40.890591 csvtojsonify-1.0.0/PKG-INFO
-drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-25 03:53:40.890457 csvtojsonify-1.0.0/csvtojsonify.egg-info/
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      225 2024-04-25 03:53:40.000000 csvtojsonify-1.0.0/csvtojsonify.egg-info/PKG-INFO
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      219 2024-04-25 03:53:40.000000 csvtojsonify-1.0.0/csvtojsonify.egg-info/SOURCES.txt
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)        1 2024-04-25 03:53:40.000000 csvtojsonify-1.0.0/csvtojsonify.egg-info/dependency_links.txt
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)       52 2024-04-25 03:53:40.000000 csvtojsonify-1.0.0/csvtojsonify.egg-info/entry_points.txt
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)       13 2024-04-25 03:53:40.000000 csvtojsonify-1.0.0/csvtojsonify.egg-info/top_level.txt
--rwxr-xr-x   0 sriramsreedhar   (501) staff       (20)      749 2024-04-25 03:20:55.000000 csvtojsonify-1.0.0/csvtojsonify.py
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)       38 2024-04-25 03:53:40.890712 csvtojsonify-1.0.0/setup.cfg
--rw-r--r--   0 sriramsreedhar   (501) staff       (20)      368 2024-04-25 03:53:02.000000 csvtojsonify-1.0.0/setup.py
+drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-25 13:45:56.399991 csvtojsonify-1.0.1/
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      116 2024-04-25 04:37:39.000000 csvtojsonify-1.0.1/MANIFEST.in
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      894 2024-04-25 13:45:56.399806 csvtojsonify-1.0.1/PKG-INFO
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      436 2024-04-25 13:37:57.000000 csvtojsonify-1.0.1/README.md
+drwxr-xr-x   0 sriramsreedhar   (501) staff       (20)        0 2024-04-25 13:45:56.399650 csvtojsonify-1.0.1/csvtojsonify.egg-info/
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      894 2024-04-25 13:45:56.000000 csvtojsonify-1.0.1/csvtojsonify.egg-info/PKG-INFO
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      225 2024-04-25 13:45:56.000000 csvtojsonify-1.0.1/csvtojsonify.egg-info/SOURCES.txt
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)        1 2024-04-25 13:45:56.000000 csvtojsonify-1.0.1/csvtojsonify.egg-info/dependency_links.txt
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)        7 2024-04-25 13:45:56.000000 csvtojsonify-1.0.1/csvtojsonify.egg-info/requires.txt
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)        1 2024-04-25 13:45:56.000000 csvtojsonify-1.0.1/csvtojsonify.egg-info/top_level.txt
+-rwxr-xr-x   0 sriramsreedhar   (501) staff       (20)      749 2024-04-25 03:20:55.000000 csvtojsonify-1.0.1/csvtojsonify.py
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)       38 2024-04-25 13:45:56.400030 csvtojsonify-1.0.1/setup.cfg
+-rw-r--r--   0 sriramsreedhar   (501) staff       (20)      665 2024-04-25 13:33:11.000000 csvtojsonify-1.0.1/setup.py
```

### Comparing `csvtojsonify-1.0.0/csvtojsonify.py` & `csvtojsonify-1.0.1/csvtojsonify.py`

 * *Files identical despite different names*

