# Comparing `tmp/progress_api-0.1.0a4.tar.gz` & `tmp/progress_api-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress_api-0.1.0a4.tar", last modified: Thu Apr 25 01:02:01 2024, max compression
+gzip compressed data, was "progress_api-0.1.0a5.tar", last modified: Fri Apr 26 19:38:06 2024, max compression
```

## Comparing `progress_api-0.1.0a4.tar` & `progress_api-0.1.0a5.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.935287 progress_api-0.1.0a4/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-25 01:02:01.935287 progress_api-0.1.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.927286 progress_api-0.1.0a4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/docs/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.927286 progress_api-0.1.0a4/docs/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/docs/backends/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.927286 progress_api-0.1.0a4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.931286 progress_api-0.1.0a4/examples/enlighten/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/.header.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/floats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/ftp_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/multicolored.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/multiple_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/multiprocessing_queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/prefixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.931286 progress_api-0.1.0a4/progress_api/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.931286 progress_api-0.1.0a4/progress_api/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/backends/enlighten.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/backends/null.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/backends/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.931286 progress_api-0.1.0a4/progress_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:02:01.935287 progress_api-0.1.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:38:06.616962 progress_api-0.1.0a5/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-26 19:38:06.616962 progress_api-0.1.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:38:06.608962 progress_api-0.1.0a5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/docs/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:38:06.608962 progress_api-0.1.0a5/docs/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/docs/backends/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:38:06.608962 progress_api-0.1.0a5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:38:06.612962 progress_api-0.1.0a5/examples/enlighten/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/.header.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/floats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/ftp_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/multicolored.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/multiple_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/multiprocessing_queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/enlighten/prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/examples/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:38:06.612962 progress_api-0.1.0a5/progress_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/progress_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/progress_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:38:06.612962 progress_api-0.1.0a5/progress_api/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/progress_api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/progress_api/backends/enlighten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/progress_api/backends/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/progress_api/backends/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/progress_api/backends/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/progress_api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/progress_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/progress_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:38:06.612962 progress_api-0.1.0a5/progress_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-26 19:38:06.000000 progress_api-0.1.0a5/progress_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-26 19:38:06.000000 progress_api-0.1.0a5/progress_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:38:06.000000 progress_api-0.1.0a5/progress_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 19:38:06.000000 progress_api-0.1.0a5/progress_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-26 19:38:06.000000 progress_api-0.1.0a5/progress_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 19:38:06.000000 progress_api-0.1.0a5/progress_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-26 19:38:02.000000 progress_api-0.1.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:38:06.616962 progress_api-0.1.0a5/setup.cfg
```

### Comparing `progress_api-0.1.0a4/.gitignore` & `progress_api-0.1.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/LICENSE.md` & `progress_api-0.1.0a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/PKG-INFO` & `progress_api-0.1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-api
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Backend-agnostic API for reporting progress.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `progress_api-0.1.0a4/docs/api.rst` & `progress_api-0.1.0a5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/docs/backends/index.rst` & `progress_api-0.1.0a5/docs/backends/index.rst`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/docs/conf.py` & `progress_api-0.1.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/docs/index.rst` & `progress_api-0.1.0a5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/examples/enlighten/LICENSE` & `progress_api-0.1.0a5/examples/enlighten/LICENSE`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/examples/enlighten/basic.py` & `progress_api-0.1.0a5/examples/enlighten/basic.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/examples/enlighten/demo.py` & `progress_api-0.1.0a5/examples/enlighten/demo.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/examples/enlighten/floats.py` & `progress_api-0.1.0a5/examples/enlighten/floats.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/examples/enlighten/ftp_downloader.py` & `progress_api-0.1.0a5/examples/enlighten/ftp_downloader.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/examples/enlighten/multicolored.py` & `progress_api-0.1.0a5/examples/enlighten/multicolored.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/examples/enlighten/multiple_logging.py` & `progress_api-0.1.0a5/examples/enlighten/multiple_logging.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/examples/enlighten/multiprocessing_queues.py` & `progress_api-0.1.0a5/examples/enlighten/multiprocessing_queues.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/examples/enlighten/prefixes.py` & `progress_api-0.1.0a5/examples/enlighten/prefixes.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/examples/training_loop.py` & `progress_api-0.1.0a5/examples/training_loop.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/progress_api/__init__.py` & `progress_api-0.1.0a5/progress_api/__init__.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/progress_api/api.py` & `progress_api-0.1.0a5/progress_api/api.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a4/progress_api/backends/__init__.py` & `progress_api-0.1.0a5/progress_api/backends/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # SPDX-License-Identifier: MIT
 
 """
 Package containing backends and the backend interface for the progress API. This
 package provides several backends, but the API is not limited to the supplied
 backends.
 """
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from logging import Logger
 from typing import NamedTuple, Optional
```

