# Comparing `tmp/IRWPy-0.0.1.tar.gz` & `tmp/IRWPy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IRWPy-0.0.1.tar", last modified: Fri Apr 26 20:02:33 2024, max compression
+gzip compressed data, was "IRWPy-0.0.2.tar", last modified: Fri Apr 26 21:07:02 2024, max compression
```

## Comparing `IRWPy-0.0.1.tar` & `IRWPy-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-26 20:02:33.070525 IRWPy-0.0.1/
--rw-r--r--   0 aeleish    (503) staff       (20)       76 2024-04-26 19:41:38.000000 IRWPy-0.0.1/CHANGELOG.txt
-drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-26 20:02:33.069929 IRWPy-0.0.1/IRWPy.egg-info/
--rw-r--r--   0 aeleish    (503) staff       (20)      211 2024-04-26 20:02:32.000000 IRWPy-0.0.1/IRWPy.egg-info/PKG-INFO
--rw-r--r--   0 aeleish    (503) staff       (20)      213 2024-04-26 20:02:32.000000 IRWPy-0.0.1/IRWPy.egg-info/SOURCES.txt
--rw-r--r--   0 aeleish    (503) staff       (20)        1 2024-04-26 20:02:32.000000 IRWPy-0.0.1/IRWPy.egg-info/dependency_links.txt
--rw-r--r--   0 aeleish    (503) staff       (20)        6 2024-04-26 20:02:32.000000 IRWPy-0.0.1/IRWPy.egg-info/requires.txt
--rw-r--r--   0 aeleish    (503) staff       (20)        1 2024-04-26 20:02:32.000000 IRWPy-0.0.1/IRWPy.egg-info/top_level.txt
--rw-r--r--   0 aeleish    (503) staff       (20)     1061 2024-04-26 19:43:47.000000 IRWPy-0.0.1/LICENSE.txt
--rw-r--r--   0 aeleish    (503) staff       (20)       25 2024-04-26 19:42:49.000000 IRWPy-0.0.1/MANIFEST.in
--rw-r--r--   0 aeleish    (503) staff       (20)      211 2024-04-26 20:02:33.070308 IRWPy-0.0.1/PKG-INFO
--rw-r--r--   0 aeleish    (503) staff       (20)      383 2024-04-26 19:40:22.000000 IRWPy-0.0.1/README.txt
--rw-r--r--   0 aeleish    (503) staff       (20)     1679 2024-04-26 19:31:38.000000 IRWPy-0.0.1/__init__.py
--rw-r--r--   0 aeleish    (503) staff       (20)       38 2024-04-26 20:02:33.070582 IRWPy-0.0.1/setup.cfg
--rw-r--r--   0 aeleish    (503) staff       (20)      520 2024-04-26 20:01:57.000000 IRWPy-0.0.1/setup.py
+drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-26 21:07:02.718024 IRWPy-0.0.2/
+-rw-r--r--   0 aeleish    (503) staff       (20)      137 2024-04-26 21:06:25.000000 IRWPy-0.0.2/CHANGELOG.txt
+drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-26 21:07:02.717459 IRWPy-0.0.2/IRWPy.egg-info/
+-rw-r--r--   0 aeleish    (503) staff       (20)      211 2024-04-26 21:07:02.000000 IRWPy-0.0.2/IRWPy.egg-info/PKG-INFO
+-rw-r--r--   0 aeleish    (503) staff       (20)      213 2024-04-26 21:07:02.000000 IRWPy-0.0.2/IRWPy.egg-info/SOURCES.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)        1 2024-04-26 21:07:02.000000 IRWPy-0.0.2/IRWPy.egg-info/dependency_links.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)        6 2024-04-26 21:07:02.000000 IRWPy-0.0.2/IRWPy.egg-info/requires.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)        1 2024-04-26 21:07:02.000000 IRWPy-0.0.2/IRWPy.egg-info/top_level.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)     1061 2024-04-26 19:43:47.000000 IRWPy-0.0.2/LICENSE.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)       25 2024-04-26 19:42:49.000000 IRWPy-0.0.2/MANIFEST.in
+-rw-r--r--   0 aeleish    (503) staff       (20)      211 2024-04-26 21:07:02.717830 IRWPy-0.0.2/PKG-INFO
+-rw-r--r--   0 aeleish    (503) staff       (20)      383 2024-04-26 19:40:22.000000 IRWPy-0.0.2/README.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)     1695 2024-04-26 21:06:36.000000 IRWPy-0.0.2/__init__.py
+-rw-r--r--   0 aeleish    (503) staff       (20)       38 2024-04-26 21:07:02.718071 IRWPy-0.0.2/setup.cfg
+-rw-r--r--   0 aeleish    (503) staff       (20)      520 2024-04-26 21:06:01.000000 IRWPy-0.0.2/setup.py
```

### Comparing `IRWPy-0.0.1/LICENSE.txt` & `IRWPy-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `IRWPy-0.0.1/__init__.py` & `IRWPy-0.0.2/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import numpy as np
+
 def inverse_radius_weighting(x, y, E, values, xi, yi, power=2, neighbors=12):
     """
     Inverse Radius Weighting (IRW) interpolation.
     
     Parameters:
     - x, y: Arrays of measured point coordinates.
     - E: Array of elevations corresponding to the points.
@@ -36,9 +38,9 @@
         distances_asc = np.asarray(sorted(tmp_distances)[0:neighbors])
         
         weights = 1.0 / ((distances_asc**power) + (np.asarray(tmp_E)**power))
 
     
     weighted_values = asc_values * weights
     interpolated_value = np.sum(weighted_values) / np.sum(weights)
-    
+
     return interpolated_value
```

### Comparing `IRWPy-0.0.1/setup.py` & `IRWPy-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	'Intended Audience :: Research',
 	'License :: MIT License',
 	'Programming Language :: Python :: 3',
 	'Topic :: Geology',
 ]
 
 setup(name='IRWPy',
-      version='0.0.1',
+      version='0.0.2',
       description='Inverse Radius Weighting Interpolation',
       author='Behnam Sadeghi',
       author_email='z5218858@zmail.unsw.edu.au',
       keywords='interpolation',
       packages=find_packages(),
       install_requires=['numpy']
      )
```

