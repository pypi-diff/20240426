# Comparing `tmp/pycanha_core-0.1.0.tar.gz` & `tmp/pycanha_core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycanha_core-0.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pycanha_core-0.1.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pycanha_core-0.1.0.tar` & `pycanha_core-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,36 @@
--rw-r--r--   0        0        0     3242 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.github/workflows/build-publish-wheels.yml
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.gitignore
--rw-r--r--   0        0        0      156 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.gitmodules
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1027 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/LICENSE
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/README.md
--rw-r--r--   0        0        0     1317 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/docs/index.md
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/docs/installation.md
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/docs/requirements.txt
--rw-r--r--   0        0        0     4185 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      560 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/CMakeLists.txt
--rw-r--r--   0        0        0      806 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/__init__.py
--rw-r--r--   0        0        0     3776 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/geometry.hpp
--rw-r--r--   0        0        0      982 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/geometrymodel.hpp
--rw-r--r--   0        0        0     8431 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/primitives.hpp
--rw-r--r--   0        0        0     1920 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/thermalmesh.hpp
--rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/transformations.hpp
--rw-r--r--   0        0        0     7877 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/trimesh.hpp
--rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/conanfile.txt.in
--rw-r--r--   0        0        0     4859 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/prepare-build-backend.py
--rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/pycanha-core-conan-profile
--rw-r--r--   0        0        0     1004 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/pycanha-core-wrapper.cpp
--rw-r--r--   0        0        0     7438 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/pycanha_core.pyi
--rw-r--r--   0        0        0     2229 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/test/primitives/test_triangle.py
--rw-r--r--   0        0        0      920 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3952 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/.github/workflows/build-publish-wheels.yml
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/.gitignore
+-rw-r--r--   0        0        0      156 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/.gitmodules
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1027 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/LICENSE
+-rw-r--r--   0        0        0      492 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/README.md
+-rw-r--r--   0        0        0     1882 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/docs/conf.py
+-rw-r--r--   0        0        0      199 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/docs/index.md
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/docs/installation.md
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/docs/modules.rst
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/docs/pycanha_core.rst
+-rw-r--r--   0        0        0       59 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0     4203 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core/__init__.py
+-rw-r--r--   0        0        0      173 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core/__init__.pyi
+-rw-r--r--   0        0        0     7555 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core/gmm.pyi
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core/py.typed
+-rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/CMakeLists.txt
+-rw-r--r--   0        0        0     3776 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/geometry.hpp
+-rw-r--r--   0        0        0      982 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/geometrymodel.hpp
+-rw-r--r--   0        0        0     8431 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/primitives.hpp
+-rw-r--r--   0        0        0     1920 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/thermalmesh.hpp
+-rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/transformations.hpp
+-rw-r--r--   0        0        0     7877 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/trimesh.hpp
+-rw-r--r--   0        0        0      630 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/conanfile.txt
+-rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/conanfile.txt.in
+-rw-r--r--   0        0        0     4922 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/prepare-build-backend.py
+-rw-r--r--   0        0        0      881 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/pycanha-core-conan-profile
+-rw-r--r--   0        0        0     1312 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/src/pycanha_core_bindings/pycanha-core-wrapper.cpp
+-rw-r--r--   0        0        0     2166 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/test/primitives/test_triangle.py
+-rw-r--r--   0        0        0     1374 2022-11-09 12:37:21.000000 pycanha_core-0.1.2/PKG-INFO
```

### Comparing `pycanha_core-0.1.0/.github/workflows/build-publish-wheels.yml` & `pycanha_core-0.1.2/.github/workflows/build-publish-wheels.yml`

 * *Files 22% similar despite different names*

```diff
@@ -74,14 +74,35 @@
 
       # Build wheels
       - name: Build sddist and wheels
         run: |
           cd pycanha-project/pycanha-core-python
           python -m build
 
