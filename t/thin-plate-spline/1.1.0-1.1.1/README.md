# Comparing `tmp/thin-plate-spline-1.1.0.tar.gz` & `tmp/thin_plate_spline-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thin-plate-spline-1.1.0.tar", last modified: Thu Mar 16 09:56:10 2023, max compression
+gzip compressed data, was "thin_plate_spline-1.1.1.tar", last modified: Fri Apr 26 09:01:35 2024, max compression
```

## Comparing `thin-plate-spline-1.1.0.tar` & `thin_plate_spline-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:56:10.862037 thin-plate-spline-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-16 09:55:56.000000 thin-plate-spline-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-03-16 09:56:10.862037 thin-plate-spline-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-16 09:55:56.000000 thin-plate-spline-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-16 09:55:56.000000 thin-plate-spline-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-16 09:56:10.862037 thin-plate-spline-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-16 09:55:56.000000 thin-plate-spline-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:56:10.862037 thin-plate-spline-1.1.0/thin_plate_spline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-03-16 09:56:10.000000 thin-plate-spline-1.1.0/thin_plate_spline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-16 09:56:10.000000 thin-plate-spline-1.1.0/thin_plate_spline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 09:56:10.000000 thin-plate-spline-1.1.0/thin_plate_spline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 09:56:10.000000 thin-plate-spline-1.1.0/thin_plate_spline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-16 09:56:10.000000 thin-plate-spline-1.1.0/thin_plate_spline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:56:10.862037 thin-plate-spline-1.1.0/tps/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-16 09:55:56.000000 thin-plate-spline-1.1.0/tps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:55:56.000000 thin-plate-spline-1.1.0/tps/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-03-16 09:55:56.000000 thin-plate-spline-1.1.0/tps/thin_plate_spline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:01:35.149549 thin_plate_spline-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 09:01:29.000000 thin_plate_spline-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-26 09:01:35.149549 thin_plate_spline-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-26 09:01:29.000000 thin_plate_spline-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 09:01:29.000000 thin_plate_spline-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-26 09:01:35.149549 thin_plate_spline-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 09:01:29.000000 thin_plate_spline-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:01:35.149549 thin_plate_spline-1.1.1/thin_plate_spline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-26 09:01:35.000000 thin_plate_spline-1.1.1/thin_plate_spline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-26 09:01:35.000000 thin_plate_spline-1.1.1/thin_plate_spline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:01:35.000000 thin_plate_spline-1.1.1/thin_plate_spline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 09:01:35.000000 thin_plate_spline-1.1.1/thin_plate_spline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-26 09:01:35.000000 thin_plate_spline-1.1.1/thin_plate_spline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:01:35.149549 thin_plate_spline-1.1.1/tps/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-26 09:01:29.000000 thin_plate_spline-1.1.1/tps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 09:01:29.000000 thin_plate_spline-1.1.1/tps/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-26 09:01:29.000000 thin_plate_spline-1.1.1/tps/thin_plate_spline.py
```

### Comparing `thin-plate-spline-1.1.0/LICENSE` & `thin_plate_spline-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thin-plate-spline-1.1.0/PKG-INFO` & `thin_plate_spline-1.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thin-plate-spline
-Version: 1.1.0
+Version: 1.1.1
 Summary: Thin Plate Spline implementation with numpy/scipy
 Home-page: https://github.com/raphaelreme/tps
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: interpolation,numpy,machine learning
 Classifier: Development Status :: 4 - Beta
