# Comparing `tmp/huckle-3.3.4.tar.gz` & `tmp/huckle-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huckle-3.3.4.tar", last modified: Mon Apr  8 00:31:34 2024, max compression
+gzip compressed data, was "huckle-3.4.0.tar", last modified: Fri Apr 26 03:25:33 2024, max compression
```

## Comparing `huckle-3.3.4.tar` & `huckle-3.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 00:31:34.714063 huckle-3.3.4/
--rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-3.3.4/LICENSE.txt
--rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-3.3.4/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)    10760 2024-04-08 00:31:34.714149 huckle-3.3.4/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)     9892 2024-04-08 00:24:35.000000 huckle-3.3.4/README.rst
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 00:31:34.713104 huckle-3.3.4/huckle/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:06.000000 huckle-3.3.4/huckle/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      885 2024-04-07 23:22:42.000000 huckle-3.3.4/huckle/__main__.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     6054 2024-04-07 23:05:17.000000 huckle-3.3.4/huckle/config.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 00:31:34.713898 huckle-3.3.4/huckle/data/
--rw-r--r--   0 jeff       (501) staff       (20)     3481 2024-04-07 23:05:17.000000 huckle-3.3.4/huckle/data/huckle.1
--rwxr-xr-x   0 jeff       (501) staff       (20)    11484 2024-04-07 23:26:21.000000 huckle-3.3.4/huckle/hclinav.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     4290 2024-04-07 23:05:17.000000 huckle-3.3.4/huckle/huckle.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      850 2024-04-07 23:05:17.000000 huckle-3.3.4/huckle/hutils.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     2955 2023-08-17 01:36:09.000000 huckle-3.3.4/huckle/logger.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      248 2024-04-08 00:21:34.000000 huckle-3.3.4/huckle/package.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-08 00:31:34.713789 huckle-3.3.4/huckle.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)    10760 2024-04-08 00:31:34.000000 huckle-3.3.4/huckle.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      398 2024-04-08 00:31:34.000000 huckle-3.3.4/huckle.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2024-04-08 00:31:34.000000 huckle-3.3.4/huckle.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       48 2024-04-08 00:31:34.000000 huckle-3.3.4/huckle.egg-info/entry_points.txt
--rw-r--r--   0 jeff       (501) staff       (20)       84 2024-04-08 00:31:34.000000 huckle-3.3.4/huckle.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)        7 2024-04-08 00:31:34.000000 huckle-3.3.4/huckle.egg-info/top_level.txt
--rwxr-x---   0 jeff       (501) staff       (20)       67 2024-04-08 00:31:34.714373 huckle-3.3.4/setup.cfg
--rw-r--r--   0 jeff       (501) staff       (20)     3335 2024-04-07 23:05:17.000000 huckle-3.3.4/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-26 03:25:33.235872 huckle-3.4.0/
+-rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-3.4.0/LICENSE.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-3.4.0/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)    10753 2024-04-26 03:25:33.235967 huckle-3.4.0/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)     9885 2024-04-26 02:48:09.000000 huckle-3.4.0/README.rst
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-26 03:25:33.234537 huckle-3.4.0/huckle/
+-rwxr-x---   0 jeff       (501) staff       (20)      463 2024-04-26 03:22:34.000000 huckle-3.4.0/huckle/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      885 2024-04-07 23:22:42.000000 huckle-3.4.0/huckle/__main__.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     6054 2024-04-07 23:05:17.000000 huckle-3.4.0/huckle/config.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-26 03:25:33.235590 huckle-3.4.0/huckle/data/
+-rw-r--r--   0 jeff       (501) staff       (20)     3481 2024-04-07 23:05:17.000000 huckle-3.4.0/huckle/data/huckle.1
+-rwxr-xr-x   0 jeff       (501) staff       (20)    11484 2024-04-07 23:26:21.000000 huckle-3.4.0/huckle/hclinav.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     4290 2024-04-26 03:07:06.000000 huckle-3.4.0/huckle/huckle.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      850 2024-04-07 23:05:17.000000 huckle-3.4.0/huckle/hutils.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     2955 2023-08-17 01:36:09.000000 huckle-3.4.0/huckle/logger.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      248 2024-04-26 02:44:25.000000 huckle-3.4.0/huckle/package.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-26 03:25:33.235471 huckle-3.4.0/huckle.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)    10753 2024-04-26 03:25:33.000000 huckle-3.4.0/huckle.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      398 2024-04-26 03:25:33.000000 huckle-3.4.0/huckle.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2024-04-26 03:25:33.000000 huckle-3.4.0/huckle.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       48 2024-04-26 03:25:33.000000 huckle-3.4.0/huckle.egg-info/entry_points.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       84 2024-04-26 03:25:33.000000 huckle-3.4.0/huckle.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        7 2024-04-26 03:25:33.000000 huckle-3.4.0/huckle.egg-info/top_level.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       67 2024-04-26 03:25:33.236250 huckle-3.4.0/setup.cfg
+-rw-r--r--   0 jeff       (501) staff       (20)     3335 2024-04-07 23:05:17.000000 huckle-3.4.0/setup.py
```

### Comparing `huckle-3.3.4/LICENSE.txt` & `huckle-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `huckle-3.3.4/PKG-INFO` & `huckle-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huckle
-Version: 3.3.4
+Version: 3.4.0
 Summary: A CLI, and python library, that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/huckle
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -124,15 +124,15 @@
 
     import flask
     import config
     import json
     import logger
     import io
 
-    from huckle.huckle import cli, stdin
+    from huckle import cli, stdin
     from flask import Flask, render_template, send_file, jsonify, Response
 
     logging = logger.Logger()
     logging.setLevel(logger.INFO)
 
 
     def webapp():
```

