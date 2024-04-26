# Comparing `tmp/pldag-0.7.3.tar.gz` & `tmp/pldag-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.7.3.tar", max compression
+gzip compressed data, was "pldag-0.7.4.tar", max compression
```

## Comparing `pldag-0.7.3.tar` & `pldag-0.7.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.3/LICENSE
--rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.3/README.md
--rw-r--r--   0        0        0    31545 2024-04-25 07:31:01.760869 pldag-0.7.3/pldag/__init__.py
--rw-r--r--   0        0        0       47 2024-04-25 07:41:38.175676 pldag-0.7.3/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1020 2024-04-25 07:41:53.592443 pldag-0.7.3/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-04-25 07:40:31.690286 pldag-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.4/LICENSE
+-rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.4/README.md
+-rw-r--r--   0        0        0    31594 2024-04-25 07:47:29.709670 pldag-0.7.4/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.7.4/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.7.4/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-04-25 07:48:03.323370 pldag-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.4/PKG-INFO
```

### Comparing `pldag-0.7.3/LICENSE` & `pldag-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.7.3/README.md` & `pldag-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.7.3/pldag/__init__.py` & `pldag-0.7.4/pldag/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from itertools import groupby, repeat
 from functools import partial, lru_cache
 from typing import Dict, List, Set, Optional
 from graphlib import TopologicalSorter
 
 from enum import Enum
 
+class NoSolutionsException(Exception):
+    pass
+
 class Solver(Enum):
     GLPK = "glpk"
 
 class PLDAG:
 
     """
         "Primitive Logic Directed Acyclic Graph" data structure, or "PL-DAG" for short, is fundamentally a Directed Acyclic Graph (DAG) where each node represents a logical relationship, and the leaf nodes correspond to literals.
```

### Comparing `pldag-0.7.3/pldag/solver/glpk_solver.py` & `pldag-0.7.4/pldag/solver/glpk_solver.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import functools
 
-from . import NoSolutionsException
+from .. import NoSolutionsException
 
 try:
     import npycvx
 except ImportError:
     raise ImportError("Please install the npycvx package to use GLPK solver module.")
 
 def solve_lp(A: np.ndarray, b: np.ndarray, objectives: np.ndarray, int_vrs: set=set()):
```

### Comparing `pldag-0.7.3/PKG-INFO` & `pldag-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.7.3
+Version: 0.7.4
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

