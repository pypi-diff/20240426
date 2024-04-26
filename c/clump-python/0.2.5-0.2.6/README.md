# Comparing `tmp/clump-python-0.2.5.tar.gz` & `tmp/clump-python-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clump-python-0.2.5.tar", last modified: Fri Apr 26 08:49:47 2024, max compression
+gzip compressed data, was "clump-python-0.2.6.tar", last modified: Fri Apr 26 09:11:02 2024, max compression
```

## Comparing `clump-python-0.2.5.tar` & `clump-python-0.2.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.829752 clump-python-0.2.5/
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.817752 clump-python-0.2.5/CLUMP/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.2.5/CLUMP/ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.2.5/CLUMP/GenerateClump_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.2.5/CLUMP/GenerateClump_Favier.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.2.5/CLUMP/GenerateClump_Ferellec_McDowell.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.2.5/CLUMP/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.821752 clump-python-0.2.5/CLUMP/examples/
--rw-rw-r--   0 utku      (1000) utku      (1000)      812 2024-04-24 17:36:11.000000 clump-python-0.2.5/CLUMP/examples/Example_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      937 2024-04-24 17:36:11.000000 clump-python-0.2.5/CLUMP/examples/Example_Euclidean_3D_Extended.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      675 2024-04-24 17:36:11.000000 clump-python-0.2.5/CLUMP/examples/Example_ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      713 2024-04-24 17:36:11.000000 clump-python-0.2.5/CLUMP/examples/Example_Favier_automatic_generation.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      743 2024-04-24 17:36:11.000000 clump-python-0.2.5/CLUMP/examples/Example_Ferellec_McDowell.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.825752 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Hexahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Human_femur.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Octahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Torus.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.5/CLUMP/examples/ParticleGeometries/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.5/CLUMP/examples/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.829752 clump-python-0.2.5/CLUMP/utils/
--rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.2.5/CLUMP/utils/MyRobustCrust.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.2.5/CLUMP/utils/ParticlePlotter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.2.5/CLUMP/utils/PatchNormals.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.2.5/CLUMP/utils/RigidBodyParameters.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.2.5/CLUMP/utils/STL_ReaderWriter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.2.5/CLUMP/utils/VTK_Writer.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.2.5/CLUMP/utils/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.2.5/LICENSE
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-26 08:49:47.829752 clump-python-0.2.5/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.2.5/README.md
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 08:49:47.829752 clump-python-0.2.5/clump_python.egg-info/
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-26 08:49:47.000000 clump-python-0.2.5/clump_python.egg-info/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     1220 2024-04-26 08:49:47.000000 clump-python-0.2.5/clump_python.egg-info/SOURCES.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-26 08:49:47.000000 clump-python-0.2.5/clump_python.egg-info/dependency_links.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-26 08:49:47.000000 clump-python-0.2.5/clump_python.egg-info/requires.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-26 08:49:47.000000 clump-python-0.2.5/clump_python.egg-info/top_level.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-26 08:49:47.829752 clump-python-0.2.5/setup.cfg
--rw-rw-r--   0 utku      (1000) utku      (1000)      970 2024-04-26 08:47:29.000000 clump-python-0.2.5/setup.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:11:02.191663 clump-python-0.2.6/
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:11:02.183663 clump-python-0.2.6/CLUMP/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8103 2024-04-26 06:08:00.000000 clump-python-0.2.6/CLUMP/ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-26 05:50:24.000000 clump-python-0.2.6/CLUMP/GenerateClump_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9304 2024-04-26 06:08:49.000000 clump-python-0.2.6/CLUMP/GenerateClump_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8727 2024-04-26 06:08:49.000000 clump-python-0.2.6/CLUMP/GenerateClump_Ferellec_McDowell.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.2.6/CLUMP/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:11:02.183663 clump-python-0.2.6/CLUMP/examples/
+-rw-rw-r--   0 utku      (1000) utku      (1000)      812 2024-04-26 05:50:01.000000 clump-python-0.2.6/CLUMP/examples/Example_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      937 2024-04-26 05:49:49.000000 clump-python-0.2.6/CLUMP/examples/Example_Euclidean_3D_Extended.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      675 2024-04-26 05:50:04.000000 clump-python-0.2.6/CLUMP/examples/Example_ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      713 2024-04-26 05:50:07.000000 clump-python-0.2.6/CLUMP/examples/Example_Favier_automatic_generation.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      743 2024-04-26 05:50:11.000000 clump-python-0.2.6/CLUMP/examples/Example_Ferellec_McDowell.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:11:02.191663 clump-python-0.2.6/CLUMP/examples/ParticleGeometries/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Hexahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Human_femur.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Octahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Torus.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.6/CLUMP/examples/ParticleGeometries/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.6/CLUMP/examples/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:11:02.191663 clump-python-0.2.6/CLUMP/utils/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-26 05:50:40.000000 clump-python-0.2.6/CLUMP/utils/MyRobustCrust.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2670 2024-04-26 05:57:34.000000 clump-python-0.2.6/CLUMP/utils/ParticlePlotter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2287 2024-04-26 05:54:26.000000 clump-python-0.2.6/CLUMP/utils/PatchNormals.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.2.6/CLUMP/utils/RigidBodyParameters.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2293 2024-04-26 05:56:57.000000 clump-python-0.2.6/CLUMP/utils/STL_ReaderWriter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1330 2024-04-26 05:51:27.000000 clump-python-0.2.6/CLUMP/utils/VTK_Writer.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.2.6/CLUMP/utils/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.2.6/LICENSE
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-26 09:11:02.191663 clump-python-0.2.6/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.2.6/README.md
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-26 09:11:02.191663 clump-python-0.2.6/clump_python.egg-info/
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-26 09:11:02.000000 clump-python-0.2.6/clump_python.egg-info/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1230 2024-04-26 09:11:02.000000 clump-python-0.2.6/clump_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-26 09:11:02.000000 clump-python-0.2.6/clump_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-26 09:11:02.000000 clump-python-0.2.6/clump_python.egg-info/requires.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-26 09:11:02.000000 clump-python-0.2.6/clump_python.egg-info/top_level.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-26 09:11:02.191663 clump-python-0.2.6/setup.cfg
+-rw-rw-r--   0 utku      (1000) utku      (1000)      970 2024-04-26 08:59:21.000000 clump-python-0.2.6/setup.py
```

### Comparing `clump-python-0.2.5/CLUMP/ExtractSurface.py` & `clump-python-0.2.6/CLUMP/ExtractSurface.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 
 """
 Tesselation of the surface of a clump into a surface mesh
 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
-2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
+2024 Translated from MATLAB to Python by A.U. Canbolat <utku.canbolat@fau.de>
 """
 
 
 def sphereContact(sphere1, sphere2):
     """ Function to perform contact detection between two spheres
     inContact: boolean: whether sphere1 and sphere2 intersect
     :param sphere1: [1 x 4] [x,y,z,r]:	test sphere 1
@@ -184,26 +184,9 @@
     vertices = np.unique(vertices, axis=0)
 
     # Generate mesh using the Crust algorithm (Amenta et al, 1999)
     faces, _ = MyRobustCrust(vertices)
 
     if visualise:
          mesh_plotter_trimesh(vertices, faces)
-    	
-# Legacy mesh_plotter using matplotlib - Does not represent the aspect ratio correctly
-#        fig = plt.figure()
-#        ax = fig.add_subplot(111, projection='3d')
-
-#        # Create a Poly3DCollection object
-#        polys = Poly3DCollection(vertices[faces], facecolors='cyan', edgecolors='k', alpha=0.70)
-#        ax.add_collection3d(polys)
-
-#        # Auto-scale to the mesh size
-#        scale = vertices.flatten('F')
-#        ax.auto_scale_xyz(scale, scale, scale)
-##        ax.set_box_aspect([1,1,1])
-##        ax.set_aspect('auto')
-#	
-#        # Show the plot
-#        plt.show()
-
+    
     return faces, vertices
```

### Comparing `clump-python-0.2.5/CLUMP/GenerateClump_Euclidean_3D.py` & `clump-python-0.2.6/CLUMP/GenerateClump_Euclidean_3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from CLUMP.utils.VTK_Writer import clump_to_VTK
 
 """
 Clump generator using the Euclidean map for voxelated, 3D particles 
 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
