# Comparing `tmp/clump-python-0.2.4.tar.gz` & `tmp/clump-python-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clump-python-0.2.4.tar", last modified: Wed Apr 24 18:19:46 2024, max compression
+gzip compressed data, was "clump-python-0.2.5.tar", last modified: Fri Apr 26 08:49:47 2024, max compression
```

## Comparing `clump-python-0.2.4.tar` & `clump-python-0.2.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 18:19:46.092106 clump-python-0.2.4/
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 18:19:46.084106 clump-python-0.2.4/CLUMP/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.2.4/CLUMP/ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.2.4/CLUMP/GenerateClump_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.2.4/CLUMP/GenerateClump_Favier.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.2.4/CLUMP/GenerateClump_Ferellec_McDowell.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.2.4/CLUMP/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 18:19:46.084106 clump-python-0.2.4/CLUMP/examples/
--rw-rw-r--   0 utku      (1000) utku      (1000)      812 2024-04-24 17:36:11.000000 clump-python-0.2.4/CLUMP/examples/Example_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      937 2024-04-24 17:36:11.000000 clump-python-0.2.4/CLUMP/examples/Example_Euclidean_3D_Extended.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      675 2024-04-24 17:36:11.000000 clump-python-0.2.4/CLUMP/examples/Example_ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      713 2024-04-24 17:36:11.000000 clump-python-0.2.4/CLUMP/examples/Example_Favier_automatic_generation.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      743 2024-04-24 17:36:11.000000 clump-python-0.2.4/CLUMP/examples/Example_Ferellec_McDowell.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 18:19:46.092106 clump-python-0.2.4/CLUMP/examples/ParticleGeometries/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Hexahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Human_femur.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Octahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Torus.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.4/CLUMP/examples/ParticleGeometries/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.4/CLUMP/examples/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 18:19:46.092106 clump-python-0.2.4/CLUMP/utils/
--rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.2.4/CLUMP/utils/MyRobustCrust.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.2.4/CLUMP/utils/ParticlePlotter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.2.4/CLUMP/utils/PatchNormals.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.2.4/CLUMP/utils/RigidBodyParameters.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.2.4/CLUMP/utils/STL_ReaderWriter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.2.4/CLUMP/utils/VTK_Writer.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.2.4/CLUMP/utils/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.2.4/LICENSE
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 18:19:46.092106 clump-python-0.2.4/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.2.4/README.md
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 18:19:46.092106 clump-python-0.2.4/clump_python.egg-info/
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 18:19:46.000000 clump-python-0.2.4/clump_python.egg-info/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     1220 2024-04-24 18:19:46.000000 clump-python-0.2.4/clump_python.egg-info/SOURCES.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 18:19:46.000000 clump-python-0.2.4/clump_python.egg-info/dependency_links.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 18:19:46.000000 clump-python-0.2.4/clump_python.egg-info/requires.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 18:19:46.000000 clump-python-0.2.4/clump_python.egg-info/top_level.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 18:19:46.092106 clump-python-0.2.4/setup.cfg
--rw-rw-r--   0 utku      (1000) utku      (1000)      970 2024-04-24 18:11:01.000000 clump-python-0.2.4/setup.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.829752 clump-python-0.2.5/
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.817752 clump-python-0.2.5/CLUMP/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.2.5/CLUMP/ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.2.5/CLUMP/GenerateClump_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.2.5/CLUMP/GenerateClump_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.2.5/CLUMP/GenerateClump_Ferellec_McDowell.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.2.5/CLUMP/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.821752 clump-python-0.2.5/CLUMP/examples/
+-rw-rw-r--   0 utku      (1000) utku      (1000)      812 2024-04-24 17:36:11.000000 clump-python-0.2.5/CLUMP/examples/Example_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      937 2024-04-24 17:36:11.000000 clump-python-0.2.5/CLUMP/examples/Example_Euclidean_3D_Extended.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      675 2024-04-24 17:36:11.000000 clump-python-0.2.5/CLUMP/examples/Example_ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      713 2024-04-24 17:36:11.000000 clump-python-0.2.5/CLUMP/examples/Example_Favier_automatic_generation.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      743 2024-04-24 17:36:11.000000 clump-python-0.2.5/CLUMP/examples/Example_Ferellec_McDowell.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.825752 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Hexahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Human_femur.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Octahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Torus.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.5/CLUMP/examples/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.829752 clump-python-0.2.5/CLUMP/utils/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.2.5/CLUMP/utils/MyRobustCrust.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.2.5/CLUMP/utils/ParticlePlotter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.2.5/CLUMP/utils/PatchNormals.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.2.5/CLUMP/utils/RigidBodyParameters.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.2.5/CLUMP/utils/STL_ReaderWriter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.2.5/CLUMP/utils/VTK_Writer.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/utils/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.2.5/LICENSE
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-26 08:49:47.829752 clump-python-0.2.5/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.2.5/README.md
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.829752 clump-python-0.2.5/clump_python.egg-info/
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-26 08:49:47.000000 clump-python-0.2.5/clump_python.egg-info/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1220 2024-04-26 08:49:47.000000 clump-python-0.2.5/clump_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-26 08:49:47.000000 clump-python-0.2.5/clump_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-26 08:49:47.000000 clump-python-0.2.5/clump_python.egg-info/requires.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-26 08:49:47.000000 clump-python-0.2.5/clump_python.egg-info/top_level.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-26 08:49:47.829752 clump-python-0.2.5/setup.cfg
+-rw-rw-r--   0 utku      (1000) utku      (1000)      970 2024-04-26 08:47:29.000000 clump-python-0.2.5/setup.py
```

### Comparing `clump-python-0.2.4/CLUMP/ExtractSurface.py` & `clump-python-0.2.5/CLUMP/ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/GenerateClump_Euclidean_3D.py` & `clump-python-0.2.5/CLUMP/GenerateClump_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/GenerateClump_Favier.py` & `clump-python-0.2.5/CLUMP/GenerateClump_Favier.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/GenerateClump_Ferellec_McDowell.py` & `clump-python-0.2.5/CLUMP/GenerateClump_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/Example_Euclidean_3D.py` & `clump-python-0.2.5/CLUMP/examples/Example_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/Example_Euclidean_3D_Extended.py` & `clump-python-0.2.5/CLUMP/examples/Example_Euclidean_3D_Extended.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/Example_ExtractSurface.py` & `clump-python-0.2.5/CLUMP/examples/Example_ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/Example_Favier_automatic_generation.py` & `clump-python-0.2.5/CLUMP/examples/Example_Favier_automatic_generation.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/Example_Ferellec_McDowell.py` & `clump-python-0.2.5/CLUMP/examples/Example_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat` & `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat` & `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl` & `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Hexahedron.stl` & `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Hexahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Human_femur.stl` & `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Human_femur.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Octahedron.stl` & `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Octahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/examples/ParticleGeometries/Torus.stl` & `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Torus.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/utils/MyRobustCrust.py` & `clump-python-0.2.5/CLUMP/utils/MyRobustCrust.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/utils/ParticlePlotter.py` & `clump-python-0.2.5/CLUMP/utils/ParticlePlotter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/utils/PatchNormals.py` & `clump-python-0.2.5/CLUMP/utils/PatchNormals.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/utils/RigidBodyParameters.py` & `clump-python-0.2.5/CLUMP/utils/RigidBodyParameters.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/utils/STL_ReaderWriter.py` & `clump-python-0.2.5/CLUMP/utils/STL_ReaderWriter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/CLUMP/utils/VTK_Writer.py` & `clump-python-0.2.5/CLUMP/utils/VTK_Writer.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/LICENSE` & `clump-python-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/PKG-INFO` & `clump-python-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.2.4
+Version: 0.2.5
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.2.4/README.md` & `clump-python-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/clump_python.egg-info/PKG-INFO` & `clump-python-0.2.5/clump_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.2.4
+Version: 0.2.5
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.2.4/clump_python.egg-info/SOURCES.txt` & `clump-python-0.2.5/clump_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.4/setup.py` & `clump-python-0.2.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clump-python",
-    version="0.2.4",
+    version="0.2.5",
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
         'numpy-stl',
         'pyvista',
         'scipy',
```

