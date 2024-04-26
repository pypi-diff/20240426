# Comparing `tmp/pylapy-0.1.0.tar.gz` & `tmp/pylapy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylapy-0.1.0.tar", last modified: Wed Oct  4 09:06:13 2023, max compression
+gzip compressed data, was "pylapy-0.1.1.tar", last modified: Fri Apr 26 17:01:57 2024, max compression
```

## Comparing `pylapy-0.1.0.tar` & `pylapy-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:06:13.268076 pylapy-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-10-04 09:05:56.000000 pylapy-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2023-10-04 09:06:13.268076 pylapy-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2023-10-04 09:05:56.000000 pylapy-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:06:13.264076 pylapy-0.1.0/pylapy/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-10-04 09:05:56.000000 pylapy-0.1.0/pylapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11956 2023-10-04 09:05:56.000000 pylapy-0.1.0/pylapy/cost_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 09:05:56.000000 pylapy-0.1.0/pylapy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2023-10-04 09:05:56.000000 pylapy-0.1.0/pylapy/shape_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2023-10-04 09:05:56.000000 pylapy-0.1.0/pylapy/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:06:13.264076 pylapy-0.1.0/pylapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2023-10-04 09:06:13.000000 pylapy-0.1.0/pylapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-10-04 09:06:13.000000 pylapy-0.1.0/pylapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 09:06:13.000000 pylapy-0.1.0/pylapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-04 09:06:13.000000 pylapy-0.1.0/pylapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-04 09:06:13.000000 pylapy-0.1.0/pylapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-10-04 09:05:56.000000 pylapy-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-10-04 09:06:13.268076 pylapy-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-10-04 09:05:56.000000 pylapy-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:01:57.545506 pylapy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 17:01:51.000000 pylapy-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-04-26 17:01:57.545506 pylapy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-04-26 17:01:51.000000 pylapy-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:01:57.541506 pylapy-0.1.1/pylapy/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 17:01:51.000000 pylapy-0.1.1/pylapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-26 17:01:51.000000 pylapy-0.1.1/pylapy/cost_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:01:51.000000 pylapy-0.1.1/pylapy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-26 17:01:51.000000 pylapy-0.1.1/pylapy/shape_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-04-26 17:01:51.000000 pylapy-0.1.1/pylapy/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:01:57.545506 pylapy-0.1.1/pylapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-04-26 17:01:57.000000 pylapy-0.1.1/pylapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-26 17:01:57.000000 pylapy-0.1.1/pylapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:01:57.000000 pylapy-0.1.1/pylapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 17:01:57.000000 pylapy-0.1.1/pylapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 17:01:57.000000 pylapy-0.1.1/pylapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 17:01:51.000000 pylapy-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-26 17:01:57.545506 pylapy-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 17:01:51.000000 pylapy-0.1.1/setup.py
```

### Comparing `pylapy-0.1.0/LICENSE` & `pylapy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylapy-0.1.0/PKG-INFO` & `pylapy-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylapy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pythonic wrapper around Linear Assignement Problem solvers
 Home-page: https://github.com/raphaelreme/pylapy
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: lap,linear programming,optimization,association problem
 Classifier: Development Status :: 4 - Beta
@@ -12,19 +12,20 @@
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
 Provides-Extra: lap
-Requires-Dist: lap; extra == "lap"
+Requires-Dist: lapx; extra == "lap"
 Provides-Extra: lapjv
 Requires-Dist: lapjv; extra == "lapjv"
 Provides-Extra: lapsolver
 Requires-Dist: lapsolver; extra == "lapsolver"
 Provides-Extra: scipy
 Requires-Dist: scipy; extra == "scipy"
 
@@ -38,27 +39,31 @@
 
 It unifies the functionality of each implementation and allows you to use the one which is the fastest
 on your problem. Note that to solve the same problem, an implementation/method can be more than 10 times slower than an other one.
 
 It also helps you to handle non square matrices and setting a soft threshold on assignements (usually leads
 to better performances than hard thresholding).
 
+We provide some benchmark (but they are a bit hard to read and messy). Given your lap problem, try to make it work with the simplest implementation (scipy) and then (if needed) try to install lap or lapjv and see if they yield better computational performances.
+
 
 ## Install
 
 ```bash
 $ pip install pylapy
 $ # By default it does not install any backend solver
 $ # You can either install by hand your favorite solver (scipy, lap, lapjv, lapsolver)
 $ pip install pylapy[scipy]  # or pylapy[lap] etc
-$ # Note that some backend requires numpy to be installed correctly
+$ # Note that some backend requires numpy to be installed correctly [for instance, the old lap distribution]
 $ # You may need to install numpy before
 $ pip install numpy
 ```
 