@@ -12,25 +12,28 @@
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
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 # tps
 
 [![Lint and Test](https://github.com/raphaelreme/tps/actions/workflows/tests.yml/badge.svg)](https://github.com/raphaelreme/tps/actions/workflows/tests.yml)
 
 
 Implementation of Thin Plate Spline.
-(For a faster implementation in torch, look at tps-torch)
+(For a faster implementation in torch, look at [torch-tps](https://github.com/raphaelreme/torch-tps))
 
 
 ## Install
 
 ### Pip
 
 ```bash
@@ -41,16 +44,15 @@
 
 Not yet available
 
 
 ## Getting started
 
 ```python
-
-import numpy 
+import numpy as np
 from tps import ThinPlateSpline
 
 # Some data
 X_c = np.random.normal(0, 1, (800, 3))
 X_t = np.random.normal(0, 2, (800, 2))
 X = np.random.normal(0, 1, (300, 3))
 
@@ -60,15 +62,26 @@
 # Fit the control and target points
 tps.fit(X_c, X_t)
 
 # Transform new points
 Y = tps.transform(X)
 ```
 
-Also have a look at `example.py`
+## Examples
+
+We provide different examples in the `example` folder. (From interpolation, to multidimensional cases and image warping).
+
+
+### Image warping
+
+The elastic deformation of TPS can be used for image warping. Here is an example of tps to increase/decrease the size of the center of the image or using random control points:
+
+![Input Image](example/images/dog_with_bbox.png)![Increased Image](example/images/increase_warped_dog.png)![Decreased Image](example/images/decrease_warped_dog.png)![Warped Image](example/images/random_warped_dog.png)
+
+Have a look at `example/image_warping.py`.
 
 
 ## Build and Deploy
 
 ```bash
 $ python -m build
 $ python -m twine upload dist/*
```

### Comparing `thin-plate-spline-1.1.0/setup.cfg` & `thin_plate_spline-1.1.1/setup.cfg`

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
 	numpy
 	scipy
```

### Comparing `thin-plate-spline-1.1.0/thin_plate_spline.egg-info/PKG-INFO` & `thin_plate_spline-1.1.1/thin_plate_spline.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thin-plate-spline
-Version: 1.1.0
+Version: 1.1.1
 Summary: Thin Plate Spline implementation with numpy/scipy
 Home-page: https://github.com/raphaelreme/tps
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: interpolation,numpy,machine learning
 Classifier: Development Status :: 4 - Beta
@@ -12,25 +12,28 @@
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
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 # tps
 
 [![Lint and Test](https://github.com/raphaelreme/tps/actions/workflows/tests.yml/badge.svg)](https://github.com/raphaelreme/tps/actions/workflows/tests.yml)
 
 
 Implementation of Thin Plate Spline.
-(For a faster implementation in torch, look at tps-torch)
+(For a faster implementation in torch, look at [torch-tps](https://github.com/raphaelreme/torch-tps))
 
 
 ## Install
 
 ### Pip
 
 ```bash
@@ -41,16 +44,15 @@
 
 Not yet available
 
 
 ## Getting started
 
 ```python
-
-import numpy 
+import numpy as np
 from tps import ThinPlateSpline
 
 # Some data
 X_c = np.random.normal(0, 1, (800, 3))
 X_t = np.random.normal(0, 2, (800, 2))
 X = np.random.normal(0, 1, (300, 3))
 
@@ -60,15 +62,26 @@
 # Fit the control and target points
 tps.fit(X_c, X_t)
 
 # Transform new points
 Y = tps.transform(X)
 ```
 
-Also have a look at `example.py`
+## Examples
+
+We provide different examples in the `example` folder. (From interpolation, to multidimensional cases and image warping).
+
+
+### Image warping
+
+The elastic deformation of TPS can be used for image warping. Here is an example of tps to increase/decrease the size of the center of the image or using random control points:
+
+![Input Image](example/images/dog_with_bbox.png)![Increased Image](example/images/increase_warped_dog.png)![Decreased Image](example/images/decrease_warped_dog.png)![Warped Image](example/images/random_warped_dog.png)
+
+Have a look at `example/image_warping.py`.
 
 
 ## Build and Deploy
 
 ```bash
 $ python -m build
 $ python -m twine upload dist/*
```

### Comparing `thin-plate-spline-1.1.0/tps/thin_plate_spline.py` & `thin_plate_spline-1.1.1/tps/thin_plate_spline.py`

 * *Files identical despite different names*

