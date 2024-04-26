# Comparing `tmp/fenics-beat-0.0.3.tar.gz` & `tmp/fenics_beat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics-beat-0.0.3.tar", last modified: Fri Apr  5 11:50:22 2024, max compression
+gzip compressed data, was "fenics_beat-0.0.4.tar", last modified: Fri Apr 26 08:41:49 2024, max compression
```

## Comparing `fenics-beat-0.0.3.tar` & `fenics_beat-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.547421 fenics-beat-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-05 11:50:22.547421 fenics-beat-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:50:22.547421 fenics-beat-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.539420 fenics-beat-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.539420 fenics-beat-0.0.3/src/beat/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/bidomain_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.539420 fenics-beat-0.0.3/src/beat/cellmodels/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22810 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/beeler_reuter_1977.py
--rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/fitzhughnagumo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.543420 fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69974 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
--rw-r--r--   0 runner    (1001) docker     (127)    70079 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py
--rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.543420 fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   294950 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/endo.py
--rw-r--r--   0 runner    (1001) docker     (127)   294986 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/epi.py
--rw-r--r--   0 runner    (1001) docker     (127)   294943 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/mid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/monodomain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/monodomain_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/odesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.547421 fenics-beat-0.0.3/src/fenics_beat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-05 11:50:22.000000 fenics-beat-0.0.3/src/fenics_beat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-05 11:50:22.000000 fenics-beat-0.0.3/src/fenics_beat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:50:22.000000 fenics-beat-0.0.3/src/fenics_beat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 11:50:22.000000 fenics-beat-0.0.3/src/fenics_beat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 11:50:22.000000 fenics-beat-0.0.3/src/fenics_beat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.543420 fenics-beat-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_bidomain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_cellmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_monodomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_monodomain_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_odesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.108979 fenics_beat-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-26 08:41:49.108979 fenics_beat-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:41:49.108979 fenics_beat-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.096979 fenics_beat-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.096979 fenics_beat-0.0.4/src/beat/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/bidomain_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.096979 fenics_beat-0.0.4/src/beat/cellmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22492 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/beeler_reuter_1977.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/fitzhughnagumo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.100979 fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68630 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68719 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68702 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.100979 fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286750 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/endo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286758 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/epi.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286743 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/mid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/monodomain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/monodomain_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/odesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/src/beat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.104979 fenics_beat-0.0.4/src/fenics_beat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-26 08:41:49.000000 fenics_beat-0.0.4/src/fenics_beat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-26 08:41:49.000000 fenics_beat-0.0.4/src/fenics_beat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:41:49.000000 fenics_beat-0.0.4/src/fenics_beat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-26 08:41:49.000000 fenics_beat-0.0.4/src/fenics_beat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 08:41:49.000000 fenics_beat-0.0.4/src/fenics_beat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:41:49.104979 fenics_beat-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_bidomain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_cellmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_monodomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_monodomain_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_odesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-26 08:41:45.000000 fenics_beat-0.0.4/tests/test_utils.py
```

### Comparing `fenics-beat-0.0.3/LICENSE` & `fenics_beat-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.3/PKG-INFO` & `fenics_beat-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: fenics-beat
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library to run cardiac EP simulations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://finsberg.github.io/fenics-beat
 Project-URL: Documentation, https://finsberg.github.io/fenics-beat
 Project-URL: Source, https://github.com/finsberg/fenics-beat
 Project-URL: Tracker, https://github.com/finsberg/fenics-beat/issues
 Keywords: cardiac,electrophysiology
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: scipy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pdbpp; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
@@ -34,14 +33,16 @@
 Requires-Dist: fenics-beat[demos]; extra == "docs"
 Provides-Extra: all
 Requires-Dist: fenics-beat[test]; extra == "all"
 Requires-Dist: fenics-beat[docs]; extra == "all"
 Requires-Dist: fenics-beat[pypi]; extra == "all"
 Requires-Dist: fenics-beat[dev]; extra == "all"
 Requires-Dist: fenics-beat[demos]; extra == "all"
+Provides-Extra: testpaths
+Requires-Dist: tests; extra == "testpaths"
 
 # fenics-beat
 
 A simplified version of `cbcbeat` for running cardiac electrophysiology simulations.
 
 - Source code: https://github.com/finsberg/fenics-beat
 - Documentation: https://finsberv.github.io/fenics-beat
```

### Comparing `fenics-beat-0.0.3/pyproject.toml` & `fenics_beat-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "fenics-beat"
-version = "0.0.3"
+version = "0.0.4"
 description = "Library to run cardiac EP simulations"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["cardiac", "electrophysiology"]
 dependencies = [
     "numpy",
-    "scipy",
 ]
 
 [project.urls]
 Homepage = "https://finsberg.github.io/fenics-beat"
 Documentation = "https://finsberg.github.io/fenics-beat"
 Source = "https://github.com/finsberg/fenics-beat"
 Tracker = "https://github.com/finsberg/fenics-beat/issues"
@@ -50,38 +49,24 @@
    "fenics-beat[docs]",
    "fenics-beat[pypi]",
    "fenics-beat[dev]",
    "fenics-beat[demos]"
 ]
 
 
-[tool.setuptools.packages.find]
-where = ["src"]
-
-
-[tool.pytest.ini_options]
-addopts = [
-   "--cov=beat",
-   "--cov-report=html",
-   "--cov-report=term-missing",
-   "-v"
-]
-
 testpaths = [
     "tests"
 ]
 
-[tool.ruff]
-# Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
-select = ["E", "F"]
-ignore = ["E402", "E741", "E743", "E731"]
+[tool.pytest.ini_options]
+markers = [
+    "skip_in_parallel: Skip test when running in parallel",
+]
 
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F"]
-unfixable = []
+[tool.ruff]
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
@@ -97,21 +82,33 @@
     "__pypackages__",
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
+    "demos",
 ]
 
 # Same as Black.
 line-length = 100
 
 # Allow unused variables when underscore-prefixed.
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 # Assume Python 3.10.
 target-version = "py310"
 
-[tool.ruff.mccabe]
+
+[tool.ruff.lint]
+# Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
+select = ["E", "F"]
+ignore = ["E402", "E741", "E743", "E731"]
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["A", "B", "C", "D", "E", "F"]
+unfixable = []
+
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+[tool.ruff.lint.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
```

### Comparing `fenics-beat-0.0.3/src/beat/__init__.py` & `fenics_beat-0.0.4/src/beat/__init__.py`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.3/src/beat/base_model.py` & `fenics_beat-0.0.4/src/beat/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from __future__ import annotations
 from typing import Any, NamedTuple
 import abc
 import logging
 from enum import Enum, auto
 
 import dolfin
-import ufl_legacy as ufl
-from ufl_legacy.core.expr import Expr
+
+try:
+    import ufl_legacy as ufl
+    from ufl_legacy.core.expr import Expr
+except ImportError:
+    import ufl
+    from ufl.core.expr import Expr
 
 
 logger = logging.getLogger(__name__)
 
 
 class Status(str, Enum):
     OK = auto()
@@ -52,69 +57,67 @@
 
         self._timestep = dolfin.Constant(self.parameters["default_timestep"])
         (self._G, self._prec) = self.variational_forms(self._timestep)
         self._lhs, self._rhs = dolfin.system(self._G)
 
         logger.debug("Preassembling monodomain matrix (and initializing vector)")
         self._lhs_matrix = dolfin.assemble(self._lhs)
-        self._rhs_vector = dolfin.Vector(
-            self._mesh.mpi_comm(), self._lhs_matrix.size(0)
-        )
+        self._rhs_vector = dolfin.Vector(self._mesh.mpi_comm(), self._lhs_matrix.size(0))
         self._lhs_matrix.init_vector(self._rhs_vector, 0)
 
         # Create linear solver (based on parameter choices)
         self.linear_solver, self._update_solver = self._create_linear_solver()
 
     @abc.abstractmethod
-    def _setup_state_space(self) -> None:
-        ...
+    def _setup_state_space(self) -> None: ...
 
     def _create_linear_solver(self):
         "Helper function for creating linear solver based on parameters."
         solver_type = self.parameters["linear_solver_type"]
+        # solver_type = "iterative"
 
         if solver_type == "direct":
-            solver = dolfin.LUSolver(self._lhs_matrix, self.parameters["lu_type"])
+            solver = dolfin.LUSolver(
+                self._mesh.mpi_comm(), self._lhs_matrix, self.parameters["lu_type"]
+            )
             solver.parameters.update(self.parameters["lu_solver"])
             update_routine = self._update_lu_solver
 
         elif solver_type == "iterative":
             # Preassemble preconditioner (will be updated if time-step
             # changes)
             logger.debug("Preassembling preconditioner")
             # Initialize KrylovSolver with matrix and preconditioner
             alg = self.parameters["algorithm"]
             prec = self.parameters["preconditioner"]
             if self.parameters["use_custom_preconditioner"]:
                 self._prec_matrix = dolfin.assemble(self._prec)
-                solver = dolfin.PETScKrylovSolver(alg, prec)
+                solver = dolfin.PETScKrylovSolver(self._mesh.mpi_comm(), alg, prec)
                 solver.parameters.update(self.parameters["krylov_solver"])
                 solver.set_operators(self._lhs_matrix, self._prec_matrix)
                 solver.ksp().setFromOptions()
             else:
-                solver = dolfin.PETScKrylovSolver(alg, prec)
+                solver = dolfin.PETScKrylovSolver(self._mesh.mpi_comm(), alg, prec)
                 solver.parameters.update(self.parameters["krylov_solver"])
                 solver.set_operator(self._lhs_matrix)
                 solver.ksp().setFromOptions()
 
             update_routine = self._update_krylov_solver
         else:
             msg = f"Unknown linear_solver_type given: {solver_type}"
             raise ValueError(msg)
 
         return (solver, update_routine)
 
     @property
     @abc.abstractmethod
-    def state(self) -> dolfin.Function:
-        ...
+    def state(self) -> dolfin.Function: ...
 
     @abc.abstractmethod
-    def assign_previous(self) -> None:
-        ...
+    def assign_previous(self) -> None: ...
 
     @staticmethod
     def default_parameters():
         def to_dict(d):
             if isinstance(d, dolfin.Parameters):
                 return to_dict(d.to_dict())
 
@@ -133,15 +136,15 @@
 
         return {
             "theta": 0.5,
             "degree": 1,
             "family": "Lagrange",
             "default_timestep": 1.0,
             "linear_solver_type": "iterative",
-            "lu_type": "default",
+            "lu_type": "superlu_dist",
             "algorithm": "cg",
             "preconditioner": "petsc_amg",
             "krylov_solver": krylov_solver_params,
             "lu_solver": lu_solver_params,
         }
 
     @abc.abstractmethod
@@ -184,14 +187,21 @@
         # Update matrix and linear solvers etc as needed
         timestep_unchanged = abs(dt - float(self._timestep)) < 1.0e-12
         self._update_solver(timestep_unchanged, dt)
 
         # Assemble right-hand-side
         dolfin.assemble(self._rhs, tensor=self._rhs_vector)
 
+        # exit()
+
+        # viewer_A = PETSc.Viewer().createBinary("sandbox/dolfin-A.dat", "w")
+        # viewer_b = PETSc.Viewer().createBinary("sandbox/dolfin-b.dat", "w")
+        # dolfin.as_backend_type(self._lhs_matrix).mat().view(viewer_A)
+        # dolfin.as_backend_type(self._rhs_vector).vec().view(viewer_b)
+
         # Solve problem
         self.linear_solver.solve(self.state.vector(), self._rhs_vector)
         # timer.stop()
 
     def _update_lu_solver(self, timestep_unchanged, dt):
         """Helper function for updating an LUSolver depending on
         whether timestep has changed."""
```

### Comparing `fenics-beat-0.0.3/src/beat/bidomain_model.py` & `fenics_beat-0.0.4/src/beat/bidomain_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from __future__ import annotations
 import logging
-import ufl_legacy as ufl
-from ufl_legacy.core.expr import Expr
 import dolfin
 
+try:
+    import ufl_legacy as ufl
+    from ufl_legacy.core.expr import Expr
+except ImportError:
+    import ufl
+    from ufl.core.expr import Expr
+
 from .base_model import BaseModel, Stimulus
 
 
 logger = logging.getLogger(__name__)
 
 
 class BidomainModel(BaseModel):
@@ -39,17 +44,15 @@
         Ue = dolfin.FiniteElement("CG", self._mesh.ufl_cell(), k)
         dolfin.FunctionSpace(self._mesh, "CG", k)
 
         use_R = self.parameters["use_avg_u_constraint"]
         if use_R:
             Re = dolfin.FiniteElement("R", self._mesh.ufl_cell(), 0)
             dolfin.FunctionSpace(self._mesh, "R", 0)
-            self.VUR = dolfin.FunctionSpace(
-                self._mesh, dolfin.MixedElement((Ve, Ue, Re))
-            )
+            self.VUR = dolfin.FunctionSpace(self._mesh, dolfin.MixedElement((Ve, Ue, Re)))
         else:
             self.VUR = dolfin.FunctionSpace(self._mesh, dolfin.MixedElement((Ve, Ue)))
 
         self.V = V
 
         # Set-up solution fields:
         self.merger = dolfin.FunctionAssigner(V, self.VUR.sub(0))
@@ -145,20 +148,15 @@
             ufl.inner(M_i * ufl.grad(v_mid), ufl.grad(w)) * dz()
             + ufl.inner(M_i * ufl.grad(u), ufl.grad(w)) * dz()
         )
         theta_elliptic = (
             ufl.inner(M_i * ufl.grad(v_mid), ufl.grad(q)) * dz()
             + ufl.inner((M_i + M_e) * ufl.grad(u), ufl.grad(q)) * dz()
         )
-        G = (
-            Dt_v_k_n * w * dz()
-            + k_n * theta_parabolic
-            + k_n * theta_elliptic
-            - k_n * rhs
-        )
+        G = Dt_v_k_n * w * dz() + k_n * theta_parabolic + k_n * theta_elliptic - k_n * rhs
 
         if use_R:
             G += k_n * (lamda * u + l * q) * dz()
 
         # Add applied current as source in elliptic equation if
         # applicable
         if self._I_a:
```

### Comparing `fenics-beat-0.0.3/src/beat/cellmodels/__init__.py` & `fenics_beat-0.0.4/src/beat/cellmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.3/src/beat/cellmodels/beeler_reuter_1977.py` & `fenics_beat-0.0.4/src/beat/cellmodels/beeler_reuter_1977.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,15 @@
     """
     Initialize parameter values
     """
     # Param values
     # E_Na=50, g_Na=0.04, g_Nac=3e-05, g_s=0.0009, IstimAmplitude=0.0,
     # IstimEnd=50000, IstimPeriod=1000, IstimPulseDuration=1,
     # IstimStart=1, C=0.01
-    init_values = np.array(
-        [50, 0.04, 3e-05, 0.0009, 0.0, 50000, 1000, 1, 1, 0.01], dtype=np.float_
-    )
+    init_values = np.array([50, 0.04, 3e-05, 0.0009, 0.0, 50000, 1000, 1, 1, 0.01], dtype=np.float_)
 
     # Parameter indices and limit checker
     param_ind = dict(
         [
             ("E_Na", 0),
             ("g_Na", 1),
             ("g_Nac", 2),
@@ -219,17 +217,15 @@
     # Expressions for the Sodium current h gate component
     alpha_h = 5.497962438709065e-10 * np.exp(-0.25 * V)
     beta_h = 1.7 / (1 + 0.1580253208896478 * np.exp(-0.082 * V))
     values[1] = (1 - h) * alpha_h - beta_h * h
 
     # Expressions for the Sodium current j gate component
     alpha_j = (
-        1.8690473007222892e-10
-        * np.exp(-0.25 * V)
-        / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
+        1.8690473007222892e-10 * np.exp(-0.25 * V) / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
     )
     beta_j = 0.3 / (1 + 0.040762203978366204 * np.exp(-0.1 * V))
     values[2] = (1 - j) * alpha_j - beta_j * j
 
     # Expressions for the Slow inward current component
     E_s = -82.3 - 13.0287 * np.log(0.001 * Cai)
     i_s = g_s * (-E_s + V) * d * f
@@ -251,30 +247,25 @@
         / (1 + 66.5465065250986 * np.exp(0.14992503748125938 * V))
     )
     beta_f = 0.0065 * np.exp(-3 / 5 - V / 50) / (1 + np.exp(-6 - V / 5))
     values[5] = (1 - f) * alpha_f - beta_f * f
 
     # Expressions for the Time dependent outward current component
     i_x1 = (
-        0.0019727757115328517
-        * (-1 + 21.75840239619708 * np.exp(0.04 * V))
-        * np.exp(-0.04 * V)
-        * x1
+        0.0019727757115328517 * (-1 + 21.75840239619708 * np.exp(0.04 * V)) * np.exp(-0.04 * V) * x1
     )
 
     # Expressions for the Time dependent outward current x1 gate component
     alpha_x1 = (
         0.031158410986342627
         * np.exp(0.08264462809917356 * V)
         / (1 + 17.41170806332765 * np.exp(0.05714285714285714 * V))
     )
     beta_x1 = (
-        0.0003916464405623223
-        * np.exp(-0.05998800239952009 * V)
-        / (1 + np.exp(-4 / 5 - V / 25))
+        0.0003916464405623223 * np.exp(-0.05998800239952009 * V) / (1 + np.exp(-4 / 5 - V / 25))
     )
     values[6] = (1 - x1) * alpha_x1 - beta_x1 * x1
 
     # Expressions for the Time independent outward current component
     i_K1 = 0.0035 * (4.6000000000000005 + 0.2 * V) / (
         1 - 0.39851904108451414 * np.exp(-0.04 * V)
     ) + 0.0035 * (-4 + 119.85640018958804 * np.exp(0.04 * V)) / (
@@ -332,17 +323,15 @@
     # Expressions for the Sodium current h gate component
     monitored[3] = 5.497962438709065e-10 * np.exp(-0.25 * V)
     monitored[4] = 1.7 / (1 + 0.1580253208896478 * np.exp(-0.082 * V))
     monitored[19] = (1 - h) * monitored[3] - h * monitored[4]
 
     # Expressions for the Sodium current j gate component
     monitored[5] = (
-        1.8690473007222892e-10
-        * np.exp(-0.25 * V)
-        / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
+        1.8690473007222892e-10 * np.exp(-0.25 * V) / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
     )
     monitored[6] = 0.3 / (1 + 0.040762203978366204 * np.exp(-0.1 * V))
     monitored[20] = (1 - j) * monitored[5] - j * monitored[6]
 
     # Expressions for the Slow inward current component
     monitored[7] = -82.3 - 13.0287 * np.log(0.001 * Cai)
     monitored[8] = g_s * (-monitored[7] + V) * d * f
@@ -364,30 +353,25 @@
         / (1 + 66.5465065250986 * np.exp(0.14992503748125938 * V))
     )
     monitored[12] = 0.0065 * np.exp(-3 / 5 - V / 50) / (1 + np.exp(-6 - V / 5))
     monitored[23] = (1 - f) * monitored[11] - f * monitored[12]
 
     # Expressions for the Time dependent outward current component
     monitored[13] = (
-        0.0019727757115328517
-        * (-1 + 21.75840239619708 * np.exp(0.04 * V))
-        * np.exp(-0.04 * V)
-        * x1
+        0.0019727757115328517 * (-1 + 21.75840239619708 * np.exp(0.04 * V)) * np.exp(-0.04 * V) * x1
     )
 
     # Expressions for the Time dependent outward current x1 gate component
     monitored[14] = (
         0.031158410986342627
         * np.exp(0.08264462809917356 * V)
         / (1 + 17.41170806332765 * np.exp(0.05714285714285714 * V))
     )
     monitored[15] = (
-        0.0003916464405623223
-        * np.exp(-0.05998800239952009 * V)
-        / (1 + np.exp(-4 / 5 - V / 25))
+        0.0003916464405623223 * np.exp(-0.05998800239952009 * V) / (1 + np.exp(-4 / 5 - V / 25))
     )
     monitored[24] = (1 - x1) * monitored[14] - monitored[15] * x1
 
     # Expressions for the Time independent outward current component
     monitored[17] = 0.0035 * (4.6000000000000005 + 0.2 * V) / (
         1 - 0.39851904108451414 * np.exp(-0.04 * V)
     ) + 0.0035 * (-4 + 119.85640018958804 * np.exp(0.04 * V)) / (
@@ -444,17 +428,15 @@
     alpha_h = 5.497962438709065e-10 * np.exp(-0.25 * V)
     beta_h = 1.7 / (1 + 0.1580253208896478 * np.exp(-0.082 * V))
     dh_dt = (1 - h) * alpha_h - beta_h * h
     states[1] = dt * dh_dt + h
 
     # Expressions for the Sodium current j gate component
     alpha_j = (
-        1.8690473007222892e-10
-        * np.exp(-0.25 * V)
-        / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
+        1.8690473007222892e-10 * np.exp(-0.25 * V) / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
     )
     beta_j = 0.3 / (1 + 0.040762203978366204 * np.exp(-0.1 * V))
     dj_dt = (1 - j) * alpha_j - beta_j * j
     states[2] = dt * dj_dt + j
 
     # Expressions for the Slow inward current component
     E_s = -82.3 - 13.0287 * np.log(0.001 * Cai)
@@ -480,30 +462,25 @@
     )
     beta_f = 0.0065 * np.exp(-3 / 5 - V / 50) / (1 + np.exp(-6 - V / 5))
     df_dt = (1 - f) * alpha_f - beta_f * f
     states[5] = dt * df_dt + f
 
     # Expressions for the Time dependent outward current component
     i_x1 = (
-        0.0019727757115328517
-        * (-1 + 21.75840239619708 * np.exp(0.04 * V))
-        * np.exp(-0.04 * V)
-        * x1
+        0.0019727757115328517 * (-1 + 21.75840239619708 * np.exp(0.04 * V)) * np.exp(-0.04 * V) * x1
     )
 
     # Expressions for the Time dependent outward current x1 gate component
     alpha_x1 = (
         0.031158410986342627
         * np.exp(0.08264462809917356 * V)
         / (1 + 17.41170806332765 * np.exp(0.05714285714285714 * V))
     )
     beta_x1 = (
-        0.0003916464405623223
-        * np.exp(-0.05998800239952009 * V)
-        / (1 + np.exp(-4 / 5 - V / 25))
+        0.0003916464405623223 * np.exp(-0.05998800239952009 * V) / (1 + np.exp(-4 / 5 - V / 25))
     )
     dx1_dt = (1 - x1) * alpha_x1 - beta_x1 * x1
     states[6] = dt * dx1_dt + x1
 
     # Expressions for the Time independent outward current component
     i_K1 = 0.0035 * (4.6000000000000005 + 0.2 * V) / (
         1 - 0.39851904108451414 * np.exp(-0.04 * V)
@@ -576,17 +553,15 @@
             dt * dh_dt,
         )
         + h
     )
 
     # Expressions for the Sodium current j gate component
     alpha_j = (
-        1.8690473007222892e-10
-        * np.exp(-0.25 * V)
-        / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
+        1.8690473007222892e-10 * np.exp(-0.25 * V) / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
     )
     beta_j = 0.3 / (1 + 0.040762203978366204 * np.exp(-0.1 * V))
     dj_dt = (1 - j) * alpha_j - beta_j * j
     dj_dt_linearized = -alpha_j - beta_j
     states[2] = (
         np.where(
             np.abs(dj_dt_linearized) > 1e-08,
@@ -643,30 +618,25 @@
             dt * df_dt,
         )
         + f
     )
 
     # Expressions for the Time dependent outward current component
     i_x1 = (
-        0.0019727757115328517
-        * (-1 + 21.75840239619708 * np.exp(0.04 * V))
-        * np.exp(-0.04 * V)
-        * x1
+        0.0019727757115328517 * (-1 + 21.75840239619708 * np.exp(0.04 * V)) * np.exp(-0.04 * V) * x1
     )
 
     # Expressions for the Time dependent outward current x1 gate component
     alpha_x1 = (
         0.031158410986342627
         * np.exp(0.08264462809917356 * V)
         / (1 + 17.41170806332765 * np.exp(0.05714285714285714 * V))
     )
     beta_x1 = (
-        0.0003916464405623223
-        * np.exp(-0.05998800239952009 * V)
-        / (1 + np.exp(-4 / 5 - V / 25))
+        0.0003916464405623223 * np.exp(-0.05998800239952009 * V) / (1 + np.exp(-4 / 5 - V / 25))
     )
     dx1_dt = (1 - x1) * alpha_x1 - beta_x1 * x1
     dx1_dt_linearized = -alpha_x1 - beta_x1
     states[6] = (
         np.where(
             np.abs(dx1_dt_linearized) > 1e-08,
             (-1 + np.exp(dt * dx1_dt_linearized)) * dx1_dt / dx1_dt_linearized,
@@ -694,24 +664,18 @@
     di_K1_dV = (
         0.0007000000000000001 / (1 - 0.39851904108451414 * np.exp(-0.04 * V))
         + 0.016779896026542326
         * np.exp(0.04 * V)
         / (8.331137487687693 * np.exp(0.04 * V) + 69.4078518387552 * np.exp(0.08 * V))
         + 0.0035
         * (-4 + 119.85640018958804 * np.exp(0.04 * V))
-        * (
-            -0.3332454995075077 * np.exp(0.04 * V)
-            - 5.552628147100417 * np.exp(0.08 * V)
-        )
+        * (-0.3332454995075077 * np.exp(0.04 * V) - 5.552628147100417 * np.exp(0.08 * V))
         / (
             (8.331137487687693 * np.exp(0.04 * V) + 69.4078518387552 * np.exp(0.08 * V))
-            * (
-                8.331137487687693 * np.exp(0.04 * V)
-                + 69.4078518387552 * np.exp(0.08 * V)
-            )
+            * (8.331137487687693 * np.exp(0.04 * V) + 69.4078518387552 * np.exp(0.08 * V))
         )
         - 5.5792665751831976e-05
         * (4.6000000000000005 + 0.2 * V)
         * np.exp(-0.04 * V)
         / (
             (1 - 0.39851904108451414 * np.exp(-0.04 * V))
             * (1 - 0.39851904108451414 * np.exp(-0.04 * V))
```

### Comparing `fenics-beat-0.0.3/src/beat/cellmodels/fitzhughnagumo.py` & `fenics_beat-0.0.4/src/beat/cellmodels/fitzhughnagumo.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,17 +159,17 @@
         values = np.zeros((2,), dtype=np.float_)
     else:
         assert isinstance(values, np.ndarray) and values.shape == (2,)
 
     # Expressions for the fitzhughnagumo component
     v_amp = v_peak - v_rest
     v_th = v_rest + a * v_amp
-    I = -c_2 * (-v_rest + v) * s / v_amp + c_1 * (v_peak - v) * (-v_rest + v) * (
-        -v_th + v
-    ) / (v_amp * v_amp)
+    I = -c_2 * (-v_rest + v) * s / v_amp + c_1 * (v_peak - v) * (-v_rest + v) * (-v_th + v) / (
+        v_amp * v_amp
+    )
     i_Stim = (
         stim_amplitude
         * (1 - 1 / (1 + np.exp(5.0 * t - 5.0 * stim_start)))
         / (1 + np.exp(5.0 * t - 5.0 * stim_duration - 5.0 * stim_start))
     )
     values[0] = I + i_Stim
     values[1] = b * (-v_rest - c_3 * s + v)
@@ -205,17 +205,17 @@
         monitored = np.zeros((6,), dtype=np.float_)
     else:
         assert isinstance(monitored, np.ndarray) and monitored.shape == (6,)
 
     # Expressions for the fitzhughnagumo component
     monitored[0] = v_peak - v_rest
     monitored[1] = v_rest + a * monitored[0]
-    monitored[2] = -c_2 * (-v_rest + v) * s / monitored[0] + c_1 * (v_peak - v) * (
-        -v_rest + v
-    ) * (-monitored[1] + v) / (monitored[0] * monitored[0])
+    monitored[2] = -c_2 * (-v_rest + v) * s / monitored[0] + c_1 * (v_peak - v) * (-v_rest + v) * (
+        -monitored[1] + v
+    ) / (monitored[0] * monitored[0])
     monitored[3] = (
         stim_amplitude
         * (1 - 1 / (1 + np.exp(5.0 * t - 5.0 * stim_start)))
         / (1 + np.exp(5.0 * t - 5.0 * stim_duration - 5.0 * stim_start))
     )
     monitored[4] = monitored[2] + monitored[3]
     monitored[5] = b * (-v_rest - c_3 * s + v)
@@ -246,17 +246,17 @@
     stim_start = parameters[8]
     v_peak = parameters[9]
     v_rest = parameters[10]
 
     # Expressions for the fitzhughnagumo component
     v_amp = v_peak - v_rest
     v_th = v_rest + a * v_amp
-    I = -c_2 * (-v_rest + v) * s / v_amp + c_1 * (v_peak - v) * (-v_rest + v) * (
-        -v_th + v
-    ) / (v_amp * v_amp)
+    I = -c_2 * (-v_rest + v) * s / v_amp + c_1 * (v_peak - v) * (-v_rest + v) * (-v_th + v) / (
+        v_amp * v_amp
+    )
     i_Stim = (
         stim_amplitude
         * (1 - 1 / (1 + np.exp(5.0 * t - 5.0 * stim_start)))
         / (1 + np.exp(5.0 * t - 5.0 * stim_duration - 5.0 * stim_start))
     )
     dv_dt = I + i_Stim
     states[0] = dt * dv_dt + v
@@ -289,17 +289,17 @@
     stim_start = parameters[8]
     v_peak = parameters[9]
     v_rest = parameters[10]
 
     # Expressions for the fitzhughnagumo component
     v_amp = v_peak - v_rest
     v_th = v_rest + a * v_amp
-    I = -c_2 * (-v_rest + v) * s / v_amp + c_1 * (v_peak - v) * (-v_rest + v) * (
-        -v_th + v
-    ) / (v_amp * v_amp)
+    I = -c_2 * (-v_rest + v) * s / v_amp + c_1 * (v_peak - v) * (-v_rest + v) * (-v_th + v) / (
+        v_amp * v_amp
+    )
     i_Stim = (
         stim_amplitude
         * (1 - 1 / (1 + np.exp(5.0 * t - 5.0 * stim_start)))
         / (1 + np.exp(5.0 * t - 5.0 * stim_duration - 5.0 * stim_start))
     )
     dv_dt = I + i_Stim
     dI_dv = (
```

### Comparing `fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py` & `fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Gotran generated code for the "tentusscher_panfilov_2006_endo_cell" model
+# Gotran generated code for the "tentusscher_panfilov_2006_epi_cell" model
 
 import numpy as np
 
 
 def init_state_values(**values):
     """
     Initialize state values
     """
     # Init values
-    # Xr1=0.00448, Xr2=0.476, Xs=0.0087, m=0.00155, h=0.7573, j=0.7225,
-    # d=3.164e-05, f=0.8009, f2=0.9778, fCass=0.9953, s=0.3212,
-    # r=2.235e-08, Ca_i=0.00013, R_prime=0.9068, Ca_SR=3.715,
-    # Ca_ss=0.00036, Na_i=10.355, V=-86.709, K_i=138.4
+    # Xr1=0.00621, Xr2=0.4712, Xs=0.0095, m=0.00172, h=0.7444, j=0.7045,
+    # d=3.373e-05, f=0.7888, f2=0.9755, fCass=0.9953, s=0.999998,
+    # r=2.42e-08, Ca_i=0.000126, R_prime=0.9073, Ca_SR=3.64,
+    # Ca_ss=0.00036, Na_i=8.604, V=-85.23, K_i=136.89
     init_values = np.array(
         [
-            0.00448,
-            0.476,
-            0.0087,
-            0.00155,
-            0.7573,
-            0.7225,
-            3.164e-05,
-            0.8009,
-            0.9778,
+            0.00621,
+            0.4712,
+            0.0095,
+            0.00172,
+            0.7444,
+            0.7045,
+            3.373e-05,
+            0.7888,
+            0.9755,
             0.9953,
-            0.3212,
-            2.235e-08,
-            0.00013,
-            0.9068,
-            3.715,
+            0.999998,
+            2.42e-08,
+            0.000126,
+            0.9073,
+            3.64,
             0.00036,
-            10.355,
-            -86.709,
-            138.4,
+            8.604,
+            -85.23,
+            136.89,
         ],
         dtype=np.float_,
     )
 
     # State indices and limit checker
     state_ind = dict(
         [
@@ -75,15 +75,15 @@
 
 def init_parameter_values(**values):
     """
     Initialize parameter values
     """
     # Param values
     # P_kna=0.03, g_K1=5.405, g_Kr=0.153, g_Ks=0.392, g_Na=14.838,
-    # g_bna=0.00029, g_CaL=0.0398, g_bca=0.000592, g_to=0.073,
+    # g_bna=0.00029, g_CaL=0.0398, g_bca=0.000592, g_to=0.294,
     # K_mNa=40.0, K_mk=1.0, P_NaK=2.724, K_NaCa=1000.0, K_sat=0.1,
     # Km_Ca=1.38, Km_Nai=87.5, alpha=2.5, gamma=0.35, K_pCa=0.0005,
     # g_pCa=0.1238, g_pK=0.0146, Buf_c=0.2, Buf_sr=10.0, Buf_ss=0.4,
     # Ca_o=2.0, EC=1.5, K_buf_c=0.001, K_buf_sr=0.3, K_buf_ss=0.00025,
     # K_up=0.00025, V_leak=0.00036, V_rel=0.102, V_sr=1094.0,
     # V_ss=54.68, V_xfer=0.0038, Vmax_up=0.006375, k1_prime=0.15,
     # k2_prime=0.045, k3=0.06, k4=0.005, max_sr=2.5, min_sr=1,
@@ -96,15 +96,15 @@
             5.405,
             0.153,
             0.392,
             14.838,
             0.00029,
             0.0398,
             0.000592,
-            0.073,
+            0.294,
             40.0,
             1.0,
             2.724,
             1000.0,
             0.1,
             1.38,
             87.5,
@@ -441,15 +441,15 @@
         return indices
     else:
         return indices[0]
 
 
 def rhs(states, t, parameters, values=None):
     """
-    Compute the right hand side of the tentusscher_panfilov_2006_endo_cell ODE
+    Compute the right hand side of the tentusscher_panfilov_2006_epi_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -592,17 +592,15 @@
     values[3] = (-m + m_inf) / tau_m
 
     # Expressions for the h gate component
     h_inf = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    alpha_h = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    alpha_h = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     beta_h = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     tau_h = 1.0 / (alpha_h + beta_h)
     values[4] = (-h + h_inf) / tau_h
@@ -617,17 +615,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     beta_j = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     tau_j = 1.0 / (alpha_j + beta_j)
     values[5] = (-j + j_inf) / tau_j
 
     # Expressions for the Sodium background current component
     i_b_Na = g_bna * (-E_Na + V)
@@ -681,16 +677,16 @@
     # Expressions for the Calcium background current component
     i_b_Ca = g_bca * (-E_Ca + V)
 
     # Expressions for the Transient outward current component
     i_to = g_to * (-E_K + V) * r * s
 
     # Expressions for the s gate component
-    s_inf = 1.0 / (1 + np.exp(28 / 5 + V / 5))
-    tau_s = 8 + 1000 * np.exp(-((67 + V) * (67 + V)) / 1000)
+    s_inf = 1.0 / (1 + np.exp(4 + V / 5))
+    tau_s = 3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
     values[10] = (-s + s_inf) / tau_s
 
     # Expressions for the r gate component
     r_inf = 1.0 / (1 + np.exp(10 / 3 - V / 6))
     tau_r = 0.8 + 9.5 * np.exp(-((40 + V) * (40 + V)) / 1800)
     values[11] = (-r + r_inf) / tau_r
 
@@ -698,74 +694,59 @@
     i_NaK = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     i_NaCa = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     i_p_Ca = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
-    i_p_K = (
-        g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
-    )
+    i_p_K = g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     ddt_Ca_i_total = (
         V_sr * (-i_up + i_leak) / V_c
         + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
         + i_xfer
     )
     f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    f_JCa_sr_free = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    f_JCa_ss_free = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    f_JCa_sr_free = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    f_JCa_ss_free = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     values[12] = ddt_Ca_i_total * f_JCa_i_free
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     values[13] = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
     ddt_Ca_sr_total = -i_leak - i_rel + i_up
-    ddt_Ca_ss_total = (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    )
+    ddt_Ca_ss_total = V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
     values[14] = ddt_Ca_sr_total * f_JCa_sr_free
     values[15] = ddt_Ca_ss_total * f_JCa_ss_free
 
     # Expressions for the Sodium dynamics component
     values[16] = Cm * (-i_Na - i_b_Na - 3 * i_NaCa - 3 * i_NaK) / (F * V_c)
 
     # Expressions for the Membrane component
@@ -790,25 +771,23 @@
         - i_b_Na
         - i_p_Ca
         - i_p_K
         - i_to
     )
 
     # Expressions for the Potassium dynamics component
-    values[18] = (
-        Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
-    )
+    values[18] = Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
 
     # Return results
     return values
 
 
 def monitor(states, t, parameters, monitored=None):
     """
-    Computes monitored expressions of the tentusscher_panfilov_2006_endo_cell\
+    Computes monitored expressions of the tentusscher_panfilov_2006_epi_cell\
         ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
@@ -899,30 +878,24 @@
     # Expressions for the Reversal potentials component
     monitored[0] = R * T * np.log(Na_o / Na_i) / F
     monitored[1] = R * T * np.log(K_o / K_i) / F
     monitored[2] = R * T * np.log((K_o + Na_o * P_kna) / (P_kna * Na_i + K_i)) / F
     monitored[3] = 0.5 * R * T * np.log(Ca_o / Ca_i) / F
 
     # Expressions for the Inward rectifier potassium current component
-    monitored[4] = 0.1 / (
-        1 + 6.14421235332821e-06 * np.exp(0.06 * V - 0.06 * monitored[1])
-    )
+    monitored[4] = 0.1 / (1 + 6.14421235332821e-06 * np.exp(0.06 * V - 0.06 * monitored[1]))
     monitored[5] = (
         0.36787944117144233 * np.exp(0.1 * V - 0.1 * monitored[1])
         + 3.0606040200802673 * np.exp(0.0002 * V - 0.0002 * monitored[1])
     ) / (1 + np.exp(0.5 * monitored[1] - 0.5 * V))
     monitored[6] = monitored[4] / (monitored[4] + monitored[5])
-    monitored[7] = (
-        0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-monitored[1] + V) * monitored[6]
-    )
+    monitored[7] = 0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-monitored[1] + V) * monitored[6]
 
     # Expressions for the Rapid time dependent potassium current component
-    monitored[8] = (
-        0.4303314829119352 * g_Kr * np.sqrt(K_o) * (-monitored[1] + V) * Xr1 * Xr2
-    )
+    monitored[8] = 0.4303314829119352 * g_Kr * np.sqrt(K_o) * (-monitored[1] + V) * Xr1 * Xr2
 
     # Expressions for the Xr1 gate component
     monitored[9] = 1.0 / (1 + np.exp(-26 / 7 - V / 7))
     monitored[10] = 450 / (1 + np.exp(-9 / 2 - V / 10))
     monitored[11] = 6 / (1 + 13.581324522578193 * np.exp(0.08695652173913043 * V))
     monitored[12] = monitored[10] * monitored[11]
     monitored[73] = (-Xr1 + monitored[9]) / monitored[12]
@@ -958,17 +931,15 @@
     monitored[76] = (-m + monitored[23]) / monitored[26]
 
     # Expressions for the h gate component
     monitored[27] = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    monitored[28] = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    monitored[28] = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     monitored[29] = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     monitored[30] = 1.0 / (monitored[28] + monitored[29])
     monitored[77] = (-h + monitored[27]) / monitored[30]
@@ -983,17 +954,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     monitored[33] = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     monitored[34] = 1.0 / (monitored[32] + monitored[33])
     monitored[78] = (-j + monitored[31]) / monitored[34]
 
     # Expressions for the Sodium background current component
     monitored[35] = g_bna * (-monitored[0] + V)
@@ -1047,16 +1016,16 @@
     # Expressions for the Calcium background current component
     monitored[48] = g_bca * (-monitored[3] + V)
 
     # Expressions for the Transient outward current component
     monitored[49] = g_to * (-monitored[1] + V) * r * s
 
     # Expressions for the s gate component
-    monitored[50] = 1.0 / (1 + np.exp(28 / 5 + V / 5))
-    monitored[51] = 8 + 1000 * np.exp(-((67 + V) * (67 + V)) / 1000)
+    monitored[50] = 1.0 / (1 + np.exp(4 + V / 5))
+    monitored[51] = 3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
     monitored[83] = (-s + monitored[50]) / monitored[51]
 
     # Expressions for the r gate component
     monitored[52] = 1.0 / (1 + np.exp(10 / 3 - V / 6))
     monitored[53] = 0.8 + 9.5 * np.exp(-((40 + V) * (40 + V)) / 1800)
     monitored[84] = (-r + monitored[52]) / monitored[53]
 
@@ -1064,91 +1033,73 @@
     monitored[54] = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     monitored[55] = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     monitored[56] = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
     monitored[57] = (
-        g_pK
-        * (-monitored[1] + V)
-        / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
+        g_pK * (-monitored[1] + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
     )
 
     # Expressions for the Calcium dynamics component
     monitored[58] = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     monitored[59] = V_leak * (-Ca_i + Ca_SR)
     monitored[60] = V_xfer * (-Ca_i + Ca_ss)
     monitored[61] = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     monitored[62] = (
         V_sr * (-monitored[58] + monitored[59]) / V_c
         + Cm * (-monitored[48] - monitored[56] + 2 * monitored[55]) / (2 * F * V_c)
         + monitored[60]
     )
     monitored[63] = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    monitored[64] = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    monitored[65] = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    monitored[64] = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    monitored[65] = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     monitored[85] = monitored[62] * monitored[63]
     monitored[66] = k1_prime / monitored[61]
     monitored[67] = k2_prime * monitored[61]
     monitored[68] = (
-        (Ca_ss * Ca_ss)
-        * R_prime
-        * monitored[66]
-        / (k3 + (Ca_ss * Ca_ss) * monitored[66])
+        (Ca_ss * Ca_ss) * R_prime * monitored[66] / (k3 + (Ca_ss * Ca_ss) * monitored[66])
     )
     monitored[86] = k4 * (1 - R_prime) - Ca_ss * R_prime * monitored[67]
     monitored[69] = V_rel * (-Ca_ss + Ca_SR) * monitored[68]
     monitored[70] = -monitored[59] - monitored[69] + monitored[58]
     monitored[71] = (
         V_sr * monitored[69] / V_ss
         - V_c * monitored[60] / V_ss
         - Cm * monitored[36] / (2 * F * V_ss)
     )
     monitored[87] = monitored[64] * monitored[70]
     monitored[88] = monitored[65] * monitored[71]
 
     # Expressions for the Sodium dynamics component
     monitored[89] = (
-        Cm
-        * (-monitored[22] - monitored[35] - 3 * monitored[54] - 3 * monitored[55])
-        / (F * V_c)
+        Cm * (-monitored[22] - monitored[35] - 3 * monitored[54] - 3 * monitored[55]) / (F * V_c)
     )
 
     # Expressions for the Membrane component
     monitored[72] = np.where(
         np.logical_and(
             t - stim_period * np.floor(t / stim_period) >= stim_start,
             t - stim_period * np.floor(t / stim_period) <= stim_duration + stim_start,
@@ -1190,15 +1141,15 @@
     # Return results
     return monitored
 
 
 def forward_explicit_euler(states, t, dt, parameters):
     """
     Compute a forward step using the explicit Euler scheme to the\
-        tentusscher_panfilov_2006_endo_cell ODE
+        tentusscher_panfilov_2006_epi_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -1339,17 +1290,15 @@
     states[3] = dt * dm_dt + m
 
     # Expressions for the h gate component
     h_inf = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    alpha_h = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    alpha_h = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     beta_h = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     tau_h = 1.0 / (alpha_h + beta_h)
     dh_dt = (-h + h_inf) / tau_h
@@ -1365,17 +1314,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     beta_j = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     tau_j = 1.0 / (alpha_j + beta_j)
     dj_dt = (-j + j_inf) / tau_j
     states[5] = dt * dj_dt + j
 
     # Expressions for the Sodium background current component
@@ -1434,16 +1381,16 @@
     # Expressions for the Calcium background current component
     i_b_Ca = g_bca * (-E_Ca + V)
 
     # Expressions for the Transient outward current component
     i_to = g_to * (-E_K + V) * r * s
 
     # Expressions for the s gate component
-    s_inf = 1.0 / (1 + np.exp(28 / 5 + V / 5))
-    tau_s = 8 + 1000 * np.exp(-((67 + V) * (67 + V)) / 1000)
+    s_inf = 1.0 / (1 + np.exp(4 + V / 5))
+    tau_s = 3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
     ds_dt = (-s + s_inf) / tau_s
     states[10] = dt * ds_dt + s
 
     # Expressions for the r gate component
     r_inf = 1.0 / (1 + np.exp(10 / 3 - V / 6))
     tau_r = 0.8 + 9.5 * np.exp(-((40 + V) * (40 + V)) / 1800)
     dr_dt = (-r + r_inf) / tau_r
@@ -1453,76 +1400,61 @@
     i_NaK = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     i_NaCa = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     i_p_Ca = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
-    i_p_K = (
-        g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
-    )
+    i_p_K = g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     ddt_Ca_i_total = (
         V_sr * (-i_up + i_leak) / V_c
         + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
         + i_xfer
     )
     f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    f_JCa_sr_free = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    f_JCa_ss_free = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    f_JCa_sr_free = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    f_JCa_ss_free = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     dCa_i_dt = ddt_Ca_i_total * f_JCa_i_free
     states[12] = dt * dCa_i_dt + Ca_i
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     dR_prime_dt = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     states[13] = dt * dR_prime_dt + R_prime
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
     ddt_Ca_sr_total = -i_leak - i_rel + i_up
-    ddt_Ca_ss_total = (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    )
+    ddt_Ca_ss_total = V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
     dCa_SR_dt = ddt_Ca_sr_total * f_JCa_sr_free
     states[14] = dt * dCa_SR_dt + Ca_SR
     dCa_ss_dt = ddt_Ca_ss_total * f_JCa_ss_free
     states[15] = dt * dCa_ss_dt + Ca_ss
 
     # Expressions for the Sodium dynamics component
     dNa_i_dt = Cm * (-i_Na - i_b_Na - 3 * i_NaCa - 3 * i_NaK) / (F * V_c)
@@ -1561,15 +1493,15 @@
     # Return results
     return states
 
 
 def forward_generalized_rush_larsen(states, t, dt, parameters):
     """
     Compute a forward step using the generalised Rush-Larsen (GRL1) scheme to\
-        the tentusscher_panfilov_2006_endo_cell ODE
+        the tentusscher_panfilov_2006_epi_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -1671,28 +1603,24 @@
     # Expressions for the Xr1 gate component
     xr1_inf = 1.0 / (1 + np.exp(-26 / 7 - V / 7))
     alpha_xr1 = 450 / (1 + np.exp(-9 / 2 - V / 10))
     beta_xr1 = 6 / (1 + 13.581324522578193 * np.exp(0.08695652173913043 * V))
     tau_xr1 = alpha_xr1 * beta_xr1
     dXr1_dt = (-Xr1 + xr1_inf) / tau_xr1
     dXr1_dt_linearized = -1 / tau_xr1
-    states[0] = (
-        -1 + np.exp(dt * dXr1_dt_linearized)
-    ) * dXr1_dt / dXr1_dt_linearized + Xr1
+    states[0] = (-1 + np.exp(dt * dXr1_dt_linearized)) * dXr1_dt / dXr1_dt_linearized + Xr1
 
     # Expressions for the Xr2 gate component
     xr2_inf = 1.0 / (1 + np.exp(11 / 3 + V / 24))
     alpha_xr2 = 3 / (1 + np.exp(-3 - V / 20))
     beta_xr2 = 1.12 / (1 + np.exp(-3 + V / 20))
     tau_xr2 = alpha_xr2 * beta_xr2
     dXr2_dt = (-Xr2 + xr2_inf) / tau_xr2
     dXr2_dt_linearized = -1 / tau_xr2
-    states[1] = (
-        -1 + np.exp(dt * dXr2_dt_linearized)
-    ) * dXr2_dt / dXr2_dt_linearized + Xr2
+    states[1] = (-1 + np.exp(dt * dXr2_dt_linearized)) * dXr2_dt / dXr2_dt_linearized + Xr2
 
     # Expressions for the Slow time dependent potassium current component
     i_Ks = g_Ks * (Xs * Xs) * (-E_Ks + V)
 
     # Expressions for the Xs gate component
     xs_inf = 1.0 / (1 + np.exp(-5 / 14 - V / 14))
     alpha_xs = 1400 / np.sqrt(1 + np.exp(5 / 6 - V / 6))
@@ -1718,17 +1646,15 @@
     states[3] = (-1 + np.exp(dt * dm_dt_linearized)) * dm_dt / dm_dt_linearized + m
 
     # Expressions for the h gate component
     h_inf = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    alpha_h = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    alpha_h = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     beta_h = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     tau_h = 1.0 / (alpha_h + beta_h)
     dh_dt = (-h + h_inf) / tau_h
@@ -1745,17 +1671,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     beta_j = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     tau_j = 1.0 / (alpha_j + beta_j)
     dj_dt = (-j + j_inf) / tau_j
     dj_dt_linearized = -1 / tau_j
     states[5] = (-1 + np.exp(dt * dj_dt_linearized)) * dj_dt / dj_dt_linearized + j
 
@@ -1810,27 +1734,25 @@
     states[8] = (-1 + np.exp(dt * df2_dt_linearized)) * df2_dt / df2_dt_linearized + f2
 
     # Expressions for the FCass gate component
     fCass_inf = 0.4 + 0.6 / (1 + 400.0 * (Ca_ss * Ca_ss))
     tau_fCass = 2 + 80 / (1 + 400.0 * (Ca_ss * Ca_ss))
     dfCass_dt = (-fCass + fCass_inf) / tau_fCass
     dfCass_dt_linearized = -1 / tau_fCass
-    states[9] = (
-        -1 + np.exp(dt * dfCass_dt_linearized)
-    ) * dfCass_dt / dfCass_dt_linearized + fCass
+    states[9] = (-1 + np.exp(dt * dfCass_dt_linearized)) * dfCass_dt / dfCass_dt_linearized + fCass
 
     # Expressions for the Calcium background current component
     i_b_Ca = g_bca * (-E_Ca + V)
 
     # Expressions for the Transient outward current component
     i_to = g_to * (-E_K + V) * r * s
 
     # Expressions for the s gate component
-    s_inf = 1.0 / (1 + np.exp(28 / 5 + V / 5))
-    tau_s = 8 + 1000 * np.exp(-((67 + V) * (67 + V)) / 1000)
+    s_inf = 1.0 / (1 + np.exp(4 + V / 5))
+    tau_s = 3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
     ds_dt = (-s + s_inf) / tau_s
     ds_dt_linearized = -1 / tau_s
     states[10] = (-1 + np.exp(dt * ds_dt_linearized)) * ds_dt / ds_dt_linearized + s
 
     # Expressions for the r gate component
     r_inf = 1.0 / (1 + np.exp(10 / 3 - V / 6))
     tau_r = 0.8 + 9.5 * np.exp(-((40 + V) * (40 + V)) / 1800)
@@ -1842,64 +1764,51 @@
     i_NaK = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     i_NaCa = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     i_p_Ca = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
-    i_p_K = (
-        g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
-    )
+    i_p_K = g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     ddt_Ca_i_total = (
         V_sr * (-i_up + i_leak) / V_c
         + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
         + i_xfer
     )
     f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    f_JCa_sr_free = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    f_JCa_ss_free = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    f_JCa_sr_free = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    f_JCa_ss_free = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     dCa_i_dt = ddt_Ca_i_total * f_JCa_i_free
     dE_Ca_dCa_i = -0.5 * R * T / (F * Ca_i)
     dddt_Ca_i_total_di_NaCa = Cm / (F * V_c)
     dddt_Ca_i_total_di_b_Ca = -Cm / (2 * F * V_c)
     dddt_Ca_i_total_di_leak = V_sr / V_c
     dddt_Ca_i_total_di_p_Ca = -Cm / (2 * F * V_c)
     dddt_Ca_i_total_di_up = -V_sr / V_c
@@ -1922,17 +1831,15 @@
         * np.exp(F * (-1 + gamma) * V / (R * T))
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
-    di_p_Ca_dCa_i = g_pCa / (K_pCa + Ca_i) - g_pCa * Ca_i / (
-        (K_pCa + Ca_i) * (K_pCa + Ca_i)
-    )
+    di_p_Ca_dCa_i = g_pCa / (K_pCa + Ca_i) - g_pCa * Ca_i / ((K_pCa + Ca_i) * (K_pCa + Ca_i))
     di_up_dCa_i = (
         2
         * Vmax_up
         * (K_up * K_up)
         / (
             ((1 + (K_up * K_up) / (Ca_i * Ca_i)) * (1 + (K_up * K_up) / (Ca_i * Ca_i)))
             * (Ca_i * Ca_i * Ca_i)
@@ -1955,26 +1862,22 @@
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     dR_prime_dt = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     dR_prime_dt_linearized = -k4 - Ca_ss * k2
     states[13] = (
         np.where(
             np.abs(dR_prime_dt_linearized) > 1e-08,
-            (-1 + np.exp(dt * dR_prime_dt_linearized))
-            * dR_prime_dt
-            / dR_prime_dt_linearized,
+            (-1 + np.exp(dt * dR_prime_dt_linearized)) * dR_prime_dt / dR_prime_dt_linearized,
             dt * dR_prime_dt,
         )
         + R_prime
     )
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
     ddt_Ca_sr_total = -i_leak - i_rel + i_up
-    ddt_Ca_ss_total = (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    )
+    ddt_Ca_ss_total = V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
     dCa_SR_dt = ddt_Ca_sr_total * f_JCa_sr_free
     dO_dk1 = (Ca_ss * Ca_ss) * R_prime / (k3 + (Ca_ss * Ca_ss) * k1) - np.power(
         Ca_ss, 4
     ) * R_prime * k1 / ((k3 + (Ca_ss * Ca_ss) * k1) * (k3 + (Ca_ss * Ca_ss) * k1))
     df_JCa_sr_free_dCa_SR = (
         2
         * Buf_sr
@@ -1993,17 +1896,15 @@
         * (EC * EC)
         * (max_sr - min_sr)
         / (
             ((1 + (EC * EC) / (Ca_SR * Ca_SR)) * (1 + (EC * EC) / (Ca_SR * Ca_SR)))
             * (Ca_SR * Ca_SR * Ca_SR)
         )
     )
-    di_rel_dCa_SR = (
-        V_rel * O + V_rel * (-Ca_ss + Ca_SR) * dO_dk1 * dk1_dkcasr * dkcasr_dCa_SR
-    )
+    di_rel_dCa_SR = V_rel * O + V_rel * (-Ca_ss + Ca_SR) * dO_dk1 * dk1_dkcasr * dkcasr_dCa_SR
     di_rel_dO = V_rel * (-Ca_ss + Ca_SR)
     dCa_SR_dt_linearized = (
         -V_leak - di_rel_dCa_SR - dO_dk1 * di_rel_dO * dk1_dkcasr * dkcasr_dCa_SR
     ) * f_JCa_sr_free + ddt_Ca_sr_total * df_JCa_sr_free_dCa_SR
     states[14] = Ca_SR + np.where(
         np.abs(dCa_SR_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCa_SR_dt_linearized)) * dCa_SR_dt / dCa_SR_dt_linearized,
@@ -2067,36 +1968,23 @@
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
     di_NaK_dNa_i = K_o * P_NaK / (
         (K_mNa + Na_i)
         * (K_mk + K_o)
-        * (
-            1
-            + 0.0353 * np.exp(-F * V / (R * T))
-            + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-        )
+        * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
     ) - K_o * P_NaK * Na_i / (
         ((K_mNa + Na_i) * (K_mNa + Na_i))
         * (K_mk + K_o)
-        * (
-            1
-            + 0.0353 * np.exp(-F * V / (R * T))
-            + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-        )
+        * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
     )
     dNa_i_dt_linearized = (
         Cm
-        * (
-            -3 * di_NaCa_dNa_i
-            - 3 * di_NaK_dNa_i
-            + g_bna * dE_Na_dNa_i
-            - dE_Na_dNa_i * di_Na_dE_Na
-        )
+        * (-3 * di_NaCa_dNa_i - 3 * di_NaK_dNa_i + g_bna * dE_Na_dNa_i - dE_Na_dNa_i * di_Na_dE_Na)
         / (F * V_c)
     )
     states[16] = Na_i + np.where(
         np.abs(dNa_i_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dNa_i_dt_linearized)) * dNa_i_dt / dNa_i_dt_linearized,
         dt * dNa_i_dt,
     )
@@ -2135,17 +2023,15 @@
     )
     dbeta_K1_dV = (
         0.0006121208040160535 * np.exp(0.0002 * V - 0.0002 * E_K)
         + 0.036787944117144235 * np.exp(0.1 * V - 0.1 * E_K)
     ) / (1 + np.exp(0.5 * E_K - 0.5 * V)) + 0.5 * (
         0.36787944117144233 * np.exp(0.1 * V - 0.1 * E_K)
         + 3.0606040200802673 * np.exp(0.0002 * V - 0.0002 * E_K)
-    ) * np.exp(
-        0.5 * E_K - 0.5 * V
-    ) / (
+    ) * np.exp(0.5 * E_K - 0.5 * V) / (
         (1 + np.exp(0.5 * E_K - 0.5 * V)) * (1 + np.exp(0.5 * E_K - 0.5 * V))
     )
     di_CaL_dV = (
         4
         * g_CaL
         * (F * F)
         * (-Ca_o + 0.25 * Ca_ss * np.exp(F * (-30 + 2 * V) / (R * T)))
@@ -2194,39 +2080,30 @@
         dalpha_K1_dV * dxK1_inf_dalpha_K1 + dbeta_K1_dV * dxK1_inf_dbeta_K1
     )
     di_K1_dxK1_inf = 0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-E_K + V)
     di_Kr_dV = 0.4303314829119352 * g_Kr * np.sqrt(K_o) * Xr1 * Xr2
     di_Ks_dV = g_Ks * (Xs * Xs)
     di_Na_dV = g_Na * (m * m * m) * h * j
     di_NaCa_dV = K_NaCa * (
-        Ca_o
-        * F
-        * gamma
-        * (Na_i * Na_i * Na_i)
-        * np.exp(F * gamma * V / (R * T))
-        / (R * T)
+        Ca_o * F * gamma * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T)) / (R * T)
         - F
         * alpha
         * (Na_o * Na_o * Na_o)
         * (-1 + gamma)
         * Ca_i
         * np.exp(F * (-1 + gamma) * V / (R * T))
         / (R * T)
     ) / (
         (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
         * (Ca_o + Km_Ca)
         * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
-    ) - F * K_NaCa * K_sat * (
-        -1 + gamma
-    ) * (
+    ) - F * K_NaCa * K_sat * (-1 + gamma) * (
         Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
         - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
-    ) * np.exp(
-        F * (-1 + gamma) * V / (R * T)
-    ) / (
+    ) * np.exp(F * (-1 + gamma) * V / (R * T)) / (
         R
         * T
         * (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
         )
         * (Ca_o + Km_Ca)
@@ -2240,24 +2117,16 @@
             + 0.012450000000000001 * F * np.exp(-0.1 * F * V / (R * T)) / (R * T)
         )
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
             * (
-                (
-                    1
-                    + 0.0353 * np.exp(-F * V / (R * T))
-                    + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-                )
-                * (
-                    1
-                    + 0.0353 * np.exp(-F * V / (R * T))
-                    + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-                )
+                (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
+                * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
             )
         )
     )
     di_p_K_dV = g_pK / (
         1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V)
     ) + 10.937327047146876 * g_pK * (-E_K + V) * np.exp(-0.16722408026755853 * V) / (
         (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
@@ -2272,16 +2141,15 @@
         - di_Kr_dV
         - di_Ks_dV
         - di_NaCa_dV
         - di_NaK_dV
         - di_Na_dV
         - di_p_K_dV
         - di_to_dV
-        - (dalpha_K1_dV * dxK1_inf_dalpha_K1 + dbeta_K1_dV * dxK1_inf_dbeta_K1)
-        * di_K1_dxK1_inf
+        - (dalpha_K1_dV * dxK1_inf_dalpha_K1 + dbeta_K1_dV * dxK1_inf_dbeta_K1) * di_K1_dxK1_inf
     )
     states[17] = (
         np.where(
             np.abs(dV_dt_linearized) > 1e-08,
             (-1 + np.exp(dt * dV_dt_linearized)) * dV_dt / dV_dt_linearized,
             dt * dV_dt,
         )
@@ -2302,17 +2170,15 @@
     )
     dbeta_K1_dE_K = (
         -0.0006121208040160535 * np.exp(0.0002 * V - 0.0002 * E_K)
         - 0.036787944117144235 * np.exp(0.1 * V - 0.1 * E_K)
     ) / (1 + np.exp(0.5 * E_K - 0.5 * V)) - 0.5 * (
         0.36787944117144233 * np.exp(0.1 * V - 0.1 * E_K)
         + 3.0606040200802673 * np.exp(0.0002 * V - 0.0002 * E_K)
-    ) * np.exp(
-        0.5 * E_K - 0.5 * V
-    ) / (
+    ) * np.exp(0.5 * E_K - 0.5 * V) / (
         (1 + np.exp(0.5 * E_K - 0.5 * V)) * (1 + np.exp(0.5 * E_K - 0.5 * V))
     )
     di_K1_dE_K = -0.4303314829119352 * g_K1 * np.sqrt(
         K_o
     ) * xK1_inf + 0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-E_K + V) * (
         dalpha_K1_dE_K * dxK1_inf_dalpha_K1 + dbeta_K1_dE_K * dxK1_inf_dbeta_K1
     )
```

### Comparing `fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py` & `fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Gotran generated code for the "tentusscher_panfilov_2006_epi_cell" model
+# Gotran generated code for the "tentusscher_panfilov_2006_M_cell" model
 
 import numpy as np
 
 
 def init_state_values(**values):
     """
     Initialize state values
     """
     # Init values
-    # Xr1=0.00621, Xr2=0.4712, Xs=0.0095, m=0.00172, h=0.7444, j=0.7045,
-    # d=3.373e-05, f=0.7888, f2=0.9755, fCass=0.9953, s=0.999998,
-    # r=2.42e-08, Ca_i=0.000126, R_prime=0.9073, Ca_SR=3.64,
-    # Ca_ss=0.00036, Na_i=8.604, V=-85.23, K_i=136.89
+    # Xr1=0.0165, Xr2=0.473, Xs=0.0174, m=0.00165, h=0.749, j=0.6788,
+    # d=3.288e-05, f=0.7026, f2=0.9526, fCass=0.9942, s=0.999998,
+    # r=2.347e-08, Ca_i=0.000153, R_prime=0.8978, Ca_SR=4.272,
+    # Ca_ss=0.00042, Na_i=10.132, V=-85.423, K_i=138.52
     init_values = np.array(
         [
-            0.00621,
-            0.4712,
-            0.0095,
-            0.00172,
-            0.7444,
-            0.7045,
-            3.373e-05,
-            0.7888,
-            0.9755,
-            0.9953,
+            0.0165,
+            0.473,
+            0.0174,
+            0.00165,
+            0.749,
+            0.6788,
+            3.288e-05,
+            0.7026,
+            0.9526,
+            0.9942,
             0.999998,
-            2.42e-08,
-            0.000126,
-            0.9073,
-            3.64,
-            0.00036,
-            8.604,
-            -85.23,
-            136.89,
+            2.347e-08,
+            0.000153,
+            0.8978,
+            4.272,
+            0.00042,
+            10.132,
+            -85.423,
+            138.52,
         ],
         dtype=np.float_,
     )
 
     # State indices and limit checker
     state_ind = dict(
         [
@@ -74,15 +74,15 @@
 
 
 def init_parameter_values(**values):
     """
     Initialize parameter values
     """
     # Param values
-    # P_kna=0.03, g_K1=5.405, g_Kr=0.153, g_Ks=0.392, g_Na=14.838,
+    # P_kna=0.03, g_K1=5.405, g_Kr=0.153, g_Ks=0.098, g_Na=14.838,
     # g_bna=0.00029, g_CaL=0.0398, g_bca=0.000592, g_to=0.294,
     # K_mNa=40.0, K_mk=1.0, P_NaK=2.724, K_NaCa=1000.0, K_sat=0.1,
     # Km_Ca=1.38, Km_Nai=87.5, alpha=2.5, gamma=0.35, K_pCa=0.0005,
     # g_pCa=0.1238, g_pK=0.0146, Buf_c=0.2, Buf_sr=10.0, Buf_ss=0.4,
     # Ca_o=2.0, EC=1.5, K_buf_c=0.001, K_buf_sr=0.3, K_buf_ss=0.00025,
     # K_up=0.00025, V_leak=0.00036, V_rel=0.102, V_sr=1094.0,
     # V_ss=54.68, V_xfer=0.0038, Vmax_up=0.006375, k1_prime=0.15,
@@ -91,15 +91,15 @@
     # stim_amplitude=-52.0, stim_duration=1.0, stim_period=1000.0,
     # stim_start=10.0, K_o=5.4
     init_values = np.array(
         [
             0.03,
             5.405,
             0.153,
-            0.392,
+            0.098,
             14.838,
             0.00029,
             0.0398,
             0.000592,
             0.294,
             40.0,
             1.0,
@@ -441,15 +441,15 @@
         return indices
     else:
         return indices[0]
 
 
 def rhs(states, t, parameters, values=None):
     """
-    Compute the right hand side of the tentusscher_panfilov_2006_epi_cell ODE
+    Compute the right hand side of the tentusscher_panfilov_2006_M_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -592,17 +592,15 @@
     values[3] = (-m + m_inf) / tau_m
 
     # Expressions for the h gate component
     h_inf = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    alpha_h = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    alpha_h = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     beta_h = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     tau_h = 1.0 / (alpha_h + beta_h)
     values[4] = (-h + h_inf) / tau_h
@@ -617,17 +615,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     beta_j = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     tau_j = 1.0 / (alpha_j + beta_j)
     values[5] = (-j + j_inf) / tau_j
 
     # Expressions for the Sodium background current component
     i_b_Na = g_bna * (-E_Na + V)
@@ -698,74 +694,59 @@
     i_NaK = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     i_NaCa = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     i_p_Ca = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
-    i_p_K = (
-        g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
-    )
+    i_p_K = g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     ddt_Ca_i_total = (
         V_sr * (-i_up + i_leak) / V_c
         + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
         + i_xfer
     )
     f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    f_JCa_sr_free = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    f_JCa_ss_free = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    f_JCa_sr_free = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    f_JCa_ss_free = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     values[12] = ddt_Ca_i_total * f_JCa_i_free
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     values[13] = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
     ddt_Ca_sr_total = -i_leak - i_rel + i_up
-    ddt_Ca_ss_total = (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    )
+    ddt_Ca_ss_total = V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
     values[14] = ddt_Ca_sr_total * f_JCa_sr_free
     values[15] = ddt_Ca_ss_total * f_JCa_ss_free
 
     # Expressions for the Sodium dynamics component
     values[16] = Cm * (-i_Na - i_b_Na - 3 * i_NaCa - 3 * i_NaK) / (F * V_c)
 
     # Expressions for the Membrane component
@@ -790,26 +771,23 @@
         - i_b_Na
         - i_p_Ca
         - i_p_K
         - i_to
     )
 
     # Expressions for the Potassium dynamics component
-    values[18] = (
-        Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
-    )
+    values[18] = Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
 
     # Return results
     return values
 
 
 def monitor(states, t, parameters, monitored=None):
     """
-    Computes monitored expressions of the tentusscher_panfilov_2006_epi_cell\
-        ODE
+    Computes monitored expressions of the tentusscher_panfilov_2006_M_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -899,30 +877,24 @@
     # Expressions for the Reversal potentials component
     monitored[0] = R * T * np.log(Na_o / Na_i) / F
     monitored[1] = R * T * np.log(K_o / K_i) / F
     monitored[2] = R * T * np.log((K_o + Na_o * P_kna) / (P_kna * Na_i + K_i)) / F
     monitored[3] = 0.5 * R * T * np.log(Ca_o / Ca_i) / F
 
     # Expressions for the Inward rectifier potassium current component
-    monitored[4] = 0.1 / (
-        1 + 6.14421235332821e-06 * np.exp(0.06 * V - 0.06 * monitored[1])
-    )
+    monitored[4] = 0.1 / (1 + 6.14421235332821e-06 * np.exp(0.06 * V - 0.06 * monitored[1]))
     monitored[5] = (
         0.36787944117144233 * np.exp(0.1 * V - 0.1 * monitored[1])
         + 3.0606040200802673 * np.exp(0.0002 * V - 0.0002 * monitored[1])
     ) / (1 + np.exp(0.5 * monitored[1] - 0.5 * V))
     monitored[6] = monitored[4] / (monitored[4] + monitored[5])
-    monitored[7] = (
-        0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-monitored[1] + V) * monitored[6]
-    )
+    monitored[7] = 0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-monitored[1] + V) * monitored[6]
 
     # Expressions for the Rapid time dependent potassium current component
-    monitored[8] = (
-        0.4303314829119352 * g_Kr * np.sqrt(K_o) * (-monitored[1] + V) * Xr1 * Xr2
-    )
+    monitored[8] = 0.4303314829119352 * g_Kr * np.sqrt(K_o) * (-monitored[1] + V) * Xr1 * Xr2
 
     # Expressions for the Xr1 gate component
     monitored[9] = 1.0 / (1 + np.exp(-26 / 7 - V / 7))
     monitored[10] = 450 / (1 + np.exp(-9 / 2 - V / 10))
     monitored[11] = 6 / (1 + 13.581324522578193 * np.exp(0.08695652173913043 * V))
     monitored[12] = monitored[10] * monitored[11]
     monitored[73] = (-Xr1 + monitored[9]) / monitored[12]
@@ -958,17 +930,15 @@
     monitored[76] = (-m + monitored[23]) / monitored[26]
 
     # Expressions for the h gate component
     monitored[27] = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    monitored[28] = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    monitored[28] = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     monitored[29] = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     monitored[30] = 1.0 / (monitored[28] + monitored[29])
     monitored[77] = (-h + monitored[27]) / monitored[30]
@@ -983,17 +953,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     monitored[33] = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     monitored[34] = 1.0 / (monitored[32] + monitored[33])
     monitored[78] = (-j + monitored[31]) / monitored[34]
 
     # Expressions for the Sodium background current component
     monitored[35] = g_bna * (-monitored[0] + V)
@@ -1048,17 +1016,15 @@
     monitored[48] = g_bca * (-monitored[3] + V)
 
     # Expressions for the Transient outward current component
     monitored[49] = g_to * (-monitored[1] + V) * r * s
 
     # Expressions for the s gate component
     monitored[50] = 1.0 / (1 + np.exp(4 + V / 5))
-    monitored[51] = (
-        3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
-    )
+    monitored[51] = 3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
     monitored[83] = (-s + monitored[50]) / monitored[51]
 
     # Expressions for the r gate component
     monitored[52] = 1.0 / (1 + np.exp(10 / 3 - V / 6))
     monitored[53] = 0.8 + 9.5 * np.exp(-((40 + V) * (40 + V)) / 1800)
     monitored[84] = (-r + monitored[52]) / monitored[53]
 
@@ -1066,91 +1032,73 @@
     monitored[54] = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     monitored[55] = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     monitored[56] = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
     monitored[57] = (
-        g_pK
-        * (-monitored[1] + V)
-        / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
+        g_pK * (-monitored[1] + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
     )
 
     # Expressions for the Calcium dynamics component
     monitored[58] = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     monitored[59] = V_leak * (-Ca_i + Ca_SR)
     monitored[60] = V_xfer * (-Ca_i + Ca_ss)
     monitored[61] = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     monitored[62] = (
         V_sr * (-monitored[58] + monitored[59]) / V_c
         + Cm * (-monitored[48] - monitored[56] + 2 * monitored[55]) / (2 * F * V_c)
         + monitored[60]
     )
     monitored[63] = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    monitored[64] = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    monitored[65] = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    monitored[64] = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    monitored[65] = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     monitored[85] = monitored[62] * monitored[63]
     monitored[66] = k1_prime / monitored[61]
     monitored[67] = k2_prime * monitored[61]
     monitored[68] = (
-        (Ca_ss * Ca_ss)
-        * R_prime
-        * monitored[66]
-        / (k3 + (Ca_ss * Ca_ss) * monitored[66])
+        (Ca_ss * Ca_ss) * R_prime * monitored[66] / (k3 + (Ca_ss * Ca_ss) * monitored[66])
     )
     monitored[86] = k4 * (1 - R_prime) - Ca_ss * R_prime * monitored[67]
     monitored[69] = V_rel * (-Ca_ss + Ca_SR) * monitored[68]
     monitored[70] = -monitored[59] - monitored[69] + monitored[58]
     monitored[71] = (
         V_sr * monitored[69] / V_ss
         - V_c * monitored[60] / V_ss
         - Cm * monitored[36] / (2 * F * V_ss)
     )
     monitored[87] = monitored[64] * monitored[70]
     monitored[88] = monitored[65] * monitored[71]
 
     # Expressions for the Sodium dynamics component
     monitored[89] = (
-        Cm
-        * (-monitored[22] - monitored[35] - 3 * monitored[54] - 3 * monitored[55])
-        / (F * V_c)
+        Cm * (-monitored[22] - monitored[35] - 3 * monitored[54] - 3 * monitored[55]) / (F * V_c)
     )
 
     # Expressions for the Membrane component
     monitored[72] = np.where(
         np.logical_and(
             t - stim_period * np.floor(t / stim_period) >= stim_start,
             t - stim_period * np.floor(t / stim_period) <= stim_duration + stim_start,
@@ -1192,15 +1140,15 @@
     # Return results
     return monitored
 
 
 def forward_explicit_euler(states, t, dt, parameters):
     """
     Compute a forward step using the explicit Euler scheme to the\
-        tentusscher_panfilov_2006_epi_cell ODE
+        tentusscher_panfilov_2006_M_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -1341,17 +1289,15 @@
     states[3] = dt * dm_dt + m
 
     # Expressions for the h gate component
     h_inf = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    alpha_h = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    alpha_h = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     beta_h = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     tau_h = 1.0 / (alpha_h + beta_h)
     dh_dt = (-h + h_inf) / tau_h
@@ -1367,17 +1313,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     beta_j = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     tau_j = 1.0 / (alpha_j + beta_j)
     dj_dt = (-j + j_inf) / tau_j
     states[5] = dt * dj_dt + j
 
     # Expressions for the Sodium background current component
@@ -1455,76 +1399,61 @@
     i_NaK = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     i_NaCa = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     i_p_Ca = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
-    i_p_K = (
-        g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
-    )
+    i_p_K = g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     ddt_Ca_i_total = (
         V_sr * (-i_up + i_leak) / V_c
         + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
         + i_xfer
     )
     f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    f_JCa_sr_free = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    f_JCa_ss_free = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    f_JCa_sr_free = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    f_JCa_ss_free = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     dCa_i_dt = ddt_Ca_i_total * f_JCa_i_free
     states[12] = dt * dCa_i_dt + Ca_i
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     dR_prime_dt = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     states[13] = dt * dR_prime_dt + R_prime
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
     ddt_Ca_sr_total = -i_leak - i_rel + i_up
-    ddt_Ca_ss_total = (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    )
+    ddt_Ca_ss_total = V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
     dCa_SR_dt = ddt_Ca_sr_total * f_JCa_sr_free
     states[14] = dt * dCa_SR_dt + Ca_SR
     dCa_ss_dt = ddt_Ca_ss_total * f_JCa_ss_free
     states[15] = dt * dCa_ss_dt + Ca_ss
 
     # Expressions for the Sodium dynamics component
     dNa_i_dt = Cm * (-i_Na - i_b_Na - 3 * i_NaCa - 3 * i_NaK) / (F * V_c)
@@ -1563,15 +1492,15 @@
     # Return results
     return states
 
 
 def forward_generalized_rush_larsen(states, t, dt, parameters):
     """
     Compute a forward step using the generalised Rush-Larsen (GRL1) scheme to\
-        the tentusscher_panfilov_2006_epi_cell ODE
+        the tentusscher_panfilov_2006_M_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -1673,28 +1602,24 @@
     # Expressions for the Xr1 gate component
     xr1_inf = 1.0 / (1 + np.exp(-26 / 7 - V / 7))
     alpha_xr1 = 450 / (1 + np.exp(-9 / 2 - V / 10))
     beta_xr1 = 6 / (1 + 13.581324522578193 * np.exp(0.08695652173913043 * V))
     tau_xr1 = alpha_xr1 * beta_xr1
     dXr1_dt = (-Xr1 + xr1_inf) / tau_xr1
     dXr1_dt_linearized = -1 / tau_xr1
-    states[0] = (
-        -1 + np.exp(dt * dXr1_dt_linearized)
-    ) * dXr1_dt / dXr1_dt_linearized + Xr1
+    states[0] = (-1 + np.exp(dt * dXr1_dt_linearized)) * dXr1_dt / dXr1_dt_linearized + Xr1
 
     # Expressions for the Xr2 gate component
     xr2_inf = 1.0 / (1 + np.exp(11 / 3 + V / 24))
     alpha_xr2 = 3 / (1 + np.exp(-3 - V / 20))
     beta_xr2 = 1.12 / (1 + np.exp(-3 + V / 20))
     tau_xr2 = alpha_xr2 * beta_xr2
     dXr2_dt = (-Xr2 + xr2_inf) / tau_xr2
     dXr2_dt_linearized = -1 / tau_xr2
-    states[1] = (
-        -1 + np.exp(dt * dXr2_dt_linearized)
-    ) * dXr2_dt / dXr2_dt_linearized + Xr2
+    states[1] = (-1 + np.exp(dt * dXr2_dt_linearized)) * dXr2_dt / dXr2_dt_linearized + Xr2
 
     # Expressions for the Slow time dependent potassium current component
     i_Ks = g_Ks * (Xs * Xs) * (-E_Ks + V)
 
     # Expressions for the Xs gate component
     xs_inf = 1.0 / (1 + np.exp(-5 / 14 - V / 14))
     alpha_xs = 1400 / np.sqrt(1 + np.exp(5 / 6 - V / 6))
@@ -1720,17 +1645,15 @@
     states[3] = (-1 + np.exp(dt * dm_dt_linearized)) * dm_dt / dm_dt_linearized + m
 
     # Expressions for the h gate component
     h_inf = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    alpha_h = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    alpha_h = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     beta_h = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     tau_h = 1.0 / (alpha_h + beta_h)
     dh_dt = (-h + h_inf) / tau_h
@@ -1747,17 +1670,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     beta_j = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     tau_j = 1.0 / (alpha_j + beta_j)
     dj_dt = (-j + j_inf) / tau_j
     dj_dt_linearized = -1 / tau_j
     states[5] = (-1 + np.exp(dt * dj_dt_linearized)) * dj_dt / dj_dt_linearized + j
 
@@ -1812,17 +1733,15 @@
     states[8] = (-1 + np.exp(dt * df2_dt_linearized)) * df2_dt / df2_dt_linearized + f2
 
     # Expressions for the FCass gate component
     fCass_inf = 0.4 + 0.6 / (1 + 400.0 * (Ca_ss * Ca_ss))
     tau_fCass = 2 + 80 / (1 + 400.0 * (Ca_ss * Ca_ss))
     dfCass_dt = (-fCass + fCass_inf) / tau_fCass
     dfCass_dt_linearized = -1 / tau_fCass
-    states[9] = (
-        -1 + np.exp(dt * dfCass_dt_linearized)
-    ) * dfCass_dt / dfCass_dt_linearized + fCass
+    states[9] = (-1 + np.exp(dt * dfCass_dt_linearized)) * dfCass_dt / dfCass_dt_linearized + fCass
 
     # Expressions for the Calcium background current component
     i_b_Ca = g_bca * (-E_Ca + V)
 
     # Expressions for the Transient outward current component
     i_to = g_to * (-E_K + V) * r * s
 
@@ -1844,64 +1763,51 @@
     i_NaK = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     i_NaCa = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     i_p_Ca = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
-    i_p_K = (
-        g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
-    )
+    i_p_K = g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     ddt_Ca_i_total = (
         V_sr * (-i_up + i_leak) / V_c
         + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
         + i_xfer
     )
     f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    f_JCa_sr_free = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    f_JCa_ss_free = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    f_JCa_sr_free = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    f_JCa_ss_free = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     dCa_i_dt = ddt_Ca_i_total * f_JCa_i_free
     dE_Ca_dCa_i = -0.5 * R * T / (F * Ca_i)
     dddt_Ca_i_total_di_NaCa = Cm / (F * V_c)
     dddt_Ca_i_total_di_b_Ca = -Cm / (2 * F * V_c)
     dddt_Ca_i_total_di_leak = V_sr / V_c
     dddt_Ca_i_total_di_p_Ca = -Cm / (2 * F * V_c)
     dddt_Ca_i_total_di_up = -V_sr / V_c
@@ -1924,17 +1830,15 @@
         * np.exp(F * (-1 + gamma) * V / (R * T))
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
-    di_p_Ca_dCa_i = g_pCa / (K_pCa + Ca_i) - g_pCa * Ca_i / (
-        (K_pCa + Ca_i) * (K_pCa + Ca_i)
-    )
+    di_p_Ca_dCa_i = g_pCa / (K_pCa + Ca_i) - g_pCa * Ca_i / ((K_pCa + Ca_i) * (K_pCa + Ca_i))
     di_up_dCa_i = (
         2
         * Vmax_up
         * (K_up * K_up)
         / (
             ((1 + (K_up * K_up) / (Ca_i * Ca_i)) * (1 + (K_up * K_up) / (Ca_i * Ca_i)))
             * (Ca_i * Ca_i * Ca_i)
@@ -1957,26 +1861,22 @@
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     dR_prime_dt = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     dR_prime_dt_linearized = -k4 - Ca_ss * k2
     states[13] = (
         np.where(
             np.abs(dR_prime_dt_linearized) > 1e-08,
-            (-1 + np.exp(dt * dR_prime_dt_linearized))
-            * dR_prime_dt
-            / dR_prime_dt_linearized,
+            (-1 + np.exp(dt * dR_prime_dt_linearized)) * dR_prime_dt / dR_prime_dt_linearized,
             dt * dR_prime_dt,
         )
         + R_prime
     )
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
     ddt_Ca_sr_total = -i_leak - i_rel + i_up
-    ddt_Ca_ss_total = (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    )
+    ddt_Ca_ss_total = V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
     dCa_SR_dt = ddt_Ca_sr_total * f_JCa_sr_free
     dO_dk1 = (Ca_ss * Ca_ss) * R_prime / (k3 + (Ca_ss * Ca_ss) * k1) - np.power(
         Ca_ss, 4
     ) * R_prime * k1 / ((k3 + (Ca_ss * Ca_ss) * k1) * (k3 + (Ca_ss * Ca_ss) * k1))
     df_JCa_sr_free_dCa_SR = (
         2
         * Buf_sr
@@ -1995,17 +1895,15 @@
         * (EC * EC)
         * (max_sr - min_sr)
         / (
             ((1 + (EC * EC) / (Ca_SR * Ca_SR)) * (1 + (EC * EC) / (Ca_SR * Ca_SR)))
             * (Ca_SR * Ca_SR * Ca_SR)
         )
     )
-    di_rel_dCa_SR = (
-        V_rel * O + V_rel * (-Ca_ss + Ca_SR) * dO_dk1 * dk1_dkcasr * dkcasr_dCa_SR
-    )
+    di_rel_dCa_SR = V_rel * O + V_rel * (-Ca_ss + Ca_SR) * dO_dk1 * dk1_dkcasr * dkcasr_dCa_SR
     di_rel_dO = V_rel * (-Ca_ss + Ca_SR)
     dCa_SR_dt_linearized = (
         -V_leak - di_rel_dCa_SR - dO_dk1 * di_rel_dO * dk1_dkcasr * dkcasr_dCa_SR
     ) * f_JCa_sr_free + ddt_Ca_sr_total * df_JCa_sr_free_dCa_SR
     states[14] = Ca_SR + np.where(
         np.abs(dCa_SR_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCa_SR_dt_linearized)) * dCa_SR_dt / dCa_SR_dt_linearized,
@@ -2069,36 +1967,23 @@
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
     di_NaK_dNa_i = K_o * P_NaK / (
         (K_mNa + Na_i)
         * (K_mk + K_o)
-        * (
-            1
-            + 0.0353 * np.exp(-F * V / (R * T))
-            + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-        )
+        * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
     ) - K_o * P_NaK * Na_i / (
         ((K_mNa + Na_i) * (K_mNa + Na_i))
         * (K_mk + K_o)
-        * (
-            1
-            + 0.0353 * np.exp(-F * V / (R * T))
-            + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-        )
+        * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
     )
     dNa_i_dt_linearized = (
         Cm
-        * (
-            -3 * di_NaCa_dNa_i
-            - 3 * di_NaK_dNa_i
-            + g_bna * dE_Na_dNa_i
-            - dE_Na_dNa_i * di_Na_dE_Na
-        )
+        * (-3 * di_NaCa_dNa_i - 3 * di_NaK_dNa_i + g_bna * dE_Na_dNa_i - dE_Na_dNa_i * di_Na_dE_Na)
         / (F * V_c)
     )
     states[16] = Na_i + np.where(
         np.abs(dNa_i_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dNa_i_dt_linearized)) * dNa_i_dt / dNa_i_dt_linearized,
         dt * dNa_i_dt,
     )
@@ -2137,17 +2022,15 @@
     )
     dbeta_K1_dV = (
         0.0006121208040160535 * np.exp(0.0002 * V - 0.0002 * E_K)
         + 0.036787944117144235 * np.exp(0.1 * V - 0.1 * E_K)
     ) / (1 + np.exp(0.5 * E_K - 0.5 * V)) + 0.5 * (
         0.36787944117144233 * np.exp(0.1 * V - 0.1 * E_K)
         + 3.0606040200802673 * np.exp(0.0002 * V - 0.0002 * E_K)
-    ) * np.exp(
-        0.5 * E_K - 0.5 * V
-    ) / (
+    ) * np.exp(0.5 * E_K - 0.5 * V) / (
         (1 + np.exp(0.5 * E_K - 0.5 * V)) * (1 + np.exp(0.5 * E_K - 0.5 * V))
     )
     di_CaL_dV = (
         4
         * g_CaL
         * (F * F)
         * (-Ca_o + 0.25 * Ca_ss * np.exp(F * (-30 + 2 * V) / (R * T)))
@@ -2196,39 +2079,30 @@
         dalpha_K1_dV * dxK1_inf_dalpha_K1 + dbeta_K1_dV * dxK1_inf_dbeta_K1
     )
     di_K1_dxK1_inf = 0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-E_K + V)
     di_Kr_dV = 0.4303314829119352 * g_Kr * np.sqrt(K_o) * Xr1 * Xr2
     di_Ks_dV = g_Ks * (Xs * Xs)
     di_Na_dV = g_Na * (m * m * m) * h * j
     di_NaCa_dV = K_NaCa * (
-        Ca_o
-        * F
-        * gamma
-        * (Na_i * Na_i * Na_i)
-        * np.exp(F * gamma * V / (R * T))
-        / (R * T)
+        Ca_o * F * gamma * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T)) / (R * T)
         - F
         * alpha
         * (Na_o * Na_o * Na_o)
         * (-1 + gamma)
         * Ca_i
         * np.exp(F * (-1 + gamma) * V / (R * T))
         / (R * T)
     ) / (
         (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
         * (Ca_o + Km_Ca)
         * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
-    ) - F * K_NaCa * K_sat * (
-        -1 + gamma
-    ) * (
+    ) - F * K_NaCa * K_sat * (-1 + gamma) * (
         Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
         - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
-    ) * np.exp(
-        F * (-1 + gamma) * V / (R * T)
-    ) / (
+    ) * np.exp(F * (-1 + gamma) * V / (R * T)) / (
         R
         * T
         * (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
         )
         * (Ca_o + Km_Ca)
@@ -2242,24 +2116,16 @@
             + 0.012450000000000001 * F * np.exp(-0.1 * F * V / (R * T)) / (R * T)
         )
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
             * (
-                (
-                    1
-                    + 0.0353 * np.exp(-F * V / (R * T))
-                    + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-                )
-                * (
-                    1
-                    + 0.0353 * np.exp(-F * V / (R * T))
-                    + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-                )
+                (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
+                * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
             )
         )
     )
     di_p_K_dV = g_pK / (
         1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V)
     ) + 10.937327047146876 * g_pK * (-E_K + V) * np.exp(-0.16722408026755853 * V) / (
         (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
@@ -2274,16 +2140,15 @@
         - di_Kr_dV
         - di_Ks_dV
         - di_NaCa_dV
         - di_NaK_dV
         - di_Na_dV
         - di_p_K_dV
         - di_to_dV
-        - (dalpha_K1_dV * dxK1_inf_dalpha_K1 + dbeta_K1_dV * dxK1_inf_dbeta_K1)
-        * di_K1_dxK1_inf
+        - (dalpha_K1_dV * dxK1_inf_dalpha_K1 + dbeta_K1_dV * dxK1_inf_dbeta_K1) * di_K1_dxK1_inf
     )
     states[17] = (
         np.where(
             np.abs(dV_dt_linearized) > 1e-08,
             (-1 + np.exp(dt * dV_dt_linearized)) * dV_dt / dV_dt_linearized,
             dt * dV_dt,
         )
@@ -2304,17 +2169,15 @@
     )
     dbeta_K1_dE_K = (
         -0.0006121208040160535 * np.exp(0.0002 * V - 0.0002 * E_K)
         - 0.036787944117144235 * np.exp(0.1 * V - 0.1 * E_K)
     ) / (1 + np.exp(0.5 * E_K - 0.5 * V)) - 0.5 * (
         0.36787944117144233 * np.exp(0.1 * V - 0.1 * E_K)
         + 3.0606040200802673 * np.exp(0.0002 * V - 0.0002 * E_K)
-    ) * np.exp(
-        0.5 * E_K - 0.5 * V
-    ) / (
+    ) * np.exp(0.5 * E_K - 0.5 * V) / (
         (1 + np.exp(0.5 * E_K - 0.5 * V)) * (1 + np.exp(0.5 * E_K - 0.5 * V))
     )
     di_K1_dE_K = -0.4303314829119352 * g_K1 * np.sqrt(
         K_o
     ) * xK1_inf + 0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-E_K + V) * (
         dalpha_K1_dE_K * dxK1_inf_dalpha_K1 + dbeta_K1_dE_K * dxK1_inf_dbeta_K1
     )
```

### Comparing `fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py` & `fenics_beat-0.0.4/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Gotran generated code for the "tentusscher_panfilov_2006_M_cell" model
+# Gotran generated code for the "tentusscher_panfilov_2006_endo_cell" model
 
 import numpy as np
 
 
 def init_state_values(**values):
     """
     Initialize state values
     """
     # Init values
-    # Xr1=0.0165, Xr2=0.473, Xs=0.0174, m=0.00165, h=0.749, j=0.6788,
-    # d=3.288e-05, f=0.7026, f2=0.9526, fCass=0.9942, s=0.999998,
-    # r=2.347e-08, Ca_i=0.000153, R_prime=0.8978, Ca_SR=4.272,
-    # Ca_ss=0.00042, Na_i=10.132, V=-85.423, K_i=138.52
+    # Xr1=0.00448, Xr2=0.476, Xs=0.0087, m=0.00155, h=0.7573, j=0.7225,
+    # d=3.164e-05, f=0.8009, f2=0.9778, fCass=0.9953, s=0.3212,
+    # r=2.235e-08, Ca_i=0.00013, R_prime=0.9068, Ca_SR=3.715,
+    # Ca_ss=0.00036, Na_i=10.355, V=-86.709, K_i=138.4
     init_values = np.array(
         [
-            0.0165,
-            0.473,
-            0.0174,
-            0.00165,
-            0.749,
-            0.6788,
-            3.288e-05,
-            0.7026,
-            0.9526,
-            0.9942,
-            0.999998,
-            2.347e-08,
-            0.000153,
-            0.8978,
-            4.272,
-            0.00042,
-            10.132,
-            -85.423,
-            138.52,
+            0.00448,
+            0.476,
+            0.0087,
+            0.00155,
+            0.7573,
+            0.7225,
+            3.164e-05,
+            0.8009,
+            0.9778,
+            0.9953,
+            0.3212,
+            2.235e-08,
+            0.00013,
+            0.9068,
+            3.715,
+            0.00036,
+            10.355,
+            -86.709,
+            138.4,
         ],
         dtype=np.float_,
     )
 
     # State indices and limit checker
     state_ind = dict(
         [
@@ -74,16 +74,16 @@
 
 
 def init_parameter_values(**values):
     """
     Initialize parameter values
     """
     # Param values
-    # P_kna=0.03, g_K1=5.405, g_Kr=0.153, g_Ks=0.098, g_Na=14.838,
-    # g_bna=0.00029, g_CaL=0.0398, g_bca=0.000592, g_to=0.294,
+    # P_kna=0.03, g_K1=5.405, g_Kr=0.153, g_Ks=0.392, g_Na=14.838,
+    # g_bna=0.00029, g_CaL=0.0398, g_bca=0.000592, g_to=0.073,
     # K_mNa=40.0, K_mk=1.0, P_NaK=2.724, K_NaCa=1000.0, K_sat=0.1,
     # Km_Ca=1.38, Km_Nai=87.5, alpha=2.5, gamma=0.35, K_pCa=0.0005,
     # g_pCa=0.1238, g_pK=0.0146, Buf_c=0.2, Buf_sr=10.0, Buf_ss=0.4,
     # Ca_o=2.0, EC=1.5, K_buf_c=0.001, K_buf_sr=0.3, K_buf_ss=0.00025,
     # K_up=0.00025, V_leak=0.00036, V_rel=0.102, V_sr=1094.0,
     # V_ss=54.68, V_xfer=0.0038, Vmax_up=0.006375, k1_prime=0.15,
     # k2_prime=0.045, k3=0.06, k4=0.005, max_sr=2.5, min_sr=1,
@@ -91,20 +91,20 @@
     # stim_amplitude=-52.0, stim_duration=1.0, stim_period=1000.0,
     # stim_start=10.0, K_o=5.4
     init_values = np.array(
         [
             0.03,
             5.405,
             0.153,
-            0.098,
+            0.392,
             14.838,
             0.00029,
             0.0398,
             0.000592,
-            0.294,
+            0.073,
             40.0,
             1.0,
             2.724,
             1000.0,
             0.1,
             1.38,
             87.5,
@@ -441,15 +441,15 @@
         return indices
     else:
         return indices[0]
 
 
 def rhs(states, t, parameters, values=None):
     """
-    Compute the right hand side of the tentusscher_panfilov_2006_M_cell ODE
+    Compute the right hand side of the tentusscher_panfilov_2006_endo_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -592,17 +592,15 @@
     values[3] = (-m + m_inf) / tau_m
 
     # Expressions for the h gate component
     h_inf = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    alpha_h = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    alpha_h = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     beta_h = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     tau_h = 1.0 / (alpha_h + beta_h)
     values[4] = (-h + h_inf) / tau_h
@@ -617,17 +615,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     beta_j = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     tau_j = 1.0 / (alpha_j + beta_j)
     values[5] = (-j + j_inf) / tau_j
 
     # Expressions for the Sodium background current component
     i_b_Na = g_bna * (-E_Na + V)
@@ -681,16 +677,16 @@
     # Expressions for the Calcium background current component
     i_b_Ca = g_bca * (-E_Ca + V)
 
     # Expressions for the Transient outward current component
     i_to = g_to * (-E_K + V) * r * s
 
     # Expressions for the s gate component
-    s_inf = 1.0 / (1 + np.exp(4 + V / 5))
-    tau_s = 3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
+    s_inf = 1.0 / (1 + np.exp(28 / 5 + V / 5))
+    tau_s = 8 + 1000 * np.exp(-((67 + V) * (67 + V)) / 1000)
     values[10] = (-s + s_inf) / tau_s
 
     # Expressions for the r gate component
     r_inf = 1.0 / (1 + np.exp(10 / 3 - V / 6))
     tau_r = 0.8 + 9.5 * np.exp(-((40 + V) * (40 + V)) / 1800)
     values[11] = (-r + r_inf) / tau_r
 
@@ -698,74 +694,59 @@
     i_NaK = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     i_NaCa = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     i_p_Ca = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
-    i_p_K = (
-        g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
-    )
+    i_p_K = g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     ddt_Ca_i_total = (
         V_sr * (-i_up + i_leak) / V_c
         + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
         + i_xfer
     )
     f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    f_JCa_sr_free = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    f_JCa_ss_free = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    f_JCa_sr_free = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    f_JCa_ss_free = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     values[12] = ddt_Ca_i_total * f_JCa_i_free
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     values[13] = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
     ddt_Ca_sr_total = -i_leak - i_rel + i_up
-    ddt_Ca_ss_total = (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    )
+    ddt_Ca_ss_total = V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
     values[14] = ddt_Ca_sr_total * f_JCa_sr_free
     values[15] = ddt_Ca_ss_total * f_JCa_ss_free
 
     # Expressions for the Sodium dynamics component
     values[16] = Cm * (-i_Na - i_b_Na - 3 * i_NaCa - 3 * i_NaK) / (F * V_c)
 
     # Expressions for the Membrane component
@@ -790,25 +771,24 @@
         - i_b_Na
         - i_p_Ca
         - i_p_K
         - i_to
     )
 
     # Expressions for the Potassium dynamics component
-    values[18] = (
-        Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
-    )
+    values[18] = Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
 
     # Return results
     return values
 
 
 def monitor(states, t, parameters, monitored=None):
     """
-    Computes monitored expressions of the tentusscher_panfilov_2006_M_cell ODE
+    Computes monitored expressions of the tentusscher_panfilov_2006_endo_cell\
+        ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -898,30 +878,24 @@
     # Expressions for the Reversal potentials component
     monitored[0] = R * T * np.log(Na_o / Na_i) / F
     monitored[1] = R * T * np.log(K_o / K_i) / F
     monitored[2] = R * T * np.log((K_o + Na_o * P_kna) / (P_kna * Na_i + K_i)) / F
     monitored[3] = 0.5 * R * T * np.log(Ca_o / Ca_i) / F
 
     # Expressions for the Inward rectifier potassium current component
-    monitored[4] = 0.1 / (
-        1 + 6.14421235332821e-06 * np.exp(0.06 * V - 0.06 * monitored[1])
-    )
+    monitored[4] = 0.1 / (1 + 6.14421235332821e-06 * np.exp(0.06 * V - 0.06 * monitored[1]))
     monitored[5] = (
         0.36787944117144233 * np.exp(0.1 * V - 0.1 * monitored[1])
         + 3.0606040200802673 * np.exp(0.0002 * V - 0.0002 * monitored[1])
     ) / (1 + np.exp(0.5 * monitored[1] - 0.5 * V))
     monitored[6] = monitored[4] / (monitored[4] + monitored[5])
-    monitored[7] = (
-        0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-monitored[1] + V) * monitored[6]
-    )
+    monitored[7] = 0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-monitored[1] + V) * monitored[6]
 
     # Expressions for the Rapid time dependent potassium current component
-    monitored[8] = (
-        0.4303314829119352 * g_Kr * np.sqrt(K_o) * (-monitored[1] + V) * Xr1 * Xr2
-    )
+    monitored[8] = 0.4303314829119352 * g_Kr * np.sqrt(K_o) * (-monitored[1] + V) * Xr1 * Xr2
 
     # Expressions for the Xr1 gate component
     monitored[9] = 1.0 / (1 + np.exp(-26 / 7 - V / 7))
     monitored[10] = 450 / (1 + np.exp(-9 / 2 - V / 10))
     monitored[11] = 6 / (1 + 13.581324522578193 * np.exp(0.08695652173913043 * V))
     monitored[12] = monitored[10] * monitored[11]
     monitored[73] = (-Xr1 + monitored[9]) / monitored[12]
@@ -957,17 +931,15 @@
     monitored[76] = (-m + monitored[23]) / monitored[26]
 
     # Expressions for the h gate component
     monitored[27] = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    monitored[28] = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    monitored[28] = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     monitored[29] = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     monitored[30] = 1.0 / (monitored[28] + monitored[29])
     monitored[77] = (-h + monitored[27]) / monitored[30]
@@ -982,17 +954,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     monitored[33] = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     monitored[34] = 1.0 / (monitored[32] + monitored[33])
     monitored[78] = (-j + monitored[31]) / monitored[34]
 
     # Expressions for the Sodium background current component
     monitored[35] = g_bna * (-monitored[0] + V)
@@ -1046,18 +1016,16 @@
     # Expressions for the Calcium background current component
     monitored[48] = g_bca * (-monitored[3] + V)
 
     # Expressions for the Transient outward current component
     monitored[49] = g_to * (-monitored[1] + V) * r * s
 
     # Expressions for the s gate component
-    monitored[50] = 1.0 / (1 + np.exp(4 + V / 5))
-    monitored[51] = (
-        3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
-    )
+    monitored[50] = 1.0 / (1 + np.exp(28 / 5 + V / 5))
+    monitored[51] = 8 + 1000 * np.exp(-((67 + V) * (67 + V)) / 1000)
     monitored[83] = (-s + monitored[50]) / monitored[51]
 
     # Expressions for the r gate component
     monitored[52] = 1.0 / (1 + np.exp(10 / 3 - V / 6))
     monitored[53] = 0.8 + 9.5 * np.exp(-((40 + V) * (40 + V)) / 1800)
     monitored[84] = (-r + monitored[52]) / monitored[53]
 
@@ -1065,91 +1033,73 @@
     monitored[54] = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     monitored[55] = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     monitored[56] = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
     monitored[57] = (
-        g_pK
-        * (-monitored[1] + V)
-        / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
+        g_pK * (-monitored[1] + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
     )
 
     # Expressions for the Calcium dynamics component
     monitored[58] = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     monitored[59] = V_leak * (-Ca_i + Ca_SR)
     monitored[60] = V_xfer * (-Ca_i + Ca_ss)
     monitored[61] = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     monitored[62] = (
         V_sr * (-monitored[58] + monitored[59]) / V_c
         + Cm * (-monitored[48] - monitored[56] + 2 * monitored[55]) / (2 * F * V_c)
         + monitored[60]
     )
     monitored[63] = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    monitored[64] = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    monitored[65] = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    monitored[64] = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    monitored[65] = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     monitored[85] = monitored[62] * monitored[63]
     monitored[66] = k1_prime / monitored[61]
     monitored[67] = k2_prime * monitored[61]
     monitored[68] = (
-        (Ca_ss * Ca_ss)
-        * R_prime
-        * monitored[66]
-        / (k3 + (Ca_ss * Ca_ss) * monitored[66])
+        (Ca_ss * Ca_ss) * R_prime * monitored[66] / (k3 + (Ca_ss * Ca_ss) * monitored[66])
     )
     monitored[86] = k4 * (1 - R_prime) - Ca_ss * R_prime * monitored[67]
     monitored[69] = V_rel * (-Ca_ss + Ca_SR) * monitored[68]
     monitored[70] = -monitored[59] - monitored[69] + monitored[58]
     monitored[71] = (
         V_sr * monitored[69] / V_ss
         - V_c * monitored[60] / V_ss
         - Cm * monitored[36] / (2 * F * V_ss)
     )
     monitored[87] = monitored[64] * monitored[70]
     monitored[88] = monitored[65] * monitored[71]
 
     # Expressions for the Sodium dynamics component
     monitored[89] = (
-        Cm
-        * (-monitored[22] - monitored[35] - 3 * monitored[54] - 3 * monitored[55])
-        / (F * V_c)
+        Cm * (-monitored[22] - monitored[35] - 3 * monitored[54] - 3 * monitored[55]) / (F * V_c)
     )
 
     # Expressions for the Membrane component
     monitored[72] = np.where(
         np.logical_and(
             t - stim_period * np.floor(t / stim_period) >= stim_start,
             t - stim_period * np.floor(t / stim_period) <= stim_duration + stim_start,
@@ -1191,15 +1141,15 @@
     # Return results
     return monitored
 
 
 def forward_explicit_euler(states, t, dt, parameters):
     """
     Compute a forward step using the explicit Euler scheme to the\
-        tentusscher_panfilov_2006_M_cell ODE
+        tentusscher_panfilov_2006_endo_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -1340,17 +1290,15 @@
     states[3] = dt * dm_dt + m
 
     # Expressions for the h gate component
     h_inf = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    alpha_h = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    alpha_h = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     beta_h = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     tau_h = 1.0 / (alpha_h + beta_h)
     dh_dt = (-h + h_inf) / tau_h
@@ -1366,17 +1314,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     beta_j = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     tau_j = 1.0 / (alpha_j + beta_j)
     dj_dt = (-j + j_inf) / tau_j
     states[5] = dt * dj_dt + j
 
     # Expressions for the Sodium background current component
@@ -1435,16 +1381,16 @@
     # Expressions for the Calcium background current component
     i_b_Ca = g_bca * (-E_Ca + V)
 
     # Expressions for the Transient outward current component
     i_to = g_to * (-E_K + V) * r * s
 
     # Expressions for the s gate component
-    s_inf = 1.0 / (1 + np.exp(4 + V / 5))
-    tau_s = 3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
+    s_inf = 1.0 / (1 + np.exp(28 / 5 + V / 5))
+    tau_s = 8 + 1000 * np.exp(-((67 + V) * (67 + V)) / 1000)
     ds_dt = (-s + s_inf) / tau_s
     states[10] = dt * ds_dt + s
 
     # Expressions for the r gate component
     r_inf = 1.0 / (1 + np.exp(10 / 3 - V / 6))
     tau_r = 0.8 + 9.5 * np.exp(-((40 + V) * (40 + V)) / 1800)
     dr_dt = (-r + r_inf) / tau_r
@@ -1454,76 +1400,61 @@
     i_NaK = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     i_NaCa = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     i_p_Ca = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
-    i_p_K = (
-        g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
-    )
+    i_p_K = g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     ddt_Ca_i_total = (
         V_sr * (-i_up + i_leak) / V_c
         + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
         + i_xfer
     )
     f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    f_JCa_sr_free = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    f_JCa_ss_free = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    f_JCa_sr_free = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    f_JCa_ss_free = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     dCa_i_dt = ddt_Ca_i_total * f_JCa_i_free
     states[12] = dt * dCa_i_dt + Ca_i
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     dR_prime_dt = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     states[13] = dt * dR_prime_dt + R_prime
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
     ddt_Ca_sr_total = -i_leak - i_rel + i_up
-    ddt_Ca_ss_total = (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    )
+    ddt_Ca_ss_total = V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
     dCa_SR_dt = ddt_Ca_sr_total * f_JCa_sr_free
     states[14] = dt * dCa_SR_dt + Ca_SR
     dCa_ss_dt = ddt_Ca_ss_total * f_JCa_ss_free
     states[15] = dt * dCa_ss_dt + Ca_ss
 
     # Expressions for the Sodium dynamics component
     dNa_i_dt = Cm * (-i_Na - i_b_Na - 3 * i_NaCa - 3 * i_NaK) / (F * V_c)
@@ -1562,15 +1493,15 @@
     # Return results
     return states
 
 
 def forward_generalized_rush_larsen(states, t, dt, parameters):
     """
     Compute a forward step using the generalised Rush-Larsen (GRL1) scheme to\
-        the tentusscher_panfilov_2006_M_cell ODE
+        the tentusscher_panfilov_2006_endo_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -1672,28 +1603,24 @@
     # Expressions for the Xr1 gate component
     xr1_inf = 1.0 / (1 + np.exp(-26 / 7 - V / 7))
     alpha_xr1 = 450 / (1 + np.exp(-9 / 2 - V / 10))
     beta_xr1 = 6 / (1 + 13.581324522578193 * np.exp(0.08695652173913043 * V))
     tau_xr1 = alpha_xr1 * beta_xr1
     dXr1_dt = (-Xr1 + xr1_inf) / tau_xr1
     dXr1_dt_linearized = -1 / tau_xr1
-    states[0] = (
-        -1 + np.exp(dt * dXr1_dt_linearized)
-    ) * dXr1_dt / dXr1_dt_linearized + Xr1
+    states[0] = (-1 + np.exp(dt * dXr1_dt_linearized)) * dXr1_dt / dXr1_dt_linearized + Xr1
 
     # Expressions for the Xr2 gate component
     xr2_inf = 1.0 / (1 + np.exp(11 / 3 + V / 24))
     alpha_xr2 = 3 / (1 + np.exp(-3 - V / 20))
     beta_xr2 = 1.12 / (1 + np.exp(-3 + V / 20))
     tau_xr2 = alpha_xr2 * beta_xr2
     dXr2_dt = (-Xr2 + xr2_inf) / tau_xr2
     dXr2_dt_linearized = -1 / tau_xr2
-    states[1] = (
-        -1 + np.exp(dt * dXr2_dt_linearized)
-    ) * dXr2_dt / dXr2_dt_linearized + Xr2
+    states[1] = (-1 + np.exp(dt * dXr2_dt_linearized)) * dXr2_dt / dXr2_dt_linearized + Xr2
 
     # Expressions for the Slow time dependent potassium current component
     i_Ks = g_Ks * (Xs * Xs) * (-E_Ks + V)
 
     # Expressions for the Xs gate component
     xs_inf = 1.0 / (1 + np.exp(-5 / 14 - V / 14))
     alpha_xs = 1400 / np.sqrt(1 + np.exp(5 / 6 - V / 6))
@@ -1719,17 +1646,15 @@
     states[3] = (-1 + np.exp(dt * dm_dt_linearized)) * dm_dt / dm_dt_linearized + m
 
     # Expressions for the h gate component
     h_inf = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
-    alpha_h = np.where(
-        V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0
-    )
+    alpha_h = np.where(V < -40, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * V), 0)
     beta_h = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     tau_h = 1.0 / (alpha_h + beta_h)
     dh_dt = (-h + h_inf) / tau_h
@@ -1746,17 +1671,15 @@
         (37.78 + V)
         * (-25428 * np.exp(0.2444 * V) - 6.948e-06 * np.exp(-0.04391 * V))
         / (1 + 50262745825.95399 * np.exp(0.311 * V)),
         0,
     )
     beta_j = np.where(
         V < -40,
-        0.02424
-        * np.exp(-0.01052 * V)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
+        0.02424 * np.exp(-0.01052 * V) / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     tau_j = 1.0 / (alpha_j + beta_j)
     dj_dt = (-j + j_inf) / tau_j
     dj_dt_linearized = -1 / tau_j
     states[5] = (-1 + np.exp(dt * dj_dt_linearized)) * dj_dt / dj_dt_linearized + j
 
@@ -1811,27 +1734,25 @@
     states[8] = (-1 + np.exp(dt * df2_dt_linearized)) * df2_dt / df2_dt_linearized + f2
 
     # Expressions for the FCass gate component
     fCass_inf = 0.4 + 0.6 / (1 + 400.0 * (Ca_ss * Ca_ss))
     tau_fCass = 2 + 80 / (1 + 400.0 * (Ca_ss * Ca_ss))
     dfCass_dt = (-fCass + fCass_inf) / tau_fCass
     dfCass_dt_linearized = -1 / tau_fCass
-    states[9] = (
-        -1 + np.exp(dt * dfCass_dt_linearized)
-    ) * dfCass_dt / dfCass_dt_linearized + fCass
+    states[9] = (-1 + np.exp(dt * dfCass_dt_linearized)) * dfCass_dt / dfCass_dt_linearized + fCass
 
     # Expressions for the Calcium background current component
     i_b_Ca = g_bca * (-E_Ca + V)
 
     # Expressions for the Transient outward current component
     i_to = g_to * (-E_K + V) * r * s
 
     # Expressions for the s gate component
-    s_inf = 1.0 / (1 + np.exp(4 + V / 5))
-    tau_s = 3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
+    s_inf = 1.0 / (1 + np.exp(28 / 5 + V / 5))
+    tau_s = 8 + 1000 * np.exp(-((67 + V) * (67 + V)) / 1000)
     ds_dt = (-s + s_inf) / tau_s
     ds_dt_linearized = -1 / tau_s
     states[10] = (-1 + np.exp(dt * ds_dt_linearized)) * ds_dt / ds_dt_linearized + s
 
     # Expressions for the r gate component
     r_inf = 1.0 / (1 + np.exp(10 / 3 - V / 6))
     tau_r = 0.8 + 9.5 * np.exp(-((40 + V) * (40 + V)) / 1800)
@@ -1843,64 +1764,51 @@
     i_NaK = (
         K_o
         * P_NaK
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
-            * (
-                1
-                + 0.0353 * np.exp(-F * V / (R * T))
-                + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-            )
+            * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
         )
     )
 
     # Expressions for the Sodium calcium exchanger current component
     i_NaCa = (
         K_NaCa
         * (
             Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
-            - alpha
-            * (Na_o * Na_o * Na_o)
-            * Ca_i
-            * np.exp(F * (-1 + gamma) * V / (R * T))
+            - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
         )
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
 
     # Expressions for the Calcium pump current component
     i_p_Ca = g_pCa * Ca_i / (K_pCa + Ca_i)
 
     # Expressions for the Potassium pump current component
-    i_p_K = (
-        g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
-    )
+    i_p_K = g_pK * (-E_K + V) / (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
     ddt_Ca_i_total = (
         V_sr * (-i_up + i_leak) / V_c
         + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
         + i_xfer
     )
     f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    f_JCa_sr_free = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
-    )
-    f_JCa_ss_free = 1.0 / (
-        1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
-    )
+    f_JCa_sr_free = 1.0 / (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
+    f_JCa_ss_free = 1.0 / (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
     dCa_i_dt = ddt_Ca_i_total * f_JCa_i_free
     dE_Ca_dCa_i = -0.5 * R * T / (F * Ca_i)
     dddt_Ca_i_total_di_NaCa = Cm / (F * V_c)
     dddt_Ca_i_total_di_b_Ca = -Cm / (2 * F * V_c)
     dddt_Ca_i_total_di_leak = V_sr / V_c
     dddt_Ca_i_total_di_p_Ca = -Cm / (2 * F * V_c)
     dddt_Ca_i_total_di_up = -V_sr / V_c
@@ -1923,17 +1831,15 @@
         * np.exp(F * (-1 + gamma) * V / (R * T))
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
-    di_p_Ca_dCa_i = g_pCa / (K_pCa + Ca_i) - g_pCa * Ca_i / (
-        (K_pCa + Ca_i) * (K_pCa + Ca_i)
-    )
+    di_p_Ca_dCa_i = g_pCa / (K_pCa + Ca_i) - g_pCa * Ca_i / ((K_pCa + Ca_i) * (K_pCa + Ca_i))
     di_up_dCa_i = (
         2
         * Vmax_up
         * (K_up * K_up)
         / (
             ((1 + (K_up * K_up) / (Ca_i * Ca_i)) * (1 + (K_up * K_up) / (Ca_i * Ca_i)))
             * (Ca_i * Ca_i * Ca_i)
@@ -1956,26 +1862,22 @@
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     dR_prime_dt = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     dR_prime_dt_linearized = -k4 - Ca_ss * k2
     states[13] = (
         np.where(
             np.abs(dR_prime_dt_linearized) > 1e-08,
-            (-1 + np.exp(dt * dR_prime_dt_linearized))
-            * dR_prime_dt
-            / dR_prime_dt_linearized,
+            (-1 + np.exp(dt * dR_prime_dt_linearized)) * dR_prime_dt / dR_prime_dt_linearized,
             dt * dR_prime_dt,
         )
         + R_prime
     )
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
     ddt_Ca_sr_total = -i_leak - i_rel + i_up
-    ddt_Ca_ss_total = (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    )
+    ddt_Ca_ss_total = V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
     dCa_SR_dt = ddt_Ca_sr_total * f_JCa_sr_free
     dO_dk1 = (Ca_ss * Ca_ss) * R_prime / (k3 + (Ca_ss * Ca_ss) * k1) - np.power(
         Ca_ss, 4
     ) * R_prime * k1 / ((k3 + (Ca_ss * Ca_ss) * k1) * (k3 + (Ca_ss * Ca_ss) * k1))
     df_JCa_sr_free_dCa_SR = (
         2
         * Buf_sr
@@ -1994,17 +1896,15 @@
         * (EC * EC)
         * (max_sr - min_sr)
         / (
             ((1 + (EC * EC) / (Ca_SR * Ca_SR)) * (1 + (EC * EC) / (Ca_SR * Ca_SR)))
             * (Ca_SR * Ca_SR * Ca_SR)
         )
     )
-    di_rel_dCa_SR = (
-        V_rel * O + V_rel * (-Ca_ss + Ca_SR) * dO_dk1 * dk1_dkcasr * dkcasr_dCa_SR
-    )
+    di_rel_dCa_SR = V_rel * O + V_rel * (-Ca_ss + Ca_SR) * dO_dk1 * dk1_dkcasr * dkcasr_dCa_SR
     di_rel_dO = V_rel * (-Ca_ss + Ca_SR)
     dCa_SR_dt_linearized = (
         -V_leak - di_rel_dCa_SR - dO_dk1 * di_rel_dO * dk1_dkcasr * dkcasr_dCa_SR
     ) * f_JCa_sr_free + ddt_Ca_sr_total * df_JCa_sr_free_dCa_SR
     states[14] = Ca_SR + np.where(
         np.abs(dCa_SR_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCa_SR_dt_linearized)) * dCa_SR_dt / dCa_SR_dt_linearized,
@@ -2068,36 +1968,23 @@
             * (Ca_o + Km_Ca)
             * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
         )
     )
     di_NaK_dNa_i = K_o * P_NaK / (
         (K_mNa + Na_i)
         * (K_mk + K_o)
-        * (
-            1
-            + 0.0353 * np.exp(-F * V / (R * T))
-            + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-        )
+        * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
     ) - K_o * P_NaK * Na_i / (
         ((K_mNa + Na_i) * (K_mNa + Na_i))
         * (K_mk + K_o)
-        * (
-            1
-            + 0.0353 * np.exp(-F * V / (R * T))
-            + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-        )
+        * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
     )
     dNa_i_dt_linearized = (
         Cm
-        * (
-            -3 * di_NaCa_dNa_i
-            - 3 * di_NaK_dNa_i
-            + g_bna * dE_Na_dNa_i
-            - dE_Na_dNa_i * di_Na_dE_Na
-        )
+        * (-3 * di_NaCa_dNa_i - 3 * di_NaK_dNa_i + g_bna * dE_Na_dNa_i - dE_Na_dNa_i * di_Na_dE_Na)
         / (F * V_c)
     )
     states[16] = Na_i + np.where(
         np.abs(dNa_i_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dNa_i_dt_linearized)) * dNa_i_dt / dNa_i_dt_linearized,
         dt * dNa_i_dt,
     )
@@ -2136,17 +2023,15 @@
     )
     dbeta_K1_dV = (
         0.0006121208040160535 * np.exp(0.0002 * V - 0.0002 * E_K)
         + 0.036787944117144235 * np.exp(0.1 * V - 0.1 * E_K)
     ) / (1 + np.exp(0.5 * E_K - 0.5 * V)) + 0.5 * (
         0.36787944117144233 * np.exp(0.1 * V - 0.1 * E_K)
         + 3.0606040200802673 * np.exp(0.0002 * V - 0.0002 * E_K)
-    ) * np.exp(
-        0.5 * E_K - 0.5 * V
-    ) / (
+    ) * np.exp(0.5 * E_K - 0.5 * V) / (
         (1 + np.exp(0.5 * E_K - 0.5 * V)) * (1 + np.exp(0.5 * E_K - 0.5 * V))
     )
     di_CaL_dV = (
         4
         * g_CaL
         * (F * F)
         * (-Ca_o + 0.25 * Ca_ss * np.exp(F * (-30 + 2 * V) / (R * T)))
@@ -2195,39 +2080,30 @@
         dalpha_K1_dV * dxK1_inf_dalpha_K1 + dbeta_K1_dV * dxK1_inf_dbeta_K1
     )
     di_K1_dxK1_inf = 0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-E_K + V)
     di_Kr_dV = 0.4303314829119352 * g_Kr * np.sqrt(K_o) * Xr1 * Xr2
     di_Ks_dV = g_Ks * (Xs * Xs)
     di_Na_dV = g_Na * (m * m * m) * h * j
     di_NaCa_dV = K_NaCa * (
-        Ca_o
-        * F
-        * gamma
-        * (Na_i * Na_i * Na_i)
-        * np.exp(F * gamma * V / (R * T))
-        / (R * T)
+        Ca_o * F * gamma * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T)) / (R * T)
         - F
         * alpha
         * (Na_o * Na_o * Na_o)
         * (-1 + gamma)
         * Ca_i
         * np.exp(F * (-1 + gamma) * V / (R * T))
         / (R * T)
     ) / (
         (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
         * (Ca_o + Km_Ca)
         * ((Km_Nai * Km_Nai * Km_Nai) + (Na_o * Na_o * Na_o))
-    ) - F * K_NaCa * K_sat * (
-        -1 + gamma
-    ) * (
+    ) - F * K_NaCa * K_sat * (-1 + gamma) * (
         Ca_o * (Na_i * Na_i * Na_i) * np.exp(F * gamma * V / (R * T))
         - alpha * (Na_o * Na_o * Na_o) * Ca_i * np.exp(F * (-1 + gamma) * V / (R * T))
-    ) * np.exp(
-        F * (-1 + gamma) * V / (R * T)
-    ) / (
+    ) * np.exp(F * (-1 + gamma) * V / (R * T)) / (
         R
         * T
         * (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
             * (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
         )
         * (Ca_o + Km_Ca)
@@ -2241,24 +2117,16 @@
             + 0.012450000000000001 * F * np.exp(-0.1 * F * V / (R * T)) / (R * T)
         )
         * Na_i
         / (
             (K_mNa + Na_i)
             * (K_mk + K_o)
             * (
-                (
-                    1
-                    + 0.0353 * np.exp(-F * V / (R * T))
-                    + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-                )
-                * (
-                    1
-                    + 0.0353 * np.exp(-F * V / (R * T))
-                    + 0.1245 * np.exp(-0.1 * F * V / (R * T))
-                )
+                (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
+                * (1 + 0.0353 * np.exp(-F * V / (R * T)) + 0.1245 * np.exp(-0.1 * F * V / (R * T)))
             )
         )
     )
     di_p_K_dV = g_pK / (
         1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V)
     ) + 10.937327047146876 * g_pK * (-E_K + V) * np.exp(-0.16722408026755853 * V) / (
         (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
@@ -2273,16 +2141,15 @@
         - di_Kr_dV
         - di_Ks_dV
         - di_NaCa_dV
         - di_NaK_dV
         - di_Na_dV
         - di_p_K_dV
         - di_to_dV
-        - (dalpha_K1_dV * dxK1_inf_dalpha_K1 + dbeta_K1_dV * dxK1_inf_dbeta_K1)
-        * di_K1_dxK1_inf
+        - (dalpha_K1_dV * dxK1_inf_dalpha_K1 + dbeta_K1_dV * dxK1_inf_dbeta_K1) * di_K1_dxK1_inf
     )
     states[17] = (
         np.where(
             np.abs(dV_dt_linearized) > 1e-08,
             (-1 + np.exp(dt * dV_dt_linearized)) * dV_dt / dV_dt_linearized,
             dt * dV_dt,
         )
@@ -2303,17 +2170,15 @@
     )
     dbeta_K1_dE_K = (
         -0.0006121208040160535 * np.exp(0.0002 * V - 0.0002 * E_K)
         - 0.036787944117144235 * np.exp(0.1 * V - 0.1 * E_K)
     ) / (1 + np.exp(0.5 * E_K - 0.5 * V)) - 0.5 * (
         0.36787944117144233 * np.exp(0.1 * V - 0.1 * E_K)
         + 3.0606040200802673 * np.exp(0.0002 * V - 0.0002 * E_K)
-    ) * np.exp(
-        0.5 * E_K - 0.5 * V
-    ) / (
+    ) * np.exp(0.5 * E_K - 0.5 * V) / (
         (1 + np.exp(0.5 * E_K - 0.5 * V)) * (1 + np.exp(0.5 * E_K - 0.5 * V))
     )
     di_K1_dE_K = -0.4303314829119352 * g_K1 * np.sqrt(
         K_o
     ) * xK1_inf + 0.4303314829119352 * g_K1 * np.sqrt(K_o) * (-E_K + V) * (
         dalpha_K1_dE_K * dxK1_inf_dalpha_K1 + dbeta_K1_dE_K * dxK1_inf_dbeta_K1
     )
```

### Comparing `fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/endo.py` & `fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/endo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1193,17 +1193,15 @@
     E1_i = x1_i / (x1_i + x2_i + x3_i + x4_i)
     E2_i = x2_i / (x1_i + x2_i + x3_i + x4_i)
     E3_i = x3_i / (x1_i + x2_i + x3_i + x4_i)
     E4_i = x4_i / (x1_i + x2_i + x3_i + x4_i)
     allo_i = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     JncxNa_i = E3_i * k4pp_i - E2_i * k3pp_i - 3 * E1_i * k8_i + 3 * E4_i * k7_i
     JncxCa_i = E2_i * k2_i - E1_i * k1_i
-    Gncx = np.where(
-        celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b)
-    )
+    Gncx = np.where(celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b))
     INaCa_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx * allo_i
     h1_ss = 1 + (1 + hna) * nass / kna3
     h2_ss = hna * nass / (kna3 * h1_ss)
     h3_ss = 1.0 / h1_ss
     h4_ss = 1 + (1 + nass / kna2) * nass / kna1
     h5_ss = (nass * nass) / (kna1 * kna2 * h4_ss)
     h6_ss = 1.0 / h4_ss
@@ -1230,17 +1228,15 @@
     x3_ss = (k2_ss + k3_ss) * k6_ss * k8_ss + (k6_ss + k7_ss) * k1_ss * k3_ss
     x4_ss = (k1_ss + k8_ss) * k3_ss * k5_ss + (k4_ss + k5_ss) * k2_ss * k8_ss
     E1_ss = x1_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E2_ss = x2_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E3_ss = x3_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E4_ss = x4_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     allo_ss = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
-    JncxNa_ss = (
-        E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
-    )
+    JncxNa_ss = E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
     JncxCa_ss = E2_ss * k2_ss - E1_ss * k1_ss
     INaCa_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx * allo_ss
 
     # Expressions for the K component
     Knai = Knai0 * np.exp(delta * vfrt / 3)
     Knao = Knao0 * np.exp((1 - delta) * vfrt / 3)
     P = eP / (1 + H / Khp + nai / Knap + ki / Kxkur)
@@ -1302,17 +1298,15 @@
     x4 = a1 * a3 * a4 + a1 * a4 * b2 + a1 * b2 * b3 + b2 * b3 * b4
     E1 = x1 / (x1 + x2 + x3 + x4)
     E2 = x2 / (x1 + x2 + x3 + x4)
     E3 = x3 / (x1 + x2 + x3 + x4)
     E4 = x4 / (x1 + x2 + x3 + x4)
     JnakNa = -3 * E2 * b3 + 3 * E1 * a3
     JnakK = -2 * E3 * a1 + 2 * E4 * b1
-    Pnak = np.where(
-        celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
-    )
+    Pnak = np.where(celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b))
     INaK = (zk * JnakK + zna * JnakNa) * Pnak
 
     # Expressions for the b component
     INab = PNab * (-nao + np.exp(vfrt) * nai) * vffrt / (-1 + np.exp(vfrt))
 
     # Expressions for the ICaL component
     dss = np.where(v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v)))
@@ -1324,17 +1318,15 @@
             3.5254214873653824 * np.exp(0.09 * vShift + 0.09 * v)
             + 0.7408182206817179 * np.exp(-0.05 * vShift - 0.05 * v)
         )
     )
     values[1] = (-d + dss) / td
     fss = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
     tff = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
-    tfs = 1000 + 1.0 / (
-        3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
-    )
+    tfs = 1000 + 1.0 / (3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6))
     Afs = 1 - Aff
     values[2] = (-ff + fss) / tff
     values[3] = (-fs + fss) / tfs
     f = Aff * ff + Afs * fs
     fcass = fss
     tfcaf = 7 + 1.0 / (0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7))
     tfcas = 100 + 1.0 / (0.00012 * np.exp(-v / 3) + 0.00012 * np.exp(v / 7))
@@ -1365,25 +1357,17 @@
     gamma_ko = np.exp(-(-0.3 * Io + np.sqrt(Io) / (1 + np.sqrt(Io))) * constA)
     PhiCaL_ss = (
         4
         * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_ss = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_ss = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
-    )
-    PCa = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    PhiCaNa_ss = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_ss = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
+    PCa = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     PCap = 1.1 * PCa
     PCaNa = 0.00125 * PCa
     PCaK = 0.0003574 * PCa
     PCaNap = 0.00125 * PCap
     PCaKp = 0.0003574 * PCap
     fICaLp = 1.0 / (1 + KmCaMK / CaMKa)
     ICaL_ss = ICaL_fractionSS * (
@@ -1406,22 +1390,16 @@
     gamma_ki = np.exp(-(-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     PhiCaL_i = (
         4
         * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_i = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_i = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
-    )
+    PhiCaNa_i = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_i = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
     ICaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * PhiCaL_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * PhiCaL_i * d * fICaLp
     )
     ICaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * PhiCaNa_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * PhiCaNa_i * d * fICaLp
@@ -1464,17 +1442,15 @@
         )
     )
     values[11] = (-m + mss) / tm
     hss = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    ah = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    ah = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     bh = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     th = 1.0 / (ah + bh)
     values[12] = (-h + hss) / th
@@ -1484,17 +1460,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     bj = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     jss = hss
     tj = 1.0 / (aj + bj)
     values[13] = (-j + jss) / tj
     hssp = 1.0 / (
         (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
         * (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
@@ -1526,74 +1500,54 @@
     values[18] = (-hLp + hLssp) / thLp
     GNaL = np.where(celltype == 1, 0.6 * GNaL_b, GNaL_b)
     fINaLp = 1.0 / (1 + KmCaMK / CaMKa)
     INaL = (-ENa + v) * ((1 - fINaLp) * hL + fINaLp * hLp) * GNaL * mL
 
     # Expressions for the Ito component
     ass = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     ta = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     values[19] = (-a + ass) / ta
     iss = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    delta_epi = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    delta_epi = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     tiF_b = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     tiS_b = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     tiF = delta_epi * tiF_b
     tiS = delta_epi * tiS_b
     AiF = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     AiS = 1 - AiF
     values[20] = (-iF + iss) / tiF
     values[21] = (-iS + iss) / tiS
     i = AiF * iF + AiS * iS
     assp = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     values[22] = (-ap + assp) / ta
     dti_develop = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
     dti_recover = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     tiFp = dti_develop * dti_recover * tiF
     tiSp = dti_develop * dti_recover * tiS
     values[23] = (-iFp + iss) / tiFp
     values[24] = (-iSp + iss) / tiSp
     ip = AiF * iFp + AiS * iSp
@@ -1608,53 +1562,42 @@
     beta_2 = 0.000349 * np.exp(-1.062 * vfrt)
     alpha_i = 0.2533 * np.exp(0.5953 * vfrt)
     beta_i = 0.06525 * np.exp(-0.8209 * vfrt)
     alpha_C2ToI = 5.2e-05 * np.exp(1.525 * vfrt)
     beta_ItoC2 = alpha_C2ToI * beta_2 * beta_i / (alpha_2 * alpha_i)
     values[25] = C2 * beta - C3 * alpha
     values[26] = beta_1 * C1 + C3 * alpha - (alpha_1 + beta) * C2
-    values[27] = (
-        alpha_1 * C2
-        + I * beta_ItoC2
-        + O * beta_2
-        - (beta_1 + alpha_2 + alpha_C2ToI) * C1
-    )
+    values[27] = alpha_1 * C2 + I * beta_ItoC2 + O * beta_2 - (beta_1 + alpha_2 + alpha_C2ToI) * C1
     values[28] = C1 * alpha_2 + I * beta_i - (alpha_i + beta_2) * O
     values[29] = C1 * alpha_C2ToI + O * alpha_i - (beta_ItoC2 + beta_i) * I
-    GKr = np.where(
-        celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
-    )
+    GKr = np.where(celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b))
     IKr = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GKr * O / 5
 
     # Expressions for the IKs component
     xs1ss = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     txs1 = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
     values[30] = (-xs1 + xs1ss) / txs1
     xs2ss = xs1ss
-    txs2 = 1.0 / (
-        0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20)
-    )
+    txs2 = 1.0 / (0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20))
     values[31] = (-xs2 + xs2ss) / txs2
     KsCa = 1 + 0.6 / (1 + 6.481821026062645e-07 * np.power(1.0 / cai, 1.4))
     GKs = np.where(celltype == 1, 1.4 * GKs_b, GKs_b)
     IKs = (-EKs + v) * GKs * KsCa * xs1 * xs2
 
     # Expressions for the IK1 component
     aK1 = 4.094 / (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
     bK1 = (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     K1ss = aK1 / (aK1 + bK1)
-    GK1 = np.where(
-        celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
-    )
+    GK1 = np.where(celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b))
     IK1 = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 * K1ss / 5
 
     # Expressions for the IKb component
     xkb = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     GKb = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     IKb = (-EK + v) * GKb * xkb
 
@@ -1690,17 +1633,15 @@
     fJrelp = 1.0 / (1 + KmCaMK / CaMKa)
     Jrel = Jrel_b * ((1 - fJrelp) * Jrel_np + Jrel_p * fJrelp)
 
     # Expressions for the Membrane component
     Istim = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     values[34] = (
         -ICaK
@@ -2009,26 +1950,18 @@
     ) * monitored[47] * monitored[57]
     monitored[61] = (monitored[48] + monitored[51]) * monitored[56] * monitored[58] + (
         monitored[56] + monitored[57]
     ) * monitored[47] * monitored[51]
     monitored[62] = (monitored[47] + monitored[58]) * monitored[51] * monitored[55] + (
         monitored[54] + monitored[55]
     ) * monitored[48] * monitored[58]
-    monitored[63] = monitored[59] / (
-        monitored[59] + monitored[60] + monitored[61] + monitored[62]
-    )
-    monitored[64] = monitored[60] / (
-        monitored[59] + monitored[60] + monitored[61] + monitored[62]
-    )
-    monitored[65] = monitored[61] / (
-        monitored[59] + monitored[60] + monitored[61] + monitored[62]
-    )
-    monitored[66] = monitored[62] / (
-        monitored[59] + monitored[60] + monitored[61] + monitored[62]
-    )
+    monitored[63] = monitored[59] / (monitored[59] + monitored[60] + monitored[61] + monitored[62])
+    monitored[64] = monitored[60] / (monitored[59] + monitored[60] + monitored[61] + monitored[62])
+    monitored[65] = monitored[61] / (monitored[59] + monitored[60] + monitored[61] + monitored[62])
+    monitored[66] = monitored[62] / (monitored[59] + monitored[60] + monitored[61] + monitored[62])
     monitored[67] = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     monitored[68] = (
         monitored[53] * monitored[65]
         - monitored[50] * monitored[64]
         - 3 * monitored[58] * monitored[63]
         + 3 * monitored[57] * monitored[66]
     )
@@ -2074,26 +2007,18 @@
     ) * monitored[84] * monitored[94]
     monitored[98] = (monitored[85] + monitored[88]) * monitored[93] * monitored[95] + (
         monitored[93] + monitored[94]
     ) * monitored[84] * monitored[88]
     monitored[99] = (monitored[84] + monitored[95]) * monitored[88] * monitored[92] + (
         monitored[91] + monitored[92]
     ) * monitored[85] * monitored[95]
-    monitored[100] = monitored[96] / (
-        monitored[96] + monitored[97] + monitored[98] + monitored[99]
-    )
-    monitored[101] = monitored[97] / (
-        monitored[96] + monitored[97] + monitored[98] + monitored[99]
-    )
-    monitored[102] = monitored[98] / (
-        monitored[96] + monitored[97] + monitored[98] + monitored[99]
-    )
-    monitored[103] = monitored[99] / (
-        monitored[96] + monitored[97] + monitored[98] + monitored[99]
-    )
+    monitored[100] = monitored[96] / (monitored[96] + monitored[97] + monitored[98] + monitored[99])
+    monitored[101] = monitored[97] / (monitored[96] + monitored[97] + monitored[98] + monitored[99])
+    monitored[102] = monitored[98] / (monitored[96] + monitored[97] + monitored[98] + monitored[99])
+    monitored[103] = monitored[99] / (monitored[96] + monitored[97] + monitored[98] + monitored[99])
     monitored[104] = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
     monitored[105] = (
         monitored[102] * monitored[90]
         - monitored[101] * monitored[87]
         - 3 * monitored[100] * monitored[95]
         + 3 * monitored[103] * monitored[94]
     )
@@ -2209,62 +2134,52 @@
     )
     monitored[125] = monitored[121] / (
         monitored[119] + monitored[120] + monitored[121] + monitored[122]
     )
     monitored[126] = monitored[122] / (
         monitored[119] + monitored[120] + monitored[121] + monitored[122]
     )
-    monitored[127] = (
-        -3 * monitored[116] * monitored[124] + 3 * monitored[115] * monitored[123]
-    )
-    monitored[128] = (
-        -2 * monitored[111] * monitored[125] + 2 * monitored[112] * monitored[126]
-    )
+    monitored[127] = -3 * monitored[116] * monitored[124] + 3 * monitored[115] * monitored[123]
+    monitored[128] = -2 * monitored[111] * monitored[125] + 2 * monitored[112] * monitored[126]
     monitored[129] = np.where(
         celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
     )
     monitored[130] = (zk * monitored[128] + zna * monitored[127]) * monitored[129]
 
     # Expressions for the b component
     monitored[131] = (
         PNab
         * (-nao + np.exp(monitored[274]) * nai)
         * monitored[273]
         / (-1 + np.exp(monitored[274]))
     )
 
     # Expressions for the ICaL component
-    monitored[140] = np.where(
-        v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v))
-    )
+    monitored[140] = np.where(v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v)))
     monitored[141] = (
         0.6
         + offset
         + 1.0
         / (
             3.5254214873653824 * np.exp(0.09 * vShift + 0.09 * v)
             + 0.7408182206817179 * np.exp(-0.05 * vShift - 0.05 * v)
         )
     )
     monitored[277] = (-d + monitored[140]) / monitored[141]
     monitored[142] = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
-    monitored[143] = 7 + 1.0 / (
-        0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10)
-    )
+    monitored[143] = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
     monitored[144] = 1000 + 1.0 / (
         3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
     )
     monitored[145] = 1 - Aff
     monitored[278] = (-ff + monitored[142]) / monitored[143]
     monitored[279] = (-fs + monitored[142]) / monitored[144]
     monitored[146] = Aff * ff + fs * monitored[145]
     monitored[147] = monitored[142]
-    monitored[148] = 7 + 1.0 / (
-        0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7)
-    )
+    monitored[148] = 7 + 1.0 / (0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7))
     monitored[149] = 100 + 1.0 / (0.00012 * np.exp(-v / 3) + 0.00012 * np.exp(v / 7))
     monitored[150] = 0.3 + 0.6 / (1 + np.exp(-1 + v / 10))
     monitored[151] = 1 - monitored[150]
     monitored[280] = (-fcaf + monitored[147]) / monitored[148]
     monitored[281] = (-fcas + monitored[147]) / monitored[149]
     monitored[152] = fcaf * monitored[150] + fcas * monitored[151]
     monitored[153] = 1.0 / (1.0 + 649.7401897235336 * np.exp(0.35821750967187277 * v))
@@ -2279,54 +2194,36 @@
     monitored[159] = 1.0 / (np.power(1 + Kmn / cass, 4) + k2n / monitored[158])
     monitored[285] = k2n * monitored[159] - monitored[158] * nca_ss
     monitored[160] = 0.0005 * clo + 0.0005 * ko + 0.0005 * nao + 0.002 * cao
     monitored[161] = 0.0005 * clss + 0.0005 * kss + 0.0005 * nass + 0.002 * cass
     monitored[162] = 1820000.0 * np.power(T * dielConstant, -1.5)
     monitored[163] = np.exp(
         -4
-        * (
-            -0.3 * monitored[161]
-            + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161]))
-        )
+        * (-0.3 * monitored[161] + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161])))
         * monitored[162]
     )
     monitored[164] = np.exp(
         -4
-        * (
-            -0.3 * monitored[160]
-            + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160]))
-        )
+        * (-0.3 * monitored[160] + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160])))
         * monitored[162]
     )
     monitored[165] = np.exp(
-        -(
-            -0.3 * monitored[161]
-            + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161]))
-        )
+        -(-0.3 * monitored[161] + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161])))
         * monitored[162]
     )
     monitored[166] = np.exp(
-        -(
-            -0.3 * monitored[160]
-            + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160]))
-        )
+        -(-0.3 * monitored[160] + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160])))
         * monitored[162]
     )
     monitored[167] = np.exp(
-        -(
-            -0.3 * monitored[161]
-            + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161]))
-        )
+        -(-0.3 * monitored[161] + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161])))
         * monitored[162]
     )
     monitored[168] = np.exp(
-        -(
-            -0.3 * monitored[160]
-            + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160]))
-        )
+        -(-0.3 * monitored[160] + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160])))
         * monitored[162]
     )
     monitored[169] = (
         4
         * (-cao * monitored[164] + cass * np.exp(2 * monitored[274]) * monitored[163])
         * monitored[273]
         / (-1 + np.exp(2 * monitored[274]))
@@ -2337,17 +2234,15 @@
         / (-1 + np.exp(monitored[274]))
     )
     monitored[171] = (
         (-ko * monitored[168] + np.exp(monitored[274]) * kss * monitored[167])
         * monitored[273]
         / (-1 + np.exp(monitored[274]))
     )
-    monitored[172] = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    monitored[172] = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     monitored[173] = 1.1 * monitored[172]
     monitored[174] = 0.00125 * monitored[172]
     monitored[175] = 0.0003574 * monitored[172]
     monitored[176] = 0.00125 * monitored[173]
     monitored[177] = 0.0003574 * monitored[173]
     monitored[178] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[179] = ICaL_fractionSS * (
@@ -2387,32 +2282,23 @@
         * monitored[178]
     )
     monitored[182] = 1.0 / (np.power(1 + Kmn / cai, 4) + k2n / monitored[158])
     monitored[286] = k2n * monitored[182] - monitored[158] * nca_i
     monitored[183] = 0.0005 * cli + 0.0005 * ki + 0.0005 * nai + 0.002 * cai
     monitored[184] = np.exp(
         -4
-        * (
-            -0.3 * monitored[183]
-            + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183]))
-        )
+        * (-0.3 * monitored[183] + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183])))
         * monitored[162]
     )
     monitored[185] = np.exp(
-        -(
-            -0.3 * monitored[183]
-            + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183]))
-        )
+        -(-0.3 * monitored[183] + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183])))
         * monitored[162]
     )
     monitored[186] = np.exp(
-        -(
-            -0.3 * monitored[183]
-            + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183]))
-        )
+        -(-0.3 * monitored[183] + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183])))
         * monitored[162]
     )
     monitored[187] = (
         4
         * (-cao * monitored[164] + cai * np.exp(2 * monitored[274]) * monitored[184])
         * monitored[273]
         / (-1 + np.exp(2 * monitored[274]))
@@ -2470,25 +2356,21 @@
     # Expressions for the SERCA component
     monitored[196] = np.where(celltype == 1, 1.3, 1)
     monitored[197] = 0.005425 * cai * monitored[196] / (0.00092 + cai)
     monitored[198] = 0.01491875 * cai * monitored[196] / (0.00075 + cai)
     monitored[199] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[200] = 0.0003255 * cansr
     monitored[201] = Jup_b * (
-        -monitored[200]
-        + (1 - monitored[199]) * monitored[197]
-        + monitored[198] * monitored[199]
+        -monitored[200] + (1 - monitored[199]) * monitored[197] + monitored[198] * monitored[199]
     )
 
     # Expressions for the I_katp component
     monitored[202] = np.power(ko / K_o_n, 0.24)
     monitored[203] = 1.0 / (1 + (A_atp * A_atp) / (K_atp * K_atp))
-    monitored[204] = (
-        fkatp * gkatp * (-monitored[10] + v) * monitored[202] * monitored[203]
-    )
+    monitored[204] = fkatp * gkatp * (-monitored[10] + v) * monitored[202] * monitored[203]
 
     # Expressions for the INa component
     monitored[19] = 1.0 / (
         (1 + 0.0018422115811651339 * np.exp(-0.1107419712070875 * v))
         * (1 + 0.0018422115811651339 * np.exp(-0.1107419712070875 * v))
     )
     monitored[20] = 0.1292 * np.exp(
@@ -2503,17 +2385,15 @@
         )
     )
     monitored[287] = (-m + monitored[19]) / monitored[20]
     monitored[21] = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    monitored[22] = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    monitored[22] = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     monitored[23] = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     monitored[24] = 1.0 / (monitored[22] + monitored[23])
     monitored[288] = (-h + monitored[21]) / monitored[24]
@@ -2523,17 +2403,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     monitored[26] = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     monitored[27] = monitored[21]
     monitored[28] = 1.0 / (monitored[25] + monitored[26])
     monitored[289] = (-j + monitored[27]) / monitored[28]
     monitored[29] = 1.0 / (
         (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
         * (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
@@ -2575,109 +2453,79 @@
         * ((1 - monitored[138]) * hL + hLp * monitored[138])
         * mL
         * monitored[137]
     )
 
     # Expressions for the Ito component
     monitored[205] = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     monitored[206] = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     monitored[295] = (-a + monitored[205]) / monitored[206]
     monitored[207] = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    monitored[208] = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    monitored[208] = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     monitored[209] = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     monitored[210] = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     monitored[211] = monitored[208] * monitored[209]
     monitored[212] = monitored[208] * monitored[210]
     monitored[213] = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     monitored[214] = 1 - monitored[213]
     monitored[296] = (-iF + monitored[207]) / monitored[211]
     monitored[297] = (-iS + monitored[207]) / monitored[212]
     monitored[215] = iF * monitored[213] + iS * monitored[214]
     monitored[216] = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     monitored[298] = (-ap + monitored[216]) / monitored[206]
     monitored[217] = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
-    )
-    monitored[218] = 1 - 0.5 / (
-        1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
+    monitored[218] = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     monitored[219] = monitored[211] * monitored[217] * monitored[218]
     monitored[220] = monitored[212] * monitored[217] * monitored[218]
     monitored[299] = (-iFp + monitored[207]) / monitored[219]
     monitored[300] = (-iSp + monitored[207]) / monitored[220]
     monitored[221] = iFp * monitored[213] + iSp * monitored[214]
-    monitored[222] = np.where(
-        celltype == 1, 2 * Gto_b, np.where(celltype == 2, 2 * Gto_b, Gto_b)
-    )
+    monitored[222] = np.where(celltype == 1, 2 * Gto_b, np.where(celltype == 2, 2 * Gto_b, Gto_b))
     monitored[223] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[224] = (
         (-monitored[10] + v)
-        * (
-            (1 - monitored[223]) * a * monitored[215]
-            + ap * monitored[221] * monitored[223]
-        )
+        * ((1 - monitored[223]) * a * monitored[215] + ap * monitored[221] * monitored[223])
         * monitored[222]
     )
 
     # Expressions for the IKr component
     monitored[225] = 0.1161 * np.exp(0.299 * monitored[274])
     monitored[226] = 0.2442 * np.exp(-1.604 * monitored[274])
     monitored[227] = 0.0578 * np.exp(0.971 * monitored[274])
     monitored[228] = 0.000349 * np.exp(-1.062 * monitored[274])
     monitored[229] = 0.2533 * np.exp(0.5953 * monitored[274])
     monitored[230] = 0.06525 * np.exp(-0.8209 * monitored[274])
     monitored[231] = 5.2e-05 * np.exp(1.525 * monitored[274])
     monitored[232] = (
-        monitored[228]
-        * monitored[230]
-        * monitored[231]
-        / (monitored[227] * monitored[229])
+        monitored[228] * monitored[230] * monitored[231] / (monitored[227] * monitored[229])
     )
     monitored[301] = C2 * monitored[226] - C3 * monitored[225]
     monitored[302] = beta_1 * C1 + C3 * monitored[225] - (alpha_1 + monitored[226]) * C2
     monitored[303] = (
         alpha_1 * C2
         + I * monitored[232]
         + O * monitored[228]
@@ -2688,17 +2536,15 @@
     )
     monitored[305] = (
         C1 * monitored[231] + O * monitored[229] - (monitored[230] + monitored[232]) * I
     )
     monitored[233] = np.where(
         celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
     )
-    monitored[234] = (
-        np.sqrt(5) * np.sqrt(ko) * (-monitored[10] + v) * O * monitored[233] / 5
-    )
+    monitored[234] = np.sqrt(5) * np.sqrt(ko) * (-monitored[10] + v) * O * monitored[233] / 5
 
     # Expressions for the IKs component
     monitored[235] = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     monitored[236] = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
@@ -2721,20 +2567,15 @@
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * monitored[10])
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * monitored[10] - 0.1629 * v))
     monitored[244] = monitored[242] / (monitored[242] + monitored[243])
     monitored[245] = np.where(
         celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
     )
     monitored[246] = (
-        np.sqrt(5)
-        * np.sqrt(ko)
-        * (-monitored[10] + v)
-        * monitored[244]
-        * monitored[245]
-        / 5
+        np.sqrt(5) * np.sqrt(ko) * (-monitored[10] + v) * monitored[244] * monitored[245] / 5
     )
 
     # Expressions for the IKb component
     monitored[247] = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     monitored[248] = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     monitored[249] = (-monitored[10] + v) * monitored[247] * monitored[248]
 
@@ -2752,43 +2593,37 @@
         * monitored[273]
         / (-1 + np.exp(2 * monitored[274]))
     )
 
     # Expressions for the Ryr component
     monitored[255] = 0.5 * bt
     monitored[256] = (
-        -monitored[179]
-        * monitored[255]
-        / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
+        -monitored[179] * monitored[255] / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
     )
     monitored[257] = np.where(celltype == 2, 1.7 * monitored[256], monitored[256])
     monitored[258] = bt / (1 + 0.0123 / cajsr)
     monitored[259] = np.where(monitored[258] < 0.001, 0.001, monitored[258])
     monitored[308] = (-Jrel_np + monitored[257]) / monitored[259]
     monitored[260] = 1.25 * bt
     monitored[261] = 0.5 * monitored[260]
     monitored[262] = (
-        -monitored[179]
-        * monitored[261]
-        / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
+        -monitored[179] * monitored[261] / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
     )
     monitored[263] = np.where(celltype == 2, 1.7 * monitored[262], monitored[262])
     monitored[264] = monitored[260] / (1 + 0.0123 / cajsr)
     monitored[265] = np.where(monitored[264] < 0.001, 0.001, monitored[264])
     monitored[309] = (-Jrel_p + monitored[263]) / monitored[265]
     monitored[266] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[267] = Jrel_b * ((1 - monitored[266]) * Jrel_np + Jrel_p * monitored[266])
 
     # Expressions for the Membrane component
     monitored[268] = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     monitored[310] = (
         -monitored[107]
@@ -2819,17 +2654,17 @@
         -monitored[131]
         - monitored[139]
         - monitored[191]
         - monitored[32]
         - 3 * monitored[130]
         - 3 * monitored[71]
     ) * monitored[2] / (F * monitored[3])
-    monitored[312] = -monitored[15] + (
-        -monitored[180] - 3 * monitored[107]
-    ) * monitored[2] / (F * monitored[6])
+    monitored[312] = -monitored[15] + (-monitored[180] - 3 * monitored[107]) * monitored[2] / (
+        F * monitored[6]
+    )
     monitored[313] = monitored[16] * monitored[6] / monitored[3] + (
         -monitored[192]
         - monitored[204]
         - monitored[224]
         - monitored[234]
         - monitored[241]
         - monitored[246]
@@ -2861,17 +2696,15 @@
     )
     monitored[318] = (
         -monitored[17]
         + monitored[267] * monitored[5] / monitored[6]
         + (-monitored[179] + 2 * monitored[107]) * monitored[2] / (2 * F * monitored[6])
     ) * monitored[271]
     monitored[319] = -monitored[275] * monitored[5] / monitored[4] + monitored[201]
-    monitored[272] = 1.0 / (
-        1 + csqnmax * kmcsqn / ((kmcsqn + cajsr) * (kmcsqn + cajsr))
-    )
+    monitored[272] = 1.0 / (1 + csqnmax * kmcsqn / ((kmcsqn + cajsr) * (kmcsqn + cajsr)))
     monitored[320] = (-monitored[267] + monitored[275]) * monitored[272]
 
     # Return results
     return monitored
 
 
 def forward_explicit_euler(states, t, dt, parameters):
@@ -3115,17 +2948,15 @@
     E1_i = x1_i / (x1_i + x2_i + x3_i + x4_i)
     E2_i = x2_i / (x1_i + x2_i + x3_i + x4_i)
     E3_i = x3_i / (x1_i + x2_i + x3_i + x4_i)
     E4_i = x4_i / (x1_i + x2_i + x3_i + x4_i)
     allo_i = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     JncxNa_i = E3_i * k4pp_i - E2_i * k3pp_i - 3 * E1_i * k8_i + 3 * E4_i * k7_i
     JncxCa_i = E2_i * k2_i - E1_i * k1_i
-    Gncx = np.where(
-        celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b)
-    )
+    Gncx = np.where(celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b))
     INaCa_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx * allo_i
     h1_ss = 1 + (1 + hna) * nass / kna3
     h2_ss = hna * nass / (kna3 * h1_ss)
     h3_ss = 1.0 / h1_ss
     h4_ss = 1 + (1 + nass / kna2) * nass / kna1
     h5_ss = (nass * nass) / (kna1 * kna2 * h4_ss)
     h6_ss = 1.0 / h4_ss
@@ -3152,17 +2983,15 @@
     x3_ss = (k2_ss + k3_ss) * k6_ss * k8_ss + (k6_ss + k7_ss) * k1_ss * k3_ss
     x4_ss = (k1_ss + k8_ss) * k3_ss * k5_ss + (k4_ss + k5_ss) * k2_ss * k8_ss
     E1_ss = x1_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E2_ss = x2_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E3_ss = x3_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E4_ss = x4_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     allo_ss = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
-    JncxNa_ss = (
-        E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
-    )
+    JncxNa_ss = E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
     JncxCa_ss = E2_ss * k2_ss - E1_ss * k1_ss
     INaCa_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx * allo_ss
 
     # Expressions for the K component
     Knai = Knai0 * np.exp(delta * vfrt / 3)
     Knao = Knao0 * np.exp((1 - delta) * vfrt / 3)
     P = eP / (1 + H / Khp + nai / Knap + ki / Kxkur)
@@ -3224,17 +3053,15 @@
     x4 = a1 * a3 * a4 + a1 * a4 * b2 + a1 * b2 * b3 + b2 * b3 * b4
     E1 = x1 / (x1 + x2 + x3 + x4)
     E2 = x2 / (x1 + x2 + x3 + x4)
     E3 = x3 / (x1 + x2 + x3 + x4)
     E4 = x4 / (x1 + x2 + x3 + x4)
     JnakNa = -3 * E2 * b3 + 3 * E1 * a3
     JnakK = -2 * E3 * a1 + 2 * E4 * b1
-    Pnak = np.where(
-        celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
-    )
+    Pnak = np.where(celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b))
     INaK = (zk * JnakK + zna * JnakNa) * Pnak
 
     # Expressions for the b component
     INab = PNab * (-nao + np.exp(vfrt) * nai) * vffrt / (-1 + np.exp(vfrt))
 
     # Expressions for the ICaL component
     dss = np.where(v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v)))
@@ -3247,17 +3074,15 @@
             + 0.7408182206817179 * np.exp(-0.05 * vShift - 0.05 * v)
         )
     )
     dd_dt = (-d + dss) / td
     states[1] = dt * dd_dt + d
     fss = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
     tff = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
-    tfs = 1000 + 1.0 / (
-        3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
-    )
+    tfs = 1000 + 1.0 / (3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6))
     Afs = 1 - Aff
     dff_dt = (-ff + fss) / tff
     states[2] = dt * dff_dt + ff
     dfs_dt = (-fs + fss) / tfs
     states[3] = dt * dfs_dt + fs
     f = Aff * ff + Afs * fs
     fcass = fss
@@ -3296,25 +3121,17 @@
     gamma_ko = np.exp(-(-0.3 * Io + np.sqrt(Io) / (1 + np.sqrt(Io))) * constA)
     PhiCaL_ss = (
         4
         * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_ss = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_ss = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
-    )
-    PCa = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    PhiCaNa_ss = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_ss = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
+    PCa = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     PCap = 1.1 * PCa
     PCaNa = 0.00125 * PCa
     PCaK = 0.0003574 * PCa
     PCaNap = 0.00125 * PCap
     PCaKp = 0.0003574 * PCap
     fICaLp = 1.0 / (1 + KmCaMK / CaMKa)
     ICaL_ss = ICaL_fractionSS * (
@@ -3338,22 +3155,16 @@
     gamma_ki = np.exp(-(-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     PhiCaL_i = (
         4
         * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_i = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_i = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
-    )
+    PhiCaNa_i = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_i = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
     ICaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * PhiCaL_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * PhiCaL_i * d * fICaLp
     )
     ICaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * PhiCaNa_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * PhiCaNa_i * d * fICaLp
@@ -3397,17 +3208,15 @@
     )
     dm_dt = (-m + mss) / tm
     states[11] = dt * dm_dt + m
     hss = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    ah = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    ah = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     bh = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     th = 1.0 / (ah + bh)
     dh_dt = (-h + hss) / th
@@ -3418,17 +3227,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     bj = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     jss = hss
     tj = 1.0 / (aj + bj)
     dj_dt = (-j + jss) / tj
     states[13] = dt * dj_dt + j
     hssp = 1.0 / (
         (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
@@ -3466,78 +3273,58 @@
     states[18] = dt * dhLp_dt + hLp
     GNaL = np.where(celltype == 1, 0.6 * GNaL_b, GNaL_b)
     fINaLp = 1.0 / (1 + KmCaMK / CaMKa)
     INaL = (-ENa + v) * ((1 - fINaLp) * hL + fINaLp * hLp) * GNaL * mL
 
     # Expressions for the Ito component
     ass = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     ta = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     da_dt = (-a + ass) / ta
     states[19] = dt * da_dt + a
     iss = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    delta_epi = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    delta_epi = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     tiF_b = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     tiS_b = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     tiF = delta_epi * tiF_b
     tiS = delta_epi * tiS_b
     AiF = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     AiS = 1 - AiF
     diF_dt = (-iF + iss) / tiF
     states[20] = dt * diF_dt + iF
     diS_dt = (-iS + iss) / tiS
     states[21] = dt * diS_dt + iS
     i = AiF * iF + AiS * iS
     assp = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     dap_dt = (-ap + assp) / ta
     states[22] = dt * dap_dt + ap
     dti_develop = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
     dti_recover = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     tiFp = dti_develop * dti_recover * tiF
     tiSp = dti_develop * dti_recover * tiS
     diFp_dt = (-iFp + iss) / tiFp
     states[23] = dt * diFp_dt + iFp
     diSp_dt = (-iSp + iss) / tiSp
@@ -3556,58 +3343,47 @@
     beta_i = 0.06525 * np.exp(-0.8209 * vfrt)
     alpha_C2ToI = 5.2e-05 * np.exp(1.525 * vfrt)
     beta_ItoC2 = alpha_C2ToI * beta_2 * beta_i / (alpha_2 * alpha_i)
     dC3_dt = C2 * beta - C3 * alpha
     states[25] = dt * dC3_dt + C3
     dC2_dt = beta_1 * C1 + C3 * alpha - (alpha_1 + beta) * C2
     states[26] = dt * dC2_dt + C2
-    dC1_dt = (
-        alpha_1 * C2
-        + I * beta_ItoC2
-        + O * beta_2
-        - (beta_1 + alpha_2 + alpha_C2ToI) * C1
-    )
+    dC1_dt = alpha_1 * C2 + I * beta_ItoC2 + O * beta_2 - (beta_1 + alpha_2 + alpha_C2ToI) * C1
     states[27] = dt * dC1_dt + C1
     dO_dt = C1 * alpha_2 + I * beta_i - (alpha_i + beta_2) * O
     states[28] = dt * dO_dt + O
     dI_dt = C1 * alpha_C2ToI + O * alpha_i - (beta_ItoC2 + beta_i) * I
     states[29] = dt * dI_dt + I
-    GKr = np.where(
-        celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
-    )
+    GKr = np.where(celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b))
     IKr = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GKr * O / 5
 
     # Expressions for the IKs component
     xs1ss = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     txs1 = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
     dxs1_dt = (-xs1 + xs1ss) / txs1
     states[30] = dt * dxs1_dt + xs1
     xs2ss = xs1ss
-    txs2 = 1.0 / (
-        0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20)
-    )
+    txs2 = 1.0 / (0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20))
     dxs2_dt = (-xs2 + xs2ss) / txs2
     states[31] = dt * dxs2_dt + xs2
     KsCa = 1 + 0.6 / (1 + 6.481821026062645e-07 * np.power(1.0 / cai, 1.4))
     GKs = np.where(celltype == 1, 1.4 * GKs_b, GKs_b)
     IKs = (-EKs + v) * GKs * KsCa * xs1 * xs2
 
     # Expressions for the IK1 component
     aK1 = 4.094 / (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
     bK1 = (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     K1ss = aK1 / (aK1 + bK1)
-    GK1 = np.where(
-        celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
-    )
+    GK1 = np.where(celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b))
     IK1 = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 * K1ss / 5
 
     # Expressions for the IKb component
     xkb = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     GKb = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     IKb = (-EK + v) * GKb * xkb
 
@@ -3645,17 +3421,15 @@
     fJrelp = 1.0 / (1 + KmCaMK / CaMKa)
     Jrel = Jrel_b * ((1 - fJrelp) * Jrel_np + Jrel_p * fJrelp)
 
     # Expressions for the Membrane component
     Istim = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     dv_dt = (
         -ICaK
@@ -3913,17 +3687,15 @@
 
     # Expressions for the CaMK component
     CaMKb = CaMKo * (1 - CaMKt) / (1 + KmCaM / cass)
     CaMKa = CaMKb + CaMKt
     dCaMKt_dt = -bCaMK * CaMKt + aCaMK * (CaMKb + CaMKt) * CaMKb
     dCaMKb_dCaMKt = -CaMKo / (1 + KmCaM / cass)
     dCaMKt_dt_linearized = (
-        -bCaMK
-        + aCaMK * (1 + dCaMKb_dCaMKt) * CaMKb
-        + aCaMK * (CaMKb + CaMKt) * dCaMKb_dCaMKt
+        -bCaMK + aCaMK * (1 + dCaMKb_dCaMKt) * CaMKb + aCaMK * (CaMKb + CaMKt) * dCaMKb_dCaMKt
     )
     states[0] = CaMKt + np.where(
         np.abs(dCaMKt_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCaMKt_dt_linearized)) * dCaMKt_dt / dCaMKt_dt_linearized,
         dt * dCaMKt_dt,
     )
 
@@ -3980,17 +3752,15 @@
     E1_i = x1_i / (x1_i + x2_i + x3_i + x4_i)
     E2_i = x2_i / (x1_i + x2_i + x3_i + x4_i)
     E3_i = x3_i / (x1_i + x2_i + x3_i + x4_i)
     E4_i = x4_i / (x1_i + x2_i + x3_i + x4_i)
     allo_i = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     JncxNa_i = E3_i * k4pp_i - E2_i * k3pp_i - 3 * E1_i * k8_i + 3 * E4_i * k7_i
     JncxCa_i = E2_i * k2_i - E1_i * k1_i
-    Gncx = np.where(
-        celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b)
-    )
+    Gncx = np.where(celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b))
     INaCa_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx * allo_i
     h1_ss = 1 + (1 + hna) * nass / kna3
     h2_ss = hna * nass / (kna3 * h1_ss)
     h3_ss = 1.0 / h1_ss
     h4_ss = 1 + (1 + nass / kna2) * nass / kna1
     h5_ss = (nass * nass) / (kna1 * kna2 * h4_ss)
     h6_ss = 1.0 / h4_ss
@@ -4017,17 +3787,15 @@
     x3_ss = (k2_ss + k3_ss) * k6_ss * k8_ss + (k6_ss + k7_ss) * k1_ss * k3_ss
     x4_ss = (k1_ss + k8_ss) * k3_ss * k5_ss + (k4_ss + k5_ss) * k2_ss * k8_ss
     E1_ss = x1_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E2_ss = x2_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E3_ss = x3_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E4_ss = x4_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     allo_ss = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
-    JncxNa_ss = (
-        E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
-    )
+    JncxNa_ss = E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
     JncxCa_ss = E2_ss * k2_ss - E1_ss * k1_ss
     INaCa_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx * allo_ss
 
     # Expressions for the K component
     Knai = Knai0 * np.exp(delta * vfrt / 3)
     Knao = Knao0 * np.exp((1 - delta) * vfrt / 3)
     P = eP / (1 + H / Khp + nai / Knap + ki / Kxkur)
@@ -4089,17 +3857,15 @@
     x4 = a1 * a3 * a4 + a1 * a4 * b2 + a1 * b2 * b3 + b2 * b3 * b4
     E1 = x1 / (x1 + x2 + x3 + x4)
     E2 = x2 / (x1 + x2 + x3 + x4)
     E3 = x3 / (x1 + x2 + x3 + x4)
     E4 = x4 / (x1 + x2 + x3 + x4)
     JnakNa = -3 * E2 * b3 + 3 * E1 * a3
     JnakK = -2 * E3 * a1 + 2 * E4 * b1
-    Pnak = np.where(
-        celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
-    )
+    Pnak = np.where(celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b))
     INaK = (zk * JnakK + zna * JnakNa) * Pnak
 
     # Expressions for the b component
     INab = PNab * (-nao + np.exp(vfrt) * nai) * vffrt / (-1 + np.exp(vfrt))
 
     # Expressions for the ICaL component
     dss = np.where(v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v)))
@@ -4113,17 +3879,15 @@
         )
     )
     dd_dt = (-d + dss) / td
     dd_dt_linearized = -1 / td
     states[1] = (-1 + np.exp(dt * dd_dt_linearized)) * dd_dt / dd_dt_linearized + d
     fss = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
     tff = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
-    tfs = 1000 + 1.0 / (
-        3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
-    )
+    tfs = 1000 + 1.0 / (3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6))
     Afs = 1 - Aff
     dff_dt = (-ff + fss) / tff
     dff_dt_linearized = -1 / tff
     states[2] = (-1 + np.exp(dt * dff_dt_linearized)) * dff_dt / dff_dt_linearized + ff
     dfs_dt = (-fs + fss) / tfs
     dfs_dt_linearized = -1 / tfs
     states[3] = (-1 + np.exp(dt * dfs_dt_linearized)) * dfs_dt / dfs_dt_linearized + fs
@@ -4131,53 +3895,41 @@
     fcass = fss
     tfcaf = 7 + 1.0 / (0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7))
     tfcas = 100 + 1.0 / (0.00012 * np.exp(-v / 3) + 0.00012 * np.exp(v / 7))
     Afcaf = 0.3 + 0.6 / (1 + np.exp(-1 + v / 10))
     Afcas = 1 - Afcaf
     dfcaf_dt = (-fcaf + fcass) / tfcaf
     dfcaf_dt_linearized = -1 / tfcaf
-    states[4] = (
-        -1 + np.exp(dt * dfcaf_dt_linearized)
-    ) * dfcaf_dt / dfcaf_dt_linearized + fcaf
+    states[4] = (-1 + np.exp(dt * dfcaf_dt_linearized)) * dfcaf_dt / dfcaf_dt_linearized + fcaf
     dfcas_dt = (-fcas + fcass) / tfcas
     dfcas_dt_linearized = -1 / tfcas
-    states[5] = (
-        -1 + np.exp(dt * dfcas_dt_linearized)
-    ) * dfcas_dt / dfcas_dt_linearized + fcas
+    states[5] = (-1 + np.exp(dt * dfcas_dt_linearized)) * dfcas_dt / dfcas_dt_linearized + fcas
     fca = Afcaf * fcaf + Afcas * fcas
     jcass = 1.0 / (1.0 + 649.7401897235336 * np.exp(0.35821750967187277 * v))
     djca_dt = (-jca + jcass) / tjca
     djca_dt_linearized = -1 / tjca
-    states[6] = (
-        -1 + np.exp(dt * djca_dt_linearized)
-    ) * djca_dt / djca_dt_linearized + jca
+    states[6] = (-1 + np.exp(dt * djca_dt_linearized)) * djca_dt / djca_dt_linearized + jca
     tffp = 2.5 * tff
     dffp_dt = (-ffp + fss) / tffp
     dffp_dt_linearized = -1 / tffp
-    states[7] = (
-        -1 + np.exp(dt * dffp_dt_linearized)
-    ) * dffp_dt / dffp_dt_linearized + ffp
+    states[7] = (-1 + np.exp(dt * dffp_dt_linearized)) * dffp_dt / dffp_dt_linearized + ffp
     fp = Aff * ffp + Afs * fs
     tfcafp = 2.5 * tfcaf
     dfcafp_dt = (-fcafp + fcass) / tfcafp
     dfcafp_dt_linearized = -1 / tfcafp
-    states[8] = (
-        -1 + np.exp(dt * dfcafp_dt_linearized)
-    ) * dfcafp_dt / dfcafp_dt_linearized + fcafp
+    states[8] = (-1 + np.exp(dt * dfcafp_dt_linearized)) * dfcafp_dt / dfcafp_dt_linearized + fcafp
     fcap = Afcaf * fcafp + Afcas * fcas
     km2n = jca
     anca_ss = 1.0 / (np.power(1 + Kmn / cass, 4) + k2n / km2n)
     dnca_ss_dt = k2n * anca_ss - km2n * nca_ss
     dnca_ss_dt_linearized = -km2n
     states[9] = (
         np.where(
             np.abs(dnca_ss_dt_linearized) > 1e-08,
-            (-1 + np.exp(dt * dnca_ss_dt_linearized))
-            * dnca_ss_dt
-            / dnca_ss_dt_linearized,
+            (-1 + np.exp(dt * dnca_ss_dt_linearized)) * dnca_ss_dt / dnca_ss_dt_linearized,
             dt * dnca_ss_dt,
         )
         + nca_ss
     )
     Io = 0.0005 * clo + 0.0005 * ko + 0.0005 * nao + 0.002 * cao
     Iss = 0.0005 * clss + 0.0005 * kss + 0.0005 * nass + 0.002 * cass
     constA = 1820000.0 * np.power(T * dielConstant, -1.5)
@@ -4189,25 +3941,17 @@
     gamma_ko = np.exp(-(-0.3 * Io + np.sqrt(Io) / (1 + np.sqrt(Io))) * constA)
     PhiCaL_ss = (
         4
         * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_ss = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_ss = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
-    )
-    PCa = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    PhiCaNa_ss = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_ss = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
+    PCa = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     PCap = 1.1 * PCa
     PCaNa = 0.00125 * PCa
     PCaK = 0.0003574 * PCa
     PCaNap = 0.00125 * PCap
     PCaKp = 0.0003574 * PCap
     fICaLp = 1.0 / (1 + KmCaMK / CaMKa)
     ICaL_ss = ICaL_fractionSS * (
@@ -4239,22 +3983,16 @@
     gamma_ki = np.exp(-(-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     PhiCaL_i = (
         4
         * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_i = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_i = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
-    )
+    PhiCaNa_i = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_i = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
     ICaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * PhiCaL_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * PhiCaL_i * d * fICaLp
     )
     ICaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * PhiCaNa_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * PhiCaNa_i * d * fICaLp
@@ -4299,17 +4037,15 @@
     dm_dt = (-m + mss) / tm
     dm_dt_linearized = -1 / tm
     states[11] = (-1 + np.exp(dt * dm_dt_linearized)) * dm_dt / dm_dt_linearized + m
     hss = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    ah = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    ah = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     bh = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     th = 1.0 / (ah + bh)
     dh_dt = (-h + hss) / th
@@ -4321,17 +4057,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     bj = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     jss = hss
     tj = 1.0 / (aj + bj)
     dj_dt = (-j + jss) / tj
     dj_dt_linearized = -1 / tj
     states[13] = (-1 + np.exp(dt * dj_dt_linearized)) * dj_dt / dj_dt_linearized + j
     hssp = 1.0 / (
@@ -4368,105 +4102,79 @@
     dhL_dt = (-hL + hLss) / thL
     dhL_dt_linearized = -1 / thL
     states[17] = (-1 + np.exp(dt * dhL_dt_linearized)) * dhL_dt / dhL_dt_linearized + hL
     hLssp = 1.0 / (1 + 275969.2903869871 * np.exp(0.13354700854700854 * v))
     thLp = 3 * thL
     dhLp_dt = (-hLp + hLssp) / thLp
     dhLp_dt_linearized = -1 / thLp
-    states[18] = (
-        -1 + np.exp(dt * dhLp_dt_linearized)
-    ) * dhLp_dt / dhLp_dt_linearized + hLp
+    states[18] = (-1 + np.exp(dt * dhLp_dt_linearized)) * dhLp_dt / dhLp_dt_linearized + hLp
     GNaL = np.where(celltype == 1, 0.6 * GNaL_b, GNaL_b)
     fINaLp = 1.0 / (1 + KmCaMK / CaMKa)
     INaL = (-ENa + v) * ((1 - fINaLp) * hL + fINaLp * hLp) * GNaL * mL
 
     # Expressions for the Ito component
     ass = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     ta = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     da_dt = (-a + ass) / ta
     da_dt_linearized = -1 / ta
     states[19] = (-1 + np.exp(dt * da_dt_linearized)) * da_dt / da_dt_linearized + a
     iss = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    delta_epi = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    delta_epi = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     tiF_b = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     tiS_b = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     tiF = delta_epi * tiF_b
     tiS = delta_epi * tiS_b
     AiF = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     AiS = 1 - AiF
     diF_dt = (-iF + iss) / tiF
     diF_dt_linearized = -1 / tiF
     states[20] = (-1 + np.exp(dt * diF_dt_linearized)) * diF_dt / diF_dt_linearized + iF
     diS_dt = (-iS + iss) / tiS
     diS_dt_linearized = -1 / tiS
     states[21] = (-1 + np.exp(dt * diS_dt_linearized)) * diS_dt / diS_dt_linearized + iS
     i = AiF * iF + AiS * iS
     assp = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     dap_dt = (-ap + assp) / ta
     dap_dt_linearized = -1 / ta
     states[22] = (-1 + np.exp(dt * dap_dt_linearized)) * dap_dt / dap_dt_linearized + ap
     dti_develop = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
     dti_recover = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     tiFp = dti_develop * dti_recover * tiF
     tiSp = dti_develop * dti_recover * tiS
     diFp_dt = (-iFp + iss) / tiFp
     diFp_dt_linearized = -1 / tiFp
-    states[23] = (
-        -1 + np.exp(dt * diFp_dt_linearized)
-    ) * diFp_dt / diFp_dt_linearized + iFp
+    states[23] = (-1 + np.exp(dt * diFp_dt_linearized)) * diFp_dt / diFp_dt_linearized + iFp
     diSp_dt = (-iSp + iss) / tiSp
     diSp_dt_linearized = -1 / tiSp
-    states[24] = (
-        -1 + np.exp(dt * diSp_dt_linearized)
-    ) * diSp_dt / diSp_dt_linearized + iSp
+    states[24] = (-1 + np.exp(dt * diSp_dt_linearized)) * diSp_dt / diSp_dt_linearized + iSp
     ip = AiF * iFp + AiS * iSp
     Gto = np.where(celltype == 1, 2 * Gto_b, np.where(celltype == 2, 2 * Gto_b, Gto_b))
     fItop = 1.0 / (1 + KmCaMK / CaMKa)
     Ito = (-EK + v) * ((1 - fItop) * a * i + ap * fItop * ip) * Gto
 
     # Expressions for the IKr component
     alpha = 0.1161 * np.exp(0.299 * vfrt)
@@ -4487,20 +4195,15 @@
     dC2_dt = beta_1 * C1 + C3 * alpha - (alpha_1 + beta) * C2
     dC2_dt_linearized = -alpha_1 - beta
     states[26] = C2 + np.where(
         np.abs(dC2_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dC2_dt_linearized)) * dC2_dt / dC2_dt_linearized,
         dt * dC2_dt,
     )
-    dC1_dt = (
-        alpha_1 * C2
-        + I * beta_ItoC2
-        + O * beta_2
-        - (beta_1 + alpha_2 + alpha_C2ToI) * C1
-    )
+    dC1_dt = alpha_1 * C2 + I * beta_ItoC2 + O * beta_2 - (beta_1 + alpha_2 + alpha_C2ToI) * C1
     dC1_dt_linearized = -beta_1 - alpha_2 - alpha_C2ToI
     states[27] = C1 + np.where(
         np.abs(dC1_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dC1_dt_linearized)) * dC1_dt / dC1_dt_linearized,
         dt * dC1_dt,
     )
     dO_dt = C1 * alpha_2 + I * beta_i - (alpha_i + beta_2) * O
@@ -4513,53 +4216,43 @@
     dI_dt = C1 * alpha_C2ToI + O * alpha_i - (beta_ItoC2 + beta_i) * I
     dI_dt_linearized = -beta_ItoC2 - beta_i
     states[29] = I + np.where(
         np.abs(dI_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dI_dt_linearized)) * dI_dt / dI_dt_linearized,
         dt * dI_dt,
     )
-    GKr = np.where(
-        celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
-    )
+    GKr = np.where(celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b))
     IKr = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GKr * O / 5
 
     # Expressions for the IKs component
     xs1ss = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     txs1 = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
     dxs1_dt = (-xs1 + xs1ss) / txs1
     dxs1_dt_linearized = -1 / txs1
-    states[30] = (
-        -1 + np.exp(dt * dxs1_dt_linearized)
-    ) * dxs1_dt / dxs1_dt_linearized + xs1
+    states[30] = (-1 + np.exp(dt * dxs1_dt_linearized)) * dxs1_dt / dxs1_dt_linearized + xs1
     xs2ss = xs1ss
-    txs2 = 1.0 / (
-        0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20)
-    )
+    txs2 = 1.0 / (0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20))
     dxs2_dt = (-xs2 + xs2ss) / txs2
     dxs2_dt_linearized = -1 / txs2
-    states[31] = (
-        -1 + np.exp(dt * dxs2_dt_linearized)
-    ) * dxs2_dt / dxs2_dt_linearized + xs2
+    states[31] = (-1 + np.exp(dt * dxs2_dt_linearized)) * dxs2_dt / dxs2_dt_linearized + xs2
     KsCa = 1 + 0.6 / (1 + 6.481821026062645e-07 * np.power(1.0 / cai, 1.4))
     GKs = np.where(celltype == 1, 1.4 * GKs_b, GKs_b)
     IKs = (-EKs + v) * GKs * KsCa * xs1 * xs2
 
     # Expressions for the IK1 component
     aK1 = 4.094 / (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
     bK1 = (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     K1ss = aK1 / (aK1 + bK1)
-    GK1 = np.where(
-        celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
-    )
+    GK1 = np.where(celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b))
     IK1 = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 * K1ss / 5
 
     # Expressions for the IKb component
     xkb = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     GKb = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     IKb = (-EK + v) * GKb * xkb
 
@@ -4603,17 +4296,15 @@
     fJrelp = 1.0 / (1 + KmCaMK / CaMKa)
     Jrel = Jrel_b * ((1 - fJrelp) * Jrel_np + Jrel_p * fJrelp)
 
     # Expressions for the Membrane component
     Istim = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     dv_dt = (
         -ICaK
@@ -4634,17 +4325,15 @@
         - INab
         - I_katp
         - IpCa
         - Istim
         - Ito
     )
     dAfcaf_dv = (
-        -0.06
-        * np.exp(-1 + v / 10)
-        / ((1 + np.exp(-1 + v / 10)) * (1 + np.exp(-1 + v / 10)))
+        -0.06 * np.exp(-1 + v / 10) / ((1 + np.exp(-1 + v / 10)) * (1 + np.exp(-1 + v / 10)))
     )
     dAiF_dv = (
         -0.0016103529885927823
         * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
         / (
             (
                 1
@@ -4654,171 +4343,122 @@
             * (
                 1
                 + 0.24348537187522867
                 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
             )
         )
     )
-    dE1_dx1 = 1.0 / (x1 + x2 + x3 + x4) - x1 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE1_dx1 = 1.0 / (x1 + x2 + x3 + x4) - x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_dx2 = -x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_dx3 = -x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_dx4 = -x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_i_dx1_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x1_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
     dE1_i_dx2_i = -x1_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE1_i_dx3_i = -x1_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE1_i_dx4_i = -x1_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE1_ss_dx1_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x1_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
-    dE1_ss_dx2_ss = -x1_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE1_ss_dx3_ss = -x1_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE1_ss_dx4_ss = -x1_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE1_ss_dx2_ss = -x1_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE1_ss_dx3_ss = -x1_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE1_ss_dx4_ss = -x1_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE2_dx1 = -x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
-    dE2_dx2 = 1.0 / (x1 + x2 + x3 + x4) - x2 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE2_dx2 = 1.0 / (x1 + x2 + x3 + x4) - x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE2_dx3 = -x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE2_dx4 = -x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE2_i_dx1_i = -x2_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE2_i_dx2_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x2_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
     dE2_i_dx3_i = -x2_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE2_i_dx4_i = -x2_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
-    dE2_ss_dx1_ss = -x2_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE2_ss_dx1_ss = -x2_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE2_ss_dx2_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x2_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
-    dE2_ss_dx3_ss = -x2_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE2_ss_dx4_ss = -x2_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE2_ss_dx3_ss = -x2_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE2_ss_dx4_ss = -x2_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE3_dx1 = -x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE3_dx2 = -x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
-    dE3_dx3 = 1.0 / (x1 + x2 + x3 + x4) - x3 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE3_dx3 = 1.0 / (x1 + x2 + x3 + x4) - x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE3_dx4 = -x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE3_i_dx1_i = -x3_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE3_i_dx2_i = -x3_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE3_i_dx3_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x3_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
     dE3_i_dx4_i = -x3_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
-    dE3_ss_dx1_ss = -x3_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE3_ss_dx2_ss = -x3_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE3_ss_dx1_ss = -x3_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE3_ss_dx2_ss = -x3_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE3_ss_dx3_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x3_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
-    dE3_ss_dx4_ss = -x3_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE3_ss_dx4_ss = -x3_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE4_dx1 = -x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE4_dx2 = -x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE4_dx3 = -x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
-    dE4_dx4 = 1.0 / (x1 + x2 + x3 + x4) - x4 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE4_dx4 = 1.0 / (x1 + x2 + x3 + x4) - x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE4_i_dx1_i = -x4_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE4_i_dx2_i = -x4_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE4_i_dx3_i = -x4_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE4_i_dx4_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x4_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
-    dE4_ss_dx1_ss = -x4_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE4_ss_dx2_ss = -x4_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE4_ss_dx3_ss = -x4_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE4_ss_dx1_ss = -x4_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE4_ss_dx2_ss = -x4_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE4_ss_dx3_ss = -x4_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE4_ss_dx4_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x4_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
     dICaK_i_dPhiCaK_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaK * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaKp * d * fICaLp
     )
-    dICaK_i_dfca = (
-        (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaK * PhiCaK_i * d * jca * nca_i
-    )
+    dICaK_i_dfca = (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaK * PhiCaK_i * d * jca * nca_i
     dICaK_i_dfcap = (1 - ICaL_fractionSS) * PCaKp * PhiCaK_i * d * fICaLp * jca * nca_i
     dICaK_ss_dPhiCaK_ss = ICaL_fractionSS * (
         (1 - fICaLp) * ((1 - nca_ss) * f + fca * jca * nca_ss) * PCaK * d
         + ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCaKp * d * fICaLp
     )
     dICaK_ss_dfca = ICaL_fractionSS * (1 - fICaLp) * PCaK * PhiCaK_ss * d * jca * nca_ss
     dICaK_ss_dfcap = ICaL_fractionSS * PCaKp * PhiCaK_ss * d * fICaLp * jca * nca_ss
     dICaL_i_dPhiCaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * d * fICaLp
     )
-    dICaL_i_dfca = (
-        (1 - ICaL_fractionSS) * (1 - fICaLp) * PCa * PhiCaL_i * d * jca * nca_i
-    )
+    dICaL_i_dfca = (1 - ICaL_fractionSS) * (1 - fICaLp) * PCa * PhiCaL_i * d * jca * nca_i
     dICaL_i_dfcap = (1 - ICaL_fractionSS) * PCap * PhiCaL_i * d * fICaLp * jca * nca_i
     dICaL_ss_dPhiCaL_ss = ICaL_fractionSS * (
         (1 - fICaLp) * ((1 - nca_ss) * f + fca * jca * nca_ss) * PCa * d
         + ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCap * d * fICaLp
     )
     dICaL_ss_dfca = ICaL_fractionSS * (1 - fICaLp) * PCa * PhiCaL_ss * d * jca * nca_ss
     dICaL_ss_dfcap = ICaL_fractionSS * PCap * PhiCaL_ss * d * fICaLp * jca * nca_ss
     dICaNa_i_dPhiCaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * d * fICaLp
     )
-    dICaNa_i_dfca = (
-        (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaNa * PhiCaNa_i * d * jca * nca_i
-    )
-    dICaNa_i_dfcap = (
-        (1 - ICaL_fractionSS) * PCaNap * PhiCaNa_i * d * fICaLp * jca * nca_i
-    )
+    dICaNa_i_dfca = (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaNa * PhiCaNa_i * d * jca * nca_i
+    dICaNa_i_dfcap = (1 - ICaL_fractionSS) * PCaNap * PhiCaNa_i * d * fICaLp * jca * nca_i
     dICaNa_ss_dPhiCaNa_ss = ICaL_fractionSS * (
         (1 - fICaLp) * ((1 - nca_ss) * f + fca * jca * nca_ss) * PCaNa * d
         + ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCaNap * d * fICaLp
     )
-    dICaNa_ss_dfca = (
-        ICaL_fractionSS * (1 - fICaLp) * PCaNa * PhiCaNa_ss * d * jca * nca_ss
-    )
+    dICaNa_ss_dfca = ICaL_fractionSS * (1 - fICaLp) * PCaNa * PhiCaNa_ss * d * jca * nca_ss
     dICaNa_ss_dfcap = ICaL_fractionSS * PCaNap * PhiCaNa_ss * d * fICaLp * jca * nca_ss
     dICab_dvffrt = (
-        4
-        * PCab
-        * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
-        / (-1 + np.exp(2 * vfrt))
+        4 * PCab * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) / (-1 + np.exp(2 * vfrt))
     )
-    dICab_dvfrt = -8 * PCab * (
-        -cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai
-    ) * np.exp(2 * vfrt) * vffrt / (
-        (-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))
-    ) + 8 * PCab * cai * np.exp(
+    dICab_dvfrt = -8 * PCab * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) * np.exp(
         2 * vfrt
-    ) * gamma_cai * vffrt / (
-        -1 + np.exp(2 * vfrt)
-    )
+    ) * vffrt / ((-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))) + 8 * PCab * cai * np.exp(
+        2 * vfrt
+    ) * gamma_cai * vffrt / (-1 + np.exp(2 * vfrt))
     dIClCa_junc_dv = Fjunc * GClCa / (1 + KdClCa / cass)
     dIClCa_sl_dv = GClCa * (1 - Fjunc) / (1 + KdClCa / cai)
     dIK1_dK1ss = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 / 5
     dK1ss_daK1 = 1.0 / (aK1 + bK1) - aK1 / ((aK1 + bK1) * (aK1 + bK1))
     dK1ss_dbK1 = -aK1 / ((aK1 + bK1) * (aK1 + bK1))
     daK1_dv = (
         -0.0011435228161993972
@@ -4827,22 +4467,18 @@
             (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
             * (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
         )
     )
     dbK1_dv = (
         6.919349479611957e-18 * np.exp(0.0618 * v - 0.0618 * EK)
         + 0.8506978434250505 * np.exp(0.0674 * v - 0.0674 * EK)
-    ) / (
-        1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)
-    ) + 0.016099950792318272 * (
+    ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)) + 0.016099950792318272 * (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
-    ) * np.exp(
-        0.1629 * EK - 0.1629 * v
-    ) / (
+    ) * np.exp(0.1629 * EK - 0.1629 * v) / (
         (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
         * (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     )
     dIK1_dv = (
         np.sqrt(5) * np.sqrt(ko) * GK1 * K1ss / 5
         + np.sqrt(5)
         * np.sqrt(ko)
@@ -4896,132 +4532,67 @@
         - 3 * (dE2_dx2 * dx2_da3 + dE2_dx3 * dx3_da3 + a1 * a4 * dE2_dx4) * b3
         + 3 * (dE1_dx2 * dx2_da3 + dE1_dx3 * dx3_da3 + a1 * a4 * dE1_dx4) * a3
     )
     dx3_i_dk3_i = (k6_i + k7_i) * k1_i + k6_i * k8_i
     dx4_i_dk3_i = (k1_i + k8_i) * k5_i
     dJncxNa_i_dk3pp_i = (
         -E2_i
-        + (
-            dE3_i_dx3_i * dx3_i_dk3_i
-            + dE3_i_dx4_i * dx4_i_dk3_i
-            + dE3_i_dx1_i * k5_i * k7_i
-        )
+        + (dE3_i_dx3_i * dx3_i_dk3_i + dE3_i_dx4_i * dx4_i_dk3_i + dE3_i_dx1_i * k5_i * k7_i)
         * k4pp_i
-        - (
-            dE2_i_dx3_i * dx3_i_dk3_i
-            + dE2_i_dx4_i * dx4_i_dk3_i
-            + dE2_i_dx1_i * k5_i * k7_i
-        )
+        - (dE2_i_dx3_i * dx3_i_dk3_i + dE2_i_dx4_i * dx4_i_dk3_i + dE2_i_dx1_i * k5_i * k7_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx3_i * dx3_i_dk3_i
-            + dE1_i_dx4_i * dx4_i_dk3_i
-            + dE1_i_dx1_i * k5_i * k7_i
-        )
+        * (dE1_i_dx3_i * dx3_i_dk3_i + dE1_i_dx4_i * dx4_i_dk3_i + dE1_i_dx1_i * k5_i * k7_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx3_i * dx3_i_dk3_i
-            + dE4_i_dx4_i * dx4_i_dk3_i
-            + dE4_i_dx1_i * k5_i * k7_i
-        )
+        * (dE4_i_dx3_i * dx3_i_dk3_i + dE4_i_dx4_i * dx4_i_dk3_i + dE4_i_dx1_i * k5_i * k7_i)
         * k7_i
     )
     dx1_i_dk4_i = (k6_i + k7_i) * k2_i
     dx2_i_dk4_i = (k1_i + k8_i) * k6_i + k1_i * k7_i
     dJncxNa_i_dk4pp_i = (
-        (
-            dE3_i_dx1_i * dx1_i_dk4_i
-            + dE3_i_dx2_i * dx2_i_dk4_i
-            + dE3_i_dx4_i * k2_i * k8_i
-        )
-        * k4pp_i
-        - (
-            dE2_i_dx1_i * dx1_i_dk4_i
-            + dE2_i_dx2_i * dx2_i_dk4_i
-            + dE2_i_dx4_i * k2_i * k8_i
-        )
+        (dE3_i_dx1_i * dx1_i_dk4_i + dE3_i_dx2_i * dx2_i_dk4_i + dE3_i_dx4_i * k2_i * k8_i) * k4pp_i
+        - (dE2_i_dx1_i * dx1_i_dk4_i + dE2_i_dx2_i * dx2_i_dk4_i + dE2_i_dx4_i * k2_i * k8_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx1_i * dx1_i_dk4_i
-            + dE1_i_dx2_i * dx2_i_dk4_i
-            + dE1_i_dx4_i * k2_i * k8_i
-        )
+        * (dE1_i_dx1_i * dx1_i_dk4_i + dE1_i_dx2_i * dx2_i_dk4_i + dE1_i_dx4_i * k2_i * k8_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx1_i * dx1_i_dk4_i
-            + dE4_i_dx2_i * dx2_i_dk4_i
-            + dE4_i_dx4_i * k2_i * k8_i
-        )
+        * (dE4_i_dx1_i * dx1_i_dk4_i + dE4_i_dx2_i * dx2_i_dk4_i + dE4_i_dx4_i * k2_i * k8_i)
         * k7_i
         + E3_i
     )
     dx1_i_dk7_i = (k2_i + k3_i) * k5_i + k2_i * k4_i
     dx2_i_dk7_i = (k4_i + k5_i) * k1_i
     dJncxNa_i_dk7_i = (
         3 * E4_i
-        + (
-            dE3_i_dx1_i * dx1_i_dk7_i
-            + dE3_i_dx2_i * dx2_i_dk7_i
-            + dE3_i_dx3_i * k1_i * k3_i
-        )
+        + (dE3_i_dx1_i * dx1_i_dk7_i + dE3_i_dx2_i * dx2_i_dk7_i + dE3_i_dx3_i * k1_i * k3_i)
         * k4pp_i
-        - (
-            dE2_i_dx1_i * dx1_i_dk7_i
-            + dE2_i_dx2_i * dx2_i_dk7_i
-            + dE2_i_dx3_i * k1_i * k3_i
-        )
+        - (dE2_i_dx1_i * dx1_i_dk7_i + dE2_i_dx2_i * dx2_i_dk7_i + dE2_i_dx3_i * k1_i * k3_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx1_i * dx1_i_dk7_i
-            + dE1_i_dx2_i * dx2_i_dk7_i
-            + dE1_i_dx3_i * k1_i * k3_i
-        )
+        * (dE1_i_dx1_i * dx1_i_dk7_i + dE1_i_dx2_i * dx2_i_dk7_i + dE1_i_dx3_i * k1_i * k3_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx1_i * dx1_i_dk7_i
-            + dE4_i_dx2_i * dx2_i_dk7_i
-            + dE4_i_dx3_i * k1_i * k3_i
-        )
+        * (dE4_i_dx1_i * dx1_i_dk7_i + dE4_i_dx2_i * dx2_i_dk7_i + dE4_i_dx3_i * k1_i * k3_i)
         * k7_i
     )
     dx3_i_dk8_i = (k2_i + k3_i) * k6_i
     dx4_i_dk8_i = (k4_i + k5_i) * k2_i + k3_i * k5_i
     dJncxNa_i_dk8_i = (
         -3 * E1_i
-        + (
-            dE3_i_dx3_i * dx3_i_dk8_i
-            + dE3_i_dx4_i * dx4_i_dk8_i
-            + dE3_i_dx2_i * k4_i * k6_i
-        )
+        + (dE3_i_dx3_i * dx3_i_dk8_i + dE3_i_dx4_i * dx4_i_dk8_i + dE3_i_dx2_i * k4_i * k6_i)
         * k4pp_i
-        - (
-            dE2_i_dx3_i * dx3_i_dk8_i
-            + dE2_i_dx4_i * dx4_i_dk8_i
-            + dE2_i_dx2_i * k4_i * k6_i
-        )
+        - (dE2_i_dx3_i * dx3_i_dk8_i + dE2_i_dx4_i * dx4_i_dk8_i + dE2_i_dx2_i * k4_i * k6_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx3_i * dx3_i_dk8_i
-            + dE1_i_dx4_i * dx4_i_dk8_i
-            + dE1_i_dx2_i * k4_i * k6_i
-        )
+        * (dE1_i_dx3_i * dx3_i_dk8_i + dE1_i_dx4_i * dx4_i_dk8_i + dE1_i_dx2_i * k4_i * k6_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx3_i * dx3_i_dk8_i
-            + dE4_i_dx4_i * dx4_i_dk8_i
-            + dE4_i_dx2_i * k4_i * k6_i
-        )
+        * (dE4_i_dx3_i * dx3_i_dk8_i + dE4_i_dx4_i * dx4_i_dk8_i + dE4_i_dx2_i * k4_i * k6_i)
         * k7_i
     )
     dx3_ss_dk3_ss = (k6_ss + k7_ss) * k1_ss + k6_ss * k8_ss
     dx4_ss_dk3_ss = (k1_ss + k8_ss) * k5_ss
     dJncxNa_ss_dk3pp_ss = (
         -E2_ss
         + (
@@ -5142,82 +4713,50 @@
             + dE4_ss_dx4_ss * dx4_ss_dk8_ss
             + dE4_ss_dx2_ss * k4_ss * k6_ss
         )
         * k7_ss
     )
     dKnai_dvfrt = Knai0 * delta * np.exp(delta * vfrt / 3) / 3
     dKnao_dvfrt = Knao0 * (1 / 3 - delta / 3) * np.exp((1 - delta) * vfrt / 3)
-    dPhiCaK_i_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaK_i_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * np.exp(
-        vfrt
-    ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
-        vfrt
-    ) * gamma_ki * ki * vffrt / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaK_ss_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaK_ss_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * np.exp(
-        vfrt
-    ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
-        vfrt
-    ) * gamma_kss * kss * vffrt / (
-        -1 + np.exp(vfrt)
-    )
+    dPhiCaK_i_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) / (-1 + np.exp(vfrt))
+    dPhiCaK_i_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * np.exp(vfrt) * vffrt / (
+        (-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))
+    ) + np.exp(vfrt) * gamma_ki * ki * vffrt / (-1 + np.exp(vfrt))
+    dPhiCaK_ss_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) / (-1 + np.exp(vfrt))
+    dPhiCaK_ss_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * np.exp(vfrt) * vffrt / (
+        (-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))
+    ) + np.exp(vfrt) * gamma_kss * kss * vffrt / (-1 + np.exp(vfrt))
     dPhiCaL_i_dvffrt = (
-        4
-        * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
-        / (-1 + np.exp(2 * vfrt))
+        4 * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) / (-1 + np.exp(2 * vfrt))
     )
-    dPhiCaL_i_dvfrt = -8 * (
-        -cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai
-    ) * np.exp(2 * vfrt) * vffrt / (
-        (-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))
-    ) + 8 * cai * np.exp(
+    dPhiCaL_i_dvfrt = -8 * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) * np.exp(
         2 * vfrt
-    ) * gamma_cai * vffrt / (
-        -1 + np.exp(2 * vfrt)
-    )
+    ) * vffrt / ((-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))) + 8 * cai * np.exp(
+        2 * vfrt
+    ) * gamma_cai * vffrt / (-1 + np.exp(2 * vfrt))
     dPhiCaL_ss_dvffrt = (
-        4
-        * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
-        / (-1 + np.exp(2 * vfrt))
+        4 * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass) / (-1 + np.exp(2 * vfrt))
     )
-    dPhiCaL_ss_dvfrt = -8 * (
-        -cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass
-    ) * np.exp(2 * vfrt) * vffrt / (
-        (-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))
-    ) + 8 * cass * np.exp(
+    dPhiCaL_ss_dvfrt = -8 * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass) * np.exp(
         2 * vfrt
-    ) * gamma_cass * vffrt / (
-        -1 + np.exp(2 * vfrt)
-    )
-    dPhiCaNa_i_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) / (
-        -1 + np.exp(vfrt)
-    )
+    ) * vffrt / ((-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))) + 8 * cass * np.exp(
+        2 * vfrt
+    ) * gamma_cass * vffrt / (-1 + np.exp(2 * vfrt))
+    dPhiCaNa_i_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) / (-1 + np.exp(vfrt))
     dPhiCaNa_i_dvfrt = -(-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * np.exp(
         vfrt
     ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
         vfrt
-    ) * gamma_nai * nai * vffrt / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaNa_ss_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) / (
-        -1 + np.exp(vfrt)
-    )
+    ) * gamma_nai * nai * vffrt / (-1 + np.exp(vfrt))
+    dPhiCaNa_ss_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) / (-1 + np.exp(vfrt))
     dPhiCaNa_ss_dvfrt = -(-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * np.exp(
         vfrt
     ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
         vfrt
-    ) * gamma_nass * nass * vffrt / (
-        -1 + np.exp(vfrt)
-    )
+    ) * gamma_nass * nass * vffrt / (-1 + np.exp(vfrt))
     da1_dKnai = -3 * k1p * (nai * nai * nai) / (
         (
             -1
             + ((1 + ki / Kki) * (1 + ki / Kki))
             + ((1 + nai / Knai) * (1 + nai / Knai) * (1 + nai / Knai))
         )
         * np.power(Knai, 4)
@@ -5307,17 +4846,15 @@
     dfca_dAfcaf = -fcas + fcaf
     dfcap_dAfcaf = -fcas + fcafp
     dh1_i_dhna = nai / kna3
     dh1_ss_dhna = nass / kna3
     dh2_i_dh1_i = -hna * nai / (kna3 * (h1_i * h1_i))
     dh2_i_dhna = nai / (kna3 * h1_i) - dh1_i_dhna * hna * nai / (kna3 * (h1_i * h1_i))
     dh2_ss_dh1_ss = -hna * nass / (kna3 * (h1_ss * h1_ss))
-    dh2_ss_dhna = nass / (kna3 * h1_ss) - dh1_ss_dhna * hna * nass / (
-        kna3 * (h1_ss * h1_ss)
-    )
+    dh2_ss_dhna = nass / (kna3 * h1_ss) - dh1_ss_dhna * hna * nass / (kna3 * (h1_ss * h1_ss))
     dh3_i_dh1_i = -1 / (h1_i * h1_i)
     dh3_ss_dh1_ss = -1 / (h1_ss * h1_ss)
     dh7_i_dhna = -nao / (kna3 * (hna * hna))
     dh7_ss_dhna = -nao / (kna3 * (hna * hna))
     dh8_i_dh7_i = -nao / (kna3 * (h7_i * h7_i) * hna)
     dh8_i_dhna = -nao / (kna3 * h7_i * (hna * hna)) - nao * dh7_i_dhna / (
         kna3 * (h7_i * h7_i) * hna
@@ -5394,19 +4931,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5419,19 +4952,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5453,19 +4982,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -5524,19 +5049,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5549,19 +5070,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5583,19 +5100,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -5657,19 +5170,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5682,19 +5191,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5716,19 +5221,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -5787,19 +5288,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5812,19 +5309,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5846,19 +5339,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -5889,26 +5378,20 @@
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaL_i_dfcap
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaL_ss_dfcap
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaNa_i_dfcap
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaNa_ss_dfcap
         - (dAiF_dv * di_dAiF - dAiF_dv * iS) * dIto_di
         - (dAiF_dv * dip_dAiF - dAiF_dv * iSp) * dIto_dip
         - (dK1ss_daK1 * daK1_dv + dK1ss_dbK1 * dbK1_dv) * dIK1_dK1ss
-        - (dPhiCaK_i_dvffrt * dvffrt_dv + dPhiCaK_i_dvfrt * dvfrt_dv)
-        * dICaK_i_dPhiCaK_i
-        - (dPhiCaK_ss_dvffrt * dvffrt_dv + dPhiCaK_ss_dvfrt * dvfrt_dv)
-        * dICaK_ss_dPhiCaK_ss
-        - (dPhiCaL_i_dvffrt * dvffrt_dv + dPhiCaL_i_dvfrt * dvfrt_dv)
-        * dICaL_i_dPhiCaL_i
-        - (dPhiCaL_ss_dvffrt * dvffrt_dv + dPhiCaL_ss_dvfrt * dvfrt_dv)
-        * dICaL_ss_dPhiCaL_ss
-        - (dPhiCaNa_i_dvffrt * dvffrt_dv + dPhiCaNa_i_dvfrt * dvfrt_dv)
-        * dICaNa_i_dPhiCaNa_i
-        - (dPhiCaNa_ss_dvffrt * dvffrt_dv + dPhiCaNa_ss_dvfrt * dvfrt_dv)
-        * dICaNa_ss_dPhiCaNa_ss
+        - (dPhiCaK_i_dvffrt * dvffrt_dv + dPhiCaK_i_dvfrt * dvfrt_dv) * dICaK_i_dPhiCaK_i
+        - (dPhiCaK_ss_dvffrt * dvffrt_dv + dPhiCaK_ss_dvfrt * dvfrt_dv) * dICaK_ss_dPhiCaK_ss
+        - (dPhiCaL_i_dvffrt * dvffrt_dv + dPhiCaL_i_dvfrt * dvfrt_dv) * dICaL_i_dPhiCaL_i
+        - (dPhiCaL_ss_dvffrt * dvffrt_dv + dPhiCaL_ss_dvfrt * dvfrt_dv) * dICaL_ss_dPhiCaL_ss
+        - (dPhiCaNa_i_dvffrt * dvffrt_dv + dPhiCaNa_i_dvfrt * dvfrt_dv) * dICaNa_i_dPhiCaNa_i
+        - (dPhiCaNa_ss_dvffrt * dvffrt_dv + dPhiCaNa_ss_dvfrt * dvfrt_dv) * dICaNa_ss_dPhiCaNa_ss
         - (
             (
                 (
                     (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
@@ -5947,19 +5430,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5972,19 +5451,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6006,19 +5481,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6077,19 +5548,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6102,19 +5569,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6136,19 +5599,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6208,19 +5667,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6233,19 +5688,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6267,19 +5718,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6339,19 +5786,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6364,19 +5807,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6398,19 +5837,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6498,19 +5933,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6523,19 +5954,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6557,19 +5984,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -6628,19 +6051,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6653,19 +6072,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6687,19 +6102,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -6759,19 +6170,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6784,19 +6191,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6818,19 +6221,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -6890,19 +6289,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6915,19 +6310,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6949,19 +6340,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -7162,19 +6549,15 @@
     dx4_db3 = a1 * b2 + b2 * b4
     dJnakNa_db3 = (
         -3 * E2
         - 3 * (dE2_dx1 * dx1_db3 + dE2_dx4 * dx4_db3 + b1 * b2 * dE2_dx3) * b3
         + 3 * (dE1_dx1 * dx1_db3 + dE1_dx4 * dx4_db3 + b1 * b2 * dE1_dx3) * a3
     )
     dP_dnai = -eP / (
-        Knap
-        * (
-            (1 + H / Khp + nai / Knap + ki / Kxkur)
-            * (1 + H / Khp + nai / Knap + ki / Kxkur)
-        )
+        Knap * ((1 + H / Khp + nai / Knap + ki / Kxkur) * (1 + H / Khp + nai / Knap + ki / Kxkur))
     )
     dPhiCaNa_i_dgamma_nai = np.exp(vfrt) * nai * vffrt / (-1 + np.exp(vfrt))
     dgamma_nai_dIi = (
         -(
             -0.3
             - 1 / (2 * ((1 + np.sqrt(Ii)) * (1 + np.sqrt(Ii))))
             + 1 / (2 * (1 + np.sqrt(Ii)) * np.sqrt(Ii))
@@ -7240,16 +6623,15 @@
         kna1 * kna2 * (h4_i * h4_i)
     )
     dh6_i_dh4_i = -1 / (h4_i * h4_i)
     dx2_i_dk6_i = (k1_i + k8_i) * k4_i
     dx3_i_dk6_i = (k2_i + k3_i) * k8_i + k1_i * k3_i
     dnai_dt_linearized = dJdiffNa_dnai * vss / vmyo + (
         -dINab_dnai
-        - (0.0005 * dPhiCaNa_i_dgamma_nai * dgamma_nai_dIi + dPhiCaNa_i_dnai)
-        * dICaNa_i_dPhiCaNa_i
+        - (0.0005 * dPhiCaNa_i_dgamma_nai * dgamma_nai_dIi + dPhiCaNa_i_dnai) * dICaNa_i_dPhiCaNa_i
         - dENa_dnai * dINaL_dENa
         - dENa_dnai * dINa_dENa
         - 3
         * (
             (
                 (
                     (
@@ -7555,53 +6937,45 @@
         - 3
         * zk
         * (
             dJnakK_da1 * da1_dnai
             - 2
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE3_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE3_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE3_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE3_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE3_dx4
                 + b1 * b2 * dE3_dx3 * dP_dnai * db3_dP
             )
             * a1
             + 2
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE4_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE4_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE4_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE4_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE4_dx4
                 + b1 * b2 * dE4_dx3 * dP_dnai * db3_dP
             )
             * b1
         )
         * Pnak
         - 3
         * zna
         * (
             -3
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE2_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE2_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE2_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE2_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE2_dx4
                 + b1 * b2 * dE2_dx3 * dP_dnai * db3_dP
             )
             * b3
             + 3
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE1_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE1_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE1_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE1_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE1_dx4
                 + b1 * b2 * dE1_dx3 * dP_dnai * db3_dP
             )
             * a3
             + dJnakNa_db3 * dP_dnai * db3_dP
         )
         * Pnak
     ) * Acap / (F * vmyo)
@@ -7626,17 +7000,15 @@
     )
     dPhiCaNa_ss_dnass = (
         (np.exp(vfrt) * gamma_nass + 0.0005 * dgamma_nass_dIss * np.exp(vfrt) * nass)
         * vffrt
         / (-1 + np.exp(vfrt))
     )
     dh1_ss_dnass = (1 + hna) / kna3
-    dh2_ss_dnass = hna / (kna3 * h1_ss) - dh1_ss_dnass * hna * nass / (
-        kna3 * (h1_ss * h1_ss)
-    )
+    dh2_ss_dnass = hna / (kna3 * h1_ss) - dh1_ss_dnass * hna * nass / (kna3 * (h1_ss * h1_ss))
     dh4_ss_dnass = (1 + nass / kna2) / kna1 + nass / (kna1 * kna2)
     dh5_ss_dh4_ss = -(nass * nass) / (kna1 * kna2 * (h4_ss * h4_ss))
     dh5_ss_dnass = 2 * nass / (kna1 * kna2 * h4_ss) - (nass * nass) * dh4_ss_dnass / (
         kna1 * kna2 * (h4_ss * h4_ss)
     )
     dh6_ss_dh4_ss = -1 / (h4_ss * h4_ss)
     dx2_ss_dk6_ss = (k1_ss + k8_ss) * k4_ss
@@ -7941,17 +7313,15 @@
                     + dh1_ss_dnass * dh3_ss_dh1_ss * dk4p_ss_dh3_ss
                 )
                 * dE4_ss_dx4_ss
                 * k2_ss
                 * k8_ss
             )
             * k7_ss
-            + wnaca
-            * (dh1_ss_dnass * dh2_ss_dh1_ss + dh2_ss_dnass)
-            * dJncxNa_ss_dk4pp_ss
+            + wnaca * (dh1_ss_dnass * dh2_ss_dh1_ss + dh2_ss_dnass) * dJncxNa_ss_dk4pp_ss
         )
         * dINaCa_ss_dJncxNa_ss
     ) * Acap / (F * vss)
     states[36] = (
         np.where(
             np.abs(dnass_dt_linearized) > 1e-08,
             (-1 + np.exp(dt * dnass_dt_linearized)) * dnass_dt / dnass_dt_linearized,
@@ -7971,22 +7341,18 @@
             (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
             * (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
         )
     )
     dbK1_dEK = (
         -6.919349479611957e-18 * np.exp(0.0618 * v - 0.0618 * EK)
         - 0.8506978434250505 * np.exp(0.0674 * v - 0.0674 * EK)
-    ) / (
-        1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)
-    ) - 0.016099950792318272 * (
+    ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)) - 0.016099950792318272 * (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
-    ) * np.exp(
-        0.1629 * EK - 0.1629 * v
-    ) / (
+    ) * np.exp(0.1629 * EK - 0.1629 * v) / (
         (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
         * (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     )
     dIK1_dEK = (
         -np.sqrt(5) * np.sqrt(ko) * GK1 * K1ss / 5
         + np.sqrt(5)
         * np.sqrt(ko)
@@ -7998,19 +7364,15 @@
     dIKb_dEK = -GKb * xkb
     dIKr_dEK = -np.sqrt(5) * np.sqrt(ko) * GKr * O / 5
     dIKs_dEKs = -GKs * KsCa * xs1 * xs2
     dI_katp_dEK = -fkatp * gkatp * akik * bkik
     dIto_dEK = -((1 - fItop) * a * i + ap * fItop * ip) * Gto
     dJdiffK_dki = -1 / tauK
     dP_dki = -eP / (
-        Kxkur
-        * (
-            (1 + H / Khp + nai / Knap + ki / Kxkur)
-            * (1 + H / Khp + nai / Knap + ki / Kxkur)
-        )
+        Kxkur * ((1 + H / Khp + nai / Knap + ki / Kxkur) * (1 + H / Khp + nai / Knap + ki / Kxkur))
     )
     dPhiCaK_i_dgamma_ki = np.exp(vfrt) * ki * vffrt / (-1 + np.exp(vfrt))
     dgamma_ki_dIi = (
         -(
             -0.3
             - 1 / (2 * ((1 + np.sqrt(Ii)) * (1 + np.sqrt(Ii))))
             + 1 / (2 * (1 + np.sqrt(Ii)) * np.sqrt(Ii))
@@ -8064,70 +7426,60 @@
                 -1
                 + ((1 + ki / Kki) * (1 + ki / Kki))
                 + ((1 + nai / Knai) * (1 + nai / Knai) * (1 + nai / Knai))
             )
         )
     )
     dki_dt_linearized = dJdiffK_dki * vss / vmyo + (
-        -(0.0005 * dPhiCaK_i_dgamma_ki * dgamma_ki_dIi + dPhiCaK_i_dki)
-        * dICaK_i_dPhiCaK_i
-        - (dEK_dki * dK1ss_daK1 * daK1_dEK + dEK_dki * dK1ss_dbK1 * dbK1_dEK)
-        * dIK1_dK1ss
+        -(0.0005 * dPhiCaK_i_dgamma_ki * dgamma_ki_dIi + dPhiCaK_i_dki) * dICaK_i_dPhiCaK_i
+        - (dEK_dki * dK1ss_daK1 * daK1_dEK + dEK_dki * dK1ss_dbK1 * dbK1_dEK) * dIK1_dK1ss
         - dEK_dki * dIK1_dEK
         - dEK_dki * dIKb_dEK
         - dEK_dki * dIKr_dEK
         - dEK_dki * dI_katp_dEK
         - dEK_dki * dIto_dEK
         - dEKs_dki * dIKs_dEKs
         + 2
         * zk
         * (
             dJnakK_da1 * da1_dki
             - 2
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE3_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE3_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE3_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE3_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE3_dx4
                 + b1 * b2 * dE3_dx3 * dP_dki * db3_dP
             )
             * a1
             + 2
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE4_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE4_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE4_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE4_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE4_dx4
                 + b1 * b2 * dE4_dx3 * dP_dki * db3_dP
             )
             * b1
         )
         * Pnak
         + 2
         * zna
         * (
             -3
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE2_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE2_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE2_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE2_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE2_dx4
                 + b1 * b2 * dE2_dx3 * dP_dki * db3_dP
             )
             * b3
             + 3
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE1_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE1_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE1_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE1_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE1_dx4
                 + b1 * b2 * dE1_dx3 * dP_dki * db3_dP
             )
             * a3
             + dJnakNa_db3 * dP_dki * db3_dP
         )
         * Pnak
     ) * Acap / (F * vmyo)
@@ -8180,17 +7532,15 @@
             dt * dcli_dt,
         )
         + cli
     )
     dclss_dt = -JdiffCl + Acap * IClCa_junc / (F * vss)
     dEClss_dclss = -R * T / (F * zcl * clss)
     dIClCa_junc_dEClss = -Fjunc * GClCa / (1 + KdClCa / cass)
-    dclss_dt_linearized = -1 / tauNa + Acap * dEClss_dclss * dIClCa_junc_dEClss / (
-        F * vss
-    )
+    dclss_dt_linearized = -1 / tauNa + Acap * dEClss_dclss * dIClCa_junc_dEClss / (F * vss)
     states[40] = (
         np.where(
             np.abs(dclss_dt_linearized) > 1e-08,
             (-1 + np.exp(dt * dclss_dt_linearized)) * dclss_dt / dclss_dt_linearized,
             dt * dclss_dt,
         )
         + clss
@@ -8229,67 +7579,55 @@
         )
         * constA
         * np.exp(-4 * (-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     )
     dICab_dcai = (
         4
         * PCab
-        * (
-            np.exp(2 * vfrt) * gamma_cai
-            + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt)
-        )
+        * (np.exp(2 * vfrt) * gamma_cai + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt))
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    dICab_dgamma_cai = (
-        4 * PCab * cai * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
-    )
+    dICab_dgamma_cai = 4 * PCab * cai * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
     dINaCa_i_dallo_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx
     dIpCa_dcai = GpCa / (KmCap + cai) - GpCa * cai / ((KmCap + cai) * (KmCap + cai))
     dJdiff_dcai = -1 / tauCa
     dJup_dJupnp = Jup_b * (1 - fJupp)
     dJupnp_dcai = 0.005425 * upScale / (0.00092 + cai) - 0.005425 * cai * upScale / (
         (0.00092 + cai) * (0.00092 + cai)
     )
     dJupp_dcai = 0.01491875 * upScale / (0.00075 + cai) - 0.01491875 * cai * upScale / (
         (0.00075 + cai) * (0.00075 + cai)
     )
     dPhiCaL_i_dcai = (
         4
-        * (
-            np.exp(2 * vfrt) * gamma_cai
-            + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt)
-        )
+        * (np.exp(2 * vfrt) * gamma_cai + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt))
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
     dPhiCaL_i_dgamma_cai = 4 * cai * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
     dallo_i_dcai = (
         2
         * (KmCaAct * KmCaAct)
         / (
-            (
-                (1 + (KmCaAct * KmCaAct) / (cai * cai))
-                * (1 + (KmCaAct * KmCaAct) / (cai * cai))
-            )
+            ((1 + (KmCaAct * KmCaAct) / (cai * cai)) * (1 + (KmCaAct * KmCaAct) / (cai * cai)))
             * (cai * cai * cai)
         )
     )
     dcai_dt_linearized = (
         Jdiff * vss / vmyo
         - Jup * vnsr / vmyo
         + (-ICaL_i - ICab - IpCa + 2 * INaCa_i) * Acap / (2 * F * vmyo)
     ) * dBcai_dcai + (
         dJdiff_dcai * vss / vmyo
         - (dJup_dJupnp * dJupnp_dcai + Jup_b * dJupp_dcai * fJupp) * vnsr / vmyo
         + (
             -dICab_dcai
             - dIpCa_dcai
-            - (0.002 * dPhiCaL_i_dgamma_cai * dgamma_cai_dIi + dPhiCaL_i_dcai)
-            * dICaL_i_dPhiCaL_i
+            - (0.002 * dPhiCaL_i_dgamma_cai * dgamma_cai_dIi + dPhiCaL_i_dcai) * dICaL_i_dPhiCaL_i
             + 2
             * (
                 (
                     kcaon * dE2_i_dx2_i * dx2_i_dk6_i * h6_i
                     + kcaon * dE2_i_dx3_i * dx3_i_dk6_i * h6_i
                     + kcaon * dE2_i_dx1_i * h6_i * k2_i * k4_i
                 )
@@ -8366,18 +7704,15 @@
         * (
             1
             + BSLmax * KmBSL / ((KmBSL + cass) * (KmBSL + cass))
             + BSRmax * KmBSR / ((KmBSR + cass) * (KmBSR + cass))
         )
     )
     dCaMKb_dcass = (
-        CaMKo
-        * KmCaM
-        * (1 - CaMKt)
-        / (((1 + KmCaM / cass) * (1 + KmCaM / cass)) * (cass * cass))
+        CaMKo * KmCaM * (1 - CaMKt) / (((1 + KmCaM / cass) * (1 + KmCaM / cass)) * (cass * cass))
     )
     dICaL_ss_dfICaLp = ICaL_fractionSS * (
         ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCap * PhiCaL_ss * d
         - ((1 - nca_ss) * f + fca * jca * nca_ss) * PCa * PhiCaL_ss * d
     )
     dINaCa_ss_dallo_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx
     dJrel_dfJrelp = Jrel_b * (-Jrel_np + Jrel_p)
@@ -8389,41 +7724,29 @@
             + 1 / (2 * (1 + np.sqrt(Iss)) * np.sqrt(Iss))
         )
         * constA
         * np.exp(-4 * (-0.3 * Iss + np.sqrt(Iss) / (1 + np.sqrt(Iss))) * constA)
     )
     dPhiCaL_ss_dcass = (
         4
-        * (
-            np.exp(2 * vfrt) * gamma_cass
-            + 0.002 * cass * dgamma_cass_dIss * np.exp(2 * vfrt)
-        )
+        * (np.exp(2 * vfrt) * gamma_cass + 0.002 * cass * dgamma_cass_dIss * np.exp(2 * vfrt))
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    dPhiCaL_ss_dgamma_cass = (
-        4 * cass * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
-    )
+    dPhiCaL_ss_dgamma_cass = 4 * cass * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
     dallo_ss_dcass = (
         2
         * (KmCaAct * KmCaAct)
         / (
-            (
-                (1 + (KmCaAct * KmCaAct) / (cass * cass))
-                * (1 + (KmCaAct * KmCaAct) / (cass * cass))
-            )
+            ((1 + (KmCaAct * KmCaAct) / (cass * cass)) * (1 + (KmCaAct * KmCaAct) / (cass * cass)))
             * (cass * cass * cass)
         )
     )
-    dfICaLp_dCaMKa = KmCaMK / (
-        ((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa)
-    )
-    dfJrelp_dCaMKa = KmCaMK / (
-        ((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa)
-    )
+    dfICaLp_dCaMKa = KmCaMK / (((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa))
+    dfJrelp_dCaMKa = KmCaMK / (((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa))
     dcass_dt_linearized = (
         -1 / tauCa
         + (
             -(0.002 * dPhiCaL_ss_dgamma_cass * dgamma_cass_dIss + dPhiCaL_ss_dcass)
             * dICaL_ss_dPhiCaL_ss
             + 2
             * (
```

### Comparing `fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/epi.py` & `fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/epi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1181,17 +1181,15 @@
     E1_i = x1_i / (x1_i + x2_i + x3_i + x4_i)
     E2_i = x2_i / (x1_i + x2_i + x3_i + x4_i)
     E3_i = x3_i / (x1_i + x2_i + x3_i + x4_i)
     E4_i = x4_i / (x1_i + x2_i + x3_i + x4_i)
     allo_i = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     JncxNa_i = E3_i * k4pp_i - E2_i * k3pp_i - 3 * E1_i * k8_i + 3 * E4_i * k7_i
     JncxCa_i = E2_i * k2_i - E1_i * k1_i
-    Gncx = np.where(
-        celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b)
-    )
+    Gncx = np.where(celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b))
     INaCa_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx * allo_i
     h1_ss = 1 + (1 + hna) * nass / kna3
     h2_ss = hna * nass / (kna3 * h1_ss)
     h3_ss = 1.0 / h1_ss
     h4_ss = 1 + (1 + nass / kna2) * nass / kna1
     h5_ss = (nass * nass) / (kna1 * kna2 * h4_ss)
     h6_ss = 1.0 / h4_ss
@@ -1218,17 +1216,15 @@
     x3_ss = (k2_ss + k3_ss) * k6_ss * k8_ss + (k6_ss + k7_ss) * k1_ss * k3_ss
     x4_ss = (k1_ss + k8_ss) * k3_ss * k5_ss + (k4_ss + k5_ss) * k2_ss * k8_ss
     E1_ss = x1_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E2_ss = x2_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E3_ss = x3_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E4_ss = x4_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     allo_ss = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
-    JncxNa_ss = (
-        E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
-    )
+    JncxNa_ss = E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
     JncxCa_ss = E2_ss * k2_ss - E1_ss * k1_ss
     INaCa_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx * allo_ss
 
     # Expressions for the K component
     Knai = Knai0 * np.exp(delta * vfrt / 3)
     Knao = Knao0 * np.exp((1 - delta) * vfrt / 3)
     P = eP / (1 + H / Khp + nai / Knap + ki / Kxkur)
@@ -1290,17 +1286,15 @@
     x4 = a1 * a3 * a4 + a1 * a4 * b2 + a1 * b2 * b3 + b2 * b3 * b4
     E1 = x1 / (x1 + x2 + x3 + x4)
     E2 = x2 / (x1 + x2 + x3 + x4)
     E3 = x3 / (x1 + x2 + x3 + x4)
     E4 = x4 / (x1 + x2 + x3 + x4)
     JnakNa = -3 * E2 * b3 + 3 * E1 * a3
     JnakK = -2 * E3 * a1 + 2 * E4 * b1
-    Pnak = np.where(
-        celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
-    )
+    Pnak = np.where(celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b))
     INaK = (zk * JnakK + zna * JnakNa) * Pnak
 
     # Expressions for the b component
     INab = PNab * (-nao + np.exp(vfrt) * nai) * vffrt / (-1 + np.exp(vfrt))
 
     # Expressions for the IpCa component
     IpCa = GpCa * cai / (KmCap + cai)
@@ -1324,17 +1318,15 @@
             3.5254214873653824 * np.exp(0.09 * vShift + 0.09 * v)
             + 0.7408182206817179 * np.exp(-0.05 * vShift - 0.05 * v)
         )
     )
     values[1] = (-d + dss) / td
     fss = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
     tff = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
-    tfs = 1000 + 1.0 / (
-        3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
-    )
+    tfs = 1000 + 1.0 / (3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6))
     Afs = 1 - Aff
     values[2] = (-ff + fss) / tff
     values[3] = (-fs + fss) / tfs
     f = Aff * ff + Afs * fs
     fcass = fss
     tfcaf = 7 + 1.0 / (0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7))
     tfcas = 100 + 1.0 / (0.00012 * np.exp(-v / 3) + 0.00012 * np.exp(v / 7))
@@ -1365,25 +1357,17 @@
     gamma_ko = np.exp(-(-0.3 * Io + np.sqrt(Io) / (1 + np.sqrt(Io))) * constA)
     PhiCaL_ss = (
         4
         * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_ss = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_ss = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
-    )
-    PCa = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    PhiCaNa_ss = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_ss = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
+    PCa = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     PCap = 1.1 * PCa
     PCaNa = 0.00125 * PCa
     PCaK = 0.0003574 * PCa
     PCaNap = 0.00125 * PCap
     PCaKp = 0.0003574 * PCap
     fICaLp = 1.0 / (1 + KmCaMK / CaMKa)
     ICaL_ss = ICaL_fractionSS * (
@@ -1406,22 +1390,16 @@
     gamma_ki = np.exp(-(-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     PhiCaL_i = (
         4
         * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_i = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_i = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
-    )
+    PhiCaNa_i = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_i = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
     ICaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * PhiCaL_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * PhiCaL_i * d * fICaLp
     )
     ICaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * PhiCaNa_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * PhiCaNa_i * d * fICaLp
@@ -1464,17 +1442,15 @@
         )
     )
     values[11] = (-m + mss) / tm
     hss = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    ah = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    ah = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     bh = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     th = 1.0 / (ah + bh)
     values[12] = (-h + hss) / th
@@ -1484,17 +1460,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     bj = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     jss = hss
     tj = 1.0 / (aj + bj)
     values[13] = (-j + jss) / tj
     hssp = 1.0 / (
         (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
         * (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
@@ -1526,74 +1500,54 @@
     values[18] = (-hLp + hLssp) / thLp
     GNaL = np.where(celltype == 1, 0.6 * GNaL_b, GNaL_b)
     fINaLp = 1.0 / (1 + KmCaMK / CaMKa)
     INaL = (-ENa + v) * ((1 - fINaLp) * hL + fINaLp * hLp) * GNaL * mL
 
     # Expressions for the Ito component
     ass = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     ta = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     values[19] = (-a + ass) / ta
     iss = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    delta_epi = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    delta_epi = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     tiF_b = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     tiS_b = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     tiF = delta_epi * tiF_b
     tiS = delta_epi * tiS_b
     AiF = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     AiS = 1 - AiF
     values[20] = (-iF + iss) / tiF
     values[21] = (-iS + iss) / tiS
     i = AiF * iF + AiS * iS
     assp = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     values[22] = (-ap + assp) / ta
     dti_develop = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
     dti_recover = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     tiFp = dti_develop * dti_recover * tiF
     tiSp = dti_develop * dti_recover * tiS
     values[23] = (-iFp + iss) / tiFp
     values[24] = (-iSp + iss) / tiSp
     ip = AiF * iFp + AiS * iSp
@@ -1608,53 +1562,42 @@
     beta_2 = 0.000349 * np.exp(-1.062 * vfrt)
     alpha_i = 0.2533 * np.exp(0.5953 * vfrt)
     beta_i = 0.06525 * np.exp(-0.8209 * vfrt)
     alpha_C2ToI = 5.2e-05 * np.exp(1.525 * vfrt)
     beta_ItoC2 = alpha_C2ToI * beta_2 * beta_i / (alpha_2 * alpha_i)
     values[25] = C2 * beta - C3 * alpha
     values[26] = beta_1 * C1 + C3 * alpha - (alpha_1 + beta) * C2
-    values[27] = (
-        alpha_1 * C2
-        + I * beta_ItoC2
-        + O * beta_2
-        - (beta_1 + alpha_2 + alpha_C2ToI) * C1
-    )
+    values[27] = alpha_1 * C2 + I * beta_ItoC2 + O * beta_2 - (beta_1 + alpha_2 + alpha_C2ToI) * C1
     values[28] = C1 * alpha_2 + I * beta_i - (alpha_i + beta_2) * O
     values[29] = C1 * alpha_C2ToI + O * alpha_i - (beta_ItoC2 + beta_i) * I
-    GKr = np.where(
-        celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
-    )
+    GKr = np.where(celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b))
     IKr = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GKr * O / 5
 
     # Expressions for the IKs component
     xs1ss = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     txs1 = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
     values[30] = (-xs1 + xs1ss) / txs1
     xs2ss = xs1ss
-    txs2 = 1.0 / (
-        0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20)
-    )
+    txs2 = 1.0 / (0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20))
     values[31] = (-xs2 + xs2ss) / txs2
     KsCa = 1 + 0.6 / (1 + 6.481821026062645e-07 * np.power(1.0 / cai, 1.4))
     GKs = np.where(celltype == 1, 1.4 * GKs_b, GKs_b)
     IKs = (-EKs + v) * GKs * KsCa * xs1 * xs2
 
     # Expressions for the IK1 component
     aK1 = 4.094 / (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
     bK1 = (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     K1ss = aK1 / (aK1 + bK1)
-    GK1 = np.where(
-        celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
-    )
+    GK1 = np.where(celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b))
     IK1 = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 * K1ss / 5
 
     # Expressions for the IKb component
     xkb = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     GKb = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     IKb = (-EK + v) * GKb * xkb
 
@@ -1690,17 +1633,15 @@
     fJrelp = 1.0 / (1 + KmCaMK / CaMKa)
     Jrel = Jrel_b * ((1 - fJrelp) * Jrel_np + Jrel_p * fJrelp)
 
     # Expressions for the Membrane component
     Istim = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     values[34] = (
         -ICaK
@@ -1997,26 +1938,18 @@
     ) * monitored[42] * monitored[52]
     monitored[56] = (monitored[43] + monitored[46]) * monitored[51] * monitored[53] + (
         monitored[51] + monitored[52]
     ) * monitored[42] * monitored[46]
     monitored[57] = (monitored[42] + monitored[53]) * monitored[46] * monitored[50] + (
         monitored[49] + monitored[50]
     ) * monitored[43] * monitored[53]
-    monitored[58] = monitored[54] / (
-        monitored[54] + monitored[55] + monitored[56] + monitored[57]
-    )
-    monitored[59] = monitored[55] / (
-        monitored[54] + monitored[55] + monitored[56] + monitored[57]
-    )
-    monitored[60] = monitored[56] / (
-        monitored[54] + monitored[55] + monitored[56] + monitored[57]
-    )
-    monitored[61] = monitored[57] / (
-        monitored[54] + monitored[55] + monitored[56] + monitored[57]
-    )
+    monitored[58] = monitored[54] / (monitored[54] + monitored[55] + monitored[56] + monitored[57])
+    monitored[59] = monitored[55] / (monitored[54] + monitored[55] + monitored[56] + monitored[57])
+    monitored[60] = monitored[56] / (monitored[54] + monitored[55] + monitored[56] + monitored[57])
+    monitored[61] = monitored[57] / (monitored[54] + monitored[55] + monitored[56] + monitored[57])
     monitored[62] = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     monitored[63] = (
         monitored[48] * monitored[60]
         - monitored[45] * monitored[59]
         - 3 * monitored[53] * monitored[58]
         + 3 * monitored[52] * monitored[61]
     )
@@ -2062,26 +1995,18 @@
     ) * monitored[79] * monitored[89]
     monitored[93] = (monitored[80] + monitored[83]) * monitored[88] * monitored[90] + (
         monitored[88] + monitored[89]
     ) * monitored[79] * monitored[83]
     monitored[94] = (monitored[79] + monitored[90]) * monitored[83] * monitored[87] + (
         monitored[86] + monitored[87]
     ) * monitored[80] * monitored[90]
-    monitored[95] = monitored[91] / (
-        monitored[91] + monitored[92] + monitored[93] + monitored[94]
-    )
-    monitored[96] = monitored[92] / (
-        monitored[91] + monitored[92] + monitored[93] + monitored[94]
-    )
-    monitored[97] = monitored[93] / (
-        monitored[91] + monitored[92] + monitored[93] + monitored[94]
-    )
-    monitored[98] = monitored[94] / (
-        monitored[91] + monitored[92] + monitored[93] + monitored[94]
-    )
+    monitored[95] = monitored[91] / (monitored[91] + monitored[92] + monitored[93] + monitored[94])
+    monitored[96] = monitored[92] / (monitored[91] + monitored[92] + monitored[93] + monitored[94])
+    monitored[97] = monitored[93] / (monitored[91] + monitored[92] + monitored[93] + monitored[94])
+    monitored[98] = monitored[94] / (monitored[91] + monitored[92] + monitored[93] + monitored[94])
     monitored[99] = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
     monitored[100] = (
         monitored[85] * monitored[97]
         - monitored[82] * monitored[96]
         - 3 * monitored[90] * monitored[95]
         + 3 * monitored[89] * monitored[98]
     )
@@ -2197,20 +2122,16 @@
     )
     monitored[120] = monitored[116] / (
         monitored[114] + monitored[115] + monitored[116] + monitored[117]
     )
     monitored[121] = monitored[117] / (
         monitored[114] + monitored[115] + monitored[116] + monitored[117]
     )
-    monitored[122] = (
-        -3 * monitored[111] * monitored[119] + 3 * monitored[110] * monitored[118]
-    )
-    monitored[123] = (
-        -2 * monitored[106] * monitored[120] + 2 * monitored[107] * monitored[121]
-    )
+    monitored[122] = -3 * monitored[111] * monitored[119] + 3 * monitored[110] * monitored[118]
+    monitored[123] = -2 * monitored[106] * monitored[120] + 2 * monitored[107] * monitored[121]
     monitored[124] = np.where(
         celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
     )
     monitored[125] = (zk * monitored[123] + zna * monitored[122]) * monitored[124]
 
     # Expressions for the b component
     monitored[126] = (
@@ -2229,42 +2150,36 @@
     monitored[138] = (-cai + cass) / tauCa
     monitored[139] = (-cli + clss) / tauNa
 
     # Expressions for the Trans flux component
     monitored[275] = -cajsr / 60 + cansr / 60
 
     # Expressions for the ICaL component
-    monitored[140] = np.where(
-        v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v))
-    )
+    monitored[140] = np.where(v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v)))
     monitored[141] = (
         0.6
         + offset
         + 1.0
         / (
             3.5254214873653824 * np.exp(0.09 * vShift + 0.09 * v)
             + 0.7408182206817179 * np.exp(-0.05 * vShift - 0.05 * v)
         )
     )
     monitored[277] = (-d + monitored[140]) / monitored[141]
     monitored[142] = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
-    monitored[143] = 7 + 1.0 / (
-        0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10)
-    )
+    monitored[143] = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
     monitored[144] = 1000 + 1.0 / (
         3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
     )
     monitored[145] = 1 - Aff
     monitored[278] = (-ff + monitored[142]) / monitored[143]
     monitored[279] = (-fs + monitored[142]) / monitored[144]
     monitored[146] = Aff * ff + fs * monitored[145]
     monitored[147] = monitored[142]
-    monitored[148] = 7 + 1.0 / (
-        0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7)
-    )
+    monitored[148] = 7 + 1.0 / (0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7))
     monitored[149] = 100 + 1.0 / (0.00012 * np.exp(-v / 3) + 0.00012 * np.exp(v / 7))
     monitored[150] = 0.3 + 0.6 / (1 + np.exp(-1 + v / 10))
     monitored[151] = 1 - monitored[150]
     monitored[280] = (-fcaf + monitored[147]) / monitored[148]
     monitored[281] = (-fcas + monitored[147]) / monitored[149]
     monitored[152] = fcaf * monitored[150] + fcas * monitored[151]
     monitored[153] = 1.0 / (1.0 + 649.7401897235336 * np.exp(0.35821750967187277 * v))
@@ -2279,54 +2194,36 @@
     monitored[159] = 1.0 / (np.power(1 + Kmn / cass, 4) + k2n / monitored[158])
     monitored[285] = k2n * monitored[159] - monitored[158] * nca_ss
     monitored[160] = 0.0005 * clo + 0.0005 * ko + 0.0005 * nao + 0.002 * cao
     monitored[161] = 0.0005 * clss + 0.0005 * kss + 0.0005 * nass + 0.002 * cass
     monitored[162] = 1820000.0 * np.power(T * dielConstant, -1.5)
     monitored[163] = np.exp(
         -4
-        * (
-            -0.3 * monitored[161]
-            + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161]))
-        )
+        * (-0.3 * monitored[161] + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161])))
         * monitored[162]
     )
     monitored[164] = np.exp(
         -4
-        * (
-            -0.3 * monitored[160]
-            + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160]))
-        )
+        * (-0.3 * monitored[160] + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160])))
         * monitored[162]
     )
     monitored[165] = np.exp(
-        -(
-            -0.3 * monitored[161]
-            + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161]))
-        )
+        -(-0.3 * monitored[161] + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161])))
         * monitored[162]
     )
     monitored[166] = np.exp(
-        -(
-            -0.3 * monitored[160]
-            + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160]))
-        )
+        -(-0.3 * monitored[160] + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160])))
         * monitored[162]
     )
     monitored[167] = np.exp(
-        -(
-            -0.3 * monitored[161]
-            + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161]))
-        )
+        -(-0.3 * monitored[161] + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161])))
         * monitored[162]
     )
     monitored[168] = np.exp(
-        -(
-            -0.3 * monitored[160]
-            + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160]))
-        )
+        -(-0.3 * monitored[160] + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160])))
         * monitored[162]
     )
     monitored[169] = (
         4
         * (-cao * monitored[164] + cass * np.exp(2 * monitored[273]) * monitored[163])
         * monitored[274]
         / (-1 + np.exp(2 * monitored[273]))
@@ -2337,17 +2234,15 @@
         / (-1 + np.exp(monitored[273]))
     )
     monitored[171] = (
         (-ko * monitored[168] + np.exp(monitored[273]) * kss * monitored[167])
         * monitored[274]
         / (-1 + np.exp(monitored[273]))
     )
-    monitored[172] = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    monitored[172] = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     monitored[173] = 1.1 * monitored[172]
     monitored[174] = 0.00125 * monitored[172]
     monitored[175] = 0.0003574 * monitored[172]
     monitored[176] = 0.00125 * monitored[173]
     monitored[177] = 0.0003574 * monitored[173]
     monitored[178] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[179] = ICaL_fractionSS * (
@@ -2387,32 +2282,23 @@
         * monitored[178]
     )
     monitored[182] = 1.0 / (np.power(1 + Kmn / cai, 4) + k2n / monitored[158])
     monitored[286] = k2n * monitored[182] - monitored[158] * nca_i
     monitored[183] = 0.0005 * cli + 0.0005 * ki + 0.0005 * nai + 0.002 * cai
     monitored[184] = np.exp(
         -4
-        * (
-            -0.3 * monitored[183]
-            + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183]))
-        )
+        * (-0.3 * monitored[183] + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183])))
         * monitored[162]
     )
     monitored[185] = np.exp(
-        -(
-            -0.3 * monitored[183]
-            + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183]))
-        )
+        -(-0.3 * monitored[183] + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183])))
         * monitored[162]
     )
     monitored[186] = np.exp(
-        -(
-            -0.3 * monitored[183]
-            + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183]))
-        )
+        -(-0.3 * monitored[183] + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183])))
         * monitored[162]
     )
     monitored[187] = (
         4
         * (-cao * monitored[164] + cai * np.exp(2 * monitored[273]) * monitored[184])
         * monitored[274]
         / (-1 + np.exp(2 * monitored[273]))
@@ -2470,25 +2356,21 @@
     # Expressions for the SERCA component
     monitored[196] = np.where(celltype == 1, 1.3, 1)
     monitored[197] = 0.005425 * cai * monitored[196] / (0.00092 + cai)
     monitored[198] = 0.01491875 * cai * monitored[196] / (0.00075 + cai)
     monitored[199] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[200] = 0.0003255 * cansr
     monitored[201] = Jup_b * (
-        -monitored[200]
-        + (1 - monitored[199]) * monitored[197]
-        + monitored[198] * monitored[199]
+        -monitored[200] + (1 - monitored[199]) * monitored[197] + monitored[198] * monitored[199]
     )
 
     # Expressions for the I_katp component
     monitored[202] = np.power(ko / K_o_n, 0.24)
     monitored[203] = 1.0 / (1 + (A_atp * A_atp) / (K_atp * K_atp))
-    monitored[204] = (
-        fkatp * gkatp * (-monitored[10] + v) * monitored[202] * monitored[203]
-    )
+    monitored[204] = fkatp * gkatp * (-monitored[10] + v) * monitored[202] * monitored[203]
 
     # Expressions for the INa component
     monitored[14] = 1.0 / (
         (1 + 0.0018422115811651339 * np.exp(-0.1107419712070875 * v))
         * (1 + 0.0018422115811651339 * np.exp(-0.1107419712070875 * v))
     )
     monitored[15] = 0.1292 * np.exp(
@@ -2503,17 +2385,15 @@
         )
     )
     monitored[287] = (-m + monitored[14]) / monitored[15]
     monitored[16] = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    monitored[17] = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    monitored[17] = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     monitored[18] = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     monitored[19] = 1.0 / (monitored[17] + monitored[18])
     monitored[288] = (-h + monitored[16]) / monitored[19]
@@ -2523,17 +2403,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     monitored[21] = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     monitored[22] = monitored[16]
     monitored[23] = 1.0 / (monitored[20] + monitored[21])
     monitored[289] = (-j + monitored[22]) / monitored[23]
     monitored[24] = 1.0 / (
         (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
         * (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
@@ -2575,109 +2453,79 @@
         * ((1 - monitored[133]) * hL + hLp * monitored[133])
         * mL
         * monitored[132]
     )
 
     # Expressions for the Ito component
     monitored[205] = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     monitored[206] = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     monitored[295] = (-a + monitored[205]) / monitored[206]
     monitored[207] = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    monitored[208] = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    monitored[208] = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     monitored[209] = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     monitored[210] = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     monitored[211] = monitored[208] * monitored[209]
     monitored[212] = monitored[208] * monitored[210]
     monitored[213] = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     monitored[214] = 1 - monitored[213]
     monitored[296] = (-iF + monitored[207]) / monitored[211]
     monitored[297] = (-iS + monitored[207]) / monitored[212]
     monitored[215] = iF * monitored[213] + iS * monitored[214]
     monitored[216] = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     monitored[298] = (-ap + monitored[216]) / monitored[206]
     monitored[217] = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
-    )
-    monitored[218] = 1 - 0.5 / (
-        1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
+    monitored[218] = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     monitored[219] = monitored[211] * monitored[217] * monitored[218]
     monitored[220] = monitored[212] * monitored[217] * monitored[218]
     monitored[299] = (-iFp + monitored[207]) / monitored[219]
     monitored[300] = (-iSp + monitored[207]) / monitored[220]
     monitored[221] = iFp * monitored[213] + iSp * monitored[214]
-    monitored[222] = np.where(
-        celltype == 1, 2 * Gto_b, np.where(celltype == 2, 2 * Gto_b, Gto_b)
-    )
+    monitored[222] = np.where(celltype == 1, 2 * Gto_b, np.where(celltype == 2, 2 * Gto_b, Gto_b))
     monitored[223] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[224] = (
         (-monitored[10] + v)
-        * (
-            (1 - monitored[223]) * a * monitored[215]
-            + ap * monitored[221] * monitored[223]
-        )
+        * ((1 - monitored[223]) * a * monitored[215] + ap * monitored[221] * monitored[223])
         * monitored[222]
     )
 
     # Expressions for the IKr component
     monitored[225] = 0.1161 * np.exp(0.299 * monitored[273])
     monitored[226] = 0.2442 * np.exp(-1.604 * monitored[273])
     monitored[227] = 0.0578 * np.exp(0.971 * monitored[273])
     monitored[228] = 0.000349 * np.exp(-1.062 * monitored[273])
     monitored[229] = 0.2533 * np.exp(0.5953 * monitored[273])
     monitored[230] = 0.06525 * np.exp(-0.8209 * monitored[273])
     monitored[231] = 5.2e-05 * np.exp(1.525 * monitored[273])
     monitored[232] = (
-        monitored[228]
-        * monitored[230]
-        * monitored[231]
-        / (monitored[227] * monitored[229])
+        monitored[228] * monitored[230] * monitored[231] / (monitored[227] * monitored[229])
     )
     monitored[301] = C2 * monitored[226] - C3 * monitored[225]
     monitored[302] = beta_1 * C1 + C3 * monitored[225] - (alpha_1 + monitored[226]) * C2
     monitored[303] = (
         alpha_1 * C2
         + I * monitored[232]
         + O * monitored[228]
@@ -2688,17 +2536,15 @@
     )
     monitored[305] = (
         C1 * monitored[231] + O * monitored[229] - (monitored[230] + monitored[232]) * I
     )
     monitored[233] = np.where(
         celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
     )
-    monitored[234] = (
-        np.sqrt(5) * np.sqrt(ko) * (-monitored[10] + v) * O * monitored[233] / 5
-    )
+    monitored[234] = np.sqrt(5) * np.sqrt(ko) * (-monitored[10] + v) * O * monitored[233] / 5
 
     # Expressions for the IKs component
     monitored[235] = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     monitored[236] = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
@@ -2721,20 +2567,15 @@
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * monitored[10])
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * monitored[10] - 0.1629 * v))
     monitored[244] = monitored[242] / (monitored[242] + monitored[243])
     monitored[245] = np.where(
         celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
     )
     monitored[246] = (
-        np.sqrt(5)
-        * np.sqrt(ko)
-        * (-monitored[10] + v)
-        * monitored[244]
-        * monitored[245]
-        / 5
+        np.sqrt(5) * np.sqrt(ko) * (-monitored[10] + v) * monitored[244] * monitored[245] / 5
     )
 
     # Expressions for the IKb component
     monitored[247] = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     monitored[248] = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     monitored[249] = (-monitored[10] + v) * monitored[247] * monitored[248]
 
@@ -2752,43 +2593,37 @@
         * monitored[274]
         / (-1 + np.exp(2 * monitored[273]))
     )
 
     # Expressions for the Ryr component
     monitored[255] = 0.5 * bt
     monitored[256] = (
-        -monitored[179]
-        * monitored[255]
-        / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
+        -monitored[179] * monitored[255] / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
     )
     monitored[257] = np.where(celltype == 2, 1.7 * monitored[256], monitored[256])
     monitored[258] = bt / (1 + 0.0123 / cajsr)
     monitored[259] = np.where(monitored[258] < 0.001, 0.001, monitored[258])
     monitored[308] = (-Jrel_np + monitored[257]) / monitored[259]
     monitored[260] = 1.25 * bt
     monitored[261] = 0.5 * monitored[260]
     monitored[262] = (
-        -monitored[179]
-        * monitored[261]
-        / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
+        -monitored[179] * monitored[261] / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
     )
     monitored[263] = np.where(celltype == 2, 1.7 * monitored[262], monitored[262])
     monitored[264] = monitored[260] / (1 + 0.0123 / cajsr)
     monitored[265] = np.where(monitored[264] < 0.001, 0.001, monitored[264])
     monitored[309] = (-Jrel_p + monitored[263]) / monitored[265]
     monitored[266] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[267] = Jrel_b * ((1 - monitored[266]) * Jrel_np + Jrel_p * monitored[266])
 
     # Expressions for the Membrane component
     monitored[268] = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     monitored[310] = (
         -monitored[102]
@@ -2819,37 +2654,33 @@
         -monitored[126]
         - monitored[134]
         - monitored[191]
         - monitored[27]
         - 3 * monitored[125]
         - 3 * monitored[66]
     ) * monitored[2] / (F * monitored[3])
-    monitored[312] = -monitored[136] + (
-        -monitored[180] - 3 * monitored[102]
-    ) * monitored[2] / (F * monitored[6])
+    monitored[312] = -monitored[136] + (-monitored[180] - 3 * monitored[102]) * monitored[2] / (
+        F * monitored[6]
+    )
     monitored[313] = monitored[137] * monitored[6] / monitored[3] + (
         -monitored[192]
         - monitored[204]
         - monitored[224]
         - monitored[234]
         - monitored[241]
         - monitored[246]
         - monitored[249]
         - monitored[268]
         + 2 * monitored[125]
     ) * monitored[2] / (F * monitored[3])
-    monitored[314] = -monitored[137] - monitored[181] * monitored[2] / (
-        F * monitored[6]
-    )
+    monitored[314] = -monitored[137] - monitored[181] * monitored[2] / (F * monitored[6])
     monitored[315] = monitored[139] * monitored[6] / monitored[3] + (
         monitored[251] + monitored[253]
     ) * monitored[2] / (F * monitored[3])
-    monitored[316] = -monitored[139] + monitored[250] * monitored[2] / (
-        F * monitored[6]
-    )
+    monitored[316] = -monitored[139] + monitored[250] * monitored[2] / (F * monitored[6])
     monitored[270] = 1.0 / (
         1
         + kmcmdn * monitored[269] / ((kmcmdn + cai) * (kmcmdn + cai))
         + kmtrpn * trpnmax / ((kmtrpn + cai) * (kmtrpn + cai))
     )
     monitored[317] = (
         monitored[138] * monitored[6] / monitored[3]
@@ -2865,17 +2696,15 @@
     )
     monitored[318] = (
         -monitored[138]
         + monitored[267] * monitored[5] / monitored[6]
         + (-monitored[179] + 2 * monitored[102]) * monitored[2] / (2 * F * monitored[6])
     ) * monitored[271]
     monitored[319] = -monitored[275] * monitored[5] / monitored[4] + monitored[201]
-    monitored[272] = 1.0 / (
-        1 + csqnmax * kmcsqn / ((kmcsqn + cajsr) * (kmcsqn + cajsr))
-    )
+    monitored[272] = 1.0 / (1 + csqnmax * kmcsqn / ((kmcsqn + cajsr) * (kmcsqn + cajsr)))
     monitored[320] = (-monitored[267] + monitored[275]) * monitored[272]
 
     # Return results
     return monitored
 
 
 def forward_explicit_euler(states, t, dt, parameters):
@@ -3107,17 +2936,15 @@
     E1_i = x1_i / (x1_i + x2_i + x3_i + x4_i)
     E2_i = x2_i / (x1_i + x2_i + x3_i + x4_i)
     E3_i = x3_i / (x1_i + x2_i + x3_i + x4_i)
     E4_i = x4_i / (x1_i + x2_i + x3_i + x4_i)
     allo_i = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     JncxNa_i = E3_i * k4pp_i - E2_i * k3pp_i - 3 * E1_i * k8_i + 3 * E4_i * k7_i
     JncxCa_i = E2_i * k2_i - E1_i * k1_i
-    Gncx = np.where(
-        celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b)
-    )
+    Gncx = np.where(celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b))
     INaCa_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx * allo_i
     h1_ss = 1 + (1 + hna) * nass / kna3
     h2_ss = hna * nass / (kna3 * h1_ss)
     h3_ss = 1.0 / h1_ss
     h4_ss = 1 + (1 + nass / kna2) * nass / kna1
     h5_ss = (nass * nass) / (kna1 * kna2 * h4_ss)
     h6_ss = 1.0 / h4_ss
@@ -3144,17 +2971,15 @@
     x3_ss = (k2_ss + k3_ss) * k6_ss * k8_ss + (k6_ss + k7_ss) * k1_ss * k3_ss
     x4_ss = (k1_ss + k8_ss) * k3_ss * k5_ss + (k4_ss + k5_ss) * k2_ss * k8_ss
     E1_ss = x1_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E2_ss = x2_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E3_ss = x3_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E4_ss = x4_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     allo_ss = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
-    JncxNa_ss = (
-        E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
-    )
+    JncxNa_ss = E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
     JncxCa_ss = E2_ss * k2_ss - E1_ss * k1_ss
     INaCa_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx * allo_ss
 
     # Expressions for the K component
     Knai = Knai0 * np.exp(delta * vfrt / 3)
     Knao = Knao0 * np.exp((1 - delta) * vfrt / 3)
     P = eP / (1 + H / Khp + nai / Knap + ki / Kxkur)
@@ -3216,17 +3041,15 @@
     x4 = a1 * a3 * a4 + a1 * a4 * b2 + a1 * b2 * b3 + b2 * b3 * b4
     E1 = x1 / (x1 + x2 + x3 + x4)
     E2 = x2 / (x1 + x2 + x3 + x4)
     E3 = x3 / (x1 + x2 + x3 + x4)
     E4 = x4 / (x1 + x2 + x3 + x4)
     JnakNa = -3 * E2 * b3 + 3 * E1 * a3
     JnakK = -2 * E3 * a1 + 2 * E4 * b1
-    Pnak = np.where(
-        celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
-    )
+    Pnak = np.where(celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b))
     INaK = (zk * JnakK + zna * JnakNa) * Pnak
 
     # Expressions for the b component
     INab = PNab * (-nao + np.exp(vfrt) * nai) * vffrt / (-1 + np.exp(vfrt))
 
     # Expressions for the IpCa component
     IpCa = GpCa * cai / (KmCap + cai)
@@ -3251,17 +3074,15 @@
             + 0.7408182206817179 * np.exp(-0.05 * vShift - 0.05 * v)
         )
     )
     dd_dt = (-d + dss) / td
     states[1] = dt * dd_dt + d
     fss = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
     tff = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
-    tfs = 1000 + 1.0 / (
-        3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
-    )
+    tfs = 1000 + 1.0 / (3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6))
     Afs = 1 - Aff
     dff_dt = (-ff + fss) / tff
     states[2] = dt * dff_dt + ff
     dfs_dt = (-fs + fss) / tfs
     states[3] = dt * dfs_dt + fs
     f = Aff * ff + Afs * fs
     fcass = fss
@@ -3300,25 +3121,17 @@
     gamma_ko = np.exp(-(-0.3 * Io + np.sqrt(Io) / (1 + np.sqrt(Io))) * constA)
     PhiCaL_ss = (
         4
         * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_ss = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_ss = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
-    )
-    PCa = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    PhiCaNa_ss = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_ss = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
+    PCa = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     PCap = 1.1 * PCa
     PCaNa = 0.00125 * PCa
     PCaK = 0.0003574 * PCa
     PCaNap = 0.00125 * PCap
     PCaKp = 0.0003574 * PCap
     fICaLp = 1.0 / (1 + KmCaMK / CaMKa)
     ICaL_ss = ICaL_fractionSS * (
@@ -3342,22 +3155,16 @@
     gamma_ki = np.exp(-(-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     PhiCaL_i = (
         4
         * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_i = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_i = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
-    )
+    PhiCaNa_i = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_i = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
     ICaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * PhiCaL_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * PhiCaL_i * d * fICaLp
     )
     ICaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * PhiCaNa_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * PhiCaNa_i * d * fICaLp
@@ -3401,17 +3208,15 @@
     )
     dm_dt = (-m + mss) / tm
     states[11] = dt * dm_dt + m
     hss = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    ah = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    ah = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     bh = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     th = 1.0 / (ah + bh)
     dh_dt = (-h + hss) / th
@@ -3422,17 +3227,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     bj = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     jss = hss
     tj = 1.0 / (aj + bj)
     dj_dt = (-j + jss) / tj
     states[13] = dt * dj_dt + j
     hssp = 1.0 / (
         (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
@@ -3470,78 +3273,58 @@
     states[18] = dt * dhLp_dt + hLp
     GNaL = np.where(celltype == 1, 0.6 * GNaL_b, GNaL_b)
     fINaLp = 1.0 / (1 + KmCaMK / CaMKa)
     INaL = (-ENa + v) * ((1 - fINaLp) * hL + fINaLp * hLp) * GNaL * mL
 
     # Expressions for the Ito component
     ass = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     ta = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     da_dt = (-a + ass) / ta
     states[19] = dt * da_dt + a
     iss = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    delta_epi = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    delta_epi = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     tiF_b = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     tiS_b = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     tiF = delta_epi * tiF_b
     tiS = delta_epi * tiS_b
     AiF = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     AiS = 1 - AiF
     diF_dt = (-iF + iss) / tiF
     states[20] = dt * diF_dt + iF
     diS_dt = (-iS + iss) / tiS
     states[21] = dt * diS_dt + iS
     i = AiF * iF + AiS * iS
     assp = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     dap_dt = (-ap + assp) / ta
     states[22] = dt * dap_dt + ap
     dti_develop = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
     dti_recover = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     tiFp = dti_develop * dti_recover * tiF
     tiSp = dti_develop * dti_recover * tiS
     diFp_dt = (-iFp + iss) / tiFp
     states[23] = dt * diFp_dt + iFp
     diSp_dt = (-iSp + iss) / tiSp
@@ -3560,58 +3343,47 @@
     beta_i = 0.06525 * np.exp(-0.8209 * vfrt)
     alpha_C2ToI = 5.2e-05 * np.exp(1.525 * vfrt)
     beta_ItoC2 = alpha_C2ToI * beta_2 * beta_i / (alpha_2 * alpha_i)
     dC3_dt = C2 * beta - C3 * alpha
     states[25] = dt * dC3_dt + C3
     dC2_dt = beta_1 * C1 + C3 * alpha - (alpha_1 + beta) * C2
     states[26] = dt * dC2_dt + C2
-    dC1_dt = (
-        alpha_1 * C2
-        + I * beta_ItoC2
-        + O * beta_2
-        - (beta_1 + alpha_2 + alpha_C2ToI) * C1
-    )
+    dC1_dt = alpha_1 * C2 + I * beta_ItoC2 + O * beta_2 - (beta_1 + alpha_2 + alpha_C2ToI) * C1
     states[27] = dt * dC1_dt + C1
     dO_dt = C1 * alpha_2 + I * beta_i - (alpha_i + beta_2) * O
     states[28] = dt * dO_dt + O
     dI_dt = C1 * alpha_C2ToI + O * alpha_i - (beta_ItoC2 + beta_i) * I
     states[29] = dt * dI_dt + I
-    GKr = np.where(
-        celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
-    )
+    GKr = np.where(celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b))
     IKr = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GKr * O / 5
 
     # Expressions for the IKs component
     xs1ss = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     txs1 = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
     dxs1_dt = (-xs1 + xs1ss) / txs1
     states[30] = dt * dxs1_dt + xs1
     xs2ss = xs1ss
-    txs2 = 1.0 / (
-        0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20)
-    )
+    txs2 = 1.0 / (0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20))
     dxs2_dt = (-xs2 + xs2ss) / txs2
     states[31] = dt * dxs2_dt + xs2
     KsCa = 1 + 0.6 / (1 + 6.481821026062645e-07 * np.power(1.0 / cai, 1.4))
     GKs = np.where(celltype == 1, 1.4 * GKs_b, GKs_b)
     IKs = (-EKs + v) * GKs * KsCa * xs1 * xs2
 
     # Expressions for the IK1 component
     aK1 = 4.094 / (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
     bK1 = (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     K1ss = aK1 / (aK1 + bK1)
-    GK1 = np.where(
-        celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
-    )
+    GK1 = np.where(celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b))
     IK1 = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 * K1ss / 5
 
     # Expressions for the IKb component
     xkb = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     GKb = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     IKb = (-EK + v) * GKb * xkb
 
@@ -3649,17 +3421,15 @@
     fJrelp = 1.0 / (1 + KmCaMK / CaMKa)
     Jrel = Jrel_b * ((1 - fJrelp) * Jrel_np + Jrel_p * fJrelp)
 
     # Expressions for the Membrane component
     Istim = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     dv_dt = (
         -ICaK
@@ -3917,17 +3687,15 @@
 
     # Expressions for the CaMK component
     CaMKb = CaMKo * (1 - CaMKt) / (1 + KmCaM / cass)
     CaMKa = CaMKb + CaMKt
     dCaMKt_dt = -bCaMK * CaMKt + aCaMK * (CaMKb + CaMKt) * CaMKb
     dCaMKb_dCaMKt = -CaMKo / (1 + KmCaM / cass)
     dCaMKt_dt_linearized = (
-        -bCaMK
-        + aCaMK * (1 + dCaMKb_dCaMKt) * CaMKb
-        + aCaMK * (CaMKb + CaMKt) * dCaMKb_dCaMKt
+        -bCaMK + aCaMK * (1 + dCaMKb_dCaMKt) * CaMKb + aCaMK * (CaMKb + CaMKt) * dCaMKb_dCaMKt
     )
     states[0] = CaMKt + np.where(
         np.abs(dCaMKt_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCaMKt_dt_linearized)) * dCaMKt_dt / dCaMKt_dt_linearized,
         dt * dCaMKt_dt,
     )
 
@@ -3972,17 +3740,15 @@
     E1_i = x1_i / (x1_i + x2_i + x3_i + x4_i)
     E2_i = x2_i / (x1_i + x2_i + x3_i + x4_i)
     E3_i = x3_i / (x1_i + x2_i + x3_i + x4_i)
     E4_i = x4_i / (x1_i + x2_i + x3_i + x4_i)
     allo_i = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     JncxNa_i = E3_i * k4pp_i - E2_i * k3pp_i - 3 * E1_i * k8_i + 3 * E4_i * k7_i
     JncxCa_i = E2_i * k2_i - E1_i * k1_i
-    Gncx = np.where(
-        celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b)
-    )
+    Gncx = np.where(celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b))
     INaCa_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx * allo_i
     h1_ss = 1 + (1 + hna) * nass / kna3
     h2_ss = hna * nass / (kna3 * h1_ss)
     h3_ss = 1.0 / h1_ss
     h4_ss = 1 + (1 + nass / kna2) * nass / kna1
     h5_ss = (nass * nass) / (kna1 * kna2 * h4_ss)
     h6_ss = 1.0 / h4_ss
@@ -4009,17 +3775,15 @@
     x3_ss = (k2_ss + k3_ss) * k6_ss * k8_ss + (k6_ss + k7_ss) * k1_ss * k3_ss
     x4_ss = (k1_ss + k8_ss) * k3_ss * k5_ss + (k4_ss + k5_ss) * k2_ss * k8_ss
     E1_ss = x1_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E2_ss = x2_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E3_ss = x3_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E4_ss = x4_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     allo_ss = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
-    JncxNa_ss = (
-        E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
-    )
+    JncxNa_ss = E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
     JncxCa_ss = E2_ss * k2_ss - E1_ss * k1_ss
     INaCa_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx * allo_ss
 
     # Expressions for the K component
     Knai = Knai0 * np.exp(delta * vfrt / 3)
     Knao = Knao0 * np.exp((1 - delta) * vfrt / 3)
     P = eP / (1 + H / Khp + nai / Knap + ki / Kxkur)
@@ -4081,17 +3845,15 @@
     x4 = a1 * a3 * a4 + a1 * a4 * b2 + a1 * b2 * b3 + b2 * b3 * b4
     E1 = x1 / (x1 + x2 + x3 + x4)
     E2 = x2 / (x1 + x2 + x3 + x4)
     E3 = x3 / (x1 + x2 + x3 + x4)
     E4 = x4 / (x1 + x2 + x3 + x4)
     JnakNa = -3 * E2 * b3 + 3 * E1 * a3
     JnakK = -2 * E3 * a1 + 2 * E4 * b1
-    Pnak = np.where(
-        celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
-    )
+    Pnak = np.where(celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b))
     INaK = (zk * JnakK + zna * JnakNa) * Pnak
 
     # Expressions for the b component
     INab = PNab * (-nao + np.exp(vfrt) * nai) * vffrt / (-1 + np.exp(vfrt))
 
     # Expressions for the IpCa component
     IpCa = GpCa * cai / (KmCap + cai)
@@ -4117,17 +3879,15 @@
         )
     )
     dd_dt = (-d + dss) / td
     dd_dt_linearized = -1 / td
     states[1] = (-1 + np.exp(dt * dd_dt_linearized)) * dd_dt / dd_dt_linearized + d
     fss = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
     tff = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
-    tfs = 1000 + 1.0 / (
-        3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
-    )
+    tfs = 1000 + 1.0 / (3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6))
     Afs = 1 - Aff
     dff_dt = (-ff + fss) / tff
     dff_dt_linearized = -1 / tff
     states[2] = (-1 + np.exp(dt * dff_dt_linearized)) * dff_dt / dff_dt_linearized + ff
     dfs_dt = (-fs + fss) / tfs
     dfs_dt_linearized = -1 / tfs
     states[3] = (-1 + np.exp(dt * dfs_dt_linearized)) * dfs_dt / dfs_dt_linearized + fs
@@ -4135,53 +3895,41 @@
     fcass = fss
     tfcaf = 7 + 1.0 / (0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7))
     tfcas = 100 + 1.0 / (0.00012 * np.exp(-v / 3) + 0.00012 * np.exp(v / 7))
     Afcaf = 0.3 + 0.6 / (1 + np.exp(-1 + v / 10))
     Afcas = 1 - Afcaf
     dfcaf_dt = (-fcaf + fcass) / tfcaf
     dfcaf_dt_linearized = -1 / tfcaf
-    states[4] = (
-        -1 + np.exp(dt * dfcaf_dt_linearized)
-    ) * dfcaf_dt / dfcaf_dt_linearized + fcaf
+    states[4] = (-1 + np.exp(dt * dfcaf_dt_linearized)) * dfcaf_dt / dfcaf_dt_linearized + fcaf
     dfcas_dt = (-fcas + fcass) / tfcas
     dfcas_dt_linearized = -1 / tfcas
-    states[5] = (
-        -1 + np.exp(dt * dfcas_dt_linearized)
-    ) * dfcas_dt / dfcas_dt_linearized + fcas
+    states[5] = (-1 + np.exp(dt * dfcas_dt_linearized)) * dfcas_dt / dfcas_dt_linearized + fcas
     fca = Afcaf * fcaf + Afcas * fcas
     jcass = 1.0 / (1.0 + 649.7401897235336 * np.exp(0.35821750967187277 * v))
     djca_dt = (-jca + jcass) / tjca
     djca_dt_linearized = -1 / tjca
-    states[6] = (
-        -1 + np.exp(dt * djca_dt_linearized)
-    ) * djca_dt / djca_dt_linearized + jca
+    states[6] = (-1 + np.exp(dt * djca_dt_linearized)) * djca_dt / djca_dt_linearized + jca
     tffp = 2.5 * tff
     dffp_dt = (-ffp + fss) / tffp
     dffp_dt_linearized = -1 / tffp
-    states[7] = (
-        -1 + np.exp(dt * dffp_dt_linearized)
-    ) * dffp_dt / dffp_dt_linearized + ffp
+    states[7] = (-1 + np.exp(dt * dffp_dt_linearized)) * dffp_dt / dffp_dt_linearized + ffp
     fp = Aff * ffp + Afs * fs
     tfcafp = 2.5 * tfcaf
     dfcafp_dt = (-fcafp + fcass) / tfcafp
     dfcafp_dt_linearized = -1 / tfcafp
-    states[8] = (
-        -1 + np.exp(dt * dfcafp_dt_linearized)
-    ) * dfcafp_dt / dfcafp_dt_linearized + fcafp
+    states[8] = (-1 + np.exp(dt * dfcafp_dt_linearized)) * dfcafp_dt / dfcafp_dt_linearized + fcafp
     fcap = Afcaf * fcafp + Afcas * fcas
     km2n = jca
     anca_ss = 1.0 / (np.power(1 + Kmn / cass, 4) + k2n / km2n)
     dnca_ss_dt = k2n * anca_ss - km2n * nca_ss
     dnca_ss_dt_linearized = -km2n
     states[9] = (
         np.where(
             np.abs(dnca_ss_dt_linearized) > 1e-08,
-            (-1 + np.exp(dt * dnca_ss_dt_linearized))
-            * dnca_ss_dt
-            / dnca_ss_dt_linearized,
+            (-1 + np.exp(dt * dnca_ss_dt_linearized)) * dnca_ss_dt / dnca_ss_dt_linearized,
             dt * dnca_ss_dt,
         )
         + nca_ss
     )
     Io = 0.0005 * clo + 0.0005 * ko + 0.0005 * nao + 0.002 * cao
     Iss = 0.0005 * clss + 0.0005 * kss + 0.0005 * nass + 0.002 * cass
     constA = 1820000.0 * np.power(T * dielConstant, -1.5)
@@ -4193,25 +3941,17 @@
     gamma_ko = np.exp(-(-0.3 * Io + np.sqrt(Io) / (1 + np.sqrt(Io))) * constA)
     PhiCaL_ss = (
         4
         * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_ss = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_ss = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
-    )
-    PCa = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    PhiCaNa_ss = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_ss = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
+    PCa = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     PCap = 1.1 * PCa
     PCaNa = 0.00125 * PCa
     PCaK = 0.0003574 * PCa
     PCaNap = 0.00125 * PCap
     PCaKp = 0.0003574 * PCap
     fICaLp = 1.0 / (1 + KmCaMK / CaMKa)
     ICaL_ss = ICaL_fractionSS * (
@@ -4243,22 +3983,16 @@
     gamma_ki = np.exp(-(-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     PhiCaL_i = (
         4
         * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_i = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_i = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
-    )
+    PhiCaNa_i = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_i = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
     ICaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * PhiCaL_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * PhiCaL_i * d * fICaLp
     )
     ICaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * PhiCaNa_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * PhiCaNa_i * d * fICaLp
@@ -4303,17 +4037,15 @@
     dm_dt = (-m + mss) / tm
     dm_dt_linearized = -1 / tm
     states[11] = (-1 + np.exp(dt * dm_dt_linearized)) * dm_dt / dm_dt_linearized + m
     hss = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    ah = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    ah = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     bh = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     th = 1.0 / (ah + bh)
     dh_dt = (-h + hss) / th
@@ -4325,17 +4057,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     bj = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     jss = hss
     tj = 1.0 / (aj + bj)
     dj_dt = (-j + jss) / tj
     dj_dt_linearized = -1 / tj
     states[13] = (-1 + np.exp(dt * dj_dt_linearized)) * dj_dt / dj_dt_linearized + j
     hssp = 1.0 / (
@@ -4372,105 +4102,79 @@
     dhL_dt = (-hL + hLss) / thL
     dhL_dt_linearized = -1 / thL
     states[17] = (-1 + np.exp(dt * dhL_dt_linearized)) * dhL_dt / dhL_dt_linearized + hL
     hLssp = 1.0 / (1 + 275969.2903869871 * np.exp(0.13354700854700854 * v))
     thLp = 3 * thL
     dhLp_dt = (-hLp + hLssp) / thLp
     dhLp_dt_linearized = -1 / thLp
-    states[18] = (
-        -1 + np.exp(dt * dhLp_dt_linearized)
-    ) * dhLp_dt / dhLp_dt_linearized + hLp
+    states[18] = (-1 + np.exp(dt * dhLp_dt_linearized)) * dhLp_dt / dhLp_dt_linearized + hLp
     GNaL = np.where(celltype == 1, 0.6 * GNaL_b, GNaL_b)
     fINaLp = 1.0 / (1 + KmCaMK / CaMKa)
     INaL = (-ENa + v) * ((1 - fINaLp) * hL + fINaLp * hLp) * GNaL * mL
 
     # Expressions for the Ito component
     ass = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     ta = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     da_dt = (-a + ass) / ta
     da_dt_linearized = -1 / ta
     states[19] = (-1 + np.exp(dt * da_dt_linearized)) * da_dt / da_dt_linearized + a
     iss = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    delta_epi = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    delta_epi = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     tiF_b = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     tiS_b = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     tiF = delta_epi * tiF_b
     tiS = delta_epi * tiS_b
     AiF = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     AiS = 1 - AiF
     diF_dt = (-iF + iss) / tiF
     diF_dt_linearized = -1 / tiF
     states[20] = (-1 + np.exp(dt * diF_dt_linearized)) * diF_dt / diF_dt_linearized + iF
     diS_dt = (-iS + iss) / tiS
     diS_dt_linearized = -1 / tiS
     states[21] = (-1 + np.exp(dt * diS_dt_linearized)) * diS_dt / diS_dt_linearized + iS
     i = AiF * iF + AiS * iS
     assp = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     dap_dt = (-ap + assp) / ta
     dap_dt_linearized = -1 / ta
     states[22] = (-1 + np.exp(dt * dap_dt_linearized)) * dap_dt / dap_dt_linearized + ap
     dti_develop = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
     dti_recover = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     tiFp = dti_develop * dti_recover * tiF
     tiSp = dti_develop * dti_recover * tiS
     diFp_dt = (-iFp + iss) / tiFp
     diFp_dt_linearized = -1 / tiFp
-    states[23] = (
-        -1 + np.exp(dt * diFp_dt_linearized)
-    ) * diFp_dt / diFp_dt_linearized + iFp
+    states[23] = (-1 + np.exp(dt * diFp_dt_linearized)) * diFp_dt / diFp_dt_linearized + iFp
     diSp_dt = (-iSp + iss) / tiSp
     diSp_dt_linearized = -1 / tiSp
-    states[24] = (
-        -1 + np.exp(dt * diSp_dt_linearized)
-    ) * diSp_dt / diSp_dt_linearized + iSp
+    states[24] = (-1 + np.exp(dt * diSp_dt_linearized)) * diSp_dt / diSp_dt_linearized + iSp
     ip = AiF * iFp + AiS * iSp
     Gto = np.where(celltype == 1, 2 * Gto_b, np.where(celltype == 2, 2 * Gto_b, Gto_b))
     fItop = 1.0 / (1 + KmCaMK / CaMKa)
     Ito = (-EK + v) * ((1 - fItop) * a * i + ap * fItop * ip) * Gto
 
     # Expressions for the IKr component
     alpha = 0.1161 * np.exp(0.299 * vfrt)
@@ -4491,20 +4195,15 @@
     dC2_dt = beta_1 * C1 + C3 * alpha - (alpha_1 + beta) * C2
     dC2_dt_linearized = -alpha_1 - beta
     states[26] = C2 + np.where(
         np.abs(dC2_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dC2_dt_linearized)) * dC2_dt / dC2_dt_linearized,
         dt * dC2_dt,
     )
-    dC1_dt = (
-        alpha_1 * C2
-        + I * beta_ItoC2
-        + O * beta_2
-        - (beta_1 + alpha_2 + alpha_C2ToI) * C1
-    )
+    dC1_dt = alpha_1 * C2 + I * beta_ItoC2 + O * beta_2 - (beta_1 + alpha_2 + alpha_C2ToI) * C1
     dC1_dt_linearized = -beta_1 - alpha_2 - alpha_C2ToI
     states[27] = C1 + np.where(
         np.abs(dC1_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dC1_dt_linearized)) * dC1_dt / dC1_dt_linearized,
         dt * dC1_dt,
     )
     dO_dt = C1 * alpha_2 + I * beta_i - (alpha_i + beta_2) * O
@@ -4517,53 +4216,43 @@
     dI_dt = C1 * alpha_C2ToI + O * alpha_i - (beta_ItoC2 + beta_i) * I
     dI_dt_linearized = -beta_ItoC2 - beta_i
     states[29] = I + np.where(
         np.abs(dI_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dI_dt_linearized)) * dI_dt / dI_dt_linearized,
         dt * dI_dt,
     )
-    GKr = np.where(
-        celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
-    )
+    GKr = np.where(celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b))
     IKr = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GKr * O / 5
 
     # Expressions for the IKs component
     xs1ss = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     txs1 = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
     dxs1_dt = (-xs1 + xs1ss) / txs1
     dxs1_dt_linearized = -1 / txs1
-    states[30] = (
-        -1 + np.exp(dt * dxs1_dt_linearized)
-    ) * dxs1_dt / dxs1_dt_linearized + xs1
+    states[30] = (-1 + np.exp(dt * dxs1_dt_linearized)) * dxs1_dt / dxs1_dt_linearized + xs1
     xs2ss = xs1ss
-    txs2 = 1.0 / (
-        0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20)
-    )
+    txs2 = 1.0 / (0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20))
     dxs2_dt = (-xs2 + xs2ss) / txs2
     dxs2_dt_linearized = -1 / txs2
-    states[31] = (
-        -1 + np.exp(dt * dxs2_dt_linearized)
-    ) * dxs2_dt / dxs2_dt_linearized + xs2
+    states[31] = (-1 + np.exp(dt * dxs2_dt_linearized)) * dxs2_dt / dxs2_dt_linearized + xs2
     KsCa = 1 + 0.6 / (1 + 6.481821026062645e-07 * np.power(1.0 / cai, 1.4))
     GKs = np.where(celltype == 1, 1.4 * GKs_b, GKs_b)
     IKs = (-EKs + v) * GKs * KsCa * xs1 * xs2
 
     # Expressions for the IK1 component
     aK1 = 4.094 / (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
     bK1 = (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     K1ss = aK1 / (aK1 + bK1)
-    GK1 = np.where(
-        celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
-    )
+    GK1 = np.where(celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b))
     IK1 = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 * K1ss / 5
 
     # Expressions for the IKb component
     xkb = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     GKb = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     IKb = (-EK + v) * GKb * xkb
 
@@ -4607,17 +4296,15 @@
     fJrelp = 1.0 / (1 + KmCaMK / CaMKa)
     Jrel = Jrel_b * ((1 - fJrelp) * Jrel_np + Jrel_p * fJrelp)
 
     # Expressions for the Membrane component
     Istim = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     dv_dt = (
         -ICaK
@@ -4638,17 +4325,15 @@
         - INab
         - I_katp
         - IpCa
         - Istim
         - Ito
     )
     dAfcaf_dv = (
-        -0.06
-        * np.exp(-1 + v / 10)
-        / ((1 + np.exp(-1 + v / 10)) * (1 + np.exp(-1 + v / 10)))
+        -0.06 * np.exp(-1 + v / 10) / ((1 + np.exp(-1 + v / 10)) * (1 + np.exp(-1 + v / 10)))
     )
     dAiF_dv = (
         -0.0016103529885927823
         * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
         / (
             (
                 1
@@ -4658,171 +4343,122 @@
             * (
                 1
                 + 0.24348537187522867
                 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
             )
         )
     )
-    dE1_dx1 = 1.0 / (x1 + x2 + x3 + x4) - x1 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE1_dx1 = 1.0 / (x1 + x2 + x3 + x4) - x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_dx2 = -x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_dx3 = -x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_dx4 = -x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_i_dx1_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x1_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
     dE1_i_dx2_i = -x1_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE1_i_dx3_i = -x1_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE1_i_dx4_i = -x1_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE1_ss_dx1_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x1_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
-    dE1_ss_dx2_ss = -x1_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE1_ss_dx3_ss = -x1_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE1_ss_dx4_ss = -x1_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE1_ss_dx2_ss = -x1_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE1_ss_dx3_ss = -x1_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE1_ss_dx4_ss = -x1_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE2_dx1 = -x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
-    dE2_dx2 = 1.0 / (x1 + x2 + x3 + x4) - x2 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE2_dx2 = 1.0 / (x1 + x2 + x3 + x4) - x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE2_dx3 = -x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE2_dx4 = -x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE2_i_dx1_i = -x2_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE2_i_dx2_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x2_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
     dE2_i_dx3_i = -x2_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE2_i_dx4_i = -x2_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
-    dE2_ss_dx1_ss = -x2_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE2_ss_dx1_ss = -x2_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE2_ss_dx2_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x2_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
-    dE2_ss_dx3_ss = -x2_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE2_ss_dx4_ss = -x2_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE2_ss_dx3_ss = -x2_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE2_ss_dx4_ss = -x2_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE3_dx1 = -x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE3_dx2 = -x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
-    dE3_dx3 = 1.0 / (x1 + x2 + x3 + x4) - x3 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE3_dx3 = 1.0 / (x1 + x2 + x3 + x4) - x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE3_dx4 = -x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE3_i_dx1_i = -x3_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE3_i_dx2_i = -x3_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE3_i_dx3_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x3_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
     dE3_i_dx4_i = -x3_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
-    dE3_ss_dx1_ss = -x3_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE3_ss_dx2_ss = -x3_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE3_ss_dx1_ss = -x3_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE3_ss_dx2_ss = -x3_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE3_ss_dx3_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x3_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
-    dE3_ss_dx4_ss = -x3_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE3_ss_dx4_ss = -x3_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE4_dx1 = -x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE4_dx2 = -x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE4_dx3 = -x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
-    dE4_dx4 = 1.0 / (x1 + x2 + x3 + x4) - x4 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE4_dx4 = 1.0 / (x1 + x2 + x3 + x4) - x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE4_i_dx1_i = -x4_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE4_i_dx2_i = -x4_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE4_i_dx3_i = -x4_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE4_i_dx4_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x4_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
-    dE4_ss_dx1_ss = -x4_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE4_ss_dx2_ss = -x4_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE4_ss_dx3_ss = -x4_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE4_ss_dx1_ss = -x4_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE4_ss_dx2_ss = -x4_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE4_ss_dx3_ss = -x4_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE4_ss_dx4_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x4_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
     dICaK_i_dPhiCaK_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaK * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaKp * d * fICaLp
     )
-    dICaK_i_dfca = (
-        (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaK * PhiCaK_i * d * jca * nca_i
-    )
+    dICaK_i_dfca = (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaK * PhiCaK_i * d * jca * nca_i
     dICaK_i_dfcap = (1 - ICaL_fractionSS) * PCaKp * PhiCaK_i * d * fICaLp * jca * nca_i
     dICaK_ss_dPhiCaK_ss = ICaL_fractionSS * (
         (1 - fICaLp) * ((1 - nca_ss) * f + fca * jca * nca_ss) * PCaK * d
         + ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCaKp * d * fICaLp
     )
     dICaK_ss_dfca = ICaL_fractionSS * (1 - fICaLp) * PCaK * PhiCaK_ss * d * jca * nca_ss
     dICaK_ss_dfcap = ICaL_fractionSS * PCaKp * PhiCaK_ss * d * fICaLp * jca * nca_ss
     dICaL_i_dPhiCaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * d * fICaLp
     )
-    dICaL_i_dfca = (
-        (1 - ICaL_fractionSS) * (1 - fICaLp) * PCa * PhiCaL_i * d * jca * nca_i
-    )
+    dICaL_i_dfca = (1 - ICaL_fractionSS) * (1 - fICaLp) * PCa * PhiCaL_i * d * jca * nca_i
     dICaL_i_dfcap = (1 - ICaL_fractionSS) * PCap * PhiCaL_i * d * fICaLp * jca * nca_i
     dICaL_ss_dPhiCaL_ss = ICaL_fractionSS * (
         (1 - fICaLp) * ((1 - nca_ss) * f + fca * jca * nca_ss) * PCa * d
         + ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCap * d * fICaLp
     )
     dICaL_ss_dfca = ICaL_fractionSS * (1 - fICaLp) * PCa * PhiCaL_ss * d * jca * nca_ss
     dICaL_ss_dfcap = ICaL_fractionSS * PCap * PhiCaL_ss * d * fICaLp * jca * nca_ss
     dICaNa_i_dPhiCaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * d * fICaLp
     )
-    dICaNa_i_dfca = (
-        (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaNa * PhiCaNa_i * d * jca * nca_i
-    )
-    dICaNa_i_dfcap = (
-        (1 - ICaL_fractionSS) * PCaNap * PhiCaNa_i * d * fICaLp * jca * nca_i
-    )
+    dICaNa_i_dfca = (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaNa * PhiCaNa_i * d * jca * nca_i
+    dICaNa_i_dfcap = (1 - ICaL_fractionSS) * PCaNap * PhiCaNa_i * d * fICaLp * jca * nca_i
     dICaNa_ss_dPhiCaNa_ss = ICaL_fractionSS * (
         (1 - fICaLp) * ((1 - nca_ss) * f + fca * jca * nca_ss) * PCaNa * d
         + ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCaNap * d * fICaLp
     )
-    dICaNa_ss_dfca = (
-        ICaL_fractionSS * (1 - fICaLp) * PCaNa * PhiCaNa_ss * d * jca * nca_ss
-    )
+    dICaNa_ss_dfca = ICaL_fractionSS * (1 - fICaLp) * PCaNa * PhiCaNa_ss * d * jca * nca_ss
     dICaNa_ss_dfcap = ICaL_fractionSS * PCaNap * PhiCaNa_ss * d * fICaLp * jca * nca_ss
     dICab_dvffrt = (
-        4
-        * PCab
-        * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
-        / (-1 + np.exp(2 * vfrt))
+        4 * PCab * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) / (-1 + np.exp(2 * vfrt))
     )
-    dICab_dvfrt = -8 * PCab * (
-        -cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai
-    ) * np.exp(2 * vfrt) * vffrt / (
-        (-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))
-    ) + 8 * PCab * cai * np.exp(
+    dICab_dvfrt = -8 * PCab * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) * np.exp(
         2 * vfrt
-    ) * gamma_cai * vffrt / (
-        -1 + np.exp(2 * vfrt)
-    )
+    ) * vffrt / ((-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))) + 8 * PCab * cai * np.exp(
+        2 * vfrt
+    ) * gamma_cai * vffrt / (-1 + np.exp(2 * vfrt))
     dIClCa_junc_dv = Fjunc * GClCa / (1 + KdClCa / cass)
     dIClCa_sl_dv = GClCa * (1 - Fjunc) / (1 + KdClCa / cai)
     dIK1_dK1ss = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 / 5
     dK1ss_daK1 = 1.0 / (aK1 + bK1) - aK1 / ((aK1 + bK1) * (aK1 + bK1))
     dK1ss_dbK1 = -aK1 / ((aK1 + bK1) * (aK1 + bK1))
     daK1_dv = (
         -0.0011435228161993972
@@ -4831,22 +4467,18 @@
             (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
             * (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
         )
     )
     dbK1_dv = (
         6.919349479611957e-18 * np.exp(0.0618 * v - 0.0618 * EK)
         + 0.8506978434250505 * np.exp(0.0674 * v - 0.0674 * EK)
-    ) / (
-        1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)
-    ) + 0.016099950792318272 * (
+    ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)) + 0.016099950792318272 * (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
-    ) * np.exp(
-        0.1629 * EK - 0.1629 * v
-    ) / (
+    ) * np.exp(0.1629 * EK - 0.1629 * v) / (
         (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
         * (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     )
     dIK1_dv = (
         np.sqrt(5) * np.sqrt(ko) * GK1 * K1ss / 5
         + np.sqrt(5)
         * np.sqrt(ko)
@@ -4900,132 +4532,67 @@
         - 3 * (dE2_dx2 * dx2_da3 + dE2_dx3 * dx3_da3 + a1 * a4 * dE2_dx4) * b3
         + 3 * (dE1_dx2 * dx2_da3 + dE1_dx3 * dx3_da3 + a1 * a4 * dE1_dx4) * a3
     )
     dx3_i_dk3_i = (k6_i + k7_i) * k1_i + k6_i * k8_i
     dx4_i_dk3_i = (k1_i + k8_i) * k5_i
     dJncxNa_i_dk3pp_i = (
         -E2_i
-        + (
-            dE3_i_dx3_i * dx3_i_dk3_i
-            + dE3_i_dx4_i * dx4_i_dk3_i
-            + dE3_i_dx1_i * k5_i * k7_i
-        )
+        + (dE3_i_dx3_i * dx3_i_dk3_i + dE3_i_dx4_i * dx4_i_dk3_i + dE3_i_dx1_i * k5_i * k7_i)
         * k4pp_i
-        - (
-            dE2_i_dx3_i * dx3_i_dk3_i
-            + dE2_i_dx4_i * dx4_i_dk3_i
-            + dE2_i_dx1_i * k5_i * k7_i
-        )
+        - (dE2_i_dx3_i * dx3_i_dk3_i + dE2_i_dx4_i * dx4_i_dk3_i + dE2_i_dx1_i * k5_i * k7_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx3_i * dx3_i_dk3_i
-            + dE1_i_dx4_i * dx4_i_dk3_i
-            + dE1_i_dx1_i * k5_i * k7_i
-        )
+        * (dE1_i_dx3_i * dx3_i_dk3_i + dE1_i_dx4_i * dx4_i_dk3_i + dE1_i_dx1_i * k5_i * k7_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx3_i * dx3_i_dk3_i
-            + dE4_i_dx4_i * dx4_i_dk3_i
-            + dE4_i_dx1_i * k5_i * k7_i
-        )
+        * (dE4_i_dx3_i * dx3_i_dk3_i + dE4_i_dx4_i * dx4_i_dk3_i + dE4_i_dx1_i * k5_i * k7_i)
         * k7_i
     )
     dx1_i_dk4_i = (k6_i + k7_i) * k2_i
     dx2_i_dk4_i = (k1_i + k8_i) * k6_i + k1_i * k7_i
     dJncxNa_i_dk4pp_i = (
-        (
-            dE3_i_dx1_i * dx1_i_dk4_i
-            + dE3_i_dx2_i * dx2_i_dk4_i
-            + dE3_i_dx4_i * k2_i * k8_i
-        )
-        * k4pp_i
-        - (
-            dE2_i_dx1_i * dx1_i_dk4_i
-            + dE2_i_dx2_i * dx2_i_dk4_i
-            + dE2_i_dx4_i * k2_i * k8_i
-        )
+        (dE3_i_dx1_i * dx1_i_dk4_i + dE3_i_dx2_i * dx2_i_dk4_i + dE3_i_dx4_i * k2_i * k8_i) * k4pp_i
+        - (dE2_i_dx1_i * dx1_i_dk4_i + dE2_i_dx2_i * dx2_i_dk4_i + dE2_i_dx4_i * k2_i * k8_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx1_i * dx1_i_dk4_i
-            + dE1_i_dx2_i * dx2_i_dk4_i
-            + dE1_i_dx4_i * k2_i * k8_i
-        )
+        * (dE1_i_dx1_i * dx1_i_dk4_i + dE1_i_dx2_i * dx2_i_dk4_i + dE1_i_dx4_i * k2_i * k8_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx1_i * dx1_i_dk4_i
-            + dE4_i_dx2_i * dx2_i_dk4_i
-            + dE4_i_dx4_i * k2_i * k8_i
-        )
+        * (dE4_i_dx1_i * dx1_i_dk4_i + dE4_i_dx2_i * dx2_i_dk4_i + dE4_i_dx4_i * k2_i * k8_i)
         * k7_i
         + E3_i
     )
     dx1_i_dk7_i = (k2_i + k3_i) * k5_i + k2_i * k4_i
     dx2_i_dk7_i = (k4_i + k5_i) * k1_i
     dJncxNa_i_dk7_i = (
         3 * E4_i
-        + (
-            dE3_i_dx1_i * dx1_i_dk7_i
-            + dE3_i_dx2_i * dx2_i_dk7_i
-            + dE3_i_dx3_i * k1_i * k3_i
-        )
+        + (dE3_i_dx1_i * dx1_i_dk7_i + dE3_i_dx2_i * dx2_i_dk7_i + dE3_i_dx3_i * k1_i * k3_i)
         * k4pp_i
-        - (
-            dE2_i_dx1_i * dx1_i_dk7_i
-            + dE2_i_dx2_i * dx2_i_dk7_i
-            + dE2_i_dx3_i * k1_i * k3_i
-        )
+        - (dE2_i_dx1_i * dx1_i_dk7_i + dE2_i_dx2_i * dx2_i_dk7_i + dE2_i_dx3_i * k1_i * k3_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx1_i * dx1_i_dk7_i
-            + dE1_i_dx2_i * dx2_i_dk7_i
-            + dE1_i_dx3_i * k1_i * k3_i
-        )
+        * (dE1_i_dx1_i * dx1_i_dk7_i + dE1_i_dx2_i * dx2_i_dk7_i + dE1_i_dx3_i * k1_i * k3_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx1_i * dx1_i_dk7_i
-            + dE4_i_dx2_i * dx2_i_dk7_i
-            + dE4_i_dx3_i * k1_i * k3_i
-        )
+        * (dE4_i_dx1_i * dx1_i_dk7_i + dE4_i_dx2_i * dx2_i_dk7_i + dE4_i_dx3_i * k1_i * k3_i)
         * k7_i
     )
     dx3_i_dk8_i = (k2_i + k3_i) * k6_i
     dx4_i_dk8_i = (k4_i + k5_i) * k2_i + k3_i * k5_i
     dJncxNa_i_dk8_i = (
         -3 * E1_i
-        + (
-            dE3_i_dx3_i * dx3_i_dk8_i
-            + dE3_i_dx4_i * dx4_i_dk8_i
-            + dE3_i_dx2_i * k4_i * k6_i
-        )
+        + (dE3_i_dx3_i * dx3_i_dk8_i + dE3_i_dx4_i * dx4_i_dk8_i + dE3_i_dx2_i * k4_i * k6_i)
         * k4pp_i
-        - (
-            dE2_i_dx3_i * dx3_i_dk8_i
-            + dE2_i_dx4_i * dx4_i_dk8_i
-            + dE2_i_dx2_i * k4_i * k6_i
-        )
+        - (dE2_i_dx3_i * dx3_i_dk8_i + dE2_i_dx4_i * dx4_i_dk8_i + dE2_i_dx2_i * k4_i * k6_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx3_i * dx3_i_dk8_i
-            + dE1_i_dx4_i * dx4_i_dk8_i
-            + dE1_i_dx2_i * k4_i * k6_i
-        )
+        * (dE1_i_dx3_i * dx3_i_dk8_i + dE1_i_dx4_i * dx4_i_dk8_i + dE1_i_dx2_i * k4_i * k6_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx3_i * dx3_i_dk8_i
-            + dE4_i_dx4_i * dx4_i_dk8_i
-            + dE4_i_dx2_i * k4_i * k6_i
-        )
+        * (dE4_i_dx3_i * dx3_i_dk8_i + dE4_i_dx4_i * dx4_i_dk8_i + dE4_i_dx2_i * k4_i * k6_i)
         * k7_i
     )
     dx3_ss_dk3_ss = (k6_ss + k7_ss) * k1_ss + k6_ss * k8_ss
     dx4_ss_dk3_ss = (k1_ss + k8_ss) * k5_ss
     dJncxNa_ss_dk3pp_ss = (
         -E2_ss
         + (
@@ -5146,82 +4713,50 @@
             + dE4_ss_dx4_ss * dx4_ss_dk8_ss
             + dE4_ss_dx2_ss * k4_ss * k6_ss
         )
         * k7_ss
     )
     dKnai_dvfrt = Knai0 * delta * np.exp(delta * vfrt / 3) / 3
     dKnao_dvfrt = Knao0 * (1 / 3 - delta / 3) * np.exp((1 - delta) * vfrt / 3)
-    dPhiCaK_i_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaK_i_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * np.exp(
-        vfrt
-    ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
-        vfrt
-    ) * gamma_ki * ki * vffrt / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaK_ss_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaK_ss_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * np.exp(
-        vfrt
-    ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
-        vfrt
-    ) * gamma_kss * kss * vffrt / (
-        -1 + np.exp(vfrt)
-    )
+    dPhiCaK_i_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) / (-1 + np.exp(vfrt))
+    dPhiCaK_i_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * np.exp(vfrt) * vffrt / (
+        (-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))
+    ) + np.exp(vfrt) * gamma_ki * ki * vffrt / (-1 + np.exp(vfrt))
+    dPhiCaK_ss_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) / (-1 + np.exp(vfrt))
+    dPhiCaK_ss_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * np.exp(vfrt) * vffrt / (
+        (-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))
+    ) + np.exp(vfrt) * gamma_kss * kss * vffrt / (-1 + np.exp(vfrt))
     dPhiCaL_i_dvffrt = (
-        4
-        * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
-        / (-1 + np.exp(2 * vfrt))
+        4 * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) / (-1 + np.exp(2 * vfrt))
     )
-    dPhiCaL_i_dvfrt = -8 * (
-        -cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai
-    ) * np.exp(2 * vfrt) * vffrt / (
-        (-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))
-    ) + 8 * cai * np.exp(
+    dPhiCaL_i_dvfrt = -8 * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) * np.exp(
         2 * vfrt
-    ) * gamma_cai * vffrt / (
-        -1 + np.exp(2 * vfrt)
-    )
+    ) * vffrt / ((-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))) + 8 * cai * np.exp(
+        2 * vfrt
+    ) * gamma_cai * vffrt / (-1 + np.exp(2 * vfrt))
     dPhiCaL_ss_dvffrt = (
-        4
-        * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
-        / (-1 + np.exp(2 * vfrt))
+        4 * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass) / (-1 + np.exp(2 * vfrt))
     )
-    dPhiCaL_ss_dvfrt = -8 * (
-        -cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass
-    ) * np.exp(2 * vfrt) * vffrt / (
-        (-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))
-    ) + 8 * cass * np.exp(
+    dPhiCaL_ss_dvfrt = -8 * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass) * np.exp(
         2 * vfrt
-    ) * gamma_cass * vffrt / (
-        -1 + np.exp(2 * vfrt)
-    )
-    dPhiCaNa_i_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) / (
-        -1 + np.exp(vfrt)
-    )
+    ) * vffrt / ((-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))) + 8 * cass * np.exp(
+        2 * vfrt
+    ) * gamma_cass * vffrt / (-1 + np.exp(2 * vfrt))
+    dPhiCaNa_i_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) / (-1 + np.exp(vfrt))
     dPhiCaNa_i_dvfrt = -(-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * np.exp(
         vfrt
     ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
         vfrt
-    ) * gamma_nai * nai * vffrt / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaNa_ss_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) / (
-        -1 + np.exp(vfrt)
-    )
+    ) * gamma_nai * nai * vffrt / (-1 + np.exp(vfrt))
+    dPhiCaNa_ss_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) / (-1 + np.exp(vfrt))
     dPhiCaNa_ss_dvfrt = -(-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * np.exp(
         vfrt
     ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
         vfrt
-    ) * gamma_nass * nass * vffrt / (
-        -1 + np.exp(vfrt)
-    )
+    ) * gamma_nass * nass * vffrt / (-1 + np.exp(vfrt))
     da1_dKnai = -3 * k1p * (nai * nai * nai) / (
         (
             -1
             + ((1 + ki / Kki) * (1 + ki / Kki))
             + ((1 + nai / Knai) * (1 + nai / Knai) * (1 + nai / Knai))
         )
         * np.power(Knai, 4)
@@ -5311,17 +4846,15 @@
     dfca_dAfcaf = -fcas + fcaf
     dfcap_dAfcaf = -fcas + fcafp
     dh1_i_dhna = nai / kna3
     dh1_ss_dhna = nass / kna3
     dh2_i_dh1_i = -hna * nai / (kna3 * (h1_i * h1_i))
     dh2_i_dhna = nai / (kna3 * h1_i) - dh1_i_dhna * hna * nai / (kna3 * (h1_i * h1_i))
     dh2_ss_dh1_ss = -hna * nass / (kna3 * (h1_ss * h1_ss))
-    dh2_ss_dhna = nass / (kna3 * h1_ss) - dh1_ss_dhna * hna * nass / (
-        kna3 * (h1_ss * h1_ss)
-    )
+    dh2_ss_dhna = nass / (kna3 * h1_ss) - dh1_ss_dhna * hna * nass / (kna3 * (h1_ss * h1_ss))
     dh3_i_dh1_i = -1 / (h1_i * h1_i)
     dh3_ss_dh1_ss = -1 / (h1_ss * h1_ss)
     dh7_i_dhna = -nao / (kna3 * (hna * hna))
     dh7_ss_dhna = -nao / (kna3 * (hna * hna))
     dh8_i_dh7_i = -nao / (kna3 * (h7_i * h7_i) * hna)
     dh8_i_dhna = -nao / (kna3 * h7_i * (hna * hna)) - nao * dh7_i_dhna / (
         kna3 * (h7_i * h7_i) * hna
@@ -5398,19 +4931,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5423,19 +4952,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5457,19 +4982,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -5528,19 +5049,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5553,19 +5070,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5587,19 +5100,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -5661,19 +5170,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5686,19 +5191,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5720,19 +5221,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -5791,19 +5288,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5816,19 +5309,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5850,19 +5339,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -5893,26 +5378,20 @@
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaL_i_dfcap
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaL_ss_dfcap
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaNa_i_dfcap
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaNa_ss_dfcap
         - (dAiF_dv * di_dAiF - dAiF_dv * iS) * dIto_di
         - (dAiF_dv * dip_dAiF - dAiF_dv * iSp) * dIto_dip
         - (dK1ss_daK1 * daK1_dv + dK1ss_dbK1 * dbK1_dv) * dIK1_dK1ss
-        - (dPhiCaK_i_dvffrt * dvffrt_dv + dPhiCaK_i_dvfrt * dvfrt_dv)
-        * dICaK_i_dPhiCaK_i
-        - (dPhiCaK_ss_dvffrt * dvffrt_dv + dPhiCaK_ss_dvfrt * dvfrt_dv)
-        * dICaK_ss_dPhiCaK_ss
-        - (dPhiCaL_i_dvffrt * dvffrt_dv + dPhiCaL_i_dvfrt * dvfrt_dv)
-        * dICaL_i_dPhiCaL_i
-        - (dPhiCaL_ss_dvffrt * dvffrt_dv + dPhiCaL_ss_dvfrt * dvfrt_dv)
-        * dICaL_ss_dPhiCaL_ss
-        - (dPhiCaNa_i_dvffrt * dvffrt_dv + dPhiCaNa_i_dvfrt * dvfrt_dv)
-        * dICaNa_i_dPhiCaNa_i
-        - (dPhiCaNa_ss_dvffrt * dvffrt_dv + dPhiCaNa_ss_dvfrt * dvfrt_dv)
-        * dICaNa_ss_dPhiCaNa_ss
+        - (dPhiCaK_i_dvffrt * dvffrt_dv + dPhiCaK_i_dvfrt * dvfrt_dv) * dICaK_i_dPhiCaK_i
+        - (dPhiCaK_ss_dvffrt * dvffrt_dv + dPhiCaK_ss_dvfrt * dvfrt_dv) * dICaK_ss_dPhiCaK_ss
+        - (dPhiCaL_i_dvffrt * dvffrt_dv + dPhiCaL_i_dvfrt * dvfrt_dv) * dICaL_i_dPhiCaL_i
+        - (dPhiCaL_ss_dvffrt * dvffrt_dv + dPhiCaL_ss_dvfrt * dvfrt_dv) * dICaL_ss_dPhiCaL_ss
+        - (dPhiCaNa_i_dvffrt * dvffrt_dv + dPhiCaNa_i_dvfrt * dvfrt_dv) * dICaNa_i_dPhiCaNa_i
+        - (dPhiCaNa_ss_dvffrt * dvffrt_dv + dPhiCaNa_ss_dvfrt * dvfrt_dv) * dICaNa_ss_dPhiCaNa_ss
         - (
             (
                 (
                     (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
@@ -5951,19 +5430,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5976,19 +5451,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6010,19 +5481,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6081,19 +5548,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6106,19 +5569,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6140,19 +5599,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6212,19 +5667,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6237,19 +5688,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6271,19 +5718,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6343,19 +5786,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6368,19 +5807,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6402,19 +5837,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6502,19 +5933,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6527,19 +5954,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6561,19 +5984,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -6632,19 +6051,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6657,19 +6072,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6691,19 +6102,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -6763,19 +6170,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6788,19 +6191,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6822,19 +6221,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -6894,19 +6289,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6919,19 +6310,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6953,19 +6340,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -7166,19 +6549,15 @@
     dx4_db3 = a1 * b2 + b2 * b4
     dJnakNa_db3 = (
         -3 * E2
         - 3 * (dE2_dx1 * dx1_db3 + dE2_dx4 * dx4_db3 + b1 * b2 * dE2_dx3) * b3
         + 3 * (dE1_dx1 * dx1_db3 + dE1_dx4 * dx4_db3 + b1 * b2 * dE1_dx3) * a3
     )
     dP_dnai = -eP / (
-        Knap
-        * (
-            (1 + H / Khp + nai / Knap + ki / Kxkur)
-            * (1 + H / Khp + nai / Knap + ki / Kxkur)
-        )
+        Knap * ((1 + H / Khp + nai / Knap + ki / Kxkur) * (1 + H / Khp + nai / Knap + ki / Kxkur))
     )
     dPhiCaNa_i_dgamma_nai = np.exp(vfrt) * nai * vffrt / (-1 + np.exp(vfrt))
     dgamma_nai_dIi = (
         -(
             -0.3
             - 1 / (2 * ((1 + np.sqrt(Ii)) * (1 + np.sqrt(Ii))))
             + 1 / (2 * (1 + np.sqrt(Ii)) * np.sqrt(Ii))
@@ -7244,16 +6623,15 @@
         kna1 * kna2 * (h4_i * h4_i)
     )
     dh6_i_dh4_i = -1 / (h4_i * h4_i)
     dx2_i_dk6_i = (k1_i + k8_i) * k4_i
     dx3_i_dk6_i = (k2_i + k3_i) * k8_i + k1_i * k3_i
     dnai_dt_linearized = dJdiffNa_dnai * vss / vmyo + (
         -dINab_dnai
-        - (0.0005 * dPhiCaNa_i_dgamma_nai * dgamma_nai_dIi + dPhiCaNa_i_dnai)
-        * dICaNa_i_dPhiCaNa_i
+        - (0.0005 * dPhiCaNa_i_dgamma_nai * dgamma_nai_dIi + dPhiCaNa_i_dnai) * dICaNa_i_dPhiCaNa_i
         - dENa_dnai * dINaL_dENa
         - dENa_dnai * dINa_dENa
         - 3
         * (
             (
                 (
                     (
@@ -7559,53 +6937,45 @@
         - 3
         * zk
         * (
             dJnakK_da1 * da1_dnai
             - 2
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE3_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE3_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE3_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE3_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE3_dx4
                 + b1 * b2 * dE3_dx3 * dP_dnai * db3_dP
             )
             * a1
             + 2
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE4_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE4_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE4_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE4_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE4_dx4
                 + b1 * b2 * dE4_dx3 * dP_dnai * db3_dP
             )
             * b1
         )
         * Pnak
         - 3
         * zna
         * (
             -3
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE2_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE2_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE2_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE2_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE2_dx4
                 + b1 * b2 * dE2_dx3 * dP_dnai * db3_dP
             )
             * b3
             + 3
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE1_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE1_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE1_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE1_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE1_dx4
                 + b1 * b2 * dE1_dx3 * dP_dnai * db3_dP
             )
             * a3
             + dJnakNa_db3 * dP_dnai * db3_dP
         )
         * Pnak
     ) * Acap / (F * vmyo)
@@ -7630,17 +7000,15 @@
     )
     dPhiCaNa_ss_dnass = (
         (np.exp(vfrt) * gamma_nass + 0.0005 * dgamma_nass_dIss * np.exp(vfrt) * nass)
         * vffrt
         / (-1 + np.exp(vfrt))
     )
     dh1_ss_dnass = (1 + hna) / kna3
-    dh2_ss_dnass = hna / (kna3 * h1_ss) - dh1_ss_dnass * hna * nass / (
-        kna3 * (h1_ss * h1_ss)
-    )
+    dh2_ss_dnass = hna / (kna3 * h1_ss) - dh1_ss_dnass * hna * nass / (kna3 * (h1_ss * h1_ss))
     dh4_ss_dnass = (1 + nass / kna2) / kna1 + nass / (kna1 * kna2)
     dh5_ss_dh4_ss = -(nass * nass) / (kna1 * kna2 * (h4_ss * h4_ss))
     dh5_ss_dnass = 2 * nass / (kna1 * kna2 * h4_ss) - (nass * nass) * dh4_ss_dnass / (
         kna1 * kna2 * (h4_ss * h4_ss)
     )
     dh6_ss_dh4_ss = -1 / (h4_ss * h4_ss)
     dx2_ss_dk6_ss = (k1_ss + k8_ss) * k4_ss
@@ -7945,17 +7313,15 @@
                     + dh1_ss_dnass * dh3_ss_dh1_ss * dk4p_ss_dh3_ss
                 )
                 * dE4_ss_dx4_ss
                 * k2_ss
                 * k8_ss
             )
             * k7_ss
-            + wnaca
-            * (dh1_ss_dnass * dh2_ss_dh1_ss + dh2_ss_dnass)
-            * dJncxNa_ss_dk4pp_ss
+            + wnaca * (dh1_ss_dnass * dh2_ss_dh1_ss + dh2_ss_dnass) * dJncxNa_ss_dk4pp_ss
         )
         * dINaCa_ss_dJncxNa_ss
     ) * Acap / (F * vss)
     states[36] = (
         np.where(
             np.abs(dnass_dt_linearized) > 1e-08,
             (-1 + np.exp(dt * dnass_dt_linearized)) * dnass_dt / dnass_dt_linearized,
@@ -7975,22 +7341,18 @@
             (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
             * (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
         )
     )
     dbK1_dEK = (
         -6.919349479611957e-18 * np.exp(0.0618 * v - 0.0618 * EK)
         - 0.8506978434250505 * np.exp(0.0674 * v - 0.0674 * EK)
-    ) / (
-        1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)
-    ) - 0.016099950792318272 * (
+    ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)) - 0.016099950792318272 * (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
-    ) * np.exp(
-        0.1629 * EK - 0.1629 * v
-    ) / (
+    ) * np.exp(0.1629 * EK - 0.1629 * v) / (
         (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
         * (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     )
     dIK1_dEK = (
         -np.sqrt(5) * np.sqrt(ko) * GK1 * K1ss / 5
         + np.sqrt(5)
         * np.sqrt(ko)
@@ -8002,19 +7364,15 @@
     dIKb_dEK = -GKb * xkb
     dIKr_dEK = -np.sqrt(5) * np.sqrt(ko) * GKr * O / 5
     dIKs_dEKs = -GKs * KsCa * xs1 * xs2
     dI_katp_dEK = -fkatp * gkatp * akik * bkik
     dIto_dEK = -((1 - fItop) * a * i + ap * fItop * ip) * Gto
     dJdiffK_dki = -1 / tauK
     dP_dki = -eP / (
-        Kxkur
-        * (
-            (1 + H / Khp + nai / Knap + ki / Kxkur)
-            * (1 + H / Khp + nai / Knap + ki / Kxkur)
-        )
+        Kxkur * ((1 + H / Khp + nai / Knap + ki / Kxkur) * (1 + H / Khp + nai / Knap + ki / Kxkur))
     )
     dPhiCaK_i_dgamma_ki = np.exp(vfrt) * ki * vffrt / (-1 + np.exp(vfrt))
     dgamma_ki_dIi = (
         -(
             -0.3
             - 1 / (2 * ((1 + np.sqrt(Ii)) * (1 + np.sqrt(Ii))))
             + 1 / (2 * (1 + np.sqrt(Ii)) * np.sqrt(Ii))
@@ -8068,70 +7426,60 @@
                 -1
                 + ((1 + ki / Kki) * (1 + ki / Kki))
                 + ((1 + nai / Knai) * (1 + nai / Knai) * (1 + nai / Knai))
             )
         )
     )
     dki_dt_linearized = dJdiffK_dki * vss / vmyo + (
-        -(0.0005 * dPhiCaK_i_dgamma_ki * dgamma_ki_dIi + dPhiCaK_i_dki)
-        * dICaK_i_dPhiCaK_i
-        - (dEK_dki * dK1ss_daK1 * daK1_dEK + dEK_dki * dK1ss_dbK1 * dbK1_dEK)
-        * dIK1_dK1ss
+        -(0.0005 * dPhiCaK_i_dgamma_ki * dgamma_ki_dIi + dPhiCaK_i_dki) * dICaK_i_dPhiCaK_i
+        - (dEK_dki * dK1ss_daK1 * daK1_dEK + dEK_dki * dK1ss_dbK1 * dbK1_dEK) * dIK1_dK1ss
         - dEK_dki * dIK1_dEK
         - dEK_dki * dIKb_dEK
         - dEK_dki * dIKr_dEK
         - dEK_dki * dI_katp_dEK
         - dEK_dki * dIto_dEK
         - dEKs_dki * dIKs_dEKs
         + 2
         * zk
         * (
             dJnakK_da1 * da1_dki
             - 2
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE3_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE3_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE3_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE3_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE3_dx4
                 + b1 * b2 * dE3_dx3 * dP_dki * db3_dP
             )
             * a1
             + 2
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE4_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE4_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE4_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE4_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE4_dx4
                 + b1 * b2 * dE4_dx3 * dP_dki * db3_dP
             )
             * b1
         )
         * Pnak
         + 2
         * zna
         * (
             -3
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE2_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE2_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE2_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE2_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE2_dx4
                 + b1 * b2 * dE2_dx3 * dP_dki * db3_dP
             )
             * b3
             + 3
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE1_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE1_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE1_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE1_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE1_dx4
                 + b1 * b2 * dE1_dx3 * dP_dki * db3_dP
             )
             * a3
             + dJnakNa_db3 * dP_dki * db3_dP
         )
         * Pnak
     ) * Acap / (F * vmyo)
@@ -8184,17 +7532,15 @@
             dt * dcli_dt,
         )
         + cli
     )
     dclss_dt = -JdiffCl + Acap * IClCa_junc / (F * vss)
     dEClss_dclss = -R * T / (F * zcl * clss)
     dIClCa_junc_dEClss = -Fjunc * GClCa / (1 + KdClCa / cass)
-    dclss_dt_linearized = -1 / tauNa + Acap * dEClss_dclss * dIClCa_junc_dEClss / (
-        F * vss
-    )
+    dclss_dt_linearized = -1 / tauNa + Acap * dEClss_dclss * dIClCa_junc_dEClss / (F * vss)
     states[40] = (
         np.where(
             np.abs(dclss_dt_linearized) > 1e-08,
             (-1 + np.exp(dt * dclss_dt_linearized)) * dclss_dt / dclss_dt_linearized,
             dt * dclss_dt,
         )
         + clss
@@ -8233,67 +7579,55 @@
         )
         * constA
         * np.exp(-4 * (-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     )
     dICab_dcai = (
         4
         * PCab
-        * (
-            np.exp(2 * vfrt) * gamma_cai
-            + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt)
-        )
+        * (np.exp(2 * vfrt) * gamma_cai + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt))
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    dICab_dgamma_cai = (
-        4 * PCab * cai * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
-    )
+    dICab_dgamma_cai = 4 * PCab * cai * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
     dINaCa_i_dallo_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx
     dIpCa_dcai = GpCa / (KmCap + cai) - GpCa * cai / ((KmCap + cai) * (KmCap + cai))
     dJdiff_dcai = -1 / tauCa
     dJup_dJupnp = Jup_b * (1 - fJupp)
     dJupnp_dcai = 0.005425 * upScale / (0.00092 + cai) - 0.005425 * cai * upScale / (
         (0.00092 + cai) * (0.00092 + cai)
     )
     dJupp_dcai = 0.01491875 * upScale / (0.00075 + cai) - 0.01491875 * cai * upScale / (
         (0.00075 + cai) * (0.00075 + cai)
     )
     dPhiCaL_i_dcai = (
         4
-        * (
-            np.exp(2 * vfrt) * gamma_cai
-            + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt)
-        )
+        * (np.exp(2 * vfrt) * gamma_cai + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt))
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
     dPhiCaL_i_dgamma_cai = 4 * cai * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
     dallo_i_dcai = (
         2
         * (KmCaAct * KmCaAct)
         / (
-            (
-                (1 + (KmCaAct * KmCaAct) / (cai * cai))
-                * (1 + (KmCaAct * KmCaAct) / (cai * cai))
-            )
+            ((1 + (KmCaAct * KmCaAct) / (cai * cai)) * (1 + (KmCaAct * KmCaAct) / (cai * cai)))
             * (cai * cai * cai)
         )
     )
     dcai_dt_linearized = (
         Jdiff * vss / vmyo
         - Jup * vnsr / vmyo
         + (-ICaL_i - ICab - IpCa + 2 * INaCa_i) * Acap / (2 * F * vmyo)
     ) * dBcai_dcai + (
         dJdiff_dcai * vss / vmyo
         - (dJup_dJupnp * dJupnp_dcai + Jup_b * dJupp_dcai * fJupp) * vnsr / vmyo
         + (
             -dICab_dcai
             - dIpCa_dcai
-            - (0.002 * dPhiCaL_i_dgamma_cai * dgamma_cai_dIi + dPhiCaL_i_dcai)
-            * dICaL_i_dPhiCaL_i
+            - (0.002 * dPhiCaL_i_dgamma_cai * dgamma_cai_dIi + dPhiCaL_i_dcai) * dICaL_i_dPhiCaL_i
             + 2
             * (
                 (
                     kcaon * dE2_i_dx2_i * dx2_i_dk6_i * h6_i
                     + kcaon * dE2_i_dx3_i * dx3_i_dk6_i * h6_i
                     + kcaon * dE2_i_dx1_i * h6_i * k2_i * k4_i
                 )
@@ -8370,18 +7704,15 @@
         * (
             1
             + BSLmax * KmBSL / ((KmBSL + cass) * (KmBSL + cass))
             + BSRmax * KmBSR / ((KmBSR + cass) * (KmBSR + cass))
         )
     )
     dCaMKb_dcass = (
-        CaMKo
-        * KmCaM
-        * (1 - CaMKt)
-        / (((1 + KmCaM / cass) * (1 + KmCaM / cass)) * (cass * cass))
+        CaMKo * KmCaM * (1 - CaMKt) / (((1 + KmCaM / cass) * (1 + KmCaM / cass)) * (cass * cass))
     )
     dICaL_ss_dfICaLp = ICaL_fractionSS * (
         ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCap * PhiCaL_ss * d
         - ((1 - nca_ss) * f + fca * jca * nca_ss) * PCa * PhiCaL_ss * d
     )
     dINaCa_ss_dallo_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx
     dJrel_dfJrelp = Jrel_b * (-Jrel_np + Jrel_p)
@@ -8393,41 +7724,29 @@
             + 1 / (2 * (1 + np.sqrt(Iss)) * np.sqrt(Iss))
         )
         * constA
         * np.exp(-4 * (-0.3 * Iss + np.sqrt(Iss) / (1 + np.sqrt(Iss))) * constA)
     )
     dPhiCaL_ss_dcass = (
         4
-        * (
-            np.exp(2 * vfrt) * gamma_cass
-            + 0.002 * cass * dgamma_cass_dIss * np.exp(2 * vfrt)
-        )
+        * (np.exp(2 * vfrt) * gamma_cass + 0.002 * cass * dgamma_cass_dIss * np.exp(2 * vfrt))
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    dPhiCaL_ss_dgamma_cass = (
-        4 * cass * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
-    )
+    dPhiCaL_ss_dgamma_cass = 4 * cass * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
     dallo_ss_dcass = (
         2
         * (KmCaAct * KmCaAct)
         / (
-            (
-                (1 + (KmCaAct * KmCaAct) / (cass * cass))
-                * (1 + (KmCaAct * KmCaAct) / (cass * cass))
-            )
+            ((1 + (KmCaAct * KmCaAct) / (cass * cass)) * (1 + (KmCaAct * KmCaAct) / (cass * cass)))
             * (cass * cass * cass)
         )
     )
-    dfICaLp_dCaMKa = KmCaMK / (
-        ((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa)
-    )
-    dfJrelp_dCaMKa = KmCaMK / (
-        ((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa)
-    )
+    dfICaLp_dCaMKa = KmCaMK / (((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa))
+    dfJrelp_dCaMKa = KmCaMK / (((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa))
     dcass_dt_linearized = (
         -1 / tauCa
         + (
             -(0.002 * dPhiCaL_ss_dgamma_cass * dgamma_cass_dIss + dPhiCaL_ss_dcass)
             * dICaL_ss_dPhiCaL_ss
             + 2
             * (
```

### Comparing `fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/mid.py` & `fenics_beat-0.0.4/src/beat/cellmodels/torord_dyn_chloride/mid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1193,17 +1193,15 @@
     E1_i = x1_i / (x1_i + x2_i + x3_i + x4_i)
     E2_i = x2_i / (x1_i + x2_i + x3_i + x4_i)
     E3_i = x3_i / (x1_i + x2_i + x3_i + x4_i)
     E4_i = x4_i / (x1_i + x2_i + x3_i + x4_i)
     allo_i = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     JncxNa_i = E3_i * k4pp_i - E2_i * k3pp_i - 3 * E1_i * k8_i + 3 * E4_i * k7_i
     JncxCa_i = E2_i * k2_i - E1_i * k1_i
-    Gncx = np.where(
-        celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b)
-    )
+    Gncx = np.where(celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b))
     INaCa_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx * allo_i
     h1_ss = 1 + (1 + hna) * nass / kna3
     h2_ss = hna * nass / (kna3 * h1_ss)
     h3_ss = 1.0 / h1_ss
     h4_ss = 1 + (1 + nass / kna2) * nass / kna1
     h5_ss = (nass * nass) / (kna1 * kna2 * h4_ss)
     h6_ss = 1.0 / h4_ss
@@ -1230,17 +1228,15 @@
     x3_ss = (k2_ss + k3_ss) * k6_ss * k8_ss + (k6_ss + k7_ss) * k1_ss * k3_ss
     x4_ss = (k1_ss + k8_ss) * k3_ss * k5_ss + (k4_ss + k5_ss) * k2_ss * k8_ss
     E1_ss = x1_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E2_ss = x2_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E3_ss = x3_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E4_ss = x4_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     allo_ss = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
-    JncxNa_ss = (
-        E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
-    )
+    JncxNa_ss = E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
     JncxCa_ss = E2_ss * k2_ss - E1_ss * k1_ss
     INaCa_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx * allo_ss
 
     # Expressions for the K component
     Knai = Knai0 * np.exp(delta * vfrt / 3)
     Knao = Knao0 * np.exp((1 - delta) * vfrt / 3)
     P = eP / (1 + H / Khp + nai / Knap + ki / Kxkur)
@@ -1302,17 +1298,15 @@
     x4 = a1 * a3 * a4 + a1 * a4 * b2 + a1 * b2 * b3 + b2 * b3 * b4
     E1 = x1 / (x1 + x2 + x3 + x4)
     E2 = x2 / (x1 + x2 + x3 + x4)
     E3 = x3 / (x1 + x2 + x3 + x4)
     E4 = x4 / (x1 + x2 + x3 + x4)
     JnakNa = -3 * E2 * b3 + 3 * E1 * a3
     JnakK = -2 * E3 * a1 + 2 * E4 * b1
-    Pnak = np.where(
-        celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
-    )
+    Pnak = np.where(celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b))
     INaK = (zk * JnakK + zna * JnakNa) * Pnak
 
     # Expressions for the b component
     INab = PNab * (-nao + np.exp(vfrt) * nai) * vffrt / (-1 + np.exp(vfrt))
 
     # Expressions for the ICaL component
     dss = np.where(v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v)))
@@ -1324,17 +1318,15 @@
             3.5254214873653824 * np.exp(0.09 * vShift + 0.09 * v)
             + 0.7408182206817179 * np.exp(-0.05 * vShift - 0.05 * v)
         )
     )
     values[1] = (-d + dss) / td
     fss = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
     tff = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
-    tfs = 1000 + 1.0 / (
-        3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
-    )
+    tfs = 1000 + 1.0 / (3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6))
     Afs = 1 - Aff
     values[2] = (-ff + fss) / tff
     values[3] = (-fs + fss) / tfs
     f = Aff * ff + Afs * fs
     fcass = fss
     tfcaf = 7 + 1.0 / (0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7))
     tfcas = 100 + 1.0 / (0.00012 * np.exp(-v / 3) + 0.00012 * np.exp(v / 7))
@@ -1365,25 +1357,17 @@
     gamma_ko = np.exp(-(-0.3 * Io + np.sqrt(Io) / (1 + np.sqrt(Io))) * constA)
     PhiCaL_ss = (
         4
         * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_ss = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_ss = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
-    )
-    PCa = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    PhiCaNa_ss = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_ss = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
+    PCa = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     PCap = 1.1 * PCa
     PCaNa = 0.00125 * PCa
     PCaK = 0.0003574 * PCa
     PCaNap = 0.00125 * PCap
     PCaKp = 0.0003574 * PCap
     fICaLp = 1.0 / (1 + KmCaMK / CaMKa)
     ICaL_ss = ICaL_fractionSS * (
@@ -1406,22 +1390,16 @@
     gamma_ki = np.exp(-(-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     PhiCaL_i = (
         4
         * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_i = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_i = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
-    )
+    PhiCaNa_i = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_i = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
     ICaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * PhiCaL_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * PhiCaL_i * d * fICaLp
     )
     ICaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * PhiCaNa_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * PhiCaNa_i * d * fICaLp
@@ -1464,17 +1442,15 @@
         )
     )
     values[11] = (-m + mss) / tm
     hss = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    ah = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    ah = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     bh = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     th = 1.0 / (ah + bh)
     values[12] = (-h + hss) / th
@@ -1484,17 +1460,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     bj = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     jss = hss
     tj = 1.0 / (aj + bj)
     values[13] = (-j + jss) / tj
     hssp = 1.0 / (
         (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
         * (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
@@ -1526,74 +1500,54 @@
     values[18] = (-hLp + hLssp) / thLp
     GNaL = np.where(celltype == 1, 0.6 * GNaL_b, GNaL_b)
     fINaLp = 1.0 / (1 + KmCaMK / CaMKa)
     INaL = (-ENa + v) * ((1 - fINaLp) * hL + fINaLp * hLp) * GNaL * mL
 
     # Expressions for the Ito component
     ass = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     ta = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     values[19] = (-a + ass) / ta
     iss = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    delta_epi = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    delta_epi = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     tiF_b = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     tiS_b = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     tiF = delta_epi * tiF_b
     tiS = delta_epi * tiS_b
     AiF = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     AiS = 1 - AiF
     values[20] = (-iF + iss) / tiF
     values[21] = (-iS + iss) / tiS
     i = AiF * iF + AiS * iS
     assp = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     values[22] = (-ap + assp) / ta
     dti_develop = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
     dti_recover = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     tiFp = dti_develop * dti_recover * tiF
     tiSp = dti_develop * dti_recover * tiS
     values[23] = (-iFp + iss) / tiFp
     values[24] = (-iSp + iss) / tiSp
     ip = AiF * iFp + AiS * iSp
@@ -1608,53 +1562,42 @@
     beta_2 = 0.000349 * np.exp(-1.062 * vfrt)
     alpha_i = 0.2533 * np.exp(0.5953 * vfrt)
     beta_i = 0.06525 * np.exp(-0.8209 * vfrt)
     alpha_C2ToI = 5.2e-05 * np.exp(1.525 * vfrt)
     beta_ItoC2 = alpha_C2ToI * beta_2 * beta_i / (alpha_2 * alpha_i)
     values[25] = C2 * beta - C3 * alpha
     values[26] = beta_1 * C1 + C3 * alpha - (alpha_1 + beta) * C2
-    values[27] = (
-        alpha_1 * C2
-        + I * beta_ItoC2
-        + O * beta_2
-        - (beta_1 + alpha_2 + alpha_C2ToI) * C1
-    )
+    values[27] = alpha_1 * C2 + I * beta_ItoC2 + O * beta_2 - (beta_1 + alpha_2 + alpha_C2ToI) * C1
     values[28] = C1 * alpha_2 + I * beta_i - (alpha_i + beta_2) * O
     values[29] = C1 * alpha_C2ToI + O * alpha_i - (beta_ItoC2 + beta_i) * I
-    GKr = np.where(
-        celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
-    )
+    GKr = np.where(celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b))
     IKr = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GKr * O / 5
 
     # Expressions for the IKs component
     xs1ss = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     txs1 = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
     values[30] = (-xs1 + xs1ss) / txs1
     xs2ss = xs1ss
-    txs2 = 1.0 / (
-        0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20)
-    )
+    txs2 = 1.0 / (0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20))
     values[31] = (-xs2 + xs2ss) / txs2
     KsCa = 1 + 0.6 / (1 + 6.481821026062645e-07 * np.power(1.0 / cai, 1.4))
     GKs = np.where(celltype == 1, 1.4 * GKs_b, GKs_b)
     IKs = (-EKs + v) * GKs * KsCa * xs1 * xs2
 
     # Expressions for the IK1 component
     aK1 = 4.094 / (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
     bK1 = (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     K1ss = aK1 / (aK1 + bK1)
-    GK1 = np.where(
-        celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
-    )
+    GK1 = np.where(celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b))
     IK1 = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 * K1ss / 5
 
     # Expressions for the IKb component
     xkb = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     GKb = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     IKb = (-EK + v) * GKb * xkb
 
@@ -1690,17 +1633,15 @@
     fJrelp = 1.0 / (1 + KmCaMK / CaMKa)
     Jrel = Jrel_b * ((1 - fJrelp) * Jrel_np + Jrel_p * fJrelp)
 
     # Expressions for the Membrane component
     Istim = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     values[34] = (
         -ICaK
@@ -2009,26 +1950,18 @@
     ) * monitored[47] * monitored[57]
     monitored[61] = (monitored[48] + monitored[51]) * monitored[56] * monitored[58] + (
         monitored[56] + monitored[57]
     ) * monitored[47] * monitored[51]
     monitored[62] = (monitored[47] + monitored[58]) * monitored[51] * monitored[55] + (
         monitored[54] + monitored[55]
     ) * monitored[48] * monitored[58]
-    monitored[63] = monitored[59] / (
-        monitored[59] + monitored[60] + monitored[61] + monitored[62]
-    )
-    monitored[64] = monitored[60] / (
-        monitored[59] + monitored[60] + monitored[61] + monitored[62]
-    )
-    monitored[65] = monitored[61] / (
-        monitored[59] + monitored[60] + monitored[61] + monitored[62]
-    )
-    monitored[66] = monitored[62] / (
-        monitored[59] + monitored[60] + monitored[61] + monitored[62]
-    )
+    monitored[63] = monitored[59] / (monitored[59] + monitored[60] + monitored[61] + monitored[62])
+    monitored[64] = monitored[60] / (monitored[59] + monitored[60] + monitored[61] + monitored[62])
+    monitored[65] = monitored[61] / (monitored[59] + monitored[60] + monitored[61] + monitored[62])
+    monitored[66] = monitored[62] / (monitored[59] + monitored[60] + monitored[61] + monitored[62])
     monitored[67] = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     monitored[68] = (
         monitored[53] * monitored[65]
         - monitored[50] * monitored[64]
         - 3 * monitored[58] * monitored[63]
         + 3 * monitored[57] * monitored[66]
     )
@@ -2074,26 +2007,18 @@
     ) * monitored[84] * monitored[94]
     monitored[98] = (monitored[85] + monitored[88]) * monitored[93] * monitored[95] + (
         monitored[93] + monitored[94]
     ) * monitored[84] * monitored[88]
     monitored[99] = (monitored[84] + monitored[95]) * monitored[88] * monitored[92] + (
         monitored[91] + monitored[92]
     ) * monitored[85] * monitored[95]
-    monitored[100] = monitored[96] / (
-        monitored[96] + monitored[97] + monitored[98] + monitored[99]
-    )
-    monitored[101] = monitored[97] / (
-        monitored[96] + monitored[97] + monitored[98] + monitored[99]
-    )
-    monitored[102] = monitored[98] / (
-        monitored[96] + monitored[97] + monitored[98] + monitored[99]
-    )
-    monitored[103] = monitored[99] / (
-        monitored[96] + monitored[97] + monitored[98] + monitored[99]
-    )
+    monitored[100] = monitored[96] / (monitored[96] + monitored[97] + monitored[98] + monitored[99])
+    monitored[101] = monitored[97] / (monitored[96] + monitored[97] + monitored[98] + monitored[99])
+    monitored[102] = monitored[98] / (monitored[96] + monitored[97] + monitored[98] + monitored[99])
+    monitored[103] = monitored[99] / (monitored[96] + monitored[97] + monitored[98] + monitored[99])
     monitored[104] = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
     monitored[105] = (
         monitored[102] * monitored[90]
         - monitored[101] * monitored[87]
         - 3 * monitored[100] * monitored[95]
         + 3 * monitored[103] * monitored[94]
     )
@@ -2209,62 +2134,52 @@
     )
     monitored[125] = monitored[121] / (
         monitored[119] + monitored[120] + monitored[121] + monitored[122]
     )
     monitored[126] = monitored[122] / (
         monitored[119] + monitored[120] + monitored[121] + monitored[122]
     )
-    monitored[127] = (
-        -3 * monitored[116] * monitored[124] + 3 * monitored[115] * monitored[123]
-    )
-    monitored[128] = (
-        -2 * monitored[111] * monitored[125] + 2 * monitored[112] * monitored[126]
-    )
+    monitored[127] = -3 * monitored[116] * monitored[124] + 3 * monitored[115] * monitored[123]
+    monitored[128] = -2 * monitored[111] * monitored[125] + 2 * monitored[112] * monitored[126]
     monitored[129] = np.where(
         celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
     )
     monitored[130] = (zk * monitored[128] + zna * monitored[127]) * monitored[129]
 
     # Expressions for the b component
     monitored[131] = (
         PNab
         * (-nao + np.exp(monitored[274]) * nai)
         * monitored[273]
         / (-1 + np.exp(monitored[274]))
     )
 
     # Expressions for the ICaL component
-    monitored[140] = np.where(
-        v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v))
-    )
+    monitored[140] = np.where(v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v)))
     monitored[141] = (
         0.6
         + offset
         + 1.0
         / (
             3.5254214873653824 * np.exp(0.09 * vShift + 0.09 * v)
             + 0.7408182206817179 * np.exp(-0.05 * vShift - 0.05 * v)
         )
     )
     monitored[277] = (-d + monitored[140]) / monitored[141]
     monitored[142] = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
-    monitored[143] = 7 + 1.0 / (
-        0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10)
-    )
+    monitored[143] = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
     monitored[144] = 1000 + 1.0 / (
         3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
     )
     monitored[145] = 1 - Aff
     monitored[278] = (-ff + monitored[142]) / monitored[143]
     monitored[279] = (-fs + monitored[142]) / monitored[144]
     monitored[146] = Aff * ff + fs * monitored[145]
     monitored[147] = monitored[142]
-    monitored[148] = 7 + 1.0 / (
-        0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7)
-    )
+    monitored[148] = 7 + 1.0 / (0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7))
     monitored[149] = 100 + 1.0 / (0.00012 * np.exp(-v / 3) + 0.00012 * np.exp(v / 7))
     monitored[150] = 0.3 + 0.6 / (1 + np.exp(-1 + v / 10))
     monitored[151] = 1 - monitored[150]
     monitored[280] = (-fcaf + monitored[147]) / monitored[148]
     monitored[281] = (-fcas + monitored[147]) / monitored[149]
     monitored[152] = fcaf * monitored[150] + fcas * monitored[151]
     monitored[153] = 1.0 / (1.0 + 649.7401897235336 * np.exp(0.35821750967187277 * v))
@@ -2279,54 +2194,36 @@
     monitored[159] = 1.0 / (np.power(1 + Kmn / cass, 4) + k2n / monitored[158])
     monitored[285] = k2n * monitored[159] - monitored[158] * nca_ss
     monitored[160] = 0.0005 * clo + 0.0005 * ko + 0.0005 * nao + 0.002 * cao
     monitored[161] = 0.0005 * clss + 0.0005 * kss + 0.0005 * nass + 0.002 * cass
     monitored[162] = 1820000.0 * np.power(T * dielConstant, -1.5)
     monitored[163] = np.exp(
         -4
-        * (
-            -0.3 * monitored[161]
-            + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161]))
-        )
+        * (-0.3 * monitored[161] + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161])))
         * monitored[162]
     )
     monitored[164] = np.exp(
         -4
-        * (
-            -0.3 * monitored[160]
-            + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160]))
-        )
+        * (-0.3 * monitored[160] + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160])))
         * monitored[162]
     )
     monitored[165] = np.exp(
-        -(
-            -0.3 * monitored[161]
-            + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161]))
-        )
+        -(-0.3 * monitored[161] + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161])))
         * monitored[162]
     )
     monitored[166] = np.exp(
-        -(
-            -0.3 * monitored[160]
-            + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160]))
-        )
+        -(-0.3 * monitored[160] + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160])))
         * monitored[162]
     )
     monitored[167] = np.exp(
-        -(
-            -0.3 * monitored[161]
-            + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161]))
-        )
+        -(-0.3 * monitored[161] + np.sqrt(monitored[161]) / (1 + np.sqrt(monitored[161])))
         * monitored[162]
     )
     monitored[168] = np.exp(
-        -(
-            -0.3 * monitored[160]
-            + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160]))
-        )
+        -(-0.3 * monitored[160] + np.sqrt(monitored[160]) / (1 + np.sqrt(monitored[160])))
         * monitored[162]
     )
     monitored[169] = (
         4
         * (-cao * monitored[164] + cass * np.exp(2 * monitored[274]) * monitored[163])
         * monitored[273]
         / (-1 + np.exp(2 * monitored[274]))
@@ -2337,17 +2234,15 @@
         / (-1 + np.exp(monitored[274]))
     )
     monitored[171] = (
         (-ko * monitored[168] + np.exp(monitored[274]) * kss * monitored[167])
         * monitored[273]
         / (-1 + np.exp(monitored[274]))
     )
-    monitored[172] = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    monitored[172] = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     monitored[173] = 1.1 * monitored[172]
     monitored[174] = 0.00125 * monitored[172]
     monitored[175] = 0.0003574 * monitored[172]
     monitored[176] = 0.00125 * monitored[173]
     monitored[177] = 0.0003574 * monitored[173]
     monitored[178] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[179] = ICaL_fractionSS * (
@@ -2387,32 +2282,23 @@
         * monitored[178]
     )
     monitored[182] = 1.0 / (np.power(1 + Kmn / cai, 4) + k2n / monitored[158])
     monitored[286] = k2n * monitored[182] - monitored[158] * nca_i
     monitored[183] = 0.0005 * cli + 0.0005 * ki + 0.0005 * nai + 0.002 * cai
     monitored[184] = np.exp(
         -4
-        * (
-            -0.3 * monitored[183]
-            + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183]))
-        )
+        * (-0.3 * monitored[183] + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183])))
         * monitored[162]
     )
     monitored[185] = np.exp(
-        -(
-            -0.3 * monitored[183]
-            + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183]))
-        )
+        -(-0.3 * monitored[183] + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183])))
         * monitored[162]
     )
     monitored[186] = np.exp(
-        -(
-            -0.3 * monitored[183]
-            + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183]))
-        )
+        -(-0.3 * monitored[183] + np.sqrt(monitored[183]) / (1 + np.sqrt(monitored[183])))
         * monitored[162]
     )
     monitored[187] = (
         4
         * (-cao * monitored[164] + cai * np.exp(2 * monitored[274]) * monitored[184])
         * monitored[273]
         / (-1 + np.exp(2 * monitored[274]))
@@ -2470,25 +2356,21 @@
     # Expressions for the SERCA component
     monitored[196] = np.where(celltype == 1, 1.3, 1)
     monitored[197] = 0.005425 * cai * monitored[196] / (0.00092 + cai)
     monitored[198] = 0.01491875 * cai * monitored[196] / (0.00075 + cai)
     monitored[199] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[200] = 0.0003255 * cansr
     monitored[201] = Jup_b * (
-        -monitored[200]
-        + (1 - monitored[199]) * monitored[197]
-        + monitored[198] * monitored[199]
+        -monitored[200] + (1 - monitored[199]) * monitored[197] + monitored[198] * monitored[199]
     )
 
     # Expressions for the I_katp component
     monitored[202] = np.power(ko / K_o_n, 0.24)
     monitored[203] = 1.0 / (1 + (A_atp * A_atp) / (K_atp * K_atp))
-    monitored[204] = (
-        fkatp * gkatp * (-monitored[10] + v) * monitored[202] * monitored[203]
-    )
+    monitored[204] = fkatp * gkatp * (-monitored[10] + v) * monitored[202] * monitored[203]
 
     # Expressions for the INa component
     monitored[19] = 1.0 / (
         (1 + 0.0018422115811651339 * np.exp(-0.1107419712070875 * v))
         * (1 + 0.0018422115811651339 * np.exp(-0.1107419712070875 * v))
     )
     monitored[20] = 0.1292 * np.exp(
@@ -2503,17 +2385,15 @@
         )
     )
     monitored[287] = (-m + monitored[19]) / monitored[20]
     monitored[21] = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    monitored[22] = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    monitored[22] = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     monitored[23] = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     monitored[24] = 1.0 / (monitored[22] + monitored[23])
     monitored[288] = (-h + monitored[21]) / monitored[24]
@@ -2523,17 +2403,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     monitored[26] = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     monitored[27] = monitored[21]
     monitored[28] = 1.0 / (monitored[25] + monitored[26])
     monitored[289] = (-j + monitored[27]) / monitored[28]
     monitored[29] = 1.0 / (
         (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
         * (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
@@ -2575,109 +2453,79 @@
         * ((1 - monitored[138]) * hL + hLp * monitored[138])
         * mL
         * monitored[137]
     )
 
     # Expressions for the Ito component
     monitored[205] = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     monitored[206] = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     monitored[295] = (-a + monitored[205]) / monitored[206]
     monitored[207] = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    monitored[208] = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    monitored[208] = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     monitored[209] = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     monitored[210] = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     monitored[211] = monitored[208] * monitored[209]
     monitored[212] = monitored[208] * monitored[210]
     monitored[213] = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     monitored[214] = 1 - monitored[213]
     monitored[296] = (-iF + monitored[207]) / monitored[211]
     monitored[297] = (-iS + monitored[207]) / monitored[212]
     monitored[215] = iF * monitored[213] + iS * monitored[214]
     monitored[216] = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     monitored[298] = (-ap + monitored[216]) / monitored[206]
     monitored[217] = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
-    )
-    monitored[218] = 1 - 0.5 / (
-        1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
+    monitored[218] = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     monitored[219] = monitored[211] * monitored[217] * monitored[218]
     monitored[220] = monitored[212] * monitored[217] * monitored[218]
     monitored[299] = (-iFp + monitored[207]) / monitored[219]
     monitored[300] = (-iSp + monitored[207]) / monitored[220]
     monitored[221] = iFp * monitored[213] + iSp * monitored[214]
-    monitored[222] = np.where(
-        celltype == 1, 2 * Gto_b, np.where(celltype == 2, 2 * Gto_b, Gto_b)
-    )
+    monitored[222] = np.where(celltype == 1, 2 * Gto_b, np.where(celltype == 2, 2 * Gto_b, Gto_b))
     monitored[223] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[224] = (
         (-monitored[10] + v)
-        * (
-            (1 - monitored[223]) * a * monitored[215]
-            + ap * monitored[221] * monitored[223]
-        )
+        * ((1 - monitored[223]) * a * monitored[215] + ap * monitored[221] * monitored[223])
         * monitored[222]
     )
 
     # Expressions for the IKr component
     monitored[225] = 0.1161 * np.exp(0.299 * monitored[274])
     monitored[226] = 0.2442 * np.exp(-1.604 * monitored[274])
     monitored[227] = 0.0578 * np.exp(0.971 * monitored[274])
     monitored[228] = 0.000349 * np.exp(-1.062 * monitored[274])
     monitored[229] = 0.2533 * np.exp(0.5953 * monitored[274])
     monitored[230] = 0.06525 * np.exp(-0.8209 * monitored[274])
     monitored[231] = 5.2e-05 * np.exp(1.525 * monitored[274])
     monitored[232] = (
-        monitored[228]
-        * monitored[230]
-        * monitored[231]
-        / (monitored[227] * monitored[229])
+        monitored[228] * monitored[230] * monitored[231] / (monitored[227] * monitored[229])
     )
     monitored[301] = C2 * monitored[226] - C3 * monitored[225]
     monitored[302] = beta_1 * C1 + C3 * monitored[225] - (alpha_1 + monitored[226]) * C2
     monitored[303] = (
         alpha_1 * C2
         + I * monitored[232]
         + O * monitored[228]
@@ -2688,17 +2536,15 @@
     )
     monitored[305] = (
         C1 * monitored[231] + O * monitored[229] - (monitored[230] + monitored[232]) * I
     )
     monitored[233] = np.where(
         celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
     )
-    monitored[234] = (
-        np.sqrt(5) * np.sqrt(ko) * (-monitored[10] + v) * O * monitored[233] / 5
-    )
+    monitored[234] = np.sqrt(5) * np.sqrt(ko) * (-monitored[10] + v) * O * monitored[233] / 5
 
     # Expressions for the IKs component
     monitored[235] = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     monitored[236] = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
@@ -2721,20 +2567,15 @@
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * monitored[10])
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * monitored[10] - 0.1629 * v))
     monitored[244] = monitored[242] / (monitored[242] + monitored[243])
     monitored[245] = np.where(
         celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
     )
     monitored[246] = (
-        np.sqrt(5)
-        * np.sqrt(ko)
-        * (-monitored[10] + v)
-        * monitored[244]
-        * monitored[245]
-        / 5
+        np.sqrt(5) * np.sqrt(ko) * (-monitored[10] + v) * monitored[244] * monitored[245] / 5
     )
 
     # Expressions for the IKb component
     monitored[247] = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     monitored[248] = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     monitored[249] = (-monitored[10] + v) * monitored[247] * monitored[248]
 
@@ -2752,43 +2593,37 @@
         * monitored[273]
         / (-1 + np.exp(2 * monitored[274]))
     )
 
     # Expressions for the Ryr component
     monitored[255] = 0.5 * bt
     monitored[256] = (
-        -monitored[179]
-        * monitored[255]
-        / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
+        -monitored[179] * monitored[255] / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
     )
     monitored[257] = np.where(celltype == 2, 1.7 * monitored[256], monitored[256])
     monitored[258] = bt / (1 + 0.0123 / cajsr)
     monitored[259] = np.where(monitored[258] < 0.001, 0.001, monitored[258])
     monitored[308] = (-Jrel_np + monitored[257]) / monitored[259]
     monitored[260] = 1.25 * bt
     monitored[261] = 0.5 * monitored[260]
     monitored[262] = (
-        -monitored[179]
-        * monitored[261]
-        / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
+        -monitored[179] * monitored[261] / (1 + np.power(cajsr_half, 8) / np.power(cajsr, 8))
     )
     monitored[263] = np.where(celltype == 2, 1.7 * monitored[262], monitored[262])
     monitored[264] = monitored[260] / (1 + 0.0123 / cajsr)
     monitored[265] = np.where(monitored[264] < 0.001, 0.001, monitored[264])
     monitored[309] = (-Jrel_p + monitored[263]) / monitored[265]
     monitored[266] = 1.0 / (1 + KmCaMK / monitored[8])
     monitored[267] = Jrel_b * ((1 - monitored[266]) * Jrel_np + Jrel_p * monitored[266])
 
     # Expressions for the Membrane component
     monitored[268] = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     monitored[310] = (
         -monitored[107]
@@ -2819,17 +2654,17 @@
         -monitored[131]
         - monitored[139]
         - monitored[191]
         - monitored[32]
         - 3 * monitored[130]
         - 3 * monitored[71]
     ) * monitored[2] / (F * monitored[3])
-    monitored[312] = -monitored[15] + (
-        -monitored[180] - 3 * monitored[107]
-    ) * monitored[2] / (F * monitored[6])
+    monitored[312] = -monitored[15] + (-monitored[180] - 3 * monitored[107]) * monitored[2] / (
+        F * monitored[6]
+    )
     monitored[313] = monitored[16] * monitored[6] / monitored[3] + (
         -monitored[192]
         - monitored[204]
         - monitored[224]
         - monitored[234]
         - monitored[241]
         - monitored[246]
@@ -2861,17 +2696,15 @@
     )
     monitored[318] = (
         -monitored[17]
         + monitored[267] * monitored[5] / monitored[6]
         + (-monitored[179] + 2 * monitored[107]) * monitored[2] / (2 * F * monitored[6])
     ) * monitored[271]
     monitored[319] = -monitored[275] * monitored[5] / monitored[4] + monitored[201]
-    monitored[272] = 1.0 / (
-        1 + csqnmax * kmcsqn / ((kmcsqn + cajsr) * (kmcsqn + cajsr))
-    )
+    monitored[272] = 1.0 / (1 + csqnmax * kmcsqn / ((kmcsqn + cajsr) * (kmcsqn + cajsr)))
     monitored[320] = (-monitored[267] + monitored[275]) * monitored[272]
 
     # Return results
     return monitored
 
 
 def forward_explicit_euler(states, t, dt, parameters):
@@ -3115,17 +2948,15 @@
     E1_i = x1_i / (x1_i + x2_i + x3_i + x4_i)
     E2_i = x2_i / (x1_i + x2_i + x3_i + x4_i)
     E3_i = x3_i / (x1_i + x2_i + x3_i + x4_i)
     E4_i = x4_i / (x1_i + x2_i + x3_i + x4_i)
     allo_i = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     JncxNa_i = E3_i * k4pp_i - E2_i * k3pp_i - 3 * E1_i * k8_i + 3 * E4_i * k7_i
     JncxCa_i = E2_i * k2_i - E1_i * k1_i
-    Gncx = np.where(
-        celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b)
-    )
+    Gncx = np.where(celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b))
     INaCa_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx * allo_i
     h1_ss = 1 + (1 + hna) * nass / kna3
     h2_ss = hna * nass / (kna3 * h1_ss)
     h3_ss = 1.0 / h1_ss
     h4_ss = 1 + (1 + nass / kna2) * nass / kna1
     h5_ss = (nass * nass) / (kna1 * kna2 * h4_ss)
     h6_ss = 1.0 / h4_ss
@@ -3152,17 +2983,15 @@
     x3_ss = (k2_ss + k3_ss) * k6_ss * k8_ss + (k6_ss + k7_ss) * k1_ss * k3_ss
     x4_ss = (k1_ss + k8_ss) * k3_ss * k5_ss + (k4_ss + k5_ss) * k2_ss * k8_ss
     E1_ss = x1_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E2_ss = x2_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E3_ss = x3_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E4_ss = x4_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     allo_ss = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
-    JncxNa_ss = (
-        E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
-    )
+    JncxNa_ss = E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
     JncxCa_ss = E2_ss * k2_ss - E1_ss * k1_ss
     INaCa_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx * allo_ss
 
     # Expressions for the K component
     Knai = Knai0 * np.exp(delta * vfrt / 3)
     Knao = Knao0 * np.exp((1 - delta) * vfrt / 3)
     P = eP / (1 + H / Khp + nai / Knap + ki / Kxkur)
@@ -3224,17 +3053,15 @@
     x4 = a1 * a3 * a4 + a1 * a4 * b2 + a1 * b2 * b3 + b2 * b3 * b4
     E1 = x1 / (x1 + x2 + x3 + x4)
     E2 = x2 / (x1 + x2 + x3 + x4)
     E3 = x3 / (x1 + x2 + x3 + x4)
     E4 = x4 / (x1 + x2 + x3 + x4)
     JnakNa = -3 * E2 * b3 + 3 * E1 * a3
     JnakK = -2 * E3 * a1 + 2 * E4 * b1
-    Pnak = np.where(
-        celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
-    )
+    Pnak = np.where(celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b))
     INaK = (zk * JnakK + zna * JnakNa) * Pnak
 
     # Expressions for the b component
     INab = PNab * (-nao + np.exp(vfrt) * nai) * vffrt / (-1 + np.exp(vfrt))
 
     # Expressions for the ICaL component
     dss = np.where(v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v)))
@@ -3247,17 +3074,15 @@
             + 0.7408182206817179 * np.exp(-0.05 * vShift - 0.05 * v)
         )
     )
     dd_dt = (-d + dss) / td
     states[1] = dt * dd_dt + d
     fss = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
     tff = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
-    tfs = 1000 + 1.0 / (
-        3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
-    )
+    tfs = 1000 + 1.0 / (3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6))
     Afs = 1 - Aff
     dff_dt = (-ff + fss) / tff
     states[2] = dt * dff_dt + ff
     dfs_dt = (-fs + fss) / tfs
     states[3] = dt * dfs_dt + fs
     f = Aff * ff + Afs * fs
     fcass = fss
@@ -3296,25 +3121,17 @@
     gamma_ko = np.exp(-(-0.3 * Io + np.sqrt(Io) / (1 + np.sqrt(Io))) * constA)
     PhiCaL_ss = (
         4
         * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_ss = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_ss = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
-    )
-    PCa = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    PhiCaNa_ss = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_ss = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
+    PCa = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     PCap = 1.1 * PCa
     PCaNa = 0.00125 * PCa
     PCaK = 0.0003574 * PCa
     PCaNap = 0.00125 * PCap
     PCaKp = 0.0003574 * PCap
     fICaLp = 1.0 / (1 + KmCaMK / CaMKa)
     ICaL_ss = ICaL_fractionSS * (
@@ -3338,22 +3155,16 @@
     gamma_ki = np.exp(-(-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     PhiCaL_i = (
         4
         * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_i = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_i = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
-    )
+    PhiCaNa_i = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_i = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
     ICaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * PhiCaL_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * PhiCaL_i * d * fICaLp
     )
     ICaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * PhiCaNa_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * PhiCaNa_i * d * fICaLp
@@ -3397,17 +3208,15 @@
     )
     dm_dt = (-m + mss) / tm
     states[11] = dt * dm_dt + m
     hss = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    ah = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    ah = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     bh = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     th = 1.0 / (ah + bh)
     dh_dt = (-h + hss) / th
@@ -3418,17 +3227,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     bj = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     jss = hss
     tj = 1.0 / (aj + bj)
     dj_dt = (-j + jss) / tj
     states[13] = dt * dj_dt + j
     hssp = 1.0 / (
         (1 + 34112.38799331305 * np.exp(0.13458950201884254 * v))
@@ -3466,78 +3273,58 @@
     states[18] = dt * dhLp_dt + hLp
     GNaL = np.where(celltype == 1, 0.6 * GNaL_b, GNaL_b)
     fINaLp = 1.0 / (1 + KmCaMK / CaMKa)
     INaL = (-ENa + v) * ((1 - fINaLp) * hL + fINaLp * hLp) * GNaL * mL
 
     # Expressions for the Ito component
     ass = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     ta = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     da_dt = (-a + ass) / ta
     states[19] = dt * da_dt + a
     iss = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    delta_epi = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    delta_epi = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     tiF_b = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     tiS_b = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     tiF = delta_epi * tiF_b
     tiS = delta_epi * tiS_b
     AiF = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     AiS = 1 - AiF
     diF_dt = (-iF + iss) / tiF
     states[20] = dt * diF_dt + iF
     diS_dt = (-iS + iss) / tiS
     states[21] = dt * diS_dt + iS
     i = AiF * iF + AiS * iS
     assp = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     dap_dt = (-ap + assp) / ta
     states[22] = dt * dap_dt + ap
     dti_develop = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
     dti_recover = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     tiFp = dti_develop * dti_recover * tiF
     tiSp = dti_develop * dti_recover * tiS
     diFp_dt = (-iFp + iss) / tiFp
     states[23] = dt * diFp_dt + iFp
     diSp_dt = (-iSp + iss) / tiSp
@@ -3556,58 +3343,47 @@
     beta_i = 0.06525 * np.exp(-0.8209 * vfrt)
     alpha_C2ToI = 5.2e-05 * np.exp(1.525 * vfrt)
     beta_ItoC2 = alpha_C2ToI * beta_2 * beta_i / (alpha_2 * alpha_i)
     dC3_dt = C2 * beta - C3 * alpha
     states[25] = dt * dC3_dt + C3
     dC2_dt = beta_1 * C1 + C3 * alpha - (alpha_1 + beta) * C2
     states[26] = dt * dC2_dt + C2
-    dC1_dt = (
-        alpha_1 * C2
-        + I * beta_ItoC2
-        + O * beta_2
-        - (beta_1 + alpha_2 + alpha_C2ToI) * C1
-    )
+    dC1_dt = alpha_1 * C2 + I * beta_ItoC2 + O * beta_2 - (beta_1 + alpha_2 + alpha_C2ToI) * C1
     states[27] = dt * dC1_dt + C1
     dO_dt = C1 * alpha_2 + I * beta_i - (alpha_i + beta_2) * O
     states[28] = dt * dO_dt + O
     dI_dt = C1 * alpha_C2ToI + O * alpha_i - (beta_ItoC2 + beta_i) * I
     states[29] = dt * dI_dt + I
-    GKr = np.where(
-        celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
-    )
+    GKr = np.where(celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b))
     IKr = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GKr * O / 5
 
     # Expressions for the IKs component
     xs1ss = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     txs1 = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
     dxs1_dt = (-xs1 + xs1ss) / txs1
     states[30] = dt * dxs1_dt + xs1
     xs2ss = xs1ss
-    txs2 = 1.0 / (
-        0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20)
-    )
+    txs2 = 1.0 / (0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20))
     dxs2_dt = (-xs2 + xs2ss) / txs2
     states[31] = dt * dxs2_dt + xs2
     KsCa = 1 + 0.6 / (1 + 6.481821026062645e-07 * np.power(1.0 / cai, 1.4))
     GKs = np.where(celltype == 1, 1.4 * GKs_b, GKs_b)
     IKs = (-EKs + v) * GKs * KsCa * xs1 * xs2
 
     # Expressions for the IK1 component
     aK1 = 4.094 / (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
     bK1 = (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     K1ss = aK1 / (aK1 + bK1)
-    GK1 = np.where(
-        celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
-    )
+    GK1 = np.where(celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b))
     IK1 = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 * K1ss / 5
 
     # Expressions for the IKb component
     xkb = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     GKb = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     IKb = (-EK + v) * GKb * xkb
 
@@ -3645,17 +3421,15 @@
     fJrelp = 1.0 / (1 + KmCaMK / CaMKa)
     Jrel = Jrel_b * ((1 - fJrelp) * Jrel_np + Jrel_p * fJrelp)
 
     # Expressions for the Membrane component
     Istim = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     dv_dt = (
         -ICaK
@@ -3913,17 +3687,15 @@
 
     # Expressions for the CaMK component
     CaMKb = CaMKo * (1 - CaMKt) / (1 + KmCaM / cass)
     CaMKa = CaMKb + CaMKt
     dCaMKt_dt = -bCaMK * CaMKt + aCaMK * (CaMKb + CaMKt) * CaMKb
     dCaMKb_dCaMKt = -CaMKo / (1 + KmCaM / cass)
     dCaMKt_dt_linearized = (
-        -bCaMK
-        + aCaMK * (1 + dCaMKb_dCaMKt) * CaMKb
-        + aCaMK * (CaMKb + CaMKt) * dCaMKb_dCaMKt
+        -bCaMK + aCaMK * (1 + dCaMKb_dCaMKt) * CaMKb + aCaMK * (CaMKb + CaMKt) * dCaMKb_dCaMKt
     )
     states[0] = CaMKt + np.where(
         np.abs(dCaMKt_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCaMKt_dt_linearized)) * dCaMKt_dt / dCaMKt_dt_linearized,
         dt * dCaMKt_dt,
     )
 
@@ -3980,17 +3752,15 @@
     E1_i = x1_i / (x1_i + x2_i + x3_i + x4_i)
     E2_i = x2_i / (x1_i + x2_i + x3_i + x4_i)
     E3_i = x3_i / (x1_i + x2_i + x3_i + x4_i)
     E4_i = x4_i / (x1_i + x2_i + x3_i + x4_i)
     allo_i = 1.0 / (1 + (KmCaAct * KmCaAct) / (cai * cai))
     JncxNa_i = E3_i * k4pp_i - E2_i * k3pp_i - 3 * E1_i * k8_i + 3 * E4_i * k7_i
     JncxCa_i = E2_i * k2_i - E1_i * k1_i
-    Gncx = np.where(
-        celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b)
-    )
+    Gncx = np.where(celltype == 1, 1.1 * Gncx_b, np.where(celltype == 2, 1.4 * Gncx_b, Gncx_b))
     INaCa_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx * allo_i
     h1_ss = 1 + (1 + hna) * nass / kna3
     h2_ss = hna * nass / (kna3 * h1_ss)
     h3_ss = 1.0 / h1_ss
     h4_ss = 1 + (1 + nass / kna2) * nass / kna1
     h5_ss = (nass * nass) / (kna1 * kna2 * h4_ss)
     h6_ss = 1.0 / h4_ss
@@ -4017,17 +3787,15 @@
     x3_ss = (k2_ss + k3_ss) * k6_ss * k8_ss + (k6_ss + k7_ss) * k1_ss * k3_ss
     x4_ss = (k1_ss + k8_ss) * k3_ss * k5_ss + (k4_ss + k5_ss) * k2_ss * k8_ss
     E1_ss = x1_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E2_ss = x2_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E3_ss = x3_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     E4_ss = x4_ss / (x1_ss + x2_ss + x3_ss + x4_ss)
     allo_ss = 1.0 / (1 + (KmCaAct * KmCaAct) / (cass * cass))
-    JncxNa_ss = (
-        E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
-    )
+    JncxNa_ss = E3_ss * k4pp_ss - E2_ss * k3pp_ss - 3 * E1_ss * k8_ss + 3 * E4_ss * k7_ss
     JncxCa_ss = E2_ss * k2_ss - E1_ss * k1_ss
     INaCa_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx * allo_ss
 
     # Expressions for the K component
     Knai = Knai0 * np.exp(delta * vfrt / 3)
     Knao = Knao0 * np.exp((1 - delta) * vfrt / 3)
     P = eP / (1 + H / Khp + nai / Knap + ki / Kxkur)
@@ -4089,17 +3857,15 @@
     x4 = a1 * a3 * a4 + a1 * a4 * b2 + a1 * b2 * b3 + b2 * b3 * b4
     E1 = x1 / (x1 + x2 + x3 + x4)
     E2 = x2 / (x1 + x2 + x3 + x4)
     E3 = x3 / (x1 + x2 + x3 + x4)
     E4 = x4 / (x1 + x2 + x3 + x4)
     JnakNa = -3 * E2 * b3 + 3 * E1 * a3
     JnakK = -2 * E3 * a1 + 2 * E4 * b1
-    Pnak = np.where(
-        celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b)
-    )
+    Pnak = np.where(celltype == 1, 0.9 * Pnak_b, np.where(celltype == 2, 0.7 * Pnak_b, Pnak_b))
     INaK = (zk * JnakK + zna * JnakNa) * Pnak
 
     # Expressions for the b component
     INab = PNab * (-nao + np.exp(vfrt) * nai) * vffrt / (-1 + np.exp(vfrt))
 
     # Expressions for the ICaL component
     dss = np.where(v >= 31.4978, 1, 1.0763 * np.exp(-1.007 * np.exp(-0.0829 * v)))
@@ -4113,17 +3879,15 @@
         )
     )
     dd_dt = (-d + dss) / td
     dd_dt_linearized = -1 / td
     states[1] = (-1 + np.exp(dt * dd_dt_linearized)) * dd_dt / dd_dt_linearized + d
     fss = 1.0 / (1 + 199.86038496778565 * np.exp(0.27056277056277056 * v))
     tff = 7 + 1.0 / (0.0045 * np.exp(-2 - v / 10) + 0.0045 * np.exp(2 + v / 10))
-    tfs = 1000 + 1.0 / (
-        3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6)
-    )
+    tfs = 1000 + 1.0 / (3.5e-05 * np.exp(-5 / 4 - v / 4) + 3.5e-05 * np.exp(5 / 6 + v / 6))
     Afs = 1 - Aff
     dff_dt = (-ff + fss) / tff
     dff_dt_linearized = -1 / tff
     states[2] = (-1 + np.exp(dt * dff_dt_linearized)) * dff_dt / dff_dt_linearized + ff
     dfs_dt = (-fs + fss) / tfs
     dfs_dt_linearized = -1 / tfs
     states[3] = (-1 + np.exp(dt * dfs_dt_linearized)) * dfs_dt / dfs_dt_linearized + fs
@@ -4131,53 +3895,41 @@
     fcass = fss
     tfcaf = 7 + 1.0 / (0.04 * np.exp(-4 / 7 + v / 7) + 0.04 * np.exp(4 / 7 - v / 7))
     tfcas = 100 + 1.0 / (0.00012 * np.exp(-v / 3) + 0.00012 * np.exp(v / 7))
     Afcaf = 0.3 + 0.6 / (1 + np.exp(-1 + v / 10))
     Afcas = 1 - Afcaf
     dfcaf_dt = (-fcaf + fcass) / tfcaf
     dfcaf_dt_linearized = -1 / tfcaf
-    states[4] = (
-        -1 + np.exp(dt * dfcaf_dt_linearized)
-    ) * dfcaf_dt / dfcaf_dt_linearized + fcaf
+    states[4] = (-1 + np.exp(dt * dfcaf_dt_linearized)) * dfcaf_dt / dfcaf_dt_linearized + fcaf
     dfcas_dt = (-fcas + fcass) / tfcas
     dfcas_dt_linearized = -1 / tfcas
-    states[5] = (
-        -1 + np.exp(dt * dfcas_dt_linearized)
-    ) * dfcas_dt / dfcas_dt_linearized + fcas
+    states[5] = (-1 + np.exp(dt * dfcas_dt_linearized)) * dfcas_dt / dfcas_dt_linearized + fcas
     fca = Afcaf * fcaf + Afcas * fcas
     jcass = 1.0 / (1.0 + 649.7401897235336 * np.exp(0.35821750967187277 * v))
     djca_dt = (-jca + jcass) / tjca
     djca_dt_linearized = -1 / tjca
-    states[6] = (
-        -1 + np.exp(dt * djca_dt_linearized)
-    ) * djca_dt / djca_dt_linearized + jca
+    states[6] = (-1 + np.exp(dt * djca_dt_linearized)) * djca_dt / djca_dt_linearized + jca
     tffp = 2.5 * tff
     dffp_dt = (-ffp + fss) / tffp
     dffp_dt_linearized = -1 / tffp
-    states[7] = (
-        -1 + np.exp(dt * dffp_dt_linearized)
-    ) * dffp_dt / dffp_dt_linearized + ffp
+    states[7] = (-1 + np.exp(dt * dffp_dt_linearized)) * dffp_dt / dffp_dt_linearized + ffp
     fp = Aff * ffp + Afs * fs
     tfcafp = 2.5 * tfcaf
     dfcafp_dt = (-fcafp + fcass) / tfcafp
     dfcafp_dt_linearized = -1 / tfcafp
-    states[8] = (
-        -1 + np.exp(dt * dfcafp_dt_linearized)
-    ) * dfcafp_dt / dfcafp_dt_linearized + fcafp
+    states[8] = (-1 + np.exp(dt * dfcafp_dt_linearized)) * dfcafp_dt / dfcafp_dt_linearized + fcafp
     fcap = Afcaf * fcafp + Afcas * fcas
     km2n = jca
     anca_ss = 1.0 / (np.power(1 + Kmn / cass, 4) + k2n / km2n)
     dnca_ss_dt = k2n * anca_ss - km2n * nca_ss
     dnca_ss_dt_linearized = -km2n
     states[9] = (
         np.where(
             np.abs(dnca_ss_dt_linearized) > 1e-08,
-            (-1 + np.exp(dt * dnca_ss_dt_linearized))
-            * dnca_ss_dt
-            / dnca_ss_dt_linearized,
+            (-1 + np.exp(dt * dnca_ss_dt_linearized)) * dnca_ss_dt / dnca_ss_dt_linearized,
             dt * dnca_ss_dt,
         )
         + nca_ss
     )
     Io = 0.0005 * clo + 0.0005 * ko + 0.0005 * nao + 0.002 * cao
     Iss = 0.0005 * clss + 0.0005 * kss + 0.0005 * nass + 0.002 * cass
     constA = 1820000.0 * np.power(T * dielConstant, -1.5)
@@ -4189,25 +3941,17 @@
     gamma_ko = np.exp(-(-0.3 * Io + np.sqrt(Io) / (1 + np.sqrt(Io))) * constA)
     PhiCaL_ss = (
         4
         * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_ss = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_ss = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
-    )
-    PCa = np.where(
-        celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b)
-    )
+    PhiCaNa_ss = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_ss = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * vffrt / (-1 + np.exp(vfrt))
+    PCa = np.where(celltype == 1, 1.2 * PCa_b, np.where(celltype == 2, 2 * PCa_b, PCa_b))
     PCap = 1.1 * PCa
     PCaNa = 0.00125 * PCa
     PCaK = 0.0003574 * PCa
     PCaNap = 0.00125 * PCap
     PCaKp = 0.0003574 * PCap
     fICaLp = 1.0 / (1 + KmCaMK / CaMKa)
     ICaL_ss = ICaL_fractionSS * (
@@ -4239,22 +3983,16 @@
     gamma_ki = np.exp(-(-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     PhiCaL_i = (
         4
         * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    PhiCaNa_i = (
-        (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai)
-        * vffrt
-        / (-1 + np.exp(vfrt))
-    )
-    PhiCaK_i = (
-        (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
-    )
+    PhiCaNa_i = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * vffrt / (-1 + np.exp(vfrt))
+    PhiCaK_i = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * vffrt / (-1 + np.exp(vfrt))
     ICaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * PhiCaL_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * PhiCaL_i * d * fICaLp
     )
     ICaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * PhiCaNa_i * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * PhiCaNa_i * d * fICaLp
@@ -4299,17 +4037,15 @@
     dm_dt = (-m + mss) / tm
     dm_dt_linearized = -1 / tm
     states[11] = (-1 + np.exp(dt * dm_dt_linearized)) * dm_dt / dm_dt_linearized + m
     hss = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * v))
     )
-    ah = np.where(
-        v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v)
-    )
+    ah = np.where(v >= -40, 0, 4.4312679295805147e-07 * np.exp(-0.14705882352941177 * v))
     bh = np.where(
         v >= -40,
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * v)),
         310000.0 * np.exp(0.3485 * v) + 2.7 * np.exp(0.079 * v),
     )
     th = 1.0 / (ah + bh)
     dh_dt = (-h + hss) / th
@@ -4321,17 +4057,15 @@
         (37.78 + v)
         * (-25428.0 * np.exp(0.2444 * v) - 6.948e-06 * np.exp(-0.04391 * v))
         / (1 + 50262745825.95399 * np.exp(0.311 * v)),
     )
     bj = np.where(
         v >= -40,
         0.6 * np.exp(0.057 * v) / (1 + 0.040762203978366204 * np.exp(-0.1 * v)),
-        0.02424
-        * np.exp(-0.01052 * v)
-        / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
+        0.02424 * np.exp(-0.01052 * v) / (1 + 0.003960868339904256 * np.exp(-0.1378 * v)),
     )
     jss = hss
     tj = 1.0 / (aj + bj)
     dj_dt = (-j + jss) / tj
     dj_dt_linearized = -1 / tj
     states[13] = (-1 + np.exp(dt * dj_dt_linearized)) * dj_dt / dj_dt_linearized + j
     hssp = 1.0 / (
@@ -4368,105 +4102,79 @@
     dhL_dt = (-hL + hLss) / thL
     dhL_dt_linearized = -1 / thL
     states[17] = (-1 + np.exp(dt * dhL_dt_linearized)) * dhL_dt / dhL_dt_linearized + hL
     hLssp = 1.0 / (1 + 275969.2903869871 * np.exp(0.13354700854700854 * v))
     thLp = 3 * thL
     dhLp_dt = (-hLp + hLssp) / thLp
     dhLp_dt_linearized = -1 / thLp
-    states[18] = (
-        -1 + np.exp(dt * dhLp_dt_linearized)
-    ) * dhLp_dt / dhLp_dt_linearized + hLp
+    states[18] = (-1 + np.exp(dt * dhLp_dt_linearized)) * dhLp_dt / dhLp_dt_linearized + hLp
     GNaL = np.where(celltype == 1, 0.6 * GNaL_b, GNaL_b)
     fINaLp = 1.0 / (1 + KmCaMK / CaMKa)
     INaL = (-ENa + v) * ((1 - fINaLp) * hL + fINaLp * hLp) * GNaL * mL
 
     # Expressions for the Ito component
     ass = 1.0 / (
-        1
-        + 2.6316508161673635
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 2.6316508161673635 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     ta = 1.0515 / (
         1.0
         / (
             1.2089
-            + 2.2621017070578837
-            * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
+            + 2.2621017070578837 * np.exp(-0.03403513787634354 * EKshift - 0.03403513787634354 * v)
         )
         + 3.5
-        / (
-            1
-            + 30.069572727397507
-            * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v)
-        )
+        / (1 + 30.069572727397507 * np.exp(0.03403513787634354 * EKshift + 0.03403513787634354 * v))
     )
     da_dt = (-a + ass) / ta
     da_dt_linearized = -1 / ta
     states[19] = (-1 + np.exp(dt * da_dt_linearized)) * da_dt / da_dt_linearized + a
     iss = 1.0 / (
-        1
-        + 2194.970764538301
-        * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
-    )
-    delta_epi = np.where(
-        celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1
+        1 + 2194.970764538301 * np.exp(0.17510068289266328 * EKshift + 0.17510068289266328 * v)
     )
+    delta_epi = np.where(celltype == 1, 1 - 0.95 / (1 + np.exp(14 + EKshift / 5 + v / 5)), 1)
     tiF_b = 4.562 + 1.0 / (
         0.3933 * np.exp(-1 - EKshift / 100 - v / 100)
-        + 1.6300896349780942
-        * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
+        + 1.6300896349780942 * np.exp(0.06027727546714889 * EKshift + 0.06027727546714889 * v)
     )
     tiS_b = 23.62 + 1.0 / (
-        0.00027617763953377436
-        * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
-        + 0.024208962804604526
-        * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
+        0.00027617763953377436 * np.exp(-0.01693480101608806 * EKshift - 0.01693480101608806 * v)
+        + 0.024208962804604526 * np.exp(0.12377769525931426 * EKshift + 0.12377769525931426 * v)
     )
     tiF = delta_epi * tiF_b
     tiS = delta_epi * tiS_b
     AiF = 1.0 / (
-        1
-        + 0.24348537187522867
-        * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
+        1 + 0.24348537187522867 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
     )
     AiS = 1 - AiF
     diF_dt = (-iF + iss) / tiF
     diF_dt_linearized = -1 / tiF
     states[20] = (-1 + np.exp(dt * diF_dt_linearized)) * diF_dt / diF_dt_linearized + iF
     diS_dt = (-iS + iss) / tiS
     diS_dt_linearized = -1 / tiS
     states[21] = (-1 + np.exp(dt * diS_dt_linearized)) * diS_dt / diS_dt_linearized + iS
     i = AiF * iF + AiS * iS
     assp = 1.0 / (
-        1
-        + 5.167428462230666
-        * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
+        1 + 5.167428462230666 * np.exp(-0.06747638326585695 * EKshift - 0.06747638326585695 * v)
     )
     dap_dt = (-ap + assp) / ta
     dap_dt_linearized = -1 / ta
     states[22] = (-1 + np.exp(dt * dap_dt_linearized)) * dap_dt / dap_dt_linearized + ap
     dti_develop = 1.354 + 0.0001 / (
-        2.6591269045230603e-05
-        * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
-        + 4.5541779737128264e24
-        * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
+        2.6591269045230603e-05 * np.exp(0.06293266205160478 * EKshift + 0.06293266205160478 * v)
+        + 4.5541779737128264e24 * np.exp(-4.642525533890436 * EKshift - 4.642525533890436 * v)
     )
     dti_recover = 1 - 0.5 / (1 + 33.11545195869231 * np.exp(0.05 * EKshift + 0.05 * v))
     tiFp = dti_develop * dti_recover * tiF
     tiSp = dti_develop * dti_recover * tiS
     diFp_dt = (-iFp + iss) / tiFp
     diFp_dt_linearized = -1 / tiFp
-    states[23] = (
-        -1 + np.exp(dt * diFp_dt_linearized)
-    ) * diFp_dt / diFp_dt_linearized + iFp
+    states[23] = (-1 + np.exp(dt * diFp_dt_linearized)) * diFp_dt / diFp_dt_linearized + iFp
     diSp_dt = (-iSp + iss) / tiSp
     diSp_dt_linearized = -1 / tiSp
-    states[24] = (
-        -1 + np.exp(dt * diSp_dt_linearized)
-    ) * diSp_dt / diSp_dt_linearized + iSp
+    states[24] = (-1 + np.exp(dt * diSp_dt_linearized)) * diSp_dt / diSp_dt_linearized + iSp
     ip = AiF * iFp + AiS * iSp
     Gto = np.where(celltype == 1, 2 * Gto_b, np.where(celltype == 2, 2 * Gto_b, Gto_b))
     fItop = 1.0 / (1 + KmCaMK / CaMKa)
     Ito = (-EK + v) * ((1 - fItop) * a * i + ap * fItop * ip) * Gto
 
     # Expressions for the IKr component
     alpha = 0.1161 * np.exp(0.299 * vfrt)
@@ -4487,20 +4195,15 @@
     dC2_dt = beta_1 * C1 + C3 * alpha - (alpha_1 + beta) * C2
     dC2_dt_linearized = -alpha_1 - beta
     states[26] = C2 + np.where(
         np.abs(dC2_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dC2_dt_linearized)) * dC2_dt / dC2_dt_linearized,
         dt * dC2_dt,
     )
-    dC1_dt = (
-        alpha_1 * C2
-        + I * beta_ItoC2
-        + O * beta_2
-        - (beta_1 + alpha_2 + alpha_C2ToI) * C1
-    )
+    dC1_dt = alpha_1 * C2 + I * beta_ItoC2 + O * beta_2 - (beta_1 + alpha_2 + alpha_C2ToI) * C1
     dC1_dt_linearized = -beta_1 - alpha_2 - alpha_C2ToI
     states[27] = C1 + np.where(
         np.abs(dC1_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dC1_dt_linearized)) * dC1_dt / dC1_dt_linearized,
         dt * dC1_dt,
     )
     dO_dt = C1 * alpha_2 + I * beta_i - (alpha_i + beta_2) * O
@@ -4513,53 +4216,43 @@
     dI_dt = C1 * alpha_C2ToI + O * alpha_i - (beta_ItoC2 + beta_i) * I
     dI_dt_linearized = -beta_ItoC2 - beta_i
     states[29] = I + np.where(
         np.abs(dI_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dI_dt_linearized)) * dI_dt / dI_dt_linearized,
         dt * dI_dt,
     )
-    GKr = np.where(
-        celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b)
-    )
+    GKr = np.where(celltype == 1, 1.3 * GKr_b, np.where(celltype == 2, 0.8 * GKr_b, GKr_b))
     IKr = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GKr * O / 5
 
     # Expressions for the IKs component
     xs1ss = 1.0 / (1 + 0.27288596035656526 * np.exp(-0.11195700850873264 * v))
     txs1 = 817.3 + 1.0 / (
         0.003504067763074858 * np.exp(0.056179775280898875 * v)
         + 0.001292 * np.exp(-21 / 23 - v / 230)
     )
     dxs1_dt = (-xs1 + xs1ss) / txs1
     dxs1_dt_linearized = -1 / txs1
-    states[30] = (
-        -1 + np.exp(dt * dxs1_dt_linearized)
-    ) * dxs1_dt / dxs1_dt_linearized + xs1
+    states[30] = (-1 + np.exp(dt * dxs1_dt_linearized)) * dxs1_dt / dxs1_dt_linearized + xs1
     xs2ss = xs1ss
-    txs2 = 1.0 / (
-        0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20)
-    )
+    txs2 = 1.0 / (0.0022561357010639103 * np.exp(-v / 31) + 0.01 * np.exp(-5 / 2 + v / 20))
     dxs2_dt = (-xs2 + xs2ss) / txs2
     dxs2_dt_linearized = -1 / txs2
-    states[31] = (
-        -1 + np.exp(dt * dxs2_dt_linearized)
-    ) * dxs2_dt / dxs2_dt_linearized + xs2
+    states[31] = (-1 + np.exp(dt * dxs2_dt_linearized)) * dxs2_dt / dxs2_dt_linearized + xs2
     KsCa = 1 + 0.6 / (1 + 6.481821026062645e-07 * np.power(1.0 / cai, 1.4))
     GKs = np.where(celltype == 1, 1.4 * GKs_b, GKs_b)
     IKs = (-EKs + v) * GKs * KsCa * xs1 * xs2
 
     # Expressions for the IK1 component
     aK1 = 4.094 / (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
     bK1 = (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
     ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     K1ss = aK1 / (aK1 + bK1)
-    GK1 = np.where(
-        celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b)
-    )
+    GK1 = np.where(celltype == 1, 1.2 * GK1_b, np.where(celltype == 2, 1.3 * GK1_b, GK1_b))
     IK1 = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 * K1ss / 5
 
     # Expressions for the IKb component
     xkb = 1.0 / (1 + 1.57503502085457 * np.exp(-0.04168907454423419 * v))
     GKb = np.where(celltype == 1, 0.6 * GKb_b, GKb_b)
     IKb = (-EK + v) * GKb * xkb
 
@@ -4603,17 +4296,15 @@
     fJrelp = 1.0 / (1 + KmCaMK / CaMKa)
     Jrel = Jrel_b * ((1 - fJrelp) * Jrel_np + Jrel_p * fJrelp)
 
     # Expressions for the Membrane component
     Istim = np.where(
         np.logical_and(
             t >= i_Stim_Start,
-            t
-            - i_Stim_Start
-            - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
+            t - i_Stim_Start - i_Stim_Period * np.floor((t - i_Stim_Start) / i_Stim_Period)
             <= i_Stim_PulseDuration,
         ),
         i_Stim_Amplitude,
         0,
     )
     dv_dt = (
         -ICaK
@@ -4634,17 +4325,15 @@
         - INab
         - I_katp
         - IpCa
         - Istim
         - Ito
     )
     dAfcaf_dv = (
-        -0.06
-        * np.exp(-1 + v / 10)
-        / ((1 + np.exp(-1 + v / 10)) * (1 + np.exp(-1 + v / 10)))
+        -0.06 * np.exp(-1 + v / 10) / ((1 + np.exp(-1 + v / 10)) * (1 + np.exp(-1 + v / 10)))
     )
     dAiF_dv = (
         -0.0016103529885927823
         * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
         / (
             (
                 1
@@ -4654,171 +4343,122 @@
             * (
                 1
                 + 0.24348537187522867
                 * np.exp(0.006613756613756614 * EKshift + 0.006613756613756614 * v)
             )
         )
     )
-    dE1_dx1 = 1.0 / (x1 + x2 + x3 + x4) - x1 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE1_dx1 = 1.0 / (x1 + x2 + x3 + x4) - x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_dx2 = -x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_dx3 = -x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_dx4 = -x1 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE1_i_dx1_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x1_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
     dE1_i_dx2_i = -x1_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE1_i_dx3_i = -x1_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE1_i_dx4_i = -x1_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE1_ss_dx1_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x1_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
-    dE1_ss_dx2_ss = -x1_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE1_ss_dx3_ss = -x1_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE1_ss_dx4_ss = -x1_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE1_ss_dx2_ss = -x1_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE1_ss_dx3_ss = -x1_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE1_ss_dx4_ss = -x1_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE2_dx1 = -x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
-    dE2_dx2 = 1.0 / (x1 + x2 + x3 + x4) - x2 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE2_dx2 = 1.0 / (x1 + x2 + x3 + x4) - x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE2_dx3 = -x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE2_dx4 = -x2 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE2_i_dx1_i = -x2_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE2_i_dx2_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x2_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
     dE2_i_dx3_i = -x2_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE2_i_dx4_i = -x2_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
-    dE2_ss_dx1_ss = -x2_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE2_ss_dx1_ss = -x2_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE2_ss_dx2_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x2_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
-    dE2_ss_dx3_ss = -x2_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE2_ss_dx4_ss = -x2_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE2_ss_dx3_ss = -x2_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE2_ss_dx4_ss = -x2_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE3_dx1 = -x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE3_dx2 = -x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
-    dE3_dx3 = 1.0 / (x1 + x2 + x3 + x4) - x3 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE3_dx3 = 1.0 / (x1 + x2 + x3 + x4) - x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE3_dx4 = -x3 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE3_i_dx1_i = -x3_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE3_i_dx2_i = -x3_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE3_i_dx3_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x3_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
     dE3_i_dx4_i = -x3_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
-    dE3_ss_dx1_ss = -x3_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE3_ss_dx2_ss = -x3_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE3_ss_dx1_ss = -x3_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE3_ss_dx2_ss = -x3_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE3_ss_dx3_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x3_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
-    dE3_ss_dx4_ss = -x3_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE3_ss_dx4_ss = -x3_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE4_dx1 = -x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE4_dx2 = -x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE4_dx3 = -x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
-    dE4_dx4 = 1.0 / (x1 + x2 + x3 + x4) - x4 / (
-        (x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4)
-    )
+    dE4_dx4 = 1.0 / (x1 + x2 + x3 + x4) - x4 / ((x1 + x2 + x3 + x4) * (x1 + x2 + x3 + x4))
     dE4_i_dx1_i = -x4_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE4_i_dx2_i = -x4_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE4_i_dx3_i = -x4_i / ((x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i))
     dE4_i_dx4_i = 1.0 / (x1_i + x2_i + x3_i + x4_i) - x4_i / (
         (x1_i + x2_i + x3_i + x4_i) * (x1_i + x2_i + x3_i + x4_i)
     )
-    dE4_ss_dx1_ss = -x4_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE4_ss_dx2_ss = -x4_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
-    dE4_ss_dx3_ss = -x4_ss / (
-        (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
-    )
+    dE4_ss_dx1_ss = -x4_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE4_ss_dx2_ss = -x4_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
+    dE4_ss_dx3_ss = -x4_ss / ((x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss))
     dE4_ss_dx4_ss = 1.0 / (x1_ss + x2_ss + x3_ss + x4_ss) - x4_ss / (
         (x1_ss + x2_ss + x3_ss + x4_ss) * (x1_ss + x2_ss + x3_ss + x4_ss)
     )
     dICaK_i_dPhiCaK_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaK * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaKp * d * fICaLp
     )
-    dICaK_i_dfca = (
-        (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaK * PhiCaK_i * d * jca * nca_i
-    )
+    dICaK_i_dfca = (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaK * PhiCaK_i * d * jca * nca_i
     dICaK_i_dfcap = (1 - ICaL_fractionSS) * PCaKp * PhiCaK_i * d * fICaLp * jca * nca_i
     dICaK_ss_dPhiCaK_ss = ICaL_fractionSS * (
         (1 - fICaLp) * ((1 - nca_ss) * f + fca * jca * nca_ss) * PCaK * d
         + ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCaKp * d * fICaLp
     )
     dICaK_ss_dfca = ICaL_fractionSS * (1 - fICaLp) * PCaK * PhiCaK_ss * d * jca * nca_ss
     dICaK_ss_dfcap = ICaL_fractionSS * PCaKp * PhiCaK_ss * d * fICaLp * jca * nca_ss
     dICaL_i_dPhiCaL_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCa * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCap * d * fICaLp
     )
-    dICaL_i_dfca = (
-        (1 - ICaL_fractionSS) * (1 - fICaLp) * PCa * PhiCaL_i * d * jca * nca_i
-    )
+    dICaL_i_dfca = (1 - ICaL_fractionSS) * (1 - fICaLp) * PCa * PhiCaL_i * d * jca * nca_i
     dICaL_i_dfcap = (1 - ICaL_fractionSS) * PCap * PhiCaL_i * d * fICaLp * jca * nca_i
     dICaL_ss_dPhiCaL_ss = ICaL_fractionSS * (
         (1 - fICaLp) * ((1 - nca_ss) * f + fca * jca * nca_ss) * PCa * d
         + ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCap * d * fICaLp
     )
     dICaL_ss_dfca = ICaL_fractionSS * (1 - fICaLp) * PCa * PhiCaL_ss * d * jca * nca_ss
     dICaL_ss_dfcap = ICaL_fractionSS * PCap * PhiCaL_ss * d * fICaLp * jca * nca_ss
     dICaNa_i_dPhiCaNa_i = (1 - ICaL_fractionSS) * (
         (1 - fICaLp) * ((1 - nca_i) * f + fca * jca * nca_i) * PCaNa * d
         + ((1 - nca_i) * fp + fcap * jca * nca_i) * PCaNap * d * fICaLp
     )
-    dICaNa_i_dfca = (
-        (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaNa * PhiCaNa_i * d * jca * nca_i
-    )
-    dICaNa_i_dfcap = (
-        (1 - ICaL_fractionSS) * PCaNap * PhiCaNa_i * d * fICaLp * jca * nca_i
-    )
+    dICaNa_i_dfca = (1 - ICaL_fractionSS) * (1 - fICaLp) * PCaNa * PhiCaNa_i * d * jca * nca_i
+    dICaNa_i_dfcap = (1 - ICaL_fractionSS) * PCaNap * PhiCaNa_i * d * fICaLp * jca * nca_i
     dICaNa_ss_dPhiCaNa_ss = ICaL_fractionSS * (
         (1 - fICaLp) * ((1 - nca_ss) * f + fca * jca * nca_ss) * PCaNa * d
         + ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCaNap * d * fICaLp
     )
-    dICaNa_ss_dfca = (
-        ICaL_fractionSS * (1 - fICaLp) * PCaNa * PhiCaNa_ss * d * jca * nca_ss
-    )
+    dICaNa_ss_dfca = ICaL_fractionSS * (1 - fICaLp) * PCaNa * PhiCaNa_ss * d * jca * nca_ss
     dICaNa_ss_dfcap = ICaL_fractionSS * PCaNap * PhiCaNa_ss * d * fICaLp * jca * nca_ss
     dICab_dvffrt = (
-        4
-        * PCab
-        * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
-        / (-1 + np.exp(2 * vfrt))
+        4 * PCab * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) / (-1 + np.exp(2 * vfrt))
     )
-    dICab_dvfrt = -8 * PCab * (
-        -cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai
-    ) * np.exp(2 * vfrt) * vffrt / (
-        (-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))
-    ) + 8 * PCab * cai * np.exp(
+    dICab_dvfrt = -8 * PCab * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) * np.exp(
         2 * vfrt
-    ) * gamma_cai * vffrt / (
-        -1 + np.exp(2 * vfrt)
-    )
+    ) * vffrt / ((-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))) + 8 * PCab * cai * np.exp(
+        2 * vfrt
+    ) * gamma_cai * vffrt / (-1 + np.exp(2 * vfrt))
     dIClCa_junc_dv = Fjunc * GClCa / (1 + KdClCa / cass)
     dIClCa_sl_dv = GClCa * (1 - Fjunc) / (1 + KdClCa / cai)
     dIK1_dK1ss = np.sqrt(5) * np.sqrt(ko) * (-EK + v) * GK1 / 5
     dK1ss_daK1 = 1.0 / (aK1 + bK1) - aK1 / ((aK1 + bK1) * (aK1 + bK1))
     dK1ss_dbK1 = -aK1 / ((aK1 + bK1) * (aK1 + bK1))
     daK1_dv = (
         -0.0011435228161993972
@@ -4827,22 +4467,18 @@
             (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
             * (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
         )
     )
     dbK1_dv = (
         6.919349479611957e-18 * np.exp(0.0618 * v - 0.0618 * EK)
         + 0.8506978434250505 * np.exp(0.0674 * v - 0.0674 * EK)
-    ) / (
-        1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)
-    ) + 0.016099950792318272 * (
+    ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)) + 0.016099950792318272 * (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
-    ) * np.exp(
-        0.1629 * EK - 0.1629 * v
-    ) / (
+    ) * np.exp(0.1629 * EK - 0.1629 * v) / (
         (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
         * (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     )
     dIK1_dv = (
         np.sqrt(5) * np.sqrt(ko) * GK1 * K1ss / 5
         + np.sqrt(5)
         * np.sqrt(ko)
@@ -4896,132 +4532,67 @@
         - 3 * (dE2_dx2 * dx2_da3 + dE2_dx3 * dx3_da3 + a1 * a4 * dE2_dx4) * b3
         + 3 * (dE1_dx2 * dx2_da3 + dE1_dx3 * dx3_da3 + a1 * a4 * dE1_dx4) * a3
     )
     dx3_i_dk3_i = (k6_i + k7_i) * k1_i + k6_i * k8_i
     dx4_i_dk3_i = (k1_i + k8_i) * k5_i
     dJncxNa_i_dk3pp_i = (
         -E2_i
-        + (
-            dE3_i_dx3_i * dx3_i_dk3_i
-            + dE3_i_dx4_i * dx4_i_dk3_i
-            + dE3_i_dx1_i * k5_i * k7_i
-        )
+        + (dE3_i_dx3_i * dx3_i_dk3_i + dE3_i_dx4_i * dx4_i_dk3_i + dE3_i_dx1_i * k5_i * k7_i)
         * k4pp_i
-        - (
-            dE2_i_dx3_i * dx3_i_dk3_i
-            + dE2_i_dx4_i * dx4_i_dk3_i
-            + dE2_i_dx1_i * k5_i * k7_i
-        )
+        - (dE2_i_dx3_i * dx3_i_dk3_i + dE2_i_dx4_i * dx4_i_dk3_i + dE2_i_dx1_i * k5_i * k7_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx3_i * dx3_i_dk3_i
-            + dE1_i_dx4_i * dx4_i_dk3_i
-            + dE1_i_dx1_i * k5_i * k7_i
-        )
+        * (dE1_i_dx3_i * dx3_i_dk3_i + dE1_i_dx4_i * dx4_i_dk3_i + dE1_i_dx1_i * k5_i * k7_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx3_i * dx3_i_dk3_i
-            + dE4_i_dx4_i * dx4_i_dk3_i
-            + dE4_i_dx1_i * k5_i * k7_i
-        )
+        * (dE4_i_dx3_i * dx3_i_dk3_i + dE4_i_dx4_i * dx4_i_dk3_i + dE4_i_dx1_i * k5_i * k7_i)
         * k7_i
     )
     dx1_i_dk4_i = (k6_i + k7_i) * k2_i
     dx2_i_dk4_i = (k1_i + k8_i) * k6_i + k1_i * k7_i
     dJncxNa_i_dk4pp_i = (
-        (
-            dE3_i_dx1_i * dx1_i_dk4_i
-            + dE3_i_dx2_i * dx2_i_dk4_i
-            + dE3_i_dx4_i * k2_i * k8_i
-        )
-        * k4pp_i
-        - (
-            dE2_i_dx1_i * dx1_i_dk4_i
-            + dE2_i_dx2_i * dx2_i_dk4_i
-            + dE2_i_dx4_i * k2_i * k8_i
-        )
+        (dE3_i_dx1_i * dx1_i_dk4_i + dE3_i_dx2_i * dx2_i_dk4_i + dE3_i_dx4_i * k2_i * k8_i) * k4pp_i
+        - (dE2_i_dx1_i * dx1_i_dk4_i + dE2_i_dx2_i * dx2_i_dk4_i + dE2_i_dx4_i * k2_i * k8_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx1_i * dx1_i_dk4_i
-            + dE1_i_dx2_i * dx2_i_dk4_i
-            + dE1_i_dx4_i * k2_i * k8_i
-        )
+        * (dE1_i_dx1_i * dx1_i_dk4_i + dE1_i_dx2_i * dx2_i_dk4_i + dE1_i_dx4_i * k2_i * k8_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx1_i * dx1_i_dk4_i
-            + dE4_i_dx2_i * dx2_i_dk4_i
-            + dE4_i_dx4_i * k2_i * k8_i
-        )
+        * (dE4_i_dx1_i * dx1_i_dk4_i + dE4_i_dx2_i * dx2_i_dk4_i + dE4_i_dx4_i * k2_i * k8_i)
         * k7_i
         + E3_i
     )
     dx1_i_dk7_i = (k2_i + k3_i) * k5_i + k2_i * k4_i
     dx2_i_dk7_i = (k4_i + k5_i) * k1_i
     dJncxNa_i_dk7_i = (
         3 * E4_i
-        + (
-            dE3_i_dx1_i * dx1_i_dk7_i
-            + dE3_i_dx2_i * dx2_i_dk7_i
-            + dE3_i_dx3_i * k1_i * k3_i
-        )
+        + (dE3_i_dx1_i * dx1_i_dk7_i + dE3_i_dx2_i * dx2_i_dk7_i + dE3_i_dx3_i * k1_i * k3_i)
         * k4pp_i
-        - (
-            dE2_i_dx1_i * dx1_i_dk7_i
-            + dE2_i_dx2_i * dx2_i_dk7_i
-            + dE2_i_dx3_i * k1_i * k3_i
-        )
+        - (dE2_i_dx1_i * dx1_i_dk7_i + dE2_i_dx2_i * dx2_i_dk7_i + dE2_i_dx3_i * k1_i * k3_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx1_i * dx1_i_dk7_i
-            + dE1_i_dx2_i * dx2_i_dk7_i
-            + dE1_i_dx3_i * k1_i * k3_i
-        )
+        * (dE1_i_dx1_i * dx1_i_dk7_i + dE1_i_dx2_i * dx2_i_dk7_i + dE1_i_dx3_i * k1_i * k3_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx1_i * dx1_i_dk7_i
-            + dE4_i_dx2_i * dx2_i_dk7_i
-            + dE4_i_dx3_i * k1_i * k3_i
-        )
+        * (dE4_i_dx1_i * dx1_i_dk7_i + dE4_i_dx2_i * dx2_i_dk7_i + dE4_i_dx3_i * k1_i * k3_i)
         * k7_i
     )
     dx3_i_dk8_i = (k2_i + k3_i) * k6_i
     dx4_i_dk8_i = (k4_i + k5_i) * k2_i + k3_i * k5_i
     dJncxNa_i_dk8_i = (
         -3 * E1_i
-        + (
-            dE3_i_dx3_i * dx3_i_dk8_i
-            + dE3_i_dx4_i * dx4_i_dk8_i
-            + dE3_i_dx2_i * k4_i * k6_i
-        )
+        + (dE3_i_dx3_i * dx3_i_dk8_i + dE3_i_dx4_i * dx4_i_dk8_i + dE3_i_dx2_i * k4_i * k6_i)
         * k4pp_i
-        - (
-            dE2_i_dx3_i * dx3_i_dk8_i
-            + dE2_i_dx4_i * dx4_i_dk8_i
-            + dE2_i_dx2_i * k4_i * k6_i
-        )
+        - (dE2_i_dx3_i * dx3_i_dk8_i + dE2_i_dx4_i * dx4_i_dk8_i + dE2_i_dx2_i * k4_i * k6_i)
         * k3pp_i
         - 3
-        * (
-            dE1_i_dx3_i * dx3_i_dk8_i
-            + dE1_i_dx4_i * dx4_i_dk8_i
-            + dE1_i_dx2_i * k4_i * k6_i
-        )
+        * (dE1_i_dx3_i * dx3_i_dk8_i + dE1_i_dx4_i * dx4_i_dk8_i + dE1_i_dx2_i * k4_i * k6_i)
         * k8_i
         + 3
-        * (
-            dE4_i_dx3_i * dx3_i_dk8_i
-            + dE4_i_dx4_i * dx4_i_dk8_i
-            + dE4_i_dx2_i * k4_i * k6_i
-        )
+        * (dE4_i_dx3_i * dx3_i_dk8_i + dE4_i_dx4_i * dx4_i_dk8_i + dE4_i_dx2_i * k4_i * k6_i)
         * k7_i
     )
     dx3_ss_dk3_ss = (k6_ss + k7_ss) * k1_ss + k6_ss * k8_ss
     dx4_ss_dk3_ss = (k1_ss + k8_ss) * k5_ss
     dJncxNa_ss_dk3pp_ss = (
         -E2_ss
         + (
@@ -5142,82 +4713,50 @@
             + dE4_ss_dx4_ss * dx4_ss_dk8_ss
             + dE4_ss_dx2_ss * k4_ss * k6_ss
         )
         * k7_ss
     )
     dKnai_dvfrt = Knai0 * delta * np.exp(delta * vfrt / 3) / 3
     dKnao_dvfrt = Knao0 * (1 / 3 - delta / 3) * np.exp((1 - delta) * vfrt / 3)
-    dPhiCaK_i_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaK_i_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * np.exp(
-        vfrt
-    ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
-        vfrt
-    ) * gamma_ki * ki * vffrt / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaK_ss_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaK_ss_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * np.exp(
-        vfrt
-    ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
-        vfrt
-    ) * gamma_kss * kss * vffrt / (
-        -1 + np.exp(vfrt)
-    )
+    dPhiCaK_i_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) / (-1 + np.exp(vfrt))
+    dPhiCaK_i_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_ki * ki) * np.exp(vfrt) * vffrt / (
+        (-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))
+    ) + np.exp(vfrt) * gamma_ki * ki * vffrt / (-1 + np.exp(vfrt))
+    dPhiCaK_ss_dvffrt = (-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) / (-1 + np.exp(vfrt))
+    dPhiCaK_ss_dvfrt = -(-ko * gamma_ko + np.exp(vfrt) * gamma_kss * kss) * np.exp(vfrt) * vffrt / (
+        (-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))
+    ) + np.exp(vfrt) * gamma_kss * kss * vffrt / (-1 + np.exp(vfrt))
     dPhiCaL_i_dvffrt = (
-        4
-        * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai)
-        / (-1 + np.exp(2 * vfrt))
+        4 * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) / (-1 + np.exp(2 * vfrt))
     )
-    dPhiCaL_i_dvfrt = -8 * (
-        -cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai
-    ) * np.exp(2 * vfrt) * vffrt / (
-        (-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))
-    ) + 8 * cai * np.exp(
+    dPhiCaL_i_dvfrt = -8 * (-cao * gamma_cao + cai * np.exp(2 * vfrt) * gamma_cai) * np.exp(
         2 * vfrt
-    ) * gamma_cai * vffrt / (
-        -1 + np.exp(2 * vfrt)
-    )
+    ) * vffrt / ((-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))) + 8 * cai * np.exp(
+        2 * vfrt
+    ) * gamma_cai * vffrt / (-1 + np.exp(2 * vfrt))
     dPhiCaL_ss_dvffrt = (
-        4
-        * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass)
-        / (-1 + np.exp(2 * vfrt))
+        4 * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass) / (-1 + np.exp(2 * vfrt))
     )
-    dPhiCaL_ss_dvfrt = -8 * (
-        -cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass
-    ) * np.exp(2 * vfrt) * vffrt / (
-        (-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))
-    ) + 8 * cass * np.exp(
+    dPhiCaL_ss_dvfrt = -8 * (-cao * gamma_cao + cass * np.exp(2 * vfrt) * gamma_cass) * np.exp(
         2 * vfrt
-    ) * gamma_cass * vffrt / (
-        -1 + np.exp(2 * vfrt)
-    )
-    dPhiCaNa_i_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) / (
-        -1 + np.exp(vfrt)
-    )
+    ) * vffrt / ((-1 + np.exp(2 * vfrt)) * (-1 + np.exp(2 * vfrt))) + 8 * cass * np.exp(
+        2 * vfrt
+    ) * gamma_cass * vffrt / (-1 + np.exp(2 * vfrt))
+    dPhiCaNa_i_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) / (-1 + np.exp(vfrt))
     dPhiCaNa_i_dvfrt = -(-nao * gamma_nao + np.exp(vfrt) * gamma_nai * nai) * np.exp(
         vfrt
     ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
         vfrt
-    ) * gamma_nai * nai * vffrt / (
-        -1 + np.exp(vfrt)
-    )
-    dPhiCaNa_ss_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) / (
-        -1 + np.exp(vfrt)
-    )
+    ) * gamma_nai * nai * vffrt / (-1 + np.exp(vfrt))
+    dPhiCaNa_ss_dvffrt = (-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) / (-1 + np.exp(vfrt))
     dPhiCaNa_ss_dvfrt = -(-nao * gamma_nao + np.exp(vfrt) * gamma_nass * nass) * np.exp(
         vfrt
     ) * vffrt / ((-1 + np.exp(vfrt)) * (-1 + np.exp(vfrt))) + np.exp(
         vfrt
-    ) * gamma_nass * nass * vffrt / (
-        -1 + np.exp(vfrt)
-    )
+    ) * gamma_nass * nass * vffrt / (-1 + np.exp(vfrt))
     da1_dKnai = -3 * k1p * (nai * nai * nai) / (
         (
             -1
             + ((1 + ki / Kki) * (1 + ki / Kki))
             + ((1 + nai / Knai) * (1 + nai / Knai) * (1 + nai / Knai))
         )
         * np.power(Knai, 4)
@@ -5307,17 +4846,15 @@
     dfca_dAfcaf = -fcas + fcaf
     dfcap_dAfcaf = -fcas + fcafp
     dh1_i_dhna = nai / kna3
     dh1_ss_dhna = nass / kna3
     dh2_i_dh1_i = -hna * nai / (kna3 * (h1_i * h1_i))
     dh2_i_dhna = nai / (kna3 * h1_i) - dh1_i_dhna * hna * nai / (kna3 * (h1_i * h1_i))
     dh2_ss_dh1_ss = -hna * nass / (kna3 * (h1_ss * h1_ss))
-    dh2_ss_dhna = nass / (kna3 * h1_ss) - dh1_ss_dhna * hna * nass / (
-        kna3 * (h1_ss * h1_ss)
-    )
+    dh2_ss_dhna = nass / (kna3 * h1_ss) - dh1_ss_dhna * hna * nass / (kna3 * (h1_ss * h1_ss))
     dh3_i_dh1_i = -1 / (h1_i * h1_i)
     dh3_ss_dh1_ss = -1 / (h1_ss * h1_ss)
     dh7_i_dhna = -nao / (kna3 * (hna * hna))
     dh7_ss_dhna = -nao / (kna3 * (hna * hna))
     dh8_i_dh7_i = -nao / (kna3 * (h7_i * h7_i) * hna)
     dh8_i_dhna = -nao / (kna3 * h7_i * (hna * hna)) - nao * dh7_i_dhna / (
         kna3 * (h7_i * h7_i) * hna
@@ -5394,19 +4931,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5419,19 +4952,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5453,19 +4982,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -5524,19 +5049,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5549,19 +5070,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5583,19 +5100,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -5657,19 +5170,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5682,19 +5191,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5716,19 +5221,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -5787,19 +5288,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5812,19 +5309,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -5846,19 +5339,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -5889,26 +5378,20 @@
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaL_i_dfcap
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaL_ss_dfcap
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaNa_i_dfcap
         - (dAfcaf_dv * dfcap_dAfcaf - dAfcaf_dv * fcas) * dICaNa_ss_dfcap
         - (dAiF_dv * di_dAiF - dAiF_dv * iS) * dIto_di
         - (dAiF_dv * dip_dAiF - dAiF_dv * iSp) * dIto_dip
         - (dK1ss_daK1 * daK1_dv + dK1ss_dbK1 * dbK1_dv) * dIK1_dK1ss
-        - (dPhiCaK_i_dvffrt * dvffrt_dv + dPhiCaK_i_dvfrt * dvfrt_dv)
-        * dICaK_i_dPhiCaK_i
-        - (dPhiCaK_ss_dvffrt * dvffrt_dv + dPhiCaK_ss_dvfrt * dvfrt_dv)
-        * dICaK_ss_dPhiCaK_ss
-        - (dPhiCaL_i_dvffrt * dvffrt_dv + dPhiCaL_i_dvfrt * dvfrt_dv)
-        * dICaL_i_dPhiCaL_i
-        - (dPhiCaL_ss_dvffrt * dvffrt_dv + dPhiCaL_ss_dvfrt * dvfrt_dv)
-        * dICaL_ss_dPhiCaL_ss
-        - (dPhiCaNa_i_dvffrt * dvffrt_dv + dPhiCaNa_i_dvfrt * dvfrt_dv)
-        * dICaNa_i_dPhiCaNa_i
-        - (dPhiCaNa_ss_dvffrt * dvffrt_dv + dPhiCaNa_ss_dvfrt * dvfrt_dv)
-        * dICaNa_ss_dPhiCaNa_ss
+        - (dPhiCaK_i_dvffrt * dvffrt_dv + dPhiCaK_i_dvfrt * dvfrt_dv) * dICaK_i_dPhiCaK_i
+        - (dPhiCaK_ss_dvffrt * dvffrt_dv + dPhiCaK_ss_dvfrt * dvfrt_dv) * dICaK_ss_dPhiCaK_ss
+        - (dPhiCaL_i_dvffrt * dvffrt_dv + dPhiCaL_i_dvfrt * dvfrt_dv) * dICaL_i_dPhiCaL_i
+        - (dPhiCaL_ss_dvffrt * dvffrt_dv + dPhiCaL_ss_dvfrt * dvfrt_dv) * dICaL_ss_dPhiCaL_ss
+        - (dPhiCaNa_i_dvffrt * dvffrt_dv + dPhiCaNa_i_dvfrt * dvfrt_dv) * dICaNa_i_dPhiCaNa_i
+        - (dPhiCaNa_ss_dvffrt * dvffrt_dv + dPhiCaNa_ss_dvfrt * dvfrt_dv) * dICaNa_ss_dPhiCaNa_ss
         - (
             (
                 (
                     (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
@@ -5947,19 +5430,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -5972,19 +5451,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6006,19 +5481,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6077,19 +5548,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6102,19 +5569,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6136,19 +5599,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6208,19 +5667,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6233,19 +5688,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6267,19 +5718,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6339,19 +5786,15 @@
                     + (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * k2_i
                     * k8_i
                     + wna
                     * (
                         dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6364,19 +5807,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx1_i_dk4_i
                     + (
                         wnaca
                         * (
                             dh8_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_i_dhna * dh8_i_dh7_i * dhna_dvfrt * dvfrt_dv
@@ -6398,19 +5837,15 @@
                     (
                         wnaca
                         * (
                             dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_i_dhca * dvfrt_dv
-                        + dh1_i_dhna
-                        * dh3_i_dh1_i
-                        * dhna_dvfrt
-                        * dk4p_i_dh3_i
-                        * dvfrt_dv
+                        + dh1_i_dhna * dh3_i_dh1_i * dhna_dvfrt * dk4p_i_dh3_i * dvfrt_dv
                     )
                     * dx2_i_dk4_i
                     + wna
                     * (
                         dh2_i_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_i_dhna * dh2_i_dh1_i * dhna_dvfrt * dvfrt_dv
                     )
@@ -6498,19 +5933,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6523,19 +5954,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6557,19 +5984,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -6628,19 +6051,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6653,19 +6072,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6687,19 +6102,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -6759,19 +6170,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6784,19 +6191,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6818,19 +6221,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -6890,19 +6289,15 @@
                     + (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * k2_ss
                     * k8_ss
                     + wna
                     * (
                         dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6915,19 +6310,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx1_ss_dk4_ss
                     + (
                         wnaca
                         * (
                             dh8_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh7_ss_dhna * dh8_ss_dh7_ss * dhna_dvfrt * dvfrt_dv
@@ -6949,19 +6340,15 @@
                     (
                         wnaca
                         * (
                             dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                             + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                         )
                         + dhca_dvfrt * dk4p_ss_dhca * dvfrt_dv
-                        + dh1_ss_dhna
-                        * dh3_ss_dh1_ss
-                        * dhna_dvfrt
-                        * dk4p_ss_dh3_ss
-                        * dvfrt_dv
+                        + dh1_ss_dhna * dh3_ss_dh1_ss * dhna_dvfrt * dk4p_ss_dh3_ss * dvfrt_dv
                     )
                     * dx2_ss_dk4_ss
                     + wna
                     * (
                         dh2_ss_dhna * dhna_dvfrt * dvfrt_dv
                         + dh1_ss_dhna * dh2_ss_dh1_ss * dhna_dvfrt * dvfrt_dv
                     )
@@ -7162,19 +6549,15 @@
     dx4_db3 = a1 * b2 + b2 * b4
     dJnakNa_db3 = (
         -3 * E2
         - 3 * (dE2_dx1 * dx1_db3 + dE2_dx4 * dx4_db3 + b1 * b2 * dE2_dx3) * b3
         + 3 * (dE1_dx1 * dx1_db3 + dE1_dx4 * dx4_db3 + b1 * b2 * dE1_dx3) * a3
     )
     dP_dnai = -eP / (
-        Knap
-        * (
-            (1 + H / Khp + nai / Knap + ki / Kxkur)
-            * (1 + H / Khp + nai / Knap + ki / Kxkur)
-        )
+        Knap * ((1 + H / Khp + nai / Knap + ki / Kxkur) * (1 + H / Khp + nai / Knap + ki / Kxkur))
     )
     dPhiCaNa_i_dgamma_nai = np.exp(vfrt) * nai * vffrt / (-1 + np.exp(vfrt))
     dgamma_nai_dIi = (
         -(
             -0.3
             - 1 / (2 * ((1 + np.sqrt(Ii)) * (1 + np.sqrt(Ii))))
             + 1 / (2 * (1 + np.sqrt(Ii)) * np.sqrt(Ii))
@@ -7240,16 +6623,15 @@
         kna1 * kna2 * (h4_i * h4_i)
     )
     dh6_i_dh4_i = -1 / (h4_i * h4_i)
     dx2_i_dk6_i = (k1_i + k8_i) * k4_i
     dx3_i_dk6_i = (k2_i + k3_i) * k8_i + k1_i * k3_i
     dnai_dt_linearized = dJdiffNa_dnai * vss / vmyo + (
         -dINab_dnai
-        - (0.0005 * dPhiCaNa_i_dgamma_nai * dgamma_nai_dIi + dPhiCaNa_i_dnai)
-        * dICaNa_i_dPhiCaNa_i
+        - (0.0005 * dPhiCaNa_i_dgamma_nai * dgamma_nai_dIi + dPhiCaNa_i_dnai) * dICaNa_i_dPhiCaNa_i
         - dENa_dnai * dINaL_dENa
         - dENa_dnai * dINa_dENa
         - 3
         * (
             (
                 (
                     (
@@ -7555,53 +6937,45 @@
         - 3
         * zk
         * (
             dJnakK_da1 * da1_dnai
             - 2
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE3_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE3_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE3_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE3_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE3_dx4
                 + b1 * b2 * dE3_dx3 * dP_dnai * db3_dP
             )
             * a1
             + 2
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE4_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE4_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE4_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE4_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE4_dx4
                 + b1 * b2 * dE4_dx3 * dP_dnai * db3_dP
             )
             * b1
         )
         * Pnak
         - 3
         * zna
         * (
             -3
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE2_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE2_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE2_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE2_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE2_dx4
                 + b1 * b2 * dE2_dx3 * dP_dnai * db3_dP
             )
             * b3
             + 3
             * (
                 (db4_dnai * dx2_db4 + a2 * a3 * da1_dnai) * dE1_dx2
-                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3)
-                * dE1_dx1
-                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3)
-                * dE1_dx4
+                + (da1_dnai * dx1_da1 + db4_dnai * dx1_db4 + dP_dnai * db3_dP * dx1_db3) * dE1_dx1
+                + (da1_dnai * dx4_da1 + b2 * b3 * db4_dnai + dP_dnai * db3_dP * dx4_db3) * dE1_dx4
                 + b1 * b2 * dE1_dx3 * dP_dnai * db3_dP
             )
             * a3
             + dJnakNa_db3 * dP_dnai * db3_dP
         )
         * Pnak
     ) * Acap / (F * vmyo)
@@ -7626,17 +7000,15 @@
     )
     dPhiCaNa_ss_dnass = (
         (np.exp(vfrt) * gamma_nass + 0.0005 * dgamma_nass_dIss * np.exp(vfrt) * nass)
         * vffrt
         / (-1 + np.exp(vfrt))
     )
     dh1_ss_dnass = (1 + hna) / kna3
-    dh2_ss_dnass = hna / (kna3 * h1_ss) - dh1_ss_dnass * hna * nass / (
-        kna3 * (h1_ss * h1_ss)
-    )
+    dh2_ss_dnass = hna / (kna3 * h1_ss) - dh1_ss_dnass * hna * nass / (kna3 * (h1_ss * h1_ss))
     dh4_ss_dnass = (1 + nass / kna2) / kna1 + nass / (kna1 * kna2)
     dh5_ss_dh4_ss = -(nass * nass) / (kna1 * kna2 * (h4_ss * h4_ss))
     dh5_ss_dnass = 2 * nass / (kna1 * kna2 * h4_ss) - (nass * nass) * dh4_ss_dnass / (
         kna1 * kna2 * (h4_ss * h4_ss)
     )
     dh6_ss_dh4_ss = -1 / (h4_ss * h4_ss)
     dx2_ss_dk6_ss = (k1_ss + k8_ss) * k4_ss
@@ -7941,17 +7313,15 @@
                     + dh1_ss_dnass * dh3_ss_dh1_ss * dk4p_ss_dh3_ss
                 )
                 * dE4_ss_dx4_ss
                 * k2_ss
                 * k8_ss
             )
             * k7_ss
-            + wnaca
-            * (dh1_ss_dnass * dh2_ss_dh1_ss + dh2_ss_dnass)
-            * dJncxNa_ss_dk4pp_ss
+            + wnaca * (dh1_ss_dnass * dh2_ss_dh1_ss + dh2_ss_dnass) * dJncxNa_ss_dk4pp_ss
         )
         * dINaCa_ss_dJncxNa_ss
     ) * Acap / (F * vss)
     states[36] = (
         np.where(
             np.abs(dnass_dt_linearized) > 1e-08,
             (-1 + np.exp(dt * dnass_dt_linearized)) * dnass_dt / dnass_dt_linearized,
@@ -7971,22 +7341,18 @@
             (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
             * (1 + 0.0022951253918281865 * np.exp(0.1217 * v - 0.1217 * EK))
         )
     )
     dbK1_dEK = (
         -6.919349479611957e-18 * np.exp(0.0618 * v - 0.0618 * EK)
         - 0.8506978434250505 * np.exp(0.0674 * v - 0.0674 * EK)
-    ) / (
-        1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)
-    ) - 0.016099950792318272 * (
+    ) / (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v)) - 0.016099950792318272 * (
         12.621629724407278 * np.exp(0.0674 * v - 0.0674 * EK)
         + 1.1196358381249121e-16 * np.exp(0.0618 * v - 0.0618 * EK)
-    ) * np.exp(
-        0.1629 * EK - 0.1629 * v
-    ) / (
+    ) * np.exp(0.1629 * EK - 0.1629 * v) / (
         (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
         * (1 + 0.09883333819716558 * np.exp(0.1629 * EK - 0.1629 * v))
     )
     dIK1_dEK = (
         -np.sqrt(5) * np.sqrt(ko) * GK1 * K1ss / 5
         + np.sqrt(5)
         * np.sqrt(ko)
@@ -7998,19 +7364,15 @@
     dIKb_dEK = -GKb * xkb
     dIKr_dEK = -np.sqrt(5) * np.sqrt(ko) * GKr * O / 5
     dIKs_dEKs = -GKs * KsCa * xs1 * xs2
     dI_katp_dEK = -fkatp * gkatp * akik * bkik
     dIto_dEK = -((1 - fItop) * a * i + ap * fItop * ip) * Gto
     dJdiffK_dki = -1 / tauK
     dP_dki = -eP / (
-        Kxkur
-        * (
-            (1 + H / Khp + nai / Knap + ki / Kxkur)
-            * (1 + H / Khp + nai / Knap + ki / Kxkur)
-        )
+        Kxkur * ((1 + H / Khp + nai / Knap + ki / Kxkur) * (1 + H / Khp + nai / Knap + ki / Kxkur))
     )
     dPhiCaK_i_dgamma_ki = np.exp(vfrt) * ki * vffrt / (-1 + np.exp(vfrt))
     dgamma_ki_dIi = (
         -(
             -0.3
             - 1 / (2 * ((1 + np.sqrt(Ii)) * (1 + np.sqrt(Ii))))
             + 1 / (2 * (1 + np.sqrt(Ii)) * np.sqrt(Ii))
@@ -8064,70 +7426,60 @@
                 -1
                 + ((1 + ki / Kki) * (1 + ki / Kki))
                 + ((1 + nai / Knai) * (1 + nai / Knai) * (1 + nai / Knai))
             )
         )
     )
     dki_dt_linearized = dJdiffK_dki * vss / vmyo + (
-        -(0.0005 * dPhiCaK_i_dgamma_ki * dgamma_ki_dIi + dPhiCaK_i_dki)
-        * dICaK_i_dPhiCaK_i
-        - (dEK_dki * dK1ss_daK1 * daK1_dEK + dEK_dki * dK1ss_dbK1 * dbK1_dEK)
-        * dIK1_dK1ss
+        -(0.0005 * dPhiCaK_i_dgamma_ki * dgamma_ki_dIi + dPhiCaK_i_dki) * dICaK_i_dPhiCaK_i
+        - (dEK_dki * dK1ss_daK1 * daK1_dEK + dEK_dki * dK1ss_dbK1 * dbK1_dEK) * dIK1_dK1ss
         - dEK_dki * dIK1_dEK
         - dEK_dki * dIKb_dEK
         - dEK_dki * dIKr_dEK
         - dEK_dki * dI_katp_dEK
         - dEK_dki * dIto_dEK
         - dEKs_dki * dIKs_dEKs
         + 2
         * zk
         * (
             dJnakK_da1 * da1_dki
             - 2
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE3_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE3_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE3_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE3_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE3_dx4
                 + b1 * b2 * dE3_dx3 * dP_dki * db3_dP
             )
             * a1
             + 2
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE4_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE4_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE4_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE4_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE4_dx4
                 + b1 * b2 * dE4_dx3 * dP_dki * db3_dP
             )
             * b1
         )
         * Pnak
         + 2
         * zna
         * (
             -3
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE2_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE2_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE2_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE2_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE2_dx4
                 + b1 * b2 * dE2_dx3 * dP_dki * db3_dP
             )
             * b3
             + 3
             * (
                 (db4_dki * dx2_db4 + a2 * a3 * da1_dki) * dE1_dx2
-                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3)
-                * dE1_dx1
-                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3)
-                * dE1_dx4
+                + (da1_dki * dx1_da1 + db4_dki * dx1_db4 + dP_dki * db3_dP * dx1_db3) * dE1_dx1
+                + (da1_dki * dx4_da1 + b2 * b3 * db4_dki + dP_dki * db3_dP * dx4_db3) * dE1_dx4
                 + b1 * b2 * dE1_dx3 * dP_dki * db3_dP
             )
             * a3
             + dJnakNa_db3 * dP_dki * db3_dP
         )
         * Pnak
     ) * Acap / (F * vmyo)
@@ -8180,17 +7532,15 @@
             dt * dcli_dt,
         )
         + cli
     )
     dclss_dt = -JdiffCl + Acap * IClCa_junc / (F * vss)
     dEClss_dclss = -R * T / (F * zcl * clss)
     dIClCa_junc_dEClss = -Fjunc * GClCa / (1 + KdClCa / cass)
-    dclss_dt_linearized = -1 / tauNa + Acap * dEClss_dclss * dIClCa_junc_dEClss / (
-        F * vss
-    )
+    dclss_dt_linearized = -1 / tauNa + Acap * dEClss_dclss * dIClCa_junc_dEClss / (F * vss)
     states[40] = (
         np.where(
             np.abs(dclss_dt_linearized) > 1e-08,
             (-1 + np.exp(dt * dclss_dt_linearized)) * dclss_dt / dclss_dt_linearized,
             dt * dclss_dt,
         )
         + clss
@@ -8229,67 +7579,55 @@
         )
         * constA
         * np.exp(-4 * (-0.3 * Ii + np.sqrt(Ii) / (1 + np.sqrt(Ii))) * constA)
     )
     dICab_dcai = (
         4
         * PCab
-        * (
-            np.exp(2 * vfrt) * gamma_cai
-            + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt)
-        )
+        * (np.exp(2 * vfrt) * gamma_cai + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt))
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    dICab_dgamma_cai = (
-        4 * PCab * cai * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
-    )
+    dICab_dgamma_cai = 4 * PCab * cai * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
     dINaCa_i_dallo_i = (1 - INaCa_fractionSS) * (zca * JncxCa_i + zna * JncxNa_i) * Gncx
     dIpCa_dcai = GpCa / (KmCap + cai) - GpCa * cai / ((KmCap + cai) * (KmCap + cai))
     dJdiff_dcai = -1 / tauCa
     dJup_dJupnp = Jup_b * (1 - fJupp)
     dJupnp_dcai = 0.005425 * upScale / (0.00092 + cai) - 0.005425 * cai * upScale / (
         (0.00092 + cai) * (0.00092 + cai)
     )
     dJupp_dcai = 0.01491875 * upScale / (0.00075 + cai) - 0.01491875 * cai * upScale / (
         (0.00075 + cai) * (0.00075 + cai)
     )
     dPhiCaL_i_dcai = (
         4
-        * (
-            np.exp(2 * vfrt) * gamma_cai
-            + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt)
-        )
+        * (np.exp(2 * vfrt) * gamma_cai + 0.002 * cai * dgamma_cai_dIi * np.exp(2 * vfrt))
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
     dPhiCaL_i_dgamma_cai = 4 * cai * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
     dallo_i_dcai = (
         2
         * (KmCaAct * KmCaAct)
         / (
-            (
-                (1 + (KmCaAct * KmCaAct) / (cai * cai))
-                * (1 + (KmCaAct * KmCaAct) / (cai * cai))
-            )
+            ((1 + (KmCaAct * KmCaAct) / (cai * cai)) * (1 + (KmCaAct * KmCaAct) / (cai * cai)))
             * (cai * cai * cai)
         )
     )
     dcai_dt_linearized = (
         Jdiff * vss / vmyo
         - Jup * vnsr / vmyo
         + (-ICaL_i - ICab - IpCa + 2 * INaCa_i) * Acap / (2 * F * vmyo)
     ) * dBcai_dcai + (
         dJdiff_dcai * vss / vmyo
         - (dJup_dJupnp * dJupnp_dcai + Jup_b * dJupp_dcai * fJupp) * vnsr / vmyo
         + (
             -dICab_dcai
             - dIpCa_dcai
-            - (0.002 * dPhiCaL_i_dgamma_cai * dgamma_cai_dIi + dPhiCaL_i_dcai)
-            * dICaL_i_dPhiCaL_i
+            - (0.002 * dPhiCaL_i_dgamma_cai * dgamma_cai_dIi + dPhiCaL_i_dcai) * dICaL_i_dPhiCaL_i
             + 2
             * (
                 (
                     kcaon * dE2_i_dx2_i * dx2_i_dk6_i * h6_i
                     + kcaon * dE2_i_dx3_i * dx3_i_dk6_i * h6_i
                     + kcaon * dE2_i_dx1_i * h6_i * k2_i * k4_i
                 )
@@ -8366,18 +7704,15 @@
         * (
             1
             + BSLmax * KmBSL / ((KmBSL + cass) * (KmBSL + cass))
             + BSRmax * KmBSR / ((KmBSR + cass) * (KmBSR + cass))
         )
     )
     dCaMKb_dcass = (
-        CaMKo
-        * KmCaM
-        * (1 - CaMKt)
-        / (((1 + KmCaM / cass) * (1 + KmCaM / cass)) * (cass * cass))
+        CaMKo * KmCaM * (1 - CaMKt) / (((1 + KmCaM / cass) * (1 + KmCaM / cass)) * (cass * cass))
     )
     dICaL_ss_dfICaLp = ICaL_fractionSS * (
         ((1 - nca_ss) * fp + fcap * jca * nca_ss) * PCap * PhiCaL_ss * d
         - ((1 - nca_ss) * f + fca * jca * nca_ss) * PCa * PhiCaL_ss * d
     )
     dINaCa_ss_dallo_ss = INaCa_fractionSS * (zca * JncxCa_ss + zna * JncxNa_ss) * Gncx
     dJrel_dfJrelp = Jrel_b * (-Jrel_np + Jrel_p)
@@ -8389,41 +7724,29 @@
             + 1 / (2 * (1 + np.sqrt(Iss)) * np.sqrt(Iss))
         )
         * constA
         * np.exp(-4 * (-0.3 * Iss + np.sqrt(Iss) / (1 + np.sqrt(Iss))) * constA)
     )
     dPhiCaL_ss_dcass = (
         4
-        * (
-            np.exp(2 * vfrt) * gamma_cass
-            + 0.002 * cass * dgamma_cass_dIss * np.exp(2 * vfrt)
-        )
+        * (np.exp(2 * vfrt) * gamma_cass + 0.002 * cass * dgamma_cass_dIss * np.exp(2 * vfrt))
         * vffrt
         / (-1 + np.exp(2 * vfrt))
     )
-    dPhiCaL_ss_dgamma_cass = (
-        4 * cass * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
-    )
+    dPhiCaL_ss_dgamma_cass = 4 * cass * np.exp(2 * vfrt) * vffrt / (-1 + np.exp(2 * vfrt))
     dallo_ss_dcass = (
         2
         * (KmCaAct * KmCaAct)
         / (
-            (
-                (1 + (KmCaAct * KmCaAct) / (cass * cass))
-                * (1 + (KmCaAct * KmCaAct) / (cass * cass))
-            )
+            ((1 + (KmCaAct * KmCaAct) / (cass * cass)) * (1 + (KmCaAct * KmCaAct) / (cass * cass)))
             * (cass * cass * cass)
         )
     )
-    dfICaLp_dCaMKa = KmCaMK / (
-        ((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa)
-    )
-    dfJrelp_dCaMKa = KmCaMK / (
-        ((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa)
-    )
+    dfICaLp_dCaMKa = KmCaMK / (((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa))
+    dfJrelp_dCaMKa = KmCaMK / (((1 + KmCaMK / CaMKa) * (1 + KmCaMK / CaMKa)) * (CaMKa * CaMKa))
     dcass_dt_linearized = (
         -1 / tauCa
         + (
             -(0.002 * dPhiCaL_ss_dgamma_cass * dgamma_cass_dIss + dPhiCaL_ss_dcass)
             * dICaL_ss_dPhiCaL_ss
             + 2
             * (
```

### Comparing `fenics-beat-0.0.3/src/beat/ecg.py` & `fenics_beat-0.0.4/src/beat/ecg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+from __future__ import annotations
 import dolfin
 from typing import NamedTuple
-import ufl_legacy as ufl
 import numpy as np
 
+try:
+    import ufl_legacy as ufl
+except ImportError:
+    import ufl
+
 
 def ecg_recovery(
     *,
     v: dolfin.Function,
     mesh: dolfin.Mesh,
     sigma_b: dolfin.Constant,
     dx: dolfin.Measure | None = None,
@@ -17,17 +22,15 @@
         # breakpoint()
         dx = dolfin.dx(domain=mesh, metadata={"quadrature_degree": 4})
     if r is None:
         r = dolfin.SpatialCoordinate(mesh) - dolfin.Constant(point)
 
     r3 = ufl.sqrt((r**2)) ** 3
     # https://carp.medunigraz.at/knowledge-base/tissue-scale-ep.html
-    return (1 / (4 * ufl.pi * sigma_b)) * dolfin.assemble(
-        (ufl.inner(ufl.grad(v), r) / r3) * dx
-    )
+    return (1 / (4 * ufl.pi * sigma_b)) * dolfin.assemble((ufl.inner(ufl.grad(v), r) / r3) * dx)
 
 
 def _check_attr(attr: np.ndarray | None):
     if attr is None:
         raise AttributeError(f"Missing attribute {attr}")
```

### Comparing `fenics-beat-0.0.3/src/beat/monodomain_model.py` & `fenics_beat-0.0.4/src/beat/monodomain_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from __future__ import annotations
 import logging
 
 import dolfin
-import ufl_legacy as ufl
-from ufl_legacy.core.expr import Expr
+
+try:
+    import ufl_legacy as ufl
+    from ufl_legacy.core.expr import Expr
+except ImportError:
+    import ufl
+    from ufl.core.expr import Expr
 
 from .base_model import BaseModel, Stimulus
 
 logger = logging.getLogger(__name__)
 
 
 class MonodomainModel(BaseModel):
@@ -85,20 +90,18 @@
         Dt_v_k_n = v - self.v_
         v_mid = theta * v + (1.0 - theta) * self.v_
 
         theta_parabolic = ufl.inner(self._M * ufl.grad(v_mid), ufl.grad(w))
         # breakpoint()
         G_stim = self._I_s.expr * w * self._I_s.dz
 
-        G = (Dt_v_k_n * w + k_n * theta_parabolic) * dolfin.dx(
-            domain=self._mesh
-        ) - k_n * G_stim
+        G = (Dt_v_k_n * w + k_n * theta_parabolic) * dolfin.dx(domain=self._mesh) - k_n * G_stim
 
         # Define preconditioner based on educated(?) guess by Marie
         if self.parameters["use_custom_preconditioner"]:
-            prec = (
-                v * w + k_n / 2.0 * ufl.inner(self._M * ufl.grad(v), ufl.grad(w))
-            ) * dolfin.dx(domain=self._mesh)
+            prec = (v * w + k_n / 2.0 * ufl.inner(self._M * ufl.grad(v), ufl.grad(w))) * dolfin.dx(
+                domain=self._mesh
+            )
         else:
             prec = None
 
         return (G, prec)
```

### Comparing `fenics-beat-0.0.3/src/beat/monodomain_solver.py` & `fenics_beat-0.0.4/src/beat/monodomain_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,23 @@
 from .monodomain_model import MonodomainModel
 
 logger = logging.getLogger(__name__)
 EPS = 1e-12
 
 
 class ODESolver(Protocol):
-    def to_dolfin(self) -> None:
-        ...
+    def to_dolfin(self) -> None: ...
 
-    def from_dolfin(self) -> None:
-        ...
+    def from_dolfin(self) -> None: ...
 
-    def ode_to_pde(self) -> None:
-        ...
+    def ode_to_pde(self) -> None: ...
 
-    def pde_to_ode(self) -> None:
-        ...
+    def pde_to_ode(self) -> None: ...
 
-    def step(self, t0: float, t1: float) -> None:
-        ...
+    def step(self, t0: float, t1: float) -> None: ...
 
 
 @dataclass
 class MonodomainSplittingSolver:
     pde: MonodomainModel
     ode: ODESolver
     theta: float = 0.5
@@ -80,17 +75,15 @@
         # If first order splitting, we are done.
         if np.isclose(theta, 1.0):
             # But first update previous value in PDE
             self.pde.assign_previous()
             return
 
         # Otherwise, we do another ode_step:
-        logger.info(
-            f"Corrective ODE step with t0={t:5f} and dt={(1.0 - theta) * dt:.5f}"
-        )
+        logger.info(f"Corrective ODE step with t0={t:5f} and dt={(1.0 - theta) * dt:.5f}")
 
         # To the correction step
         self.ode.step(t, (1.0 - theta) * dt)
         # And copy the solution back to FEniCS
         self.ode.to_dolfin()  # numpy array (ODE solver) -> dolfin function
         self.ode.ode_to_pde()  # dolfin function in ODE space (quad?) -> CG1 dolfin function
         self.pde.assign_previous()
```

### Comparing `fenics-beat-0.0.3/src/beat/odesolver.py` & `fenics_beat-0.0.4/src/beat/odesolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,15 @@
         return self.states.shape[1]
 
     @property
     def num_states(self) -> int:
         return self.states.shape[0]
 
     def step(self, t0: float, dt: float) -> None:
-        self.states[:] = self.fun(
-            states=self.states, t=t0, parameters=self.parameters, dt=dt
-        )
+        self.states[:] = self.fun(states=self.states, t=t0, parameters=self.parameters, dt=dt)
 
 
 class BaseDolfinODESolver(abc.ABC):
     v_ode: dolfin.Function
     v_pde: dolfin.Function
     _metadata: dict[str, Any] | None = None
 
@@ -128,15 +126,15 @@
             states=self._values,
             parameters=self.parameters,
         )
         self._initialize_metadata()
 
     def to_dolfin(self) -> None:
         """Assign values from numpy array to dolfin function"""
-        self.v_ode.vector().set_local(self._values[self.v_index, :])
+        self.v_ode.vector()[:] = self._values[self.v_index, :]
 
     def from_dolfin(self) -> None:
         """Assign values from dolfin function to numpy array"""
         self._values[self.v_index, :] = self.v_ode.vector().get_local()
 
     @property
     def values(self):
@@ -148,15 +146,15 @@
 
     @property
     def shape(self) -> tuple[int, int]:
         return (self.num_states, self.num_points)
 
     @property
     def num_points(self) -> int:
-        return self.v_ode.vector().size()
+        return self.v_ode.vector().local_size()
 
     def step(self, t0: float, dt: float):
         self._ode.step(t0=t0, dt=dt)
 
     @property
     def full_values(self):
         return self._values
@@ -171,17 +169,15 @@
     parameters: dict[int, npt.NDArray]
     fun: dict[int, Callable]
     num_states: dict[int, int]
     v_index: dict[int, int]
 
     def __post_init__(self):
         if self.v_ode.vector().size() != self.markers.vector().size():
-            raise RuntimeError(
-                "Marker and voltage need to be in the same function space"
-            )
+            raise RuntimeError("Marker and voltage need to be in the same function space")
 
         self._marker_values = tuple(self.init_states.keys())
         self._num_points = {}
         self._odes = {}
         self._values = {}
         self._inds = {}
 
@@ -203,28 +199,27 @@
                 states=self._values[marker],
                 parameters=self.parameters[marker],
             )
         self._initialize_metadata()
 
     def _initialize_full_values(self):
         self._all_states_equal_size = (
-            np.array(tuple(self.num_states.values()))
-            == tuple(self.num_states.values())[0]
+            np.array(tuple(self.num_states.values())) == tuple(self.num_states.values())[0]
         ).all()
         if self._all_states_equal_size:
             self._full_values = np.zeros(
                 (next(iter(self.num_states.values())), self.markers.vector().size())
             )
 
     def to_dolfin(self) -> None:
         """Assign values from numpy array to dolfin function"""
         arr = self.v_ode.vector().get_local().copy()
         for marker in self._marker_values:
             arr[self._inds[marker]] = self._values[marker][self.v_index[marker], :]
-        self.v_ode.vector().set_local(arr)
+        self.v_ode.vector()[:] = arr
 
     def from_dolfin(self) -> None:
         """Assign values from dolifn function to numpy array"""
         arr = self.v_ode.vector().get_local()
         for marker in self._marker_values:
             self._values[marker][self.v_index[marker], :] = arr[self._inds[marker]]
```

### Comparing `fenics-beat-0.0.3/src/beat/utils.py` & `fenics_beat-0.0.4/src/beat/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,46 @@
 from __future__ import annotations
 from typing import Any
 import logging
+from contextlib import contextmanager
 import dolfin
 import numpy.typing as npt
 import numpy as np
-import ufl_legacy as ufl
-from contextlib import contextmanager
+from mpi4py import MPI as pyMPI
+
+try:
+    import ufl_legacy as ufl
+except ImportError:
+    import ufl
 
 
 logger = logging.getLogger(__name__)
 
 
+def mpi4py_comm(comm):
+    """Get mpi4py communicator"""
+    try:
+        return comm.tompi4py()
+    except AttributeError:
+        return comm
+
+
+def peval(f, *x):
+    """Parallel synced eval"""
+    try:
+        yloc = f(*x)
+    except RuntimeError:
+        yloc = np.inf * np.ones(f.value_shape())
+
+    comm = mpi4py_comm(f.function_space().mesh().mpi_comm())
+    yglob = np.zeros_like(yloc)
+    comm.Allreduce(yloc, yglob, op=pyMPI.MIN)
+    return yglob
+
+
 def expand_layer(
     markers: dolfin.Function,
     mfun: dolfin.MeshFunction,
     endo_markers: list[int],
     epi_markers: list[int],
     endo_marker: int,
     epi_marker: int,
@@ -141,15 +167,14 @@
     v_ = dolfin.TestFunction(V)
     a_proj = ufl.inner(dv, v_) * ufl.dx(metadata=metadata)
     b_proj = ufl.inner(v, v_) * ufl.dx(metadata=metadata)
 
     if metadata is None:
         solver = dolfin.LocalSolver(a_proj, b_proj)
     else:
-
         with form_compiler_representation("quadrature"):
             solver = dolfin.LocalSolver(a_proj, b_proj)
 
     solver.factorize()
     if u is None:
         u = dolfin.Function(V)
     solver.solve_local_rhs(u)
```

### Comparing `fenics-beat-0.0.3/src/fenics_beat.egg-info/PKG-INFO` & `fenics_beat-0.0.4/src/fenics_beat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: fenics-beat
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library to run cardiac EP simulations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://finsberg.github.io/fenics-beat
 Project-URL: Documentation, https://finsberg.github.io/fenics-beat
 Project-URL: Source, https://github.com/finsberg/fenics-beat
 Project-URL: Tracker, https://github.com/finsberg/fenics-beat/issues
 Keywords: cardiac,electrophysiology
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: scipy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pdbpp; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
@@ -34,14 +33,16 @@
 Requires-Dist: fenics-beat[demos]; extra == "docs"
 Provides-Extra: all
 Requires-Dist: fenics-beat[test]; extra == "all"
 Requires-Dist: fenics-beat[docs]; extra == "all"
 Requires-Dist: fenics-beat[pypi]; extra == "all"
 Requires-Dist: fenics-beat[dev]; extra == "all"
 Requires-Dist: fenics-beat[demos]; extra == "all"
+Provides-Extra: testpaths
+Requires-Dist: tests; extra == "testpaths"
 
 # fenics-beat
 
 A simplified version of `cbcbeat` for running cardiac electrophysiology simulations.
 
 - Source code: https://github.com/finsberg/fenics-beat
 - Documentation: https://finsberv.github.io/fenics-beat
```

### Comparing `fenics-beat-0.0.3/src/fenics_beat.egg-info/SOURCES.txt` & `fenics_beat-0.0.4/src/fenics_beat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.3/tests/test_bidomain_model.py` & `fenics_beat-0.0.4/tests/test_bidomain_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 def test_bidomain_model():
     dt = 0.001
     T = 10 * dt
     N = 15
     theta = 0.5
     mesh = dolfin.UnitSquareMesh(N, N)
     time = dolfin.Constant(0.0)
-    ac_str = (
-        "cos(t)*cos(pi*x[0])*cos(pi*x[1]) + pow(pi, 2)*cos(pi*x[0])*cos(pi*x[1])*sin(t)"
-    )
+    ac_str = "cos(t)*cos(pi*x[0])*cos(pi*x[1]) + pow(pi, 2)*cos(pi*x[0])*cos(pi*x[1])*sin(t)"
     stimulus = dolfin.Expression(ac_str, t=time, degree=5)
     M_i = 1.0
     M_e = 1.0
 
     # Set-up solver
     params = beat.BidomainModel.default_parameters()
     params["theta"] = theta
```

### Comparing `fenics-beat-0.0.3/tests/test_cellmodels.py` & `fenics_beat-0.0.4/tests/test_cellmodels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import pytest
 import beat
 import numpy as np
 
 
-@pytest.mark.parametrize(
-    "rhs", ("forward_explicit_euler", "forward_generalized_rush_larsen")
-)
+@pytest.mark.parametrize("rhs", ("forward_explicit_euler", "forward_generalized_rush_larsen"))
 @pytest.mark.parametrize("model", beat.cellmodels.all_cellmodels())
 def test_all_cellmodels(rhs, model):
     states = model.init_state_values()
     old_states = states.copy()
 
     ode = beat.odesolver.ODESystemSolver(
         fun=getattr(model, rhs),
```

### Comparing `fenics-beat-0.0.3/tests/test_ecg.py` & `fenics_beat-0.0.4/tests/test_ecg.py`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.3/tests/test_monodomain.py` & `fenics_beat-0.0.4/tests/test_monodomain.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     v_exact = dolfin.Expression(exact, t=T, degree=3)
 
     v_error = dolfin.errornorm(v_exact, res.state, "L2", degree_rise=2)
     assert v_error < err
 
 
+@pytest.mark.skip_in_parallel
 def test_monodomain_spatial_convergence():
     time = dolfin.Constant(0.0)
     ac_str = "cos(2*pi*x[0])*cos(2*pi*x[1])*(cos(t) +  8*pow(pi, 2)*sin(t))"
 
     I_s = dolfin.Expression(ac_str, t=time, degree=5)
 
     theta = 0.5
@@ -63,25 +64,24 @@
     params = dict(theta=theta, linear_solver_type="direct")  # , default_timestep=dt)
     v_exact = dolfin.Expression("cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)", t=T, degree=3)
 
     errors = []
     Ns = [2**level for level in (2, 3, 4, 5)]
     for N in Ns:
         mesh = dolfin.UnitSquareMesh(N, N)
-        model = beat.MonodomainModel(
-            time=time, mesh=mesh, M=1.0, I_s=I_s, params=params
-        )
+        model = beat.MonodomainModel(time=time, mesh=mesh, M=1.0, I_s=I_s, params=params)
         res = model.solve((0, T), dt=dt)
         v_error = dolfin.errornorm(v_exact, res.state, "L2", degree_rise=2)
         errors.append(v_error)
 
     rates = [np.log(e1 / e2) / np.log(2) for e1, e2 in zip(errors[:-1], errors[1:])]
     assert all(rate >= 2.0 for rate in rates)
 
 
+@pytest.mark.skip_in_parallel
 def test_monodomain_temporal_convergence():
     time = dolfin.Constant(0.0)
     ac_str = "cos(2*pi*x[0])*cos(2*pi*x[1])*(cos(t) +  8*pow(pi, 2)*sin(t))"
 
     I_s = dolfin.Expression(ac_str, t=time, degree=5)
 
     theta = 0.5
@@ -92,16 +92,14 @@
 
     params = dict(theta=theta, linear_solver_type="direct")  # , default_timestep=dt)
     v_exact = dolfin.Expression("cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)", t=T, degree=3)
 
     errors = []
     dts = [1.0 / (2**level) for level in (0, 1, 2, 3)]
     for dt in dts:
-        model = beat.MonodomainModel(
-            time=time, mesh=mesh, M=1.0, I_s=I_s, params=params
-        )
+        model = beat.MonodomainModel(time=time, mesh=mesh, M=1.0, I_s=I_s, params=params)
         res = model.solve((0, T), dt=dt)
         v_error = dolfin.errornorm(v_exact, res.state, "L2", degree_rise=2)
         errors.append(v_error)
 
     rates = [np.log(e1 / e2) / np.log(2) for e1, e2 in zip(errors[:-1], errors[1:])]
     assert all(rate >= 2.0 for rate in rates)
```

### Comparing `fenics-beat-0.0.3/tests/test_monodomain_solver.py` & `fenics_beat-0.0.4/tests/test_monodomain_solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     # Source term
     ac_str = "8*pow(pi, 2)*cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
     s_exact = dolfin.Expression(s_exact_str, t=0, degree=1)
 
     family = "Lagrange"
     degree = 1
     N = 50
-    mesh = dolfin.UnitSquareMesh(N, N)
+    comm = dolfin.MPI.comm_world
+    mesh = dolfin.UnitSquareMesh(comm, N, N)
     time = dolfin.Constant(0.0)
     I_s = dolfin.Expression(ac_str, t=time, degree=5)
     M = 1.0
     # T = 4.0
     dt = 0.01
     T = dt
     t0 = 0.0
@@ -50,17 +51,15 @@
         "degree": degree,
         "linear_solver_type": "direct",
     }
 
     pde = beat.MonodomainModel(time=time, mesh=mesh, M=M, I_s=I_s, params=params)
 
     family, degree = odespace.split("_")
-    element = dolfin.FiniteElement(
-        family, mesh.ufl_cell(), int(degree), quad_scheme="default"
-    )
+    element = dolfin.FiniteElement(family, mesh.ufl_cell(), int(degree), quad_scheme="default")
     V_ode = dolfin.FunctionSpace(mesh, element)
     v_ode = dolfin.Function(V_ode)
 
     s = dolfin.interpolate(s_exact, V_ode)
     s_arr = s.vector().get_local()
     init_states = np.zeros((2, s_arr.size))
     init_states[1, :] = s_arr
@@ -77,15 +76,14 @@
     solver = beat.MonodomainSplittingSolver(pde=pde, ode=ode)
     solver.solve((t0, T), dt=dt)
 
     v_exact = dolfin.Expression(v_exact_str, t=T, degree=3)
     v_error = dolfin.errornorm(v_exact, pde.state, "L2", degree_rise=2)
     # dolfin.File("v_exact.pvd") << dolfin.interpolate(v_exact, pde.V)
     # dolfin.File("v.pvd") << pde.state
-    print(v_error)
     assert v_error < 0.002
 
 
 @pytest.mark.parametrize(
     "odespace",
     [
         "CG_1",
@@ -115,20 +113,20 @@
     t0 = 0.0
 
     params = {
         "family": family,
         "degree": degree,
         "linear_solver_type": "direct",
     }
-
     errors = []
     ode_family, ode_degree = odespace.split("_")
     Ns = [2**level for level in (3, 4, 5)]
+    comm = dolfin.MPI.comm_world
     for N in Ns:
-        mesh = dolfin.UnitSquareMesh(N, N)
+        mesh = dolfin.UnitSquareMesh(comm, N, N)
         time = dolfin.Constant(0.0)
         I_s = dolfin.Expression(ac_str, t=time, degree=5)
 
         pde = beat.MonodomainModel(time=time, mesh=mesh, M=M, I_s=I_s, params=params)
         s_exact = dolfin.Expression(s_exact_str, t=0, degree=1)
 
         element = dolfin.FiniteElement(
@@ -147,27 +145,38 @@
             v_pde=pde.state,
             fun=simple_ode_forward_euler,
             init_states=init_states,
             num_states=2,
             parameters=None,
             v_index=0,
         )
+
         solver = beat.MonodomainSplittingSolver(pde=pde, ode=ode)
         solver.solve((t0, T), dt=dt)
 
         v_exact = dolfin.Expression(v_exact_str, t=T, degree=3)
         v_error = dolfin.errornorm(v_exact, pde.state, "L2", degree_rise=2)
         errors.append(v_error)
 
     rates = [np.log(e1 / e2) / np.log(2) for e1, e2 in zip(errors[:-1], errors[1:])]
     cvg_rate = sum(rates) / len(rates)
     assert np.isclose(cvg_rate, degree + 1, rtol=0.1)
 
 
-def test_monodomain_splitting_temporal_convergence():
+@pytest.mark.parametrize(
+    "odespace",
+    [
+        "CG_1",
+        "CG_2",
+        "DG_1",
+        "Quadrature_2",
+        "Quadrature_4",
+    ],
+)
+def test_monodomain_splitting_temporal_convergence(odespace):
     # Exact solutions
     v_exact_str = "cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
     s_exact_str = "-cos(2*pi*x[0])*cos(2*pi*x[1])*cos(t)"
 
     # Source term
     ac_str = "8*pow(pi, 2)*cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
 
@@ -183,46 +192,55 @@
 
     params = {
         "family": family,
         "degree": degree,
         "linear_solver_type": "direct",
     }
 
+    ode_family, ode_degree = odespace.split("_")
+
     errors = []
-    mesh = dolfin.UnitSquareMesh(150, 150)
+    comm = dolfin.MPI.comm_world
+    mesh = dolfin.UnitSquareMesh(comm, 150, 150)
+
+    element = dolfin.FiniteElement(
+        ode_family, mesh.ufl_cell(), int(ode_degree), quad_scheme="default"
+    )
+    V_ode = dolfin.FunctionSpace(mesh, element)
+    v_ode = dolfin.Function(V_ode)
     dts = [1.0 / (2**level) for level in (2, 3, 4)]
     for dt in dts:
         time = dolfin.Constant(0.0)
         I_s = dolfin.Expression(ac_str, t=time, degree=5)
 
         pde = beat.MonodomainModel(time=time, mesh=mesh, M=M, I_s=I_s, params=params)
         s_exact = dolfin.Expression(s_exact_str, t=0, degree=1)
-        s = dolfin.interpolate(s_exact, pde.V)
+        s = dolfin.interpolate(s_exact, V_ode)
         s_arr = s.vector().get_local()
         init_states = np.zeros((2, s_arr.size))
         init_states[1, :] = s_arr
 
         ode = beat.odesolver.DolfinODESolver(
-            v_ode=dolfin.Function(pde.V),
+            v_ode=v_ode,
             v_pde=pde.state,
             fun=simple_ode_forward_euler,
             init_states=init_states,
             num_states=2,
             parameters=None,
             v_index=0,
         )
-        solver = beat.MonodomainSplittingSolver(pde=pde, ode=ode)
+        solver = beat.MonodomainSplittingSolver(pde=pde, ode=ode, theta=0.5)
         solver.solve((t0, T), dt=dt)
 
         v_exact = dolfin.Expression(v_exact_str, t=T, degree=3)
         v_error = dolfin.errornorm(v_exact, pde.state, "L2", degree_rise=2)
         errors.append(v_error)
 
     rates = [np.log(e1 / e2) / np.log(2) for e1, e2 in zip(errors[:-1], errors[1:])]
-    cvg_rate = sum(rates) / len(rates)
+    cvg_rate = np.mean(rates)
     # Forward Euler has error of order one in time
     assert np.greater_equal(cvg_rate, 0.99)
 
 
 @pytest.mark.parametrize(
     "odespace",
     [
@@ -242,15 +260,16 @@
     # Source term
     ac_str = "8*pow(pi, 2)*cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
     s_exact = dolfin.Expression(s_exact_str, t=0, degree=1)
 
     family = "Lagrange"
     degree = 1
     N = 50
-    mesh = dolfin.UnitSquareMesh(N, N)
+    comm = dolfin.MPI.comm_world
+    mesh = dolfin.UnitSquareMesh(comm, N, N)
     time = dolfin.Constant(0.0)
     I_s = dolfin.Expression(ac_str, t=time, degree=5)
     M = 1.0
     # T = 4.0
     dt = 0.01
     T = dt
     t0 = 0.0
@@ -260,17 +279,15 @@
         "degree": degree,
         "linear_solver_type": "direct",
     }
 
     pde = beat.MonodomainModel(time=time, mesh=mesh, M=M, I_s=I_s, params=params)
 
     family, degree = odespace.split("_")
-    element = dolfin.FiniteElement(
-        family, mesh.ufl_cell(), int(degree), quad_scheme="default"
-    )
+    element = dolfin.FiniteElement(family, mesh.ufl_cell(), int(degree), quad_scheme="default")
     V_ode = dolfin.FunctionSpace(mesh, element)
     v_ode = dolfin.Function(V_ode)
 
     s = dolfin.interpolate(s_exact, V_ode)
     s_arr = s.vector().get_local()
     init_states = np.zeros((2, s_arr.size))
     init_states[1, :] = s_arr
```

### Comparing `fenics-beat-0.0.3/tests/test_odesolver.py` & `fenics_beat-0.0.4/tests/test_odesolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import dolfin
+import pytest
 
 import beat
 from beat.odesolver import ODESystemSolver, DolfinODESolver, DolfinMultiODESolver
 
 
 def test_simple_ode_odesystemsolver():
     def simple_ode_forward_euler(states, t, dt, parameters):
@@ -139,20 +140,23 @@
     assert np.allclose(ode.v_ode.vector().get_local(), init_states[v_index])
     ode.to_dolfin()
     ode.ode_to_pde()
     assert np.allclose(ode.v_pde.vector().get_local(), 42.0)
 
     # Now update dolfin function for v
     ode.v_pde.assign(dolfin.Constant(13.0))
+
     ode.pde_to_ode()
     ode.from_dolfin()
+
     assert np.allclose(ode.values[v_index, :], 13.0)
     assert np.allclose(ode.full_values[v_index, :], 13.0)
 
 
+@pytest.mark.skipif(dolfin.MPI.comm_world.size > 1, reason="Need to be fixed for parallel")
 def test_ode_with_markers_3D_to_and_from_dolfin():
     model = beat.cellmodels.tentusscher_panfilov_2006
     mesh = dolfin.UnitCubeMesh(3, 3, 3)
     V = dolfin.FunctionSpace(mesh, "Lagrange", 1)
     markers = dolfin.Function(V)
     arr = markers.vector().get_local().copy()
     v2d = dolfin.vertex_to_dof_map(V)
```

### Comparing `fenics-beat-0.0.3/tests/test_utils.py` & `fenics_beat-0.0.4/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,37 @@
 import numpy as np
 import dolfin
 import beat
+from mpi4py import MPI as pyMPI
+
+
+def mpi4py_comm(comm):
+    """Get mpi4py communicator"""
+    try:
+        return comm.tompi4py()
+    except AttributeError:
+        return comm
+
+
+def peval(f, *x):
+    """Parallel synced eval"""
+    try:
+        yloc = f(*x)
+    except RuntimeError:
+        yloc = np.inf * np.ones(f.value_shape())
+
+    comm = mpi4py_comm(f.function_space().mesh().mpi_comm())
+    yglob = np.zeros_like(yloc)
+    comm.Allreduce(yloc, yglob, op=pyMPI.MIN)
+    return yglob
 
 
 def test_expand_layer_single():
-    mesh = dolfin.UnitSquareMesh(10, 10)
+    comm = dolfin.MPI.comm_world
+    mesh = dolfin.UnitSquareMesh(comm, 10, 10)
 
     mfun = dolfin.MeshFunction("size_t", mesh, mesh.topology().dim() - 1)
     mfun.set_all(0)
     mid_marker = 0
     endo_marker = 1
     epi_marker = 2
     dolfin.CompiledSubDomain("near(x[0], 0)").mark(mfun, endo_marker)
@@ -28,17 +51,17 @@
     )
 
     markers.vector().set_local(arr)
 
     # Just check a few values
     for x in [0.0, 0.1, 0.2]:
         for y in [0.0, 0.5, 1.0]:
-            assert np.isclose(markers(x, y), endo_marker)
-            assert np.isclose(markers(x + 0.4, y), mid_marker)
-            assert np.isclose(markers(1 - x, y), epi_marker)
+            assert np.isclose(peval(markers, (x, y)), endo_marker)
+            assert np.isclose(peval(markers, (x + 0.4, y)), mid_marker)
+            assert np.isclose(peval(markers, (1 - x, y)), epi_marker)
 
 
 def test_expand_layer_double():
     mesh = dolfin.UnitSquareMesh(10, 10)
 
     mfun = dolfin.MeshFunction("size_t", mesh, mesh.topology().dim() - 1)
     mfun.set_all(0)
@@ -64,10 +87,10 @@
     )
 
     markers.vector().set_local(arr)
 
     # Just check a few values
     for x in [0.0, 0.1, 0.2]:
         for y in [0.0, 0.5, 1.0]:
-            assert np.isclose(markers(x, y), endo_marker)
-            assert np.isclose(markers(x + 0.4, y), mid_marker)
-            assert np.isclose(markers(1 - x, y), epi_marker)
+            assert np.isclose(peval(markers, (x, y)), endo_marker)
+            assert np.isclose(peval(markers, (x + 0.4, y)), mid_marker)
+            assert np.isclose(peval(markers, (1 - x, y)), epi_marker)
```