-2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
+2024 Translated from MATLAB to Python by A.U. Canbolat <utku.canbolat@fau.de>
 
 The main concept of this methodology:
 
 1. We import the surface mesh of a particle.
 2. We transform the mesh into a voxelated representation, i.e. a binary
    3D image, where each voxel belonging to the particle is equal to zero.
 3. The Euclidean distance transform of the 3D image is computed and
```

### Comparing `clump-python-0.2.5/CLUMP/GenerateClump_Favier.py` & `clump-python-0.2.6/CLUMP/GenerateClump_Favier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,35 @@
+# Legacy mesh_plotter using matplotlib - Does not represent the aspect ratio correctly
+#        fig = plt.figure()
+#        ax = fig.add_subplot(111, projection='3d')
+
+#        # Create a Poly3DCollection object
+#        polys = Poly3DCollection(vertices[faces], facecolors='cyan', edgecolors='k', alpha=0.70)
+#        ax.add_collection3d(polys)
+
+#        # Auto-scale to the mesh size
+#        scale = vertices.flatten('F')
+#        ax.auto_scale_xyz(scale, scale, scale)
+##        ax.set_box_aspect([1,1,1])
+##        ax.set_aspect('auto')
+#	
+#        # Show the plot
+#        plt.show()
 import numpy as np
 import CLUMP.utils.RigidBodyParameters as RigidBodyParameters
 import CLUMP.utils.STL_ReaderWriter as STL_ReaderWriter
 from CLUMP.utils.ParticlePlotter import clump_plotter_pyvista
 from CLUMP.utils.VTK_Writer import clump_to_VTK
 
 """
 Implementation of the clump-generation concept proposed by Favier et al. (1999) [1]
 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
-2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
+2024 Translated from MATLAB to Python by A.U. Canbolat <utku.canbolat@fau.de>
 
 [1] Favier, J.F., Fard, M.H., Kremmer, M. and Raji, A.O., 1999. Engineering Computations: Int J for Computer-Aided Engineering, 16(4), pp.467-480.
 
 The main concept of this methodology:
 
 1. We import the geometry of a particle either as a surface mesh or a voxelated 3D image.
 2. If a voxelated image is given, we transform it into a surface mesh, providing its vertices and faces (vertex connectivity).
```

### Comparing `clump-python-0.2.5/CLUMP/GenerateClump_Ferellec_McDowell.py` & `clump-python-0.2.6/CLUMP/GenerateClump_Ferellec_McDowell.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,37 @@
+# Legacy mesh_plotter using matplotlib - Does not represent the aspect ratio correctly
+#        fig = plt.figure()
+#        ax = fig.add_subplot(111, projection='3d')
+
+#        # Create a Poly3DCollection object
+#        polys = Poly3DCollection(vertices[faces], facecolors='cyan', edgecolors='k', alpha=0.70)
+#        ax.add_collection3d(polys)
+
+#        # Auto-scale to the mesh size
+#        scale = vertices.flatten('F')
+#        ax.auto_scale_xyz(scale, scale, scale)
+##        ax.set_box_aspect([1,1,1])
+##        ax.set_aspect('auto')
+#
+#        # Show the plot
+#        plt.show()
 import numpy as np
 import CLUMP.utils.PatchNormals as PatchNormals
 import CLUMP.utils.RigidBodyParameters as RigidBodyParameters
 import CLUMP.utils.STL_ReaderWriter as STL_ReaderWriter
 from CLUMP.utils.ParticlePlotter import clump_plotter_pyvista
 from CLUMP.utils.VTK_Writer import clump_to_VTK
 import trimesh
 
 """
 Implementation of the clump-generation concept proposed by Ferellec and McDowell (2010) [1]
 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
