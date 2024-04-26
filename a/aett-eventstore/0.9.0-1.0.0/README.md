# Comparing `tmp/aett_eventstore-0.9.0.tar.gz` & `tmp/aett_eventstore-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_eventstore-0.9.0.tar", last modified: Mon Apr 22 13:59:29 2024, max compression
+gzip compressed data, was "aett_eventstore-1.0.0.tar", last modified: Fri Apr 26 16:18:53 2024, max compression
```

## Comparing `aett_eventstore-0.9.0.tar` & `aett_eventstore-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:29.527779 aett_eventstore-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 13:59:19.000000 aett_eventstore-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 13:59:19.000000 aett_eventstore-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-22 13:59:29.527779 aett_eventstore-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-22 13:59:19.000000 aett_eventstore-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-22 13:59:19.000000 aett_eventstore-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:59:29.527779 aett_eventstore-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:29.523779 aett_eventstore-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:29.523779 aett_eventstore-0.9.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:29.523779 aett_eventstore-0.9.0/src/aett/eventstore/
--rw-r--r--   0 runner    (1001) docker     (127)    16203 2024-04-22 13:59:19.000000 aett_eventstore-0.9.0/src/aett/eventstore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:29.523779 aett_eventstore-0.9.0/src/aett_eventstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-22 13:59:29.000000 aett_eventstore-0.9.0/src/aett_eventstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-22 13:59:29.000000 aett_eventstore-0.9.0/src/aett_eventstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:59:29.000000 aett_eventstore-0.9.0/src/aett_eventstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 13:59:29.000000 aett_eventstore-0.9.0/src/aett_eventstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 13:59:29.000000 aett_eventstore-0.9.0/src/aett_eventstore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:29.523779 aett_eventstore-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-22 13:59:19.000000 aett_eventstore-0.9.0/tests/test_EventStream.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-22 13:59:19.000000 aett_eventstore-0.9.0/tests/test_Memento.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-22 13:59:19.000000 aett_eventstore-0.9.0/tests/test_Serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-22 13:59:19.000000 aett_eventstore-0.9.0/tests/test_Topics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.555541 aett_eventstore-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-26 16:18:53.555541 aett_eventstore-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:53.555541 aett_eventstore-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.551541 aett_eventstore-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.551541 aett_eventstore-1.0.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.551541 aett_eventstore-1.0.0/src/aett/eventstore/
+-rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/src/aett/eventstore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.551541 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-26 16:18:53.000000 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-26 16:18:53.000000 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:53.000000 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 16:18:53.000000 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:53.000000 aett_eventstore-1.0.0/src/aett_eventstore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:53.551541 aett_eventstore-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/tests/test_Memento.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/tests/test_Serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-26 16:18:48.000000 aett_eventstore-1.0.0/tests/test_Topics.py
```

### Comparing `aett_eventstore-0.9.0/LICENSE` & `aett_eventstore-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_eventstore-0.9.0/PKG-INFO` & `aett_eventstore-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-eventstore
-Version: 0.9.0
+Version: 1.0.0
 Summary: Event store for Python
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aett_eventstore-0.9.0/README.md` & `aett_eventstore-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_eventstore-0.9.0/pyproject.toml` & `aett_eventstore-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-# pyproject.toml
-
 [build-system]
-requires = ["setuptools>=69.1.1", "wheel"]
+requires = ["setuptools>=69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.eventstore"]
 
 [project]
 name = "aett-eventstore"
-version = "0.9.0"
+version = "1.0.0"
 description = "Event store for Python"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `aett_eventstore-0.9.0/src/aett_eventstore.egg-info/PKG-INFO` & `aett_eventstore-1.0.0/src/aett_eventstore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-eventstore
-Version: 0.9.0
+Version: 1.0.0
 Summary: Event store for Python
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aett_eventstore-0.9.0/tests/test_Topics.py` & `aett_eventstore-1.0.0/tests/test_Topics.py`

 * *Files identical despite different names*