+As of today, lapjv do not support macos, lapsolver do not support python > 3.10. We now use [lapx](https://github.com/rathaROG/lapx) which distributes correctly the lap package.
+
 
 ## Getting started
 
 ```python
 
 import numpy as np
 import pylapy
@@ -141,11 +146,11 @@
 We have also tested `lapmod` from lap [2] for sparse matrices. It can sometimes be faster than other implementations but it is less stable and we do not add the support of this algorithm in the wrapper. (Note that for unfeasible problems, it yields a segfault).
 
 Warning: For rectangular matrices, lapjv seems to sometimes output a non-optimal cost (though very close to the optimal one)
 
 ## References
 
 * [1] R. Jonker and A. Volgenant, "A Shortest Augmenting Path Algorithm for Dense and Sparse Linear Assignment Problems", Computing 38, 325-340 (1987)
-* [2] "lap: Linear Assignment Problem solver", https://github.com/gatagat/lap
+* [2] "lap: Linear Assignment Problem solver", https://github.com/gatagat/lap (Now maintained at https://github.com/rathaROG/lapx)
 * [3] "lapjv: Linear Assignment Problem solver using Jonker-Volgenant algorithm", https://github.com/src-d/lapjv
 * [4] "scipy: linear_sum_assignment", https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.linear_sum_assignment.html#scipy.optimize.linear_sum_assignment
 * [5] "py-lapsolver", https://github.com/cheind/py-lapsolver
```

### Comparing `pylapy-0.1.0/README.md` & `pylapy-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 
 It unifies the functionality of each implementation and allows you to use the one which is the fastest
 on your problem. Note that to solve the same problem, an implementation/method can be more than 10 times slower than an other one.
 
 It also helps you to handle non square matrices and setting a soft threshold on assignements (usually leads
 to better performances than hard thresholding).
 
+We provide some benchmark (but they are a bit hard to read and messy). Given your lap problem, try to make it work with the simplest implementation (scipy) and then (if needed) try to install lap or lapjv and see if they yield better computational performances.
+
 
 ## Install
 
 ```bash
 $ pip install pylapy
 $ # By default it does not install any backend solver
 $ # You can either install by hand your favorite solver (scipy, lap, lapjv, lapsolver)
 $ pip install pylapy[scipy]  # or pylapy[lap] etc
-$ # Note that some backend requires numpy to be installed correctly
+$ # Note that some backend requires numpy to be installed correctly [for instance, the old lap distribution]
 $ # You may need to install numpy before
 $ pip install numpy
 ```
 
+As of today, lapjv do not support macos, lapsolver do not support python > 3.10. We now use [lapx](https://github.com/rathaROG/lapx) which distributes correctly the lap package.
+
 
 ## Getting started
 
 ```python
 
 import numpy as np
 import pylapy
@@ -111,11 +115,11 @@
 We have also tested `lapmod` from lap [2] for sparse matrices. It can sometimes be faster than other implementations but it is less stable and we do not add the support of this algorithm in the wrapper. (Note that for unfeasible problems, it yields a segfault).
 
 Warning: For rectangular matrices, lapjv seems to sometimes output a non-optimal cost (though very close to the optimal one)
 
 ## References
 
 * [1] R. Jonker and A. Volgenant, "A Shortest Augmenting Path Algorithm for Dense and Sparse Linear Assignment Problems", Computing 38, 325-340 (1987)
-* [2] "lap: Linear Assignment Problem solver", https://github.com/gatagat/lap
+* [2] "lap: Linear Assignment Problem solver", https://github.com/gatagat/lap (Now maintained at https://github.com/rathaROG/lapx)
 * [3] "lapjv: Linear Assignment Problem solver using Jonker-Volgenant algorithm", https://github.com/src-d/lapjv
 * [4] "scipy: linear_sum_assignment", https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.linear_sum_assignment.html#scipy.optimize.linear_sum_assignment
 * [5] "py-lapsolver", https://github.com/cheind/py-lapsolver
```

### Comparing `pylapy-0.1.0/pylapy/cost_extension.py` & `pylapy-0.1.1/pylapy/cost_extension.py`

 * *Files identical despite different names*

### Comparing `pylapy-0.1.0/pylapy/shape_extension.py` & `pylapy-0.1.1/pylapy/shape_extension.py`

 * *Files identical despite different names*

### Comparing `pylapy-0.1.0/pylapy/solver.py` & `pylapy-0.1.1/pylapy/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,16 @@
 
         return links
 
     @staticmethod
     def _lap(dist: np.ndarray) -> np.ndarray:
         """Solve with lap (https://github.com/gatagat/lap)
 
+        Note: We are now using the lapx distribution from https://github.com/rathaROG/lapx.
+
         You should not call this method directly. To enforce using lap,
         rather set `implem` attribute to "lap" and call `solve`.
 
         Args:
             dist (np.ndarray): Dist matrix
                 Shape: (N, N), dtype: float
 
@@ -220,15 +222,15 @@
 
         i, j = scipy.optimize.linear_sum_assignment(dist)
 
         return np.array([i, j], dtype=np.uint16).transpose()
 
     @staticmethod
     def _lapsolver(dist: np.ndarray) -> np.ndarray:
-        """Solve with lapjv (https://github.com/src-d/lapjv)
+        """Solve with lapsolver (https://github.com/cheind/py-lapsolver)
 
         You should not call this method directly. To enforce using lapsolver,
         rather set `implem` attribute to "lapsolver" and call `solve`.
 
         Args:
             dist (np.ndarray): Dist matrix
                 Shape: (N, N), dtype: float
```

### Comparing `pylapy-0.1.0/pylapy.egg-info/PKG-INFO` & `pylapy-0.1.1/pylapy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylapy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pythonic wrapper around Linear Assignement Problem solvers
 Home-page: https://github.com/raphaelreme/pylapy
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: lap,linear programming,optimization,association problem
 Classifier: Development Status :: 4 - Beta
@@ -12,19 +12,20 @@
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
 Provides-Extra: lap
-Requires-Dist: lap; extra == "lap"
+Requires-Dist: lapx; extra == "lap"
 Provides-Extra: lapjv
 Requires-Dist: lapjv; extra == "lapjv"
 Provides-Extra: lapsolver
 Requires-Dist: lapsolver; extra == "lapsolver"
 Provides-Extra: scipy
 Requires-Dist: scipy; extra == "scipy"
 
@@ -38,27 +39,31 @@
 
 It unifies the functionality of each implementation and allows you to use the one which is the fastest
 on your problem. Note that to solve the same problem, an implementation/method can be more than 10 times slower than an other one.
 
 It also helps you to handle non square matrices and setting a soft threshold on assignements (usually leads
 to better performances than hard thresholding).
 
+We provide some benchmark (but they are a bit hard to read and messy). Given your lap problem, try to make it work with the simplest implementation (scipy) and then (if needed) try to install lap or lapjv and see if they yield better computational performances.
+
 
 ## Install
 
 ```bash
 $ pip install pylapy
 $ # By default it does not install any backend solver
 $ # You can either install by hand your favorite solver (scipy, lap, lapjv, lapsolver)
 $ pip install pylapy[scipy]  # or pylapy[lap] etc
-$ # Note that some backend requires numpy to be installed correctly
+$ # Note that some backend requires numpy to be installed correctly [for instance, the old lap distribution]
 $ # You may need to install numpy before
 $ pip install numpy
 ```
 
+As of today, lapjv do not support macos, lapsolver do not support python > 3.10. We now use [lapx](https://github.com/rathaROG/lapx) which distributes correctly the lap package.
+
 
 ## Getting started
 
 ```python
 
 import numpy as np
 import pylapy
@@ -141,11 +146,11 @@
 We have also tested `lapmod` from lap [2] for sparse matrices. It can sometimes be faster than other implementations but it is less stable and we do not add the support of this algorithm in the wrapper. (Note that for unfeasible problems, it yields a segfault).
 
 Warning: For rectangular matrices, lapjv seems to sometimes output a non-optimal cost (though very close to the optimal one)
 
 ## References
 
 * [1] R. Jonker and A. Volgenant, "A Shortest Augmenting Path Algorithm for Dense and Sparse Linear Assignment Problems", Computing 38, 325-340 (1987)
-* [2] "lap: Linear Assignment Problem solver", https://github.com/gatagat/lap
+* [2] "lap: Linear Assignment Problem solver", https://github.com/gatagat/lap (Now maintained at https://github.com/rathaROG/lapx)
 * [3] "lapjv: Linear Assignment Problem solver using Jonker-Volgenant algorithm", https://github.com/src-d/lapjv
 * [4] "scipy: linear_sum_assignment", https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.linear_sum_assignment.html#scipy.optimize.linear_sum_assignment
 * [5] "py-lapsolver", https://github.com/cheind/py-lapsolver
```

### Comparing `pylapy-0.1.0/setup.cfg` & `pylapy-0.1.1/setup.cfg`

 * *Files 18% similar despite different names*

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
 include_package_data = False
 
@@ -31,16 +32,16 @@
 * = py.typed
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [options.extras_require]
-lap = lap
-lapjv = lapjv
-lapsolver = lapsolver
-scipy = scipy
+lap = lapx  # Now works everywhere ?
+lapjv = lapjv  # Do not work for macos
+lapsolver = lapsolver  # Do not work for python > 3.10
+scipy = scipy  # Works everywhere
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

