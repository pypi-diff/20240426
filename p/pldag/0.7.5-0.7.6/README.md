# Comparing `tmp/pldag-0.7.5.tar.gz` & `tmp/pldag-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.7.5.tar", max compression
+gzip compressed data, was "pldag-0.7.6.tar", max compression
```

## Comparing `pldag-0.7.5.tar` & `pldag-0.7.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.5/LICENSE
--rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.5/README.md
--rw-r--r--   0        0        0    32526 2024-04-26 06:40:47.732022 pldag-0.7.5/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.7.5/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.7.5/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-04-26 06:47:19.456855 pldag-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.6/LICENSE
+-rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.6/README.md
+-rw-r--r--   0        0        0    33042 2024-04-26 10:50:44.132872 pldag-0.7.6/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.7.6/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.7.6/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-04-26 10:52:09.301047 pldag-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.6/PKG-INFO
```

### Comparing `pldag-0.7.5/LICENSE` & `pldag-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.7.5/README.md` & `pldag-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.7.5/pldag/__init__.py` & `pldag-0.7.6/pldag/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from hashlib import sha1
-from itertools import groupby, repeat
+from itertools import groupby, repeat, starmap
 from functools import partial, lru_cache
 from typing import Dict, List, Set, Optional
 from graphlib import TopologicalSorter
 
 from enum import Enum
 
 class NoSolutionsException(Exception):
@@ -38,15 +38,15 @@
         # Alias to id mapping
         self._amap = {}
 
     def __hash__(self) -> int:
         return hash(self.sha1())
     
     def sha1(self) -> str:
-        return sha1("".join(self._imap.keys()).encode()).hexdigest()
+        return sha1(("".join(self._imap.keys()) + "".join(map(lambda c: f"{c.real}{c.imag}", self._dvec))).encode()).hexdigest()
 
     @property
     def bounds(self) -> np.ndarray:
         """Get the bounds of all aliases"""
         return self._dvec
     
     @property
