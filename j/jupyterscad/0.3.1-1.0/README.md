# Comparing `tmp/jupyterscad-0.3.1.tar.gz` & `tmp/jupyterscad-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterscad-0.3.1.tar", last modified: Mon Feb 26 20:09:46 2024, max compression
+gzip compressed data, was "jupyterscad-1.0.tar", last modified: Fri Apr 26 19:16:02 2024, max compression
```

## Comparing `jupyterscad-0.3.1.tar` & `jupyterscad-1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:09:46.642678 jupyterscad-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-02-26 20:09:23.000000 jupyterscad-0.3.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-26 20:09:23.000000 jupyterscad-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-02-26 20:09:46.642678 jupyterscad-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-02-26 20:09:23.000000 jupyterscad-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-26 20:09:23.000000 jupyterscad-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 20:09:46.642678 jupyterscad-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:09:46.634678 jupyterscad-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:09:46.638678 jupyterscad-0.3.1/src/jupyterscad/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-26 20:09:23.000000 jupyterscad-0.3.1/src/jupyterscad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-02-26 20:09:23.000000 jupyterscad-0.3.1/src/jupyterscad/_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-02-26 20:09:23.000000 jupyterscad-0.3.1/src/jupyterscad/_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-26 20:09:23.000000 jupyterscad-0.3.1/src/jupyterscad/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:09:46.638678 jupyterscad-0.3.1/src/jupyterscad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-02-26 20:09:46.000000 jupyterscad-0.3.1/src/jupyterscad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-26 20:09:46.000000 jupyterscad-0.3.1/src/jupyterscad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 20:09:46.000000 jupyterscad-0.3.1/src/jupyterscad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-26 20:09:46.000000 jupyterscad-0.3.1/src/jupyterscad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-26 20:09:46.000000 jupyterscad-0.3.1/src/jupyterscad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:09:46.638678 jupyterscad-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-02-26 20:09:23.000000 jupyterscad-0.3.1/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-26 20:09:23.000000 jupyterscad-0.3.1/tests/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:16:02.236003 jupyterscad-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-04-26 19:15:48.000000 jupyterscad-1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-26 19:15:48.000000 jupyterscad-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-26 19:16:02.236003 jupyterscad-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-26 19:15:48.000000 jupyterscad-1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-26 19:15:48.000000 jupyterscad-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:16:02.236003 jupyterscad-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:16:02.232003 jupyterscad-1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:16:02.236003 jupyterscad-1.0/src/jupyterscad/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-26 19:15:48.000000 jupyterscad-1.0/src/jupyterscad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-26 19:15:48.000000 jupyterscad-1.0/src/jupyterscad/_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-26 19:15:48.000000 jupyterscad-1.0/src/jupyterscad/_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-26 19:15:48.000000 jupyterscad-1.0/src/jupyterscad/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:16:02.236003 jupyterscad-1.0/src/jupyterscad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-26 19:16:02.000000 jupyterscad-1.0/src/jupyterscad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-26 19:16:02.000000 jupyterscad-1.0/src/jupyterscad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:16:02.000000 jupyterscad-1.0/src/jupyterscad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 19:16:02.000000 jupyterscad-1.0/src/jupyterscad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 19:16:02.000000 jupyterscad-1.0/src/jupyterscad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:16:02.236003 jupyterscad-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-26 19:15:48.000000 jupyterscad-1.0/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-26 19:15:48.000000 jupyterscad-1.0/tests/test_view.py
```

### Comparing `jupyterscad-0.3.1/COPYING` & `jupyterscad-1.0/COPYING`

 * *Files identical despite different names*

### Comparing `jupyterscad-0.3.1/PKG-INFO` & `jupyterscad-1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: jupyterscad
-Version: 0.3.1
+Version: 1.0
 Summary: Solid 3D Cad (SCAD) renderer and viewer for Jupyter
 Author: Jennifer Reiber Kyle
 License: GPLv3
 Project-URL: Homepage, https://jreiberkyle.github.io/jupyterscad/
 Project-URL: Documentation, https://jreiberkyle.github.io/jupyterscad/
 Project-URL: Repository, https://github.com/jreiberkyle/jupyterscad
 Project-URL: Changelog, https://github.com/jreiberkyle/jupyterscad/blob/main/CHANGELOG.md
 Keywords: openscad,scad,jupyter,jupyterlab,notebook,viewer,render,solidpython,solidpython2
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 6 - Mature
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYING
 Requires-Dist: numpy-stl
 Requires-Dist: ipywidgets
