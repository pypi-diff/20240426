# Comparing `tmp/rbfmeshgen-1.0.1.tar.gz` & `tmp/rbfmeshgen-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbfmeshgen-1.0.1.tar", last modified: Wed Apr 24 23:21:14 2024, max compression
+gzip compressed data, was "rbfmeshgen-1.0.2.tar", last modified: Fri Apr 26 19:04:06 2024, max compression
```

## Comparing `rbfmeshgen-1.0.1.tar` & `rbfmeshgen-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:14.402235 rbfmeshgen-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-24 23:21:14.402235 rbfmeshgen-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:14.402235 rbfmeshgen-1.0.1/RBFMeshGen/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-24 23:21:06.000000 rbfmeshgen-1.0.1/RBFMeshGen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-24 23:21:06.000000 rbfmeshgen-1.0.1/RBFMeshGen/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-04-24 23:21:06.000000 rbfmeshgen-1.0.1/RBFMeshGen/mesh_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-24 23:21:06.000000 rbfmeshgen-1.0.1/RBFMeshGen/visualization_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:14.402235 rbfmeshgen-1.0.1/RBFMeshGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-24 23:21:14.000000 rbfmeshgen-1.0.1/RBFMeshGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 23:21:14.000000 rbfmeshgen-1.0.1/RBFMeshGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:21:14.000000 rbfmeshgen-1.0.1/RBFMeshGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 23:21:14.000000 rbfmeshgen-1.0.1/RBFMeshGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 23:21:14.000000 rbfmeshgen-1.0.1/RBFMeshGen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-24 23:21:06.000000 rbfmeshgen-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 23:21:14.402235 rbfmeshgen-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-24 23:21:06.000000 rbfmeshgen-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:04:06.911209 rbfmeshgen-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-26 19:04:06.911209 rbfmeshgen-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:04:06.911209 rbfmeshgen-1.0.2/RBFMeshGen/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/RBFMeshGen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/RBFMeshGen/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/RBFMeshGen/mesh_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/RBFMeshGen/visualization_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:04:06.911209 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-26 19:04:06.000000 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-26 19:04:06.000000 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:04:06.000000 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-26 19:04:06.000000 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 19:04:06.000000 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:04:06.911209 rbfmeshgen-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/setup.py
```

### Comparing `rbfmeshgen-1.0.1/PKG-INFO` & `rbfmeshgen-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RBFMeshGen
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for generating random meshes based on radial basis functions.
 Home-page: https://github.com/LDBreton/RBFMeshGen
 Author: Louis Breton
 Author-email: louis.breton@ciencias.unam.mx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rbfmeshgen-1.0.1/RBFMeshGen/geometry_utils.py` & `rbfmeshgen-1.0.2/RBFMeshGen/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `rbfmeshgen-1.0.1/RBFMeshGen/mesh_generation.py` & `rbfmeshgen-1.0.2/RBFMeshGen/mesh_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     def __init__(self, *borders: Border, abs_tol=1e-04):
         self.borders = list(borders)
         self.Points = []
         self.Boundary_Points = []
         self.outer_polygons = []
         self.holes_polygons = []
+        self.region_polygons = []
         self.abs_tol = abs_tol
 
     def generate_points(self, num_points, boundary_distance=1.0e-5):
         """-
         Generates random points within the polygons defined by the borders.
 
         Args:
@@ -69,14 +70,15 @@
         # Step 1: Exclude nested polygons
         outer_polygons = exclude_nested_polygons(outer_polygons)
         self.outer_polygons = outer_polygons
         self.holes_polygons = hole_polygons
 
         # Step 2: generate_regions
         region_poly = generate_regions(outer_polygons, hole_polygons)
+        self.region_polygons = region_poly
 
         # Step 3: Calculate points allocation
         points_allocation = calculate_point_allocation(region_poly, num_points)
 
         # Step 4: Generate points
         self.Points.extend(generate_points_within_polygons(region_poly, points_allocation, boundary_distance))
```

### Comparing `rbfmeshgen-1.0.1/RBFMeshGen/visualization_tools.py` & `rbfmeshgen-1.0.2/RBFMeshGen/visualization_tools.py`

 * *Files identical despite different names*

### Comparing `rbfmeshgen-1.0.1/RBFMeshGen.egg-info/PKG-INFO` & `rbfmeshgen-1.0.2/RBFMeshGen.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RBFMeshGen
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for generating random meshes based on radial basis functions.
 Home-page: https://github.com/LDBreton/RBFMeshGen
 Author: Louis Breton
 Author-email: louis.breton@ciencias.unam.mx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rbfmeshgen-1.0.1/README.md` & `rbfmeshgen-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rbfmeshgen-1.0.1/setup.py` & `rbfmeshgen-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="RBFMeshGen",
-    version="1.0.1",
+    version="1.0.2",
     author="Louis Breton",
     author_email="louis.breton@ciencias.unam.mx",
     description="A Python package for generating random meshes based on radial basis functions.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/LDBreton/RBFMeshGen",
     packages=find_packages(),
```