@@ -704,15 +704,15 @@
         """
         return self.set_xor([
             self.set_and(references),
             self.set_not(references),
         ], alias)
     
     @lru_cache
-    def to_polyhedron(self, **fix) -> tuple:
+    def to_polyhedron(self, **fix: Dict[str, complex]) -> tuple:
 
         """
             Constructs a polyhedron of matrix A and bias vector b,
             such that A.dot(x) >= b, where x is the vector of variables.
             Every composite variable A is its own column in the matrix where
             A -> (A's composite proposition) is true. 
 
@@ -722,15 +722,15 @@
                 A dictionary of variables to fix.
 
             Examples
             --------
             >>> model = PLDAG()
             >>> model.set_primitives("xyz")
             >>> a = model.set_atleast("xyz", 1)
-            >>> A,b,vs = model.to_polyhedron()
+            >>> A, b = model.to_polyhedron()
             >>> np.array_equal(A, np.array([[1,1,1,-1]]))
             True
         """
 
         # Create the matrix
         A = np.zeros(self._amat.shape, dtype=np.int64)
 
@@ -758,17 +758,29 @@
         # Fill the composite id's with the mx value
         A[range(A.shape[0]), cidx] = eq_bounds.real
 
         # Create the bias vector. The linear equation should be increased
         # by the flipped minimum value
         b = eq_bounds.real - self._bvec.real
 
-        # Fix the columns in `fix`
-        for i, vs in groupby(zip(fix.values(), fix.keys()), key=lambda x: x[0]):
-            v = list(map(lambda x: x[1], vs))
+        # Fix constant variables
+        for i, vs in groupby(
+            sorted(
+                map(
+                    lambda x: (x[0], int(x[1].real)), 
+                    filter(
+                        lambda x: x[1].real == x[1].imag, 
+                        fix.items()
+                    )
+                ),
+                key=lambda x: x[1] 
+            ), 
+            key=lambda x: x[1]
+        ):
+            v = list(map(lambda x: x[0], vs))
             a = np.zeros(A.shape[1], dtype=np.int64)
             a[np.array(list(map(self._col, v)))] = 1
             if i > 0 or i < 0:
                 _b = a.sum() * i
             else:
                 _b = 0
 
@@ -777,44 +789,45 @@
 
         # Set bounds for integer variables
         int_vars = list(set(np.argwhere((self._dvec.real != 0) | (self._dvec.imag != 1)).T[0].tolist()))
 
         # Declare new constraints for upper and lower bound for integer variables
         A_int = np.zeros((len(int_vars) * 2, A.shape[1]), dtype=np.int64)
         b_int = np.zeros((len(int_vars) * 2, ), dtype=np.int64)
+
+        # Setup dvec as real and imag parts
+        d_real = self._dvec.real
+        d_imag = self._dvec.imag
+
+        # Also, if fix has tighter bounds set we use them instead
+        for i, bound in filter(
+            lambda x: (x[1].real != x[1].imag), 
+            starmap(
+                lambda k,v: (self._col(k), v),
+                fix.items()
+            )
+        ):
+            if bound.real > d_real[i]:
+                d_real[i] = bound.real
+            elif bound.imag < d_imag[i]:
+                d_imag[i] = bound.imag
         
         # Lower bound for integers..
         A_int[np.arange(len(int_vars) * 2, step=2), int_vars] = 1
-        b_int[np.arange(len(int_vars) * 2, step=2)] = self._dvec[int_vars].real
+        b_int[np.arange(len(int_vars) * 2, step=2)] = d_real[int_vars]
         
         # Upper bound for integers..
         A_int[np.arange(len(int_vars) * 2, step=2) + 1, int_vars] = -1
-        b_int[np.arange(len(int_vars) * 2, step=2) + 1] = -1 * self._dvec[int_vars].imag
+        b_int[np.arange(len(int_vars) * 2, step=2) + 1] = -1 * d_imag[int_vars]
 
         # Add them onto polyhedron
         A = np.vstack([A, A_int])
         b = np.append(b, b_int)
 
-        # Reverse index map
-        rimap = dict(map(lambda x: (x[1], x[0]), self._imap.items()))
-
-        # Create the variable list
-        variables = np.array(
-            list(
-                map(
-                    lambda i: (
-                        rimap[i],
-                        self._dvec[i],
-                    ),
-                    np.array(list(self._imap.values()))
-                )
-            )
-        )
-
-        return A, b, variables
+        return A, b
     
     def _from_indices(self, row_idxs: np.ndarray, col_idxs: np.ndarray) -> 'PLDAG':
         """
             Create a PLDAG from the given row and column indices.
 
             Parameters
             ----------
@@ -887,43 +900,44 @@
                 break
             matching_variables.update(new_matching_variables)
 
         col_idxs = np.array(sorted(list(map(col_vars.index, matching_variables))))
         row_idxs = np.array(sorted(list(map(row_vars.index, filter(lambda v: v in self._row_vars, matching_variables)))))
         return self._from_indices(row_idxs, col_idxs)
     
-    def solve(self, objectives: List[Dict[str, int]], fix: Dict[str, int], solver: Solver) -> List[Dict[str, int]]:
+    def solve(self, objectives: List[Dict[str, int]], fix: Dict[str, complex], solver: Solver) -> List[Dict[str, complex]]:
         """
             Solves the model with the given objectives.
 
             Parameters
             ----------
             objectives : List[Dict[str, int]]
                 The objectives to solve for.
 
-            fix : Dict[str, int]
+            fix : Dict[str, complex]
                 The variables to fix.
 
             solver : Solver
                 The solver to use.
 
             Examples
             --------
             >>> model = PLDAG()
             >>> model.set_primitives("xyz")
             >>> a = model.set_atleast("xyz", 1)
-            >>> model.solve([{"x": 0, "y": 1, "z": 0}], Solver.GLPK)
-            [{'x': 0, 'y': 1, 'z': 0}]
+            >>> model.solve([{"x": 0, "y": 1, "z": 0}], {}, Solver.GLPK)
+            [{'x': 0j, 'y': 1+1j, 'z': 0j}]
 
             Returns
             -------
-            List[Dict[str, int]]
+            List[Dict[str, complex]]
                 The solutions for the objectives.
         """
-        A, b, variables = self.to_polyhedron(**fix)
+        A, b = self.to_polyhedron(**fix)
+        variables = self._col_vars
         obj_mat = np.zeros((len(objectives), len(variables)), dtype=np.int64)
         for i, obj in enumerate(objectives):
             obj_mat[i, [self._col(k) for k in obj]] = list(obj.values())
 
         if solver == Solver.GLPK:
             from pldag.solver.glpk_solver import solve_lp
             solutions = solve_lp(A, b, obj_mat, set(np.argwhere((self._dvec.real != 0) | (self._dvec.imag != 1)).T[0].tolist()))
```

### Comparing `pldag-0.7.5/pldag/solver/glpk_solver.py` & `pldag-0.7.6/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.7.5/PKG-INFO` & `pldag-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.7.5
+Version: 0.7.6
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