### Comparing `huckle-3.3.4/README.rst` & `huckle-3.4.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     import flask
     import config
     import json
     import logger
     import io
 
-    from huckle.huckle import cli, stdin
+    from huckle import cli, stdin
     from flask import Flask, render_template, send_file, jsonify, Response
 
     logging = logger.Logger()
     logging.setLevel(logger.INFO)
 
 
     def webapp():
```

### Comparing `huckle-3.3.4/huckle/__main__.py` & `huckle-3.4.0/huckle/__main__.py`

 * *Files identical despite different names*

### Comparing `huckle-3.3.4/huckle/config.py` & `huckle-3.4.0/huckle/config.py`

 * *Files identical despite different names*

### Comparing `huckle-3.3.4/huckle/data/huckle.1` & `huckle-3.4.0/huckle/data/huckle.1`

 * *Files identical despite different names*

### Comparing `huckle-3.3.4/huckle/hclinav.py` & `huckle-3.4.0/huckle/hclinav.py`

 * *Files identical despite different names*

### Comparing `huckle-3.3.4/huckle/huckle.py` & `huckle-3.4.0/huckle/huckle.py`

 * *Files identical despite different names*

### Comparing `huckle-3.3.4/huckle/hutils.py` & `huckle-3.4.0/huckle/hutils.py`

 * *Files identical despite different names*

### Comparing `huckle-3.3.4/huckle/logger.py` & `huckle-3.4.0/huckle/logger.py`

 * *Files identical despite different names*

### Comparing `huckle-3.3.4/huckle.egg-info/PKG-INFO` & `huckle-3.4.0/huckle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huckle
-Version: 3.3.4
+Version: 3.4.0
 Summary: A CLI, and python library, that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/huckle
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -124,15 +124,15 @@
 
     import flask
     import config
     import json
     import logger
     import io
 
-    from huckle.huckle import cli, stdin
+    from huckle import cli, stdin
     from flask import Flask, render_template, send_file, jsonify, Response
 
     logging = logger.Logger()
     logging.setLevel(logger.INFO)
 
 
     def webapp():
```

### Comparing `huckle-3.3.4/setup.py` & `huckle-3.4.0/setup.py`

 * *Files identical despite different names*