@@ -29,14 +29,23 @@
 # Jupyter SCAD: SCAD in Jupyter
 
 
 Jupyter SCAD provides rendering and interactive visualization for 3D objects described in [SolidPython2](https://github.com/jeff-dh/SolidPython) within a Jupyter notebook. Additionally, it provides interactive visualization for STLs.
 
 This program is focused on the use case of generating stl files with Python (aka SolidPython2) interactively within a Jupyter notebook.
 
+## Status: MATURE
+
+This project has reached it's goal, a basic Jupyter notebook viewer for SolidPython2. Any further improvements are best served by just using the OpenSCAD
+GUI (see Alternatives below).
+
+At this time, the only work that is planned for this project is bugfixes. If you are interested in continuing to add functionality,
+make an issue expressing your interest and we can discuss passing the baton.
+
+
 ## Documentation
 
 Documentation is hosted at https://jreiberkyle.github.io/jupyterscad/.
 
 ## Quick Start
 
 Jupyter SCAD can be installed with `pip`:
```

### Comparing `jupyterscad-0.3.1/README.md` & `jupyterscad-1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Jupyter SCAD: SCAD in Jupyter
 
 
 Jupyter SCAD provides rendering and interactive visualization for 3D objects described in [SolidPython2](https://github.com/jeff-dh/SolidPython) within a Jupyter notebook. Additionally, it provides interactive visualization for STLs.
 
 This program is focused on the use case of generating stl files with Python (aka SolidPython2) interactively within a Jupyter notebook.
 
+## Status: MATURE
+
+This project has reached it's goal, a basic Jupyter notebook viewer for SolidPython2. Any further improvements are best served by just using the OpenSCAD
+GUI (see Alternatives below).
+
+At this time, the only work that is planned for this project is bugfixes. If you are interested in continuing to add functionality,
+make an issue expressing your interest and we can discuss passing the baton.
+
+
 ## Documentation
 
 Documentation is hosted at https://jreiberkyle.github.io/jupyterscad/.
 
 ## Quick Start
 
 Jupyter SCAD can be installed with `pip`:
```

### Comparing `jupyterscad-0.3.1/pyproject.toml` & `jupyterscad-1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jupyterscad"
-version = "0.3.1"
+version = "1.0"
 authors = [{name = "Jennifer Reiber Kyle"}]
 description = "Solid 3D Cad (SCAD) renderer and viewer for Jupyter"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "openscad",
     "scad",
@@ -13,15 +13,15 @@
     "notebook",
     "viewer",
     "render",
     "solidpython",
     "solidpython2"]
 license = {text = "GPLv3"}
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 6 - Mature",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "numpy-stl",
     "ipywidgets",
     "pythreejs",
 ]
```

### Comparing `jupyterscad-0.3.1/src/jupyterscad/__init__.py` & `jupyterscad-1.0/src/jupyterscad/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterscad-0.3.1/src/jupyterscad/_render.py` & `jupyterscad-1.0/src/jupyterscad/_render.py`

 * *Files identical despite different names*

### Comparing `jupyterscad-0.3.1/src/jupyterscad/_view.py` & `jupyterscad-1.0/src/jupyterscad/_view.py`

 * *Files identical despite different names*

### Comparing `jupyterscad-0.3.1/src/jupyterscad/exceptions.py` & `jupyterscad-1.0/src/jupyterscad/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupyterscad-0.3.1/src/jupyterscad.egg-info/PKG-INFO` & `jupyterscad-1.0/src/jupyterscad.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: jupyterscad
-Version: 0.3.1
+Version: 1.0
 Summary: Solid 3D Cad (SCAD) renderer and viewer for Jupyter
 Author: Jennifer Reiber Kyle
 License: GPLv3
 Project-URL: Homepage, https://jreiberkyle.github.io/jupyterscad/
 Project-URL: Documentation, https://jreiberkyle.github.io/jupyterscad/
 Project-URL: Repository, https://github.com/jreiberkyle/jupyterscad
 Project-URL: Changelog, https://github.com/jreiberkyle/jupyterscad/blob/main/CHANGELOG.md
 Keywords: openscad,scad,jupyter,jupyterlab,notebook,viewer,render,solidpython,solidpython2
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 6 - Mature
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYING
 Requires-Dist: numpy-stl
 Requires-Dist: ipywidgets
@@ -29,14 +29,23 @@
 # Jupyter SCAD: SCAD in Jupyter
 
 
 Jupyter SCAD provides rendering and interactive visualization for 3D objects described in [SolidPython2](https://github.com/jeff-dh/SolidPython) within a Jupyter notebook. Additionally, it provides interactive visualization for STLs.
 
 This program is focused on the use case of generating stl files with Python (aka SolidPython2) interactively within a Jupyter notebook.
 
+## Status: MATURE
+
+This project has reached it's goal, a basic Jupyter notebook viewer for SolidPython2. Any further improvements are best served by just using the OpenSCAD
+GUI (see Alternatives below).
+
+At this time, the only work that is planned for this project is bugfixes. If you are interested in continuing to add functionality,
+make an issue expressing your interest and we can discuss passing the baton.
+
+
 ## Documentation
 
 Documentation is hosted at https://jreiberkyle.github.io/jupyterscad/.
 
 ## Quick Start
 
 Jupyter SCAD can be installed with `pip`:
```

### Comparing `jupyterscad-0.3.1/tests/test_render.py` & `jupyterscad-1.0/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `jupyterscad-0.3.1/tests/test_view.py` & `jupyterscad-1.0/tests/test_view.py`

 * *Files identical despite different names*