-2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
+2024 Translated from MATLAB to Python by A.U. Canbolat <utku.canbolat@fau.de>
 
 [1] Ferellec, J.F. and McDowell, G.R., 2010. Granular Matter, 12(5), pp.459-467. DOI 10.1007/s10035-010-0205-8
 
 The main concept of this methodology:
 
 1. We import the surface mesh of a particle.
 2. We calculate the normal of each vertex pointing inwards.
```

### Comparing `clump-python-0.2.5/CLUMP/examples/Example_Euclidean_3D.py` & `clump-python-0.2.6/CLUMP/examples/Example_Euclidean_3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Script to run GenerateClump_Euclidean_3D
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
-# 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
+# 2024 Translated from MATLAB to Python by A.U. Canbolat <utku.canbolat@fau.de>
 
 
 from CLUMP import GenerateClump_Euclidean_3D
 import sys
 import os
 sys.path.append('../../')
```

### Comparing `clump-python-0.2.5/CLUMP/examples/Example_Euclidean_3D_Extended.py` & `clump-python-0.2.6/CLUMP/examples/Example_Euclidean_3D_Extended.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Script to run GenerateClump_Euclidean_3D (Extended Euclidean method)
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
-# 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
+# 2024 Translated from MATLAB to Python by A.U. Canbolat <utku.canbolat@fau.de>
 
 
 from CLUMP import GenerateClump_Euclidean_3D
 import sys
 import os
 sys.path.append('../../')
