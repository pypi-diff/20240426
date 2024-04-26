# Comparing `tmp/prefect_dask-0.2.7.tar.gz` & `tmp/prefect_dask-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_dask-0.2.7.tar", last modified: Thu Apr 25 19:20:15 2024, max compression
+gzip compressed data, was "prefect_dask-0.2.8.tar", last modified: Fri Apr 26 15:04:00 2024, max compression
```

## Comparing `prefect_dask-0.2.7.tar` & `prefect_dask-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:15.103096 prefect_dask-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-25 19:20:15.103096 prefect_dask-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:15.099096 prefect_dask-0.2.7/prefect_dask/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/prefect_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/prefect_dask/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/prefect_dask/task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/prefect_dask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:15.103096 prefect_dask-0.2.7/prefect_dask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-25 19:20:15.000000 prefect_dask-0.2.7/prefect_dask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:15.103096 prefect_dask-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:15.103096 prefect_dask-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/test_task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.916526 prefect_dask-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-04-26 15:04:00.916526 prefect_dask-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.912526 prefect_dask-0.2.8/prefect_dask/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/prefect_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/prefect_dask/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/prefect_dask/task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/prefect_dask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.912526 prefect_dask-0.2.8/prefect_dask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:00.916526 prefect_dask-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.912526 prefect_dask-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/test_task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/test_version.py
```

### Comparing `prefect_dask-0.2.7/PKG-INFO` & `prefect_dask-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-dask
-Version: 0.2.7
+Version: 0.2.8
 Summary: Prefect integrations with the Dask execution framework.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dask
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: anyio<4.0.0,>=3.7.1
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: distributed==2022.2.0; python_version < "3.8"
 Requires-Dist: distributed!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*,>=2022.5.0; python_version >= "3.8"
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
```

### Comparing `prefect_dask-0.2.7/README.md` & `prefect_dask-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.7/prefect_dask/task_runners.py` & `prefect_dask-0.2.8/prefect_dask/task_runners.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 import inspect
 from contextlib import AsyncExitStack
 from typing import Awaitable, Callable, Dict, Optional, Union
 from uuid import UUID
 
 import distributed
 
+from prefect.client.schemas.objects import State
 from prefect.context import FlowRunContext
 from prefect.futures import PrefectFuture
-from prefect.server.schemas.states import State
 from prefect.states import exception_to_crashed_state
 from prefect.task_runners import BaseTaskRunner, R, TaskConcurrencyType
 from prefect.utilities.collections import visit_collection
 from prefect.utilities.importtools import from_qualified_name, to_qualified_name
 
 
 class DaskTaskRunner(BaseTaskRunner):
```

### Comparing `prefect_dask-0.2.7/prefect_dask/utils.py` & `prefect_dask-0.2.8/prefect_dask/utils.py`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.7/prefect_dask.egg-info/PKG-INFO` & `prefect_dask-0.2.8/prefect_dask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-dask
-Version: 0.2.7
+Version: 0.2.8
 Summary: Prefect integrations with the Dask execution framework.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dask
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: anyio<4.0.0,>=3.7.1
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: distributed==2022.2.0; python_version < "3.8"
 Requires-Dist: distributed!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*,>=2022.5.0; python_version >= "3.8"
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
```

### Comparing `prefect_dask-0.2.7/pyproject.toml` & `prefect_dask-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.7/tests/conftest.py` & `prefect_dask-0.2.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.7/tests/test_block_standards.py` & `prefect_dask-0.2.8/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.7/tests/test_task_runners.py` & `prefect_dask-0.2.8/tests/test_task_runners.py`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.7/tests/test_utils.py` & `prefect_dask-0.2.8/tests/test_utils.py`

 * *Files identical despite different names*

