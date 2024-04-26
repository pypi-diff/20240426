# Comparing `tmp/celldega-0.1.6.tar.gz` & `tmp/celldega-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celldega-0.1.6.tar", last modified: Fri Apr 26 17:26:24 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `celldega-0.1.6.tar` & `celldega-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,10 @@
-drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.239168 celldega-0.1.6/
--rw-r--r--   0 feni       (503) staff       (20)     1526 2024-04-26 17:26:24.238843 celldega-0.1.6/PKG-INFO
--rw-r--r--   0 feni       (503) staff       (20)     1009 2024-04-23 17:00:35.000000 celldega-0.1.6/README.md
--rw-r--r--   0 feni       (503) staff       (20)      930 2024-04-26 17:23:39.000000 celldega-0.1.6/pyproject.toml
--rw-r--r--   0 feni       (503) staff       (20)       38 2024-04-26 17:26:24.239230 celldega-0.1.6/setup.cfg
-drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.234991 celldega-0.1.6/src/
-drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.235781 celldega-0.1.6/src/celldega/
--rw-r--r--   0 feni       (503) staff       (20)      285 2024-04-23 17:00:35.000000 celldega-0.1.6/src/celldega/__init__.py
-drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.237309 celldega-0.1.6/src/celldega/pre/
--rw-r--r--   0 feni       (503) staff       (20)    16313 2024-04-26 17:21:20.000000 celldega-0.1.6/src/celldega/pre/__init__.py
-drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.237976 celldega-0.1.6/src/celldega/viz/
--rw-r--r--   0 feni       (503) staff       (20)       66 2024-04-23 17:00:35.000000 celldega-0.1.6/src/celldega/viz/__init__.py
--rw-r--r--   0 feni       (503) staff       (20)     1702 2024-04-25 18:31:07.000000 celldega-0.1.6/src/celldega/viz/widget.py
-drwxr-xr-x   0 feni       (503) staff       (20)        0 2024-04-26 17:26:24.238339 celldega-0.1.6/src/celldega.egg-info/
--rw-r--r--   0 feni       (503) staff       (20)     1526 2024-04-26 17:26:24.000000 celldega-0.1.6/src/celldega.egg-info/PKG-INFO
--rw-r--r--   0 feni       (503) staff       (20)      313 2024-04-26 17:26:24.000000 celldega-0.1.6/src/celldega.egg-info/SOURCES.txt
--rw-r--r--   0 feni       (503) staff       (20)        1 2024-04-26 17:26:24.000000 celldega-0.1.6/src/celldega.egg-info/dependency_links.txt
--rw-r--r--   0 feni       (503) staff       (20)      199 2024-04-26 17:26:24.000000 celldega-0.1.6/src/celldega.egg-info/requires.txt
--rw-r--r--   0 feni       (503) staff       (20)        9 2024-04-26 17:26:24.000000 celldega-0.1.6/src/celldega.egg-info/top_level.txt
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/__init__.py
+-rw-r--r--   0        0        0    16313 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/pre/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/static/widget.css
+-rw-r--r--   0        0        0  6847229 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/static/widget.js
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/viz/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 celldega-0.1.7/src/celldega/viz/widget.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 celldega-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 celldega-0.1.7/README.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 celldega-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 celldega-0.1.7/PKG-INFO
```

### Comparing `celldega-0.1.6/PKG-INFO` & `celldega-0.1.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: celldega
-Version: 0.1.6
-Description-Content-Type: text/markdown
+Version: 0.1.7
 Requires-Dist: anywidget~=0.9.7
-Requires-Dist: pandas~=2.2.2
-Requires-Dist: pyvips~=2.2.2
 Requires-Dist: geopandas~=0.14.3
-Requires-Dist: pyarrow~=15.0.2
+Requires-Dist: imagecodecs~=2024.1.1
 Requires-Dist: matplotlib~=3.8.4
-Requires-Dist: geopandas~=0.14.3
-Requires-Dist: zarr~=2.17.2
+Requires-Dist: pandas~=2.2.2
+Requires-Dist: pyarrow~=15.0.2
+Requires-Dist: pyvips~=2.2.2
 Requires-Dist: tifffile~=2024.4.18
-Requires-Dist: imagecodecs~=2024.1.1
+Requires-Dist: zarr~=2.17.2
 Provides-Extra: dev
-Requires-Dist: watchfiles; extra == "dev"
-Requires-Dist: jupyterlab; extra == "dev"
+Requires-Dist: jupyterlab; extra == 'dev'
+Requires-Dist: watchfiles; extra == 'dev'
+Description-Content-Type: text/markdown
 
 # celldega
 
 ## Installation
 
 ```sh
 pip install celldega
@@ -55,7 +54,22 @@
 npm run dev
 ```
 
 Open `example.ipynb` in JupyterLab, VS Code, or your favorite editor
 to start developing. Changes made in `js/` will be reflected
 in the notebook.
 
+### PyPI
+Increment version in `project.toml` and
+
+```
+$ hatch build
+$ hatch publish
+```
+
+### NPM
+Increment version in `package.json` and
+
+```
+$ npm build
+$ npm publish
+```
```

### Comparing `celldega-0.1.6/pyproject.toml` & `celldega-0.1.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
 [project]
 name = "celldega"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
     "anywidget~=0.9.7",
     "pandas~=2.2.2",
     "pyvips~=2.2.2",
     "geopandas~=0.14.3",
     "pyarrow~=15.0.2",
     "matplotlib~=3.8.4",
```

### Comparing `celldega-0.1.6/src/celldega/pre/__init__.py` & `celldega-0.1.7/src/celldega/pre/__init__.py`

 * *Files identical despite different names*

### Comparing `celldega-0.1.6/src/celldega/viz/widget.py` & `celldega-0.1.7/src/celldega/viz/widget.py`

 * *Files identical despite different names*

### Comparing `celldega-0.1.6/src/celldega.egg-info/PKG-INFO` & `celldega-0.1.7/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: celldega
-Version: 0.1.6
-Description-Content-Type: text/markdown
-Requires-Dist: anywidget~=0.9.7
-Requires-Dist: pandas~=2.2.2
-Requires-Dist: pyvips~=2.2.2
-Requires-Dist: geopandas~=0.14.3
-Requires-Dist: pyarrow~=15.0.2
-Requires-Dist: matplotlib~=3.8.4
-Requires-Dist: geopandas~=0.14.3
-Requires-Dist: zarr~=2.17.2
-Requires-Dist: tifffile~=2024.4.18
-Requires-Dist: imagecodecs~=2024.1.1
-Provides-Extra: dev
-Requires-Dist: watchfiles; extra == "dev"
-Requires-Dist: jupyterlab; extra == "dev"
-
 # celldega
 
 ## Installation
 
 ```sh
 pip install celldega
 ```
@@ -55,7 +37,22 @@
 npm run dev
 ```
 
 Open `example.ipynb` in JupyterLab, VS Code, or your favorite editor
 to start developing. Changes made in `js/` will be reflected
 in the notebook.
 
+### PyPI
+Increment version in `project.toml` and
+
+```
+$ hatch build
+$ hatch publish
+```
+
+### NPM
+Increment version in `package.json` and
+
+```
+$ npm build
+$ npm publish
+```
```