```

### Comparing `clump-python-0.2.5/CLUMP/examples/Example_ExtractSurface.py` & `clump-python-0.2.6/CLUMP/examples/Example_ExtractSurface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Script to demonstrate the ExtractSurface function
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
-# 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
+# 2024 Translated from MATLAB to Python by A.U. Canbolat <utku.canbolat@fau.de>
 
 import numpy as np
 from CLUMP import ExtractSurface
 from CLUMP.utils.STL_ReaderWriter import write_stl
 
 clump = np.array([[1, 0, 0, 1.1],
                   [2, 1, 0, 1.1],
```

### Comparing `clump-python-0.2.5/CLUMP/examples/Example_Favier_automatic_generation.py` & `clump-python-0.2.6/CLUMP/examples/Example_Favier_automatic_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Script to run GenerateClump_Favier
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
-# 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
+# 2024 Translated from MATLAB to Python by A.U. Canbolat <utku.canbolat@fau.de>
 
 from CLUMP import GenerateClump_Favier
 import sys
 import os
 sys.path.append('../../')
 
 inputGeom = os.path.join(os.path.dirname(__file__), 'ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl')
```

### Comparing `clump-python-0.2.5/CLUMP/examples/Example_Ferellec_McDowell.py` & `clump-python-0.2.6/CLUMP/examples/Example_Ferellec_McDowell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Script to run GenerateClump_Ferellec_McDowell
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
-# 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
+# 2024 Translated from MATLAB to Python by A.U. Canbolat <utku.canbolat@fau.de>
 
 from CLUMP import GenerateClump_Ferellec_McDowell
 import sys
 import os
 sys.path.append('../../')
 
 inputGeom = os.path.join(os.path.dirname(__file__), 'ParticleGeometries/Torus.stl')
```

### Comparing `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat` & `clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat` & `clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl` & `clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Hexahedron.stl` & `clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Hexahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Human_femur.stl` & `clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Human_femur.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Octahedron.stl` & `clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Octahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.5/CLUMP/examples/ParticleGeometries/Torus.stl` & `clump-python-0.2.6/CLUMP/examples/ParticleGeometries/Torus.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.5/CLUMP/utils/MyRobustCrust.py` & `clump-python-0.2.6/CLUMP/utils/MyRobustCrust.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import time
 from scipy.spatial import Delaunay
 
 """
 2017 Original author in MATLAB is Luigi Giaccari: https://www.mathworks.com/matlabcentral/fileexchange/63731-surface-reconstruction-from-scattered-points-cloud-open-surfaces?s_tid=srchtitle
 
-2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
+2024 Translated from MATLAB to Python by A.U. Canbolat <utku.canbolat@fau.de>
 """
 
 def MyRobustCrust(p):
     # error check
     if len(p.shape) > 2 or p.shape[1] != 3:
         raise ValueError("Input 3D points must be stored in a Nx3 array")
```

### Comparing `clump-python-0.2.5/CLUMP/utils/ParticlePlotter.py` & `clump-python-0.2.6/CLUMP/utils/ParticlePlotter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import pyvista as pv
 import trimesh
 
+"2024 Python implementation by A.U. Canbolat and V. Angelidakis  <utku.canbolat@fau.de>"
+
 def clump_plotter(P, F, clump):
     """Plots 3D spheres using trisurf"""
     fig = plt.figure()
     ax = fig.add_subplot(111, projection='3d')
 
     # Create patch
     ax.plot_trisurf(P[:, 0], P[:, 1], P[:, 2], triangles=F, color=[0, 1, 0, 0.2], edgecolor='none')
@@ -23,52 +25,46 @@
         Y = r * np.sin(u) * np.sin(v) + y
         Z = r * np.cos(v) + z
         ax.plot_surface(X, Y, Z, color=np.random.rand(3), edgecolor='none')
 
     plt.show()
 
 
+def add_sphere_to_plotter(plotter, center, radius, color, opacity, phi_res, theta_res):
+    """Utility function to add a sphere to the plotter."""
+    sphere = pv.Sphere(radius=radius, center=center, phi_resolution=phi_res, theta_resolution=theta_res)
+    plotter.add_mesh(sphere, color=color, opacity=opacity)
+
+
 def clump_plotter_pyvista(clump, opacity=1.0, phi_res=50, theta_res=50):
     """Plots 3D spheres using PyVista with increased opacity, a white background, and a finer mesh.
     Each sphere is defined by its center (x, y, z) and radius r.
-    :param spheres_data: Array of sphere data [[x1, y1, z1, r1], ..., [xn, yn, zn, rn]]
-    :param opacity: Opacity of the spheres, default is 1.0
-    :param phi_res: Resolution of the mesh in the azimuthal direction
-    :param theta_res: Resolution of the mesh in the polar direction
     """
-
     spheres_data = np.hstack((clump.positions, clump.radii))
-
     plotter = pv.Plotter()
 
-    # Precompute colors for all spheres
-    colors = [plt.cm.jet(i / len(spheres_data)) for i in range(len(spheres_data))]
+    colors = [plt.cm.jet(i / len(spheres_data)) for i in range(len(spheres_data))]  # Color mapping for spheres
 
-    # Batch process the spheres
-    for (x, y, z, r), color in zip(spheres_data, colors):
-        sphere = pv.Sphere(radius=r, center=(x, y, z), phi_resolution=phi_res, theta_resolution=theta_res)
-        plotter.add_mesh(sphere, color=color, opacity=opacity)
+    for sphere_data, color in zip(spheres_data, colors):
+        add_sphere_to_plotter(plotter, sphere_data[:3], sphere_data[3], color, opacity, phi_res, theta_res)
 
     plotter.show(interactive=True)
 
 
-def mesh_plotter_trimesh(vertices, faces):
-    # Create a trimesh object
+def mesh_plotter_trimesh(vertices, faces, spheresList, phi_res=50, theta_res=50):
+    """Plots a wireframe mesh and spheres using trimesh and PyVista."""
     mesh = trimesh.Trimesh(vertices=vertices, faces=faces)
-
-    # Create a PyVista mesh
     pv_mesh = pv.wrap(mesh)
 
-    # Create a plotter
     plotter = pv.Plotter()
+    plotter.add_mesh(pv_mesh, style='wireframe', color='black', line_width=2)
 
-    # Add the mesh to the plotter
-    plotter.add_mesh(pv_mesh, color='blue', opacity=0.5, show_edges=True)
+    for (x, y, z, r) in spheresList:
+        add_sphere_to_plotter(plotter, (x, y, z), r, 'white', 0.5, phi_res, theta_res)
 
-    # Set the camera position
-    plotter.camera_position = [(np.min(vertices[:, 0]) + np.max(vertices[:, 0])) / 2,
-                               (np.min(vertices[:, 1]) + np.max(vertices[:, 1])) / 2,
-                               np.max(vertices[:, 2]) * 2]
+    plotter.camera_position = [
+        (np.min(vertices[:, 0]) + np.max(vertices[:, 0])) / 2,
+        (np.min(vertices[:, 1]) + np.max(vertices[:, 1])) / 2,
+        np.max(vertices[:, 2]) * 2
+    ]
 
-    # Show the plot
     plotter.show()
-
```

### Comparing `clump-python-0.2.5/CLUMP/utils/RigidBodyParameters.py` & `clump-python-0.2.6/CLUMP/utils/RigidBodyParameters.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.5/CLUMP/utils/STL_ReaderWriter.py` & `clump-python-0.2.6/CLUMP/utils/STL_ReaderWriter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 from stl.mesh import Mesh
 
+"2024 Python implementation by A.U. Canbolat <utku.canbolat@fau.de>"
+
 def read_stl(stl_dir, is_duplicated=False):
     """ Read stl files into mesh. mesh contains all the required information"""
     mesh = Mesh.from_file(stl_dir)
 
     # extract the vectors of vertices
     P = mesh.points.reshape(-1, 3)
 
@@ -18,47 +20,14 @@
         # it discards the common vertices to avoid duplication.
         P_unique, indices = np.unique(P, return_inverse=True, axis=0)
 
         F_unique = indices.reshape(-1, 3)
 
         return F_unique, P_unique
 
-
-"""def read_stl(stl_dir, isDuplicated=False):
-    # read stl files into mesh. mesh contains all the required information
-    mesh = Mesh.from_file(stl_dir)
-
-    # extract the vectors of vertices
-    # note: below can be vectorized. it is good for now.
-    P = np.zeros((mesh.points.shape[0] * 3, 3))
-    k = 0
-    for row in mesh.points:
-        P[k, :] = row[0:3]
-        P[k + 1, :] = row[3:6]
-        P[k + 2, :] = row[6:9]
-        k += 3
-
-    # face enumeration
-    F = np.arange(0, P.shape[0]).reshape(mesh.points.shape[0], 3)  # BE CAREFUL INDEXING. IT STARTS FROM 0 NOT 1
-
-    # now take unique values to do stl.SlimVerts.m's job
-    # it discards the common vertices to avoid dublication. This can be controlled by isDuplicated flag.
-    F_redefine = np.arange(0, P.shape[0])  # BE CAREFUL INDEXING. IT STARTS FROM 0 NOT 1
-    P_unique, indices = np.unique(P, return_inverse=True, axis=0)
-
-    F_unique = F_redefine[indices]
-    F_unique = F_unique.reshape(F_unique.shape[0] // 3, 3)
-
-    if isDuplicated:
-        return F, P
-    else:
-        return F_unique, P_unique"""
-
-
-
 def compute_normal(v1, v2, v3):
     """ Compute the normal vector of a triangle given its vertices.
 
     Parameters:
         v1, v2, v3 (tuple): Vertices of the triangle.
 
     Returns:
```

### Comparing `clump-python-0.2.5/CLUMP/utils/VTK_Writer.py` & `clump-python-0.2.6/CLUMP/utils/VTK_Writer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 import os
 
+"2024 Python implementation by A.U. Canbolat <utku.canbolat@fau.de>"
+
 def clump_to_VTK(clump, filepath=os.path.join(os.getcwd(), "spheres.vtk")):
     """ Write sphere data to a VTK file without using external libraries.
 
     Parameters:
     spheres (np.array): Numpy array containing sphere data (positions and radii).
     output_dir (str): Directory where the VTK file will be saved.
     filename (str): Name of the VTK file.
```

### Comparing `clump-python-0.2.5/LICENSE` & `clump-python-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.5/PKG-INFO` & `clump-python-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.2.5
+Version: 0.2.6
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.2.5/README.md` & `clump-python-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.5/clump_python.egg-info/PKG-INFO` & `clump-python-0.2.6/clump_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.2.5
+Version: 0.2.6
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.2.5/clump_python.egg-info/SOURCES.txt` & `clump-python-0.2.6/clump_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
 CLUMP/ExtractSurface.py
 CLUMP/GenerateClump_Euclidean_3D.py
 CLUMP/GenerateClump_Favier.py
 CLUMP/GenerateClump_Ferellec_McDowell.py
 CLUMP/__init__.py
 CLUMP/examples/Example_Euclidean_3D.py
```

### Comparing `clump-python-0.2.5/setup.py` & `clump-python-0.2.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clump-python",
-    version="0.2.5",
+    version="0.2.6",
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
         'numpy-stl',
         'pyvista',
         'scipy',
```