+      # Repair wheel with auditwheel (only for Ubuntu)
+      - name: Repair wheel with auditwheel
+        if: matrix.os == 'ubuntu'
+        run: |
+          cd pycanha-project/pycanha-core-python/dist   
+          # Install auditwheel
+          python -m pip install auditwheel
+          # Install patchelf
+          sudo apt-get update
+          sudo apt-get install patchelf
+          # Repair the wheel
+          for whl in *.whl; do
+            auditwheel repair "$whl" --plat manylinux_2_34_x86_64 -w output
+          done
+          # Remove the original, non-repaired wheels
+          rm *.whl
+          # Move repaired wheels to dist for artifact upload
+          mv output/* .
+          rm -r output
+
+
       # Upload the artifacts wheels
       - uses: actions/upload-artifact@v4
         with:
           name: pycanha-dist-files-${{ matrix.os }}-${{ matrix.python-version }}
           path: pycanha-project/pycanha-core-python/dist/*.whl
 
       - name: Upload sdist
```

### Comparing `pycanha_core-0.1.0/.pytest_cache/v/cache/nodeids` & `pycanha_core-0.1.2/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.1.0/.readthedocs.yaml` & `pycanha_core-0.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.1.0/LICENSE` & `pycanha_core-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.1.0/pyproject.toml` & `pycanha_core-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["scikit-build-core>=0.8", "pybind11", "cmake", "conan>=2.0, !=2.2.0", "toml"]
 # For a "regular" build with scikit-build-core, you would just use:
 # build-backend = "scikit_build_core.build"
 build-backend = "prepare-build-backend" # Custom wrapper around scikit_build_core.build See comments in prepare-build-backend.py.
 backend-path = [
-    "src/pycanha_core",
+    "src/pycanha_core_bindings",
 ] #For in-tree builds, we need to add the directory to the path. See: https://peps.python.org/pep-0517/#in-tree-build-backends
 
 [project]
 name = "pycanha-core"
-version = "0.1.0"
+version = "0.1.2"
 description = "Python bindings for pycanha-core with Pybind11"
 readme = "README.md"
 authors = [{ name = "Javier Piqueras Carreño", email = "javier.piqueras@upm.es" }]
 requires-python = ">=3.11"
 classifiers = [
     #Add licence classifiers
     #Add development status classifiers
@@ -39,15 +39,15 @@
 # Fallback on gmake/make if available and ninja is missing (Unix). Will only
 # fallback on platforms without a known ninja wheel.
 ninja.make-fallback = false
 
 # Extra args for CMake. Pip, unlike build, does not support lists, so semicolon
 # can be used to separate. Setting this in config or envvar will override the
 # entire list. See also cmake.define.
-cmake.args = ["--preset=conan-release", "-S src/pycanha_core"]
+cmake.args = ["--preset=conan-release", "-S src/pycanha_core_bindings"]
 
 # This activates verbose builds
 cmake.verbose = true
 
 # This controls the CMake build type
 cmake.build-type = "Release"
```

### Comparing `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/geometry.hpp` & `pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/geometry.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/geometrymodel.hpp` & `pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/geometrymodel.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/primitives.hpp` & `pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/primitives.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/thermalmesh.hpp` & `pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/thermalmesh.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/transformations.hpp` & `pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/transformations.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/trimesh.hpp` & `pycanha_core-0.1.2/src/pycanha_core_bindings/bindings/gmm/trimesh.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.1.0/src/pycanha_core/conanfile.txt.in` & `pycanha_core-0.1.2/src/pycanha_core_bindings/conanfile.txt.in`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.1.0/src/pycanha_core/prepare-build-backend.py` & `pycanha_core-0.1.2/src/pycanha_core_bindings/prepare-build-backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 # Get version of the bindings from pyproject.toml
 import toml
 
 pyproject = toml.load("pyproject.toml")
 bindings_version_str = ".".join(pyproject["project"]["version"].split(".")[:2])
 
 # Configure the binding version in conanfile.txt (of the bindings)
-with open("src/pycanha_core/conanfile.txt.in", "r") as file:
+with open("src/pycanha_core_bindings/conanfile.txt.in", "r") as file:
     conanfile_txt_in = file.read()
     conanfile_txt = conanfile_txt_in.replace(
         "@CONFIG_PYCANHA_CORE_VERSION@", bindings_version_str
     )
-    with open("src/pycanha_core/conanfile.txt", "w") as file:
+    with open("src/pycanha_core_bindings/conanfile.txt", "w") as file:
         file.write(conanfile_txt)
 
 
 # Check pycanha-core is available in ../pycanha-core. If available, check the version is correct.
 # Read ../pycanha-core/conanfile.py
 import re
 
@@ -60,16 +60,16 @@
 
 result = subprocess.run(
     [
         "conan",
         "create",
         "../pycanha-core",
         "--build=missing",
-        "-pr:h=src/pycanha_core/pycanha-core-conan-profile",
-        "-pr:b=src/pycanha_core/pycanha-core-conan-profile",
+        "-pr:h=src/pycanha_core_bindings/pycanha-core-conan-profile",
+        "-pr:b=src/pycanha_core_bindings/pycanha-core-conan-profile",
     ],
     stdout=subprocess.PIPE,
     stderr=subprocess.PIPE,
 )
 if result.returncode == 0:
     print("Success!")
 else:
@@ -80,18 +80,18 @@
     # raise RuntimeError("Conan install failed. See error above.")
 
 # "Inject" the conan install before the build hooks are called.
 result = subprocess.run(
     [
         "conan",
         "install",
-        "src/pycanha_core",
+        "src/pycanha_core_bindings",
         "--build=missing",
-        "-pr:h=src/pycanha_core/pycanha-core-conan-profile",
-        "-pr:b=src/pycanha_core/pycanha-core-conan-profile",
+        "-pr:h=src/pycanha_core_bindings/pycanha-core-conan-profile",
+        "-pr:b=src/pycanha_core_bindings/pycanha-core-conan-profile",
     ],
     stdout=subprocess.PIPE,
     stderr=subprocess.PIPE,
 )
 if result.returncode == 0:
     print("Success!")
 else:
```

### Comparing `pycanha_core-0.1.0/src/pycanha_core/pycanha_core.pyi` & `pycanha_core-0.1.2/src/pycanha_core/gmm.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import numpy as np
 
 class Point3D(np.ndarray):
     """A 3D point represented as a numpy array of floats."""
+
     pass
 
 class Vector3D(np.ndarray):
     """A 3D vector represented as a numpy array of floats."""
+
     pass
 
 class Point2D(np.ndarray):
     """A 2D point represented as a numpy array of floats."""
-    pass
 
+    pass
 
 class Triangle:
     """A class representing a triangle in 3D space."""
 
     def __init__(self, p1: Point3D, p2: Point3D, p3: Point3D) -> None:
         """Constructs a triangle with the three vertices."""
         pass
@@ -199,15 +201,23 @@
     def from_2D_to_3D(self, p2D: Point2D) -> Point3D:
         """Maps a point from the 2D space of the quadrilateral to 3D space."""
         pass
 
 class Cylinder:
     """A class representing a cylinder in 3D space."""
 
-    def __init__(self, p1: Point3D, p2: Point3D, p3: Point3D, radius: float, start_angle: float, end_angle: float) -> None:
+    def __init__(
+        self,
+        p1: Point3D,
+        p2: Point3D,
+        p3: Point3D,
+        radius: float,
+        start_angle: float,
+        end_angle: float,
+    ) -> None:
         """Constructs a cylinder with the three vertices and additional parameters."""
         pass
 
     @property
     def p1(self) -> Point3D:
         """The first vertex of the cylinder."""
         pass
@@ -279,7 +289,9 @@
         """Maps a point from 3D space to the 2D space of the cylinder."""
         pass
 
     def from_2D_to_3D(self, p2D: Point2D) -> Point3D:
         """Maps a point from the 2D space of the cylinder to 3D space."""
         pass
 
+# Remove foreign packages from the namespace
+del np
```

### Comparing `pycanha_core-0.1.0/test/primitives/test_triangle.py` & `pycanha_core-0.1.2/test/primitives/test_triangle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 import numpy as np
 
-# Assuming `pycanha_core` is the module where Triangle and related classes are defined
-from pycanha_core import Triangle
+import pycanha_core
+
+Triangle = pycanha_core.gmm.Triangle
 
 
 @pytest.fixture
 def point3d_1():
     return np.array([1.0, 2.0, 3.0])
```

### Comparing `pycanha_core-0.1.0/PKG-INFO` & `pycanha_core-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pycanha-core
-Version: 0.1.0
+Version: 0.1.2
 Summary: Python bindings for pycanha-core with Pybind11
-Author-Email: Javier Piqueras Carreño <javier.piqueras@upm.es>
+Author-Email: =?utf-8?q?Javier_Piqueras_Carre=C3=B1o?= <javier.piqueras@upm.es>
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Homepage, https://github.com/pycanha-project/pycanha-core-python
 Project-URL: Bug tracker, https://github.com/pycanha-project/pycanha-core-python/issues
 Requires-Python: >=3.11
 Requires-Dist: numpy>=1.24.0
@@ -16,10 +16,14 @@
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx-autoapi; extra == "docs"
 Provides-Extra: test
 Provides-Extra: build
 Provides-Extra: docs
 Description-Content-Type: text/markdown
 
-# pycanha-core
+# Python bindings for pycanha-core
 
-The python bindings for pycanha-core.
+
+[![Build and publish wheels](https://github.com/pycanha-project/pycanha-core-python/actions/workflows/build-publish-wheels.yml/badge.svg)](https://github.com/pycanha-project/pycanha-core-python/actions/workflows/build-publish-wheels.yml)
+[![Documentation Status](https://readthedocs.org/projects/pycanha-core-python/badge/?version=latest)](https://pycanha-core-python.readthedocs.io/latest/?badge=latest)
+
+The python bindings for the C++ core of Pycanha.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

