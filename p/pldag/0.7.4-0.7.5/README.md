# Comparing `tmp/pldag-0.7.4.tar.gz` & `tmp/pldag-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.7.4.tar", max compression
+gzip compressed data, was "pldag-0.7.5.tar", max compression
```

## Comparing `pldag-0.7.4.tar` & `pldag-0.7.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.4/LICENSE
--rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.4/README.md
--rw-r--r--   0        0        0    31594 2024-04-25 07:47:29.709670 pldag-0.7.4/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.7.4/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.7.4/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-04-25 07:48:03.323370 pldag-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.5/LICENSE
+-rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.5/README.md
+-rw-r--r--   0        0        0    32526 2024-04-26 06:40:47.732022 pldag-0.7.5/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.7.5/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.7.5/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-04-26 06:47:19.456855 pldag-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.5/PKG-INFO
```

### Comparing `pldag-0.7.4/LICENSE` & `pldag-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.7.4/README.md` & `pldag-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.7.4/pldag/__init__.py` & `pldag-0.7.5/pldag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,14 +318,42 @@
             )
         )
     
     def get(self, *id: str) -> np.ndarray:
         """Get the bounds of the given ID(s)"""
         return self._dvec[list(map(self._col, id))]
     
+    def delete(self, id: str) -> True:
+        """
+            Delete the given ID.
+        """
+        try:
+            if id in self.composites:
+                row_id = self._row(id)
+                self._bvec = np.delete(self._bvec, row_id)
+                self._nvec = np.delete(self._nvec, row_id)
+                self._amap = dict(filter(lambda x: x[1] != id, self._amap.items()))
+                self._amat = np.delete(self._amat, row_id, axis=0)
+
+            col_id = self._col(id)
+            self._amat = np.delete(self._amat, col_id, axis=1)
+            self._dvec = np.delete(self._dvec, col_id)
+            self._cvec = np.delete(self._cvec, col_id)
+            del self._imap[id]
+            self._imap = dict(
+                zip(
+                    self._imap.keys(),
+                    range(len(self._imap))
+                )
+            )
+
+            return True
+        except:
+            return False
+    
     def exists(self, id: str) -> bool:
         """Check if the given id exists"""
         return (id in self._imap)
     
     def dependencies(self, id: str) -> Set[str]:
         """
             Get the dependencies of the given ID.
```

### Comparing `pldag-0.7.4/pldag/solver/glpk_solver.py` & `pldag-0.7.5/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.7.4/PKG-INFO` & `pldag-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.7.4
+Version: 0.7.5
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