### Comparing `progress_api-0.1.0a4/progress_api/backends/enlighten.py` & `progress_api-0.1.0a5/progress_api/backends/enlighten.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # SPDX-License-Identifier: MIT
 
 """
 Progress backend using `Enlighten`_ to display progress bars.  It supports
 multiple bars (well) and multi-state bars, and interacts well with logging
 and other output to standard output and error streams.
 """
+
 # pyright: basic
 from __future__ import annotations
 
 from typing import Optional
 
 from enlighten import Counter, Manager
```

### Comparing `progress_api-0.1.0a4/progress_api/backends/null.py` & `progress_api-0.1.0a5/progress_api/backends/null.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (C) 2023 - 2024 Drexel University and contributors
 # Licensed under the MIT license, see LICENSE.md for details.
 # SPDX-License-Identifier: MIT
 
 """
 Null backend that doesn't supply any progress.
 """
+
 from __future__ import annotations
 
 from typing import Optional
 
 from .. import api
 from . import ProgressBackend, ProgressBarSpec
```

### Comparing `progress_api-0.1.0a4/progress_api/backends/tqdm.py` & `progress_api-0.1.0a5/progress_api/backends/tqdm.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Progress bar backend for `tqdm`_.  This backend is quite limited;
 it does not support multiple states, and it does not have good
 support for multiple progress bars or inteaction with logging,
 unless used in a Jupyter notebook environment.
 
 .. _tqdm: https://tqdm.github.io/docs/tqdm/
 """
+
 # pyright: basic
 from __future__ import annotations
 
 from typing import Optional
 
 from tqdm import tqdm
 from tqdm.auto import tqdm as auto_tqdm
```

### Comparing `progress_api-0.1.0a4/progress_api/config.py` & `progress_api-0.1.0a5/progress_api/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,28 +40,25 @@
 
     if _backend is None:
         raise RuntimeError("backend not initialized")
     return _backend
 
 
 @overload
-def set_backend(impl: backends.ProgressBackend) -> None:
-    ...
+def set_backend(impl: backends.ProgressBackend) -> None: ...
 
 
 @overload
 def set_backend(
     impl: Callable[BCP, backends.ProgressBackend], *args: BCP.args, **kwargs: BCP.kwargs
-) -> None:
-    ...
+) -> None: ...
 
 
 @overload
-def set_backend(impl: str, *args: Any, **kwargs: Any) -> None:
-    ...
+def set_backend(impl: str, *args: Any, **kwargs: Any) -> None: ...
 
 
 def set_backend(
     impl: str | backends.ProgressBackend | Callable[BCP, backends.ProgressBackend],
     *args: Any,
     **kwargs: Any,
 ) -> None:
@@ -82,14 +79,14 @@
         *args, **kwargs: Arguments to pass to the implementation constructor.
     """
     global _backend
 
     if isinstance(impl, str):
         eps = entry_points(name=impl, group="progress_api.backend")
         if eps:
-            impl = eps[0].load()
+            impl = eps[impl].load()
         else:
             raise ValueError(f"unknown progress backend {impl}")
 
     if isinstance(impl, type):
         impl = impl(*args, **kwargs)
     _backend = cast(backends.ProgressBackend, impl)
```

### Comparing `progress_api-0.1.0a4/progress_api.egg-info/PKG-INFO` & `progress_api-0.1.0a5/progress_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-api
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Backend-agnostic API for reporting progress.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `progress_api-0.1.0a4/progress_api.egg-info/SOURCES.txt` & `progress_api-0.1.0a5/progress_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,9 +32,10 @@
 progress_api.egg-info/SOURCES.txt
 progress_api.egg-info/dependency_links.txt
 progress_api.egg-info/entry_points.txt
 progress_api.egg-info/requires.txt
 progress_api.egg-info/top_level.txt
 progress_api/backends/__init__.py
 progress_api/backends/enlighten.py
+progress_api/backends/mock.py
 progress_api/backends/null.py
 progress_api/backends/tqdm.py
```

### Comparing `progress_api-0.1.0a4/pyproject.toml` & `progress_api-0.1.0a5/pyproject.toml`

 * *Files identical despite different names*

