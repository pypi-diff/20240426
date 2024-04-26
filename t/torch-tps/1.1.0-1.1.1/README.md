# Comparing `tmp/torch-tps-1.1.0.tar.gz` & `tmp/torch_tps-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-tps-1.1.0.tar", last modified: Thu Mar 16 10:20:32 2023, max compression
+gzip compressed data, was "torch_tps-1.1.1.tar", last modified: Fri Apr 26 09:19:29 2024, max compression
```

## Comparing `torch-tps-1.1.0.tar` & `torch_tps-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:20:32.947307 torch-tps-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-16 10:20:20.000000 torch-tps-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-16 10:20:32.947307 torch-tps-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-16 10:20:20.000000 torch-tps-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-16 10:20:20.000000 torch-tps-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-16 10:20:32.947307 torch-tps-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-16 10:20:20.000000 torch-tps-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:20:32.947307 torch-tps-1.1.0/torch_tps/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-16 10:20:20.000000 torch-tps-1.1.0/torch_tps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:20:20.000000 torch-tps-1.1.0/torch_tps/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-03-16 10:20:20.000000 torch-tps-1.1.0/torch_tps/thin_plate_spline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:20:32.947307 torch-tps-1.1.0/torch_tps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-16 10:20:32.000000 torch-tps-1.1.0/torch_tps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-16 10:20:32.000000 torch-tps-1.1.0/torch_tps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 10:20:32.000000 torch-tps-1.1.0/torch_tps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-16 10:20:32.000000 torch-tps-1.1.0/torch_tps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 10:20:32.000000 torch-tps-1.1.0/torch_tps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:19:29.188190 torch_tps-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 09:19:23.000000 torch_tps-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-26 09:19:29.188190 torch_tps-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-26 09:19:23.000000 torch_tps-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 09:19:23.000000 torch_tps-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-26 09:19:29.192190 torch_tps-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 09:19:23.000000 torch_tps-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:19:29.188190 torch_tps-1.1.1/torch_tps/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-26 09:19:23.000000 torch_tps-1.1.1/torch_tps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 09:19:23.000000 torch_tps-1.1.1/torch_tps/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-26 09:19:23.000000 torch_tps-1.1.1/torch_tps/thin_plate_spline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:19:29.188190 torch_tps-1.1.1/torch_tps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-26 09:19:29.000000 torch_tps-1.1.1/torch_tps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-26 09:19:29.000000 torch_tps-1.1.1/torch_tps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:19:29.000000 torch_tps-1.1.1/torch_tps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 09:19:29.000000 torch_tps-1.1.1/torch_tps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 09:19:29.000000 torch_tps-1.1.1/torch_tps.egg-info/top_level.txt
```

### Comparing `torch-tps-1.1.0/LICENSE` & `torch_tps-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-tps-1.1.0/PKG-INFO` & `torch_tps-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-tps
-Version: 1.1.0
+Version: 1.1.1
 Summary: Thin Plate Spline implementation with PyTorch
 Home-page: https://github.com/raphaelreme/torch-tps
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: interpolation,pytorch,machine learning
 Classifier: Development Status :: 4 - Beta
@@ -12,24 +12,26 @@
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
+Requires-Dist: torch
 
 # torch-tps
 
 [![Lint and Test](https://github.com/raphaelreme/torch-tps/actions/workflows/tests.yml/badge.svg)](https://github.com/raphaelreme/torch-tps/actions/workflows/tests.yml)
 
 Implementation of Thin Plate Spline.
-(See numpy implementation with thin-plate-spline library)
+(See numpy implementation with [thin-plate-spline](https://github.com/raphaelreme/tps) library)
 
 
 ## Install
 
 ### Pip
 
 ```bash
@@ -59,16 +61,26 @@
 # Fit the control and target points
 tps.fit(X_c, X_t)
 
 # Transform new points
 Y = tps.transform(X)
 ```
 
-Also have a look at `example.py`
+## Examples
 
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
```

### Comparing `torch-tps-1.1.0/setup.cfg` & `torch_tps-1.1.1/setup.cfg`

 * *Files 27% similar despite different names*

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
 	torch
 include_package_data = False
```

### Comparing `torch-tps-1.1.0/torch_tps/thin_plate_spline.py` & `torch_tps-1.1.1/torch_tps/thin_plate_spline.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 torch.hstack([phi + self.alpha * torch.eye(n_c, device=self.device), X_p]),
                 torch.hstack([X_p.T, torch.zeros((d_s + 1, d_s + 1), device=self.device)]),
             ]
         )
 
         Y = torch.vstack([Y, torch.zeros((d_s + 1, Y.shape[1]), device=self.device)])
 
-        self.parameters = torch.linalg.solve(A, Y)
+        self.parameters = torch.linalg.solve(A, Y)  # pylint: disable=not-callable
         self._fitted = True
 
         return self
 
     def transform(self, X: torch.Tensor) -> torch.Tensor:
         """Map source space to target space
```

### Comparing `torch-tps-1.1.0/torch_tps.egg-info/PKG-INFO` & `torch_tps-1.1.1/torch_tps.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-tps
-Version: 1.1.0
+Version: 1.1.1
 Summary: Thin Plate Spline implementation with PyTorch
 Home-page: https://github.com/raphaelreme/torch-tps
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: interpolation,pytorch,machine learning
 Classifier: Development Status :: 4 - Beta
@@ -12,24 +12,26 @@
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
+Requires-Dist: torch
 
 # torch-tps
 
 [![Lint and Test](https://github.com/raphaelreme/torch-tps/actions/workflows/tests.yml/badge.svg)](https://github.com/raphaelreme/torch-tps/actions/workflows/tests.yml)
 
 Implementation of Thin Plate Spline.
-(See numpy implementation with thin-plate-spline library)
+(See numpy implementation with [thin-plate-spline](https://github.com/raphaelreme/tps) library)
 
 
 ## Install
 
 ### Pip
 
 ```bash
@@ -59,16 +61,26 @@
 # Fit the control and target points
 tps.fit(X_c, X_t)
 
 # Transform new points
 Y = tps.transform(X)
 ```
 
-Also have a look at `example.py`
+## Examples
 
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
```

