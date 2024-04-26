# Comparing `tmp/celldega-0.1.7.tar.gz` & `tmp/celldega-0.1.8.tar.gz`

## Comparing `celldega-0.1.7.tar` & `celldega-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/__init__.py
--rw-r--r--   0        0        0    16313 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/pre/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/static/widget.css
--rw-r--r--   0        0        0  6847229 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/static/widget.js
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/viz/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/viz/widget.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 celldega-0.1.7/.gitignore
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 celldega-0.1.7/README.md
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 celldega-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 celldega-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 celldega-0.1.8/src/celldega/__init__.py
+-rw-r--r--   0        0        0    16313 2020-02-02 00:00:00.000000 celldega-0.1.8/src/celldega/pre/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 celldega-0.1.8/src/celldega/static/widget.css
+-rw-r--r--   0        0        0  6847229 2020-02-02 00:00:00.000000 celldega-0.1.8/src/celldega/static/widget.js
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 celldega-0.1.8/src/celldega/viz/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 celldega-0.1.8/src/celldega/viz/widget.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 celldega-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 celldega-0.1.8/README.md
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 celldega-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 celldega-0.1.8/PKG-INFO
```

### Comparing `celldega-0.1.7/src/celldega/pre/__init__.py` & `celldega-0.1.8/src/celldega/pre/__init__.py`

 * *Files identical despite different names*

### Comparing `celldega-0.1.7/src/celldega/static/widget.js` & `celldega-0.1.8/src/celldega/static/widget.js`

 * *Files identical despite different names*

### Comparing `celldega-0.1.7/src/celldega/viz/widget.py` & `celldega-0.1.8/src/celldega/viz/widget.py`

 * *Files identical despite different names*

### Comparing `celldega-0.1.7/README.md` & `celldega-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `celldega-0.1.7/pyproject.toml` & `celldega-0.1.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "celldega"
-version = "0.1.7"
+version = "0.1.8    "
 dependencies = [
-    "anywidget~=0.9.7",
+    "anywidget==0.9.6",
     "pandas~=2.2.2",
-    "pyvips~=2.2.2",
+    # "pyvips~=2.2.2",
     "geopandas~=0.14.3",
     "pyarrow~=15.0.2",
     "matplotlib~=3.8.4",
     "geopandas~=0.14.3",    
     "zarr~=2.17.2",
     "tifffile~=2024.4.18",
     "imagecodecs~=2024.1.1"
```

### Comparing `celldega-0.1.7/PKG-INFO` & `celldega-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.3
 Name: celldega
-Version: 0.1.7
-Requires-Dist: anywidget~=0.9.7
+Version: 0.1.8
+Requires-Dist: anywidget==0.9.6
 Requires-Dist: geopandas~=0.14.3
 Requires-Dist: imagecodecs~=2024.1.1
 Requires-Dist: matplotlib~=3.8.4
 Requires-Dist: pandas~=2.2.2
 Requires-Dist: pyarrow~=15.0.2
-Requires-Dist: pyvips~=2.2.2
 Requires-Dist: tifffile~=2024.4.18
 Requires-Dist: zarr~=2.17.2
 Provides-Extra: dev
 Requires-Dist: jupyterlab; extra == 'dev'
 Requires-Dist: watchfiles; extra == 'dev'
 Description-Content-Type: text/markdown
```

