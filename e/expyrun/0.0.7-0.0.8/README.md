# Comparing `tmp/expyrun-0.0.7.tar.gz` & `tmp/expyrun-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expyrun-0.0.7.tar", last modified: Fri Mar  3 16:52:39 2023, max compression
+gzip compressed data, was "expyrun-0.0.8.tar", last modified: Fri Apr 26 09:21:51 2024, max compression
```

## Comparing `expyrun-0.0.7.tar` & `expyrun-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:52:39.469410 expyrun-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-03 16:52:27.000000 expyrun-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-03-03 16:52:39.469410 expyrun-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-03-03 16:52:27.000000 expyrun-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:52:39.469410 expyrun-0.0.7/expyrun/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-03 16:52:27.000000 expyrun-0.0.7/expyrun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-03-03 16:52:27.000000 expyrun-0.0.7/expyrun/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-03-03 16:52:27.000000 expyrun-0.0.7/expyrun/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 16:52:27.000000 expyrun-0.0.7/expyrun/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:52:39.469410 expyrun-0.0.7/expyrun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-03-03 16:52:39.000000 expyrun-0.0.7/expyrun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-03 16:52:39.000000 expyrun-0.0.7/expyrun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 16:52:39.000000 expyrun-0.0.7/expyrun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-03 16:52:39.000000 expyrun-0.0.7/expyrun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-03 16:52:39.000000 expyrun-0.0.7/expyrun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-03 16:52:39.000000 expyrun-0.0.7/expyrun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 16:52:27.000000 expyrun-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-03 16:52:39.469410 expyrun-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-03 16:52:27.000000 expyrun-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:21:51.973379 expyrun-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 09:21:46.000000 expyrun-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-04-26 09:21:51.973379 expyrun-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-04-26 09:21:46.000000 expyrun-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:21:51.973379 expyrun-0.0.8/expyrun/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 09:21:46.000000 expyrun-0.0.8/expyrun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-04-26 09:21:46.000000 expyrun-0.0.8/expyrun/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-26 09:21:46.000000 expyrun-0.0.8/expyrun/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 09:21:46.000000 expyrun-0.0.8/expyrun/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:21:51.973379 expyrun-0.0.8/expyrun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-04-26 09:21:51.000000 expyrun-0.0.8/expyrun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-26 09:21:51.000000 expyrun-0.0.8/expyrun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:21:51.000000 expyrun-0.0.8/expyrun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 09:21:51.000000 expyrun-0.0.8/expyrun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 09:21:51.000000 expyrun-0.0.8/expyrun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 09:21:51.000000 expyrun-0.0.8/expyrun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 09:21:46.000000 expyrun-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-26 09:21:51.973379 expyrun-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 09:21:46.000000 expyrun-0.0.8/setup.py
```

### Comparing `expyrun-0.0.7/LICENSE` & `expyrun-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `expyrun-0.0.7/PKG-INFO` & `expyrun-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expyrun
-Version: 0.0.7
+Version: 0.0.8
 Summary: Run reproducible experiments from yaml configuration file
 Home-page: https://github.com/raphaelreme/expyrun
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: experiments,reproducibility,machine learning
 Classifier: Development Status :: 4 - Beta
@@ -12,17 +12,19 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
 
 # Expyrun
 
 [![Lint and Test](https://github.com/raphaelreme/expyrun/actions/workflows/tests.yml/badge.svg)](https://github.com/raphaelreme/expyrun/actions/workflows/tests.yml)
 
 Running reproducible experiments from a yaml configuration file.
```

### Comparing `expyrun-0.0.7/README.md` & `expyrun-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `expyrun-0.0.7/expyrun/config.py` & `expyrun-0.0.8/expyrun/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Read a yaml file and convert it into a dict.
 The format is a bit more restrictive than yaml, you cannot build list of Objects,
 only list of values (int, float, bool, str). "." cannot be used inside a key name.
 
 Also some specific keys are used by this library in the root level. See README.md about this.
 """
 
-
 import copy
 import os
 import pathlib
 import re
 from typing import Set, cast, Dict, List, Union
 import warnings
```

### Comparing `expyrun-0.0.7/expyrun/main.py` & `expyrun-0.0.8/expyrun/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
    You can therefore write directly in the current directory in the main function.
 5- Finally the main function is loaded and run.
 
 In DEBUG mode, the code is not copied in the output dir, the code is directly run from the current
 directory
 """
 
-
 import argparse
 import atexit
 import importlib
 import os
 import pathlib
 import sys
 from typing import Dict, cast, List, TextIO, Union
```

### Comparing `expyrun-0.0.7/expyrun.egg-info/PKG-INFO` & `expyrun-0.0.8/expyrun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expyrun
-Version: 0.0.7
+Version: 0.0.8
 Summary: Run reproducible experiments from yaml configuration file
 Home-page: https://github.com/raphaelreme/expyrun
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: experiments,reproducibility,machine learning
 Classifier: Development Status :: 4 - Beta
@@ -12,17 +12,19 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
 
 # Expyrun
 
 [![Lint and Test](https://github.com/raphaelreme/expyrun/actions/workflows/tests.yml/badge.svg)](https://github.com/raphaelreme/expyrun/actions/workflows/tests.yml)
 
 Running reproducible experiments from a yaml configuration file.
```

### Comparing `expyrun-0.0.7/setup.cfg` & `expyrun-0.0.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	pyyaml
 include_package_data = False
```

