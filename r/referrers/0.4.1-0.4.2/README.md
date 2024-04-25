# Comparing `tmp/referrers-0.4.1.tar.gz` & `tmp/referrers-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "referrers-0.4.1.tar", max compression
+gzip compressed data, was "referrers-0.4.2.tar", max compression
```

## Comparing `referrers-0.4.1.tar` & `referrers-0.4.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-04-25 15:54:48.793777 referrers-0.4.1/LICENSE
--rw-r--r--   0        0        0     8135 2024-04-25 15:54:48.793777 referrers-0.4.1/README.md
--rw-r--r--   0        0        0      372 2024-04-25 15:54:48.793777 referrers-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      130 2024-04-25 15:54:48.793777 referrers-0.4.1/src/referrers/__init__.py
--rw-r--r--   0        0        0    38820 2024-04-25 15:54:48.793777 referrers-0.4.1/src/referrers/impl.py
--rw-r--r--   0        0        0     8668 1970-01-01 00:00:00.000000 referrers-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 17:17:03.976040 referrers-0.4.2/LICENSE
+-rw-r--r--   0        0        0     8135 2024-04-25 17:17:03.976040 referrers-0.4.2/README.md
+-rw-r--r--   0        0        0      372 2024-04-25 17:17:03.976040 referrers-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-04-25 17:17:03.976040 referrers-0.4.2/src/referrers/__init__.py
+-rw-r--r--   0        0        0    39364 2024-04-25 17:17:03.976040 referrers-0.4.2/src/referrers/impl.py
+-rw-r--r--   0        0        0     8668 1970-01-01 00:00:00.000000 referrers-0.4.2/PKG-INFO
```

### Comparing `referrers-0.4.1/LICENSE` & `referrers-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `referrers-0.4.1/README.md` & `referrers-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `referrers-0.4.1/src/referrers/impl.py` & `referrers-0.4.2/src/referrers/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,23 +310,31 @@
 
 
 class ClosureVariableNameFinder(NameFinder):
     def __init__(self):
         self._closure_function_names: Dict[int, List[str]] = collections.defaultdict(
             list
         )
-        for var_value in gc.get_objects():
-            if (
-                inspect.isroutine(var_value)
-                and hasattr(var_value, "__closure__")
-                and var_value.__closure__
-            ):
-                for cell in var_value.__closure__:
-                    self._closure_function_names[id(cell.cell_contents)].append(
-                        f"{str(var_value)} ({_TYPE_CLOSURE})"
+        for obj in gc.get_objects():
+            if inspect.isfunction(obj) or inspect.ismethod(obj):
+                try:
+                    closure_vars = inspect.getclosurevars(obj)
+                except TypeError:
+                    # It's not clear why, but some things that claim to be functions
+                    # return a TypeError with "is not a Python function" here, so we
+                    # just skip them.
+                    continue
+                except ValueError:
+                    # The inspect.getclosurevars fuction raises a ValueError with
+                    # "Cell is empty" in some cases. it's not clear how to avoid this
+                    # so we just skip these cases.
+                    continue
+                for var_name, var_value in closure_vars.nonlocals.items():
+                    self._closure_function_names[id(var_value)].append(
+                        f"{str(obj)}.{var_name} ({_TYPE_CLOSURE})"
                     )
 
     def get_names(self, target_object: Any) -> Set[str]:
         return set(self._closure_function_names.get(id(target_object), []))
 
     def get_type(self) -> str:
         return _TYPE_CLOSURE
```

### Comparing `referrers-0.4.1/PKG-INFO` & `referrers-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: referrers
-Version: 0.4.1
+Version: 0.4.2
 Summary: Finds the graph of referrers for a Python object
 Author: Neil Ferguson
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

