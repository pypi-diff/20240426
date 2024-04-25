# Comparing `tmp/gingerai-0.1.8.tar.gz` & `tmp/gingerai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gingerai-0.1.8.tar", last modified: Thu Apr 25 23:27:45 2024, max compression
+gzip compressed data, was "gingerai-0.1.9.tar", last modified: Thu Apr 25 23:34:03 2024, max compression
```

## Comparing `gingerai-0.1.8.tar` & `gingerai-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tranie     (501) staff       (20)        0 2024-04-25 23:27:45.887085 gingerai-0.1.8/
--rw-r--r--   0 tranie     (501) staff       (20)      389 2024-04-25 23:27:45.886749 gingerai-0.1.8/PKG-INFO
--rw-r--r--   0 tranie     (501) staff       (20)        0 2024-04-25 23:27:45.000000 gingerai-0.1.8/README.md
-drwxr-xr-x   0 tranie     (501) staff       (20)        0 2024-04-25 23:27:45.883194 gingerai-0.1.8/gingerai/
--rw-r--r--   0 tranie     (501) staff       (20)     3077 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai/ModelUploader.py
--rw-r--r--   0 tranie     (501) staff       (20)       90 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai/__init__.py
-drwxr-xr-x   0 tranie     (501) staff       (20)        0 2024-04-25 23:27:45.886150 gingerai-0.1.8/gingerai.egg-info/
--rw-r--r--   0 tranie     (501) staff       (20)      389 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai.egg-info/PKG-INFO
--rw-r--r--   0 tranie     (501) staff       (20)      224 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai.egg-info/SOURCES.txt
--rw-r--r--   0 tranie     (501) staff       (20)        1 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai.egg-info/dependency_links.txt
--rw-r--r--   0 tranie     (501) staff       (20)       34 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai.egg-info/requires.txt
--rw-r--r--   0 tranie     (501) staff       (20)        9 2024-04-25 23:27:45.000000 gingerai-0.1.8/gingerai.egg-info/top_level.txt
--rw-r--r--   0 tranie     (501) staff       (20)       38 2024-04-25 23:27:45.887160 gingerai-0.1.8/setup.cfg
--rw-r--r--   0 tranie     (501) staff       (20)      476 2024-04-25 23:27:45.000000 gingerai-0.1.8/setup.py
+drwxr-xr-x   0 tranie     (501) staff       (20)        0 2024-04-25 23:34:03.094480 gingerai-0.1.9/
+-rw-r--r--   0 tranie     (501) staff       (20)      389 2024-04-25 23:34:03.090132 gingerai-0.1.9/PKG-INFO
+-rw-r--r--   0 tranie     (501) staff       (20)        0 2024-04-25 23:34:02.000000 gingerai-0.1.9/README.md
+drwxr-xr-x   0 tranie     (501) staff       (20)        0 2024-04-25 23:34:03.075469 gingerai-0.1.9/gingerai/
+-rw-r--r--   0 tranie     (501) staff       (20)     3077 2024-04-25 23:34:02.000000 gingerai-0.1.9/gingerai/ModelUploader.py
+-rw-r--r--   0 tranie     (501) staff       (20)       91 2024-04-25 23:34:02.000000 gingerai-0.1.9/gingerai/__init__.py
+drwxr-xr-x   0 tranie     (501) staff       (20)        0 2024-04-25 23:34:03.081127 gingerai-0.1.9/gingerai.egg-info/
+-rw-r--r--   0 tranie     (501) staff       (20)      389 2024-04-25 23:34:03.000000 gingerai-0.1.9/gingerai.egg-info/PKG-INFO
+-rw-r--r--   0 tranie     (501) staff       (20)      224 2024-04-25 23:34:03.000000 gingerai-0.1.9/gingerai.egg-info/SOURCES.txt
+-rw-r--r--   0 tranie     (501) staff       (20)        1 2024-04-25 23:34:03.000000 gingerai-0.1.9/gingerai.egg-info/dependency_links.txt
+-rw-r--r--   0 tranie     (501) staff       (20)       34 2024-04-25 23:34:03.000000 gingerai-0.1.9/gingerai.egg-info/requires.txt
+-rw-r--r--   0 tranie     (501) staff       (20)        9 2024-04-25 23:34:03.000000 gingerai-0.1.9/gingerai.egg-info/top_level.txt
+-rw-r--r--   0 tranie     (501) staff       (20)       38 2024-04-25 23:34:03.094575 gingerai-0.1.9/setup.cfg
+-rw-r--r--   0 tranie     (501) staff       (20)      476 2024-04-25 23:34:02.000000 gingerai-0.1.9/setup.py
```

### Comparing `gingerai-0.1.8/gingerai/ModelUploader.py` & `gingerai-0.1.9/gingerai/ModelUploader.py`

 * *Files identical despite different names*

