# Comparing `tmp/earthkit-geo-0.0.1.tar.gz` & `tmp/earthkit_geo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit-geo-0.0.1.tar", last modified: Mon Mar 11 15:31:28 2024, max compression
+gzip compressed data, was "earthkit_geo-0.1.0.tar", last modified: Fri Apr 26 10:48:05 2024, max compression
```

## Comparing `earthkit-geo-0.0.1.tar` & `earthkit_geo-0.1.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-11 15:31:28.725761 earthkit-geo-0.0.1/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-11 15:31:28.622479 earthkit-geo-0.0.1/.github/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-11 15:31:28.663322 earthkit-geo-0.0.1/.github/workflows/
--rw-r--r--   0 cgr        (501) staff       (20)     3667 2024-03-11 14:51:37.000000 earthkit-geo-0.0.1/.github/workflows/ci_other.yml
--rw-r--r--   0 cgr        (501) staff       (20)      235 2024-03-11 14:42:05.000000 earthkit-geo-0.0.1/.github/workflows/label-public-pr.yml
--rw-r--r--   0 cgr        (501) staff       (20)      275 2024-03-11 14:42:09.000000 earthkit-geo-0.0.1/.github/workflows/notify-new-issue.yml
--rw-r--r--   0 cgr        (501) staff       (20)      279 2024-03-11 14:42:12.000000 earthkit-geo-0.0.1/.github/workflows/notify-new-pr.yml
--rw-r--r--   0 cgr        (501) staff       (20)     7224 2024-03-11 14:48:54.000000 earthkit-geo-0.0.1/.gitignore
--rw-r--r--   0 cgr        (501) staff       (20)     1132 2024-03-11 12:36:15.000000 earthkit-geo-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 cgr        (501) staff       (20)      137 2024-03-11 12:36:48.000000 earthkit-geo-0.0.1/.readthedocs.yml
--rw-r--r--   0 cgr        (501) staff       (20)    11382 2024-03-11 15:30:26.000000 earthkit-geo-0.0.1/LICENSE
--rw-r--r--   0 cgr        (501) staff       (20)      753 2024-03-11 13:44:31.000000 earthkit-geo-0.0.1/Makefile
--rw-r--r--   0 cgr        (501) staff       (20)     3086 2024-03-11 15:31:28.725610 earthkit-geo-0.0.1/PKG-INFO
--rw-r--r--   0 cgr        (501) staff       (20)     2030 2024-03-11 15:30:26.000000 earthkit-geo-0.0.1/README.md
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-11 15:31:28.684744 earthkit-geo-0.0.1/docs/
--rw-r--r--   0 cgr        (501) staff       (20)      634 2024-03-11 14:29:21.000000 earthkit-geo-0.0.1/docs/Makefile
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-11 15:31:28.688359 earthkit-geo-0.0.1/docs/_static/
--rw-r--r--   0 cgr        (501) staff       (20)        0 2024-03-11 14:30:22.000000 earthkit-geo-0.0.1/docs/_static/.gitkeep
--rw-r--r--   0 cgr        (501) staff       (20)      832 2024-03-11 14:30:54.000000 earthkit-geo-0.0.1/docs/_static/style.css
--rw-r--r--   0 cgr        (501) staff       (20)     2610 2024-03-11 14:47:43.000000 earthkit-geo-0.0.1/docs/conf.py
--rw-r--r--   0 cgr        (501) staff       (20)     1514 2024-03-11 15:19:51.000000 earthkit-geo-0.0.1/docs/development.rst
--rw-r--r--   0 cgr        (501) staff       (20)      818 2024-03-11 13:59:08.000000 earthkit-geo-0.0.1/docs/index.rst
--rw-r--r--   0 cgr        (501) staff       (20)      337 2024-03-11 15:30:26.000000 earthkit-geo-0.0.1/docs/install.rst
--rw-r--r--   0 cgr        (501) staff       (20)      813 2024-03-11 14:29:01.000000 earthkit-geo-0.0.1/docs/licence.rst
--rw-r--r--   0 cgr        (501) staff       (20)      224 2024-03-11 14:33:16.000000 earthkit-geo-0.0.1/docs/references.rst
--rw-r--r--   0 cgr        (501) staff       (20)      129 2024-03-11 14:29:49.000000 earthkit-geo-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-11 15:31:28.623160 earthkit-geo-0.0.1/earthkit/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-11 15:31:28.699873 earthkit-geo-0.0.1/earthkit/geo/
--rw-r--r--   0 cgr        (501) staff       (20)      939 2024-03-11 12:46:30.000000 earthkit-geo-0.0.1/earthkit/geo/__init__.py
--rw-r--r--   0 cgr        (501) staff       (20)      707 2024-03-11 14:32:24.000000 earthkit-geo-0.0.1/earthkit/geo/constants.py
--rw-r--r--   0 cgr        (501) staff       (20)     8278 2024-03-11 14:37:08.000000 earthkit-geo-0.0.1/earthkit/geo/distance.py
--rw-r--r--   0 cgr        (501) staff       (20)       72 2024-03-11 15:31:28.000000 earthkit-geo-0.0.1/earthkit/geo/version.py
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-11 15:31:28.724529 earthkit-geo-0.0.1/earthkit_geo.egg-info/
--rw-r--r--   0 cgr        (501) staff       (20)     3086 2024-03-11 15:31:28.000000 earthkit-geo-0.0.1/earthkit_geo.egg-info/PKG-INFO
--rw-r--r--   0 cgr        (501) staff       (20)      861 2024-03-11 15:31:28.000000 earthkit-geo-0.0.1/earthkit_geo.egg-info/SOURCES.txt
--rw-r--r--   0 cgr        (501) staff       (20)        1 2024-03-11 15:31:28.000000 earthkit-geo-0.0.1/earthkit_geo.egg-info/dependency_links.txt
--rw-r--r--   0 cgr        (501) staff       (20)       80 2024-03-11 15:31:28.000000 earthkit-geo-0.0.1/earthkit_geo.egg-info/requires.txt
--rw-r--r--   0 cgr        (501) staff       (20)        9 2024-03-11 15:31:28.000000 earthkit-geo-0.0.1/earthkit_geo.egg-info/top_level.txt
--rw-r--r--   0 cgr        (501) staff       (20)      232 2024-03-11 14:44:53.000000 earthkit-geo-0.0.1/environment.yml
--rw-r--r--   0 cgr        (501) staff       (20)      405 2024-03-11 12:40:53.000000 earthkit-geo-0.0.1/pyproject.toml
--rw-r--r--   0 cgr        (501) staff       (20)       48 2024-03-11 14:45:38.000000 earthkit-geo-0.0.1/pytest.ini
--rw-r--r--   0 cgr        (501) staff       (20)     1064 2024-03-11 15:31:28.726765 earthkit-geo-0.0.1/setup.cfg
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-11 15:31:28.719050 earthkit-geo-0.0.1/tests/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-11 15:31:28.722107 earthkit-geo-0.0.1/tests/distance/
--rw-r--r--   0 cgr        (501) staff       (20)     5226 2024-03-11 14:38:33.000000 earthkit-geo-0.0.1/tests/distance/test_distance.py
--rw-r--r--   0 cgr        (501) staff       (20)       38 2024-03-11 14:48:54.000000 earthkit-geo-0.0.1/tests/downstream-ci-requirements.txt
--rw-r--r--   0 cgr        (501) staff       (20)      258 2024-03-11 14:48:54.000000 earthkit-geo-0.0.1/tests/environment-unit-tests.yml
--rw-r--r--   0 cgr        (501) staff       (20)      491 2024-03-11 13:45:59.000000 earthkit-geo-0.0.1/tests/test_version.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.795639 earthkit_geo-0.1.0/
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.756049 earthkit_geo-0.1.0/.github/
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.766875 earthkit_geo-0.1.0/.github/workflows/
+-rw-r--r--   0 cgr        (501) staff       (20)     3667 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.github/workflows/ci_other.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      235 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.github/workflows/label-public-pr.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      275 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.github/workflows/notify-new-issue.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      279 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.github/workflows/notify-new-pr.yml
+-rw-r--r--   0 cgr        (501) staff       (20)     7224 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.gitignore
+-rw-r--r--   0 cgr        (501) staff       (20)     1132 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 cgr        (501) staff       (20)      137 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/.readthedocs.yml
+-rw-r--r--   0 cgr        (501) staff       (20)    11382 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/LICENSE
+-rw-r--r--   0 cgr        (501) staff       (20)      753 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/Makefile
+-rw-r--r--   0 cgr        (501) staff       (20)     3086 2024-04-26 10:48:05.795473 earthkit_geo-0.1.0/PKG-INFO
+-rw-r--r--   0 cgr        (501) staff       (20)     2030 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/README.md
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.776152 earthkit_geo-0.1.0/docs/
+-rw-r--r--   0 cgr        (501) staff       (20)      634 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/Makefile
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.777799 earthkit_geo-0.1.0/docs/_static/
+-rw-r--r--   0 cgr        (501) staff       (20)        0 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/_static/.gitkeep
+-rw-r--r--   0 cgr        (501) staff       (20)      832 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/_static/style.css
+-rw-r--r--   0 cgr        (501) staff       (20)     2610 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/conf.py
+-rw-r--r--   0 cgr        (501) staff       (20)     1514 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/development.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      818 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/index.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      337 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/install.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      813 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/licence.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      224 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/references.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      129 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/docs/requirements.txt
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.756756 earthkit_geo-0.1.0/earthkit/
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.787150 earthkit_geo-0.1.0/earthkit/geo/
+-rw-r--r--   0 cgr        (501) staff       (20)     1028 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/earthkit/geo/__init__.py
+-rw-r--r--   0 cgr        (501) staff       (20)      482 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/earthkit/geo/constants.py
+-rw-r--r--   0 cgr        (501) staff       (20)     9817 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/earthkit/geo/distance.py
+-rw-r--r--   0 cgr        (501) staff       (20)     1444 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/earthkit/geo/figure.py
+-rw-r--r--   0 cgr        (501) staff       (20)       72 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit/geo/version.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.794685 earthkit_geo-0.1.0/earthkit_geo.egg-info/
+-rw-r--r--   0 cgr        (501) staff       (20)     3086 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit_geo.egg-info/PKG-INFO
+-rw-r--r--   0 cgr        (501) staff       (20)      884 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 cgr        (501) staff       (20)        1 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 cgr        (501) staff       (20)       80 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit_geo.egg-info/requires.txt
+-rw-r--r--   0 cgr        (501) staff       (20)        9 2024-04-26 10:48:05.000000 earthkit_geo-0.1.0/earthkit_geo.egg-info/top_level.txt
+-rw-r--r--   0 cgr        (501) staff       (20)      232 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/environment.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      405 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/pyproject.toml
+-rw-r--r--   0 cgr        (501) staff       (20)       48 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/pytest.ini
+-rw-r--r--   0 cgr        (501) staff       (20)     1064 2024-04-26 10:48:05.796331 earthkit_geo-0.1.0/setup.cfg
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.793886 earthkit_geo-0.1.0/tests/
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-04-26 10:48:05.794276 earthkit_geo-0.1.0/tests/distance/
+-rw-r--r--   0 cgr        (501) staff       (20)     6069 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/tests/distance/test_distance.py
+-rw-r--r--   0 cgr        (501) staff       (20)       38 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/tests/downstream-ci-requirements.txt
+-rw-r--r--   0 cgr        (501) staff       (20)      258 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/tests/environment-unit-tests.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      491 2024-04-26 10:46:05.000000 earthkit_geo-0.1.0/tests/test_version.py
```

### Comparing `earthkit-geo-0.0.1/.github/workflows/ci_other.yml` & `earthkit_geo-0.1.0/.github/workflows/ci_other.yml`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/.gitignore` & `earthkit_geo-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/.pre-commit-config.yaml` & `earthkit_geo-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/LICENSE` & `earthkit_geo-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/Makefile` & `earthkit_geo-0.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/PKG-INFO` & `earthkit_geo-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-geo
-Version: 0.0.1
+Version: 0.1.0
 Summary: A format-agnostic Python interface for geospatial data
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `earthkit-geo-0.0.1/README.md` & `earthkit_geo-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/docs/Makefile` & `earthkit_geo-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/docs/_static/style.css` & `earthkit_geo-0.1.0/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/docs/conf.py` & `earthkit_geo-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/docs/development.rst` & `earthkit_geo-0.1.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/docs/index.rst` & `earthkit_geo-0.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/docs/licence.rst` & `earthkit_geo-0.1.0/docs/licence.rst`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/earthkit/geo/__init__.py` & `earthkit_geo-0.1.0/earthkit/geo/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 
 from earthkit.geo.distance import (
     GeoKDTree,
     haversine_distance,
     nearest_point_haversine,
     nearest_point_kdtree,
 )
+from earthkit.geo.figure import IFS_SPHERE, UNIT_SPHERE
 
 __all__ = [
     "GeoKDTree",
     "haversine_distance",
+    IFS_SPHERE,
     "nearest_point_haversine",
     "nearest_point_kdtree",
+    UNIT_SPHERE,
     "__version__",
 ]
```

### Comparing `earthkit-geo-0.0.1/earthkit/geo/distance.py` & `earthkit_geo-0.1.0/earthkit/geo/distance.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,39 +4,42 @@
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import numpy as np
-from scipy.spatial import KDTree
 
 from . import constants
+from .figure import IFS_SPHERE, UNIT_SPHERE
 
 
-def regulate_lat(lat):
+def _regulate_lat(lat):
     return np.where(np.abs(lat) > constants.north, np.nan, lat)
 
 
-def haversine_distance(p1, p2):
-    """Compute haversine distance between two (sets of) points on Earth.
+def haversine_distance(p1, p2, figure=IFS_SPHERE):
+    """Compute haversine distance between two (sets of) points on a spheroid.
 
     Parameters
     ----------
     p1: pair of array-like
         Locations of the first points. The first item specifies the latitudes,
         the second the longitudes (degrees)
     p2: pair of array-like
         Locations of the second points. The first item specifies the latitudes,
         the second the longitudes (degrees)
+    figure: :class:`geo.figure.Figure`, optional
+        Figure of the spheroid (default: :obj:`geo.figure.IFS_SPHERE`)
 
     Returns
     -------
     number or ndarray
-        Spherical distance on the surface in Earth (m)
+        Distance (m) on the surface of the spheroid defined by ``figure``.
+
 
     Either ``p1`` or ``p2`` must be a single point.
 
     Examples
     --------
     Compute the distance between Reading and Bologna.
 
@@ -70,50 +73,52 @@
         raise ValueError(
             f"haversine_distance: lat and lon in p2 must have the same shape! {lat2.shape} != {lon2.shape}"
         )
 
     if lat1.size != 1 and lat2.size != 1:
         raise ValueError("haversine_distance: either p1 or p2 must be a single point")
 
-    lat1 = regulate_lat(lat1)
-    lat2 = regulate_lat(lat2)
+    lat1 = _regulate_lat(lat1)
+    lat2 = _regulate_lat(lat2)
 
     lat1, lon1, lat2, lon2 = map(np.deg2rad, [lat1, lon1, lat2, lon2])
     d_lon = lon2 - lon1
     d_lat = lat2 - lat1
 
     a = np.sqrt(
         np.sin(d_lat / 2) ** 2 + np.cos(lat1) * np.cos(lat2) * np.sin(d_lon / 2) ** 2
     )
-    c = 2 * np.arcsin(a)
-    distance = constants.R_earth * c
+    distance = 2 * np.arcsin(a)
 
-    return distance
+    return figure.scale(distance)
 
 
-def nearest_point_haversine(ref_points, points):
-    """Find the index of the nearest point to all ``ref_points`` in a set of ``points`` using the
-       haversine distance formula.
+def nearest_point_haversine(ref_points, points, figure=IFS_SPHERE):
+    """Find the index of the nearest point to all ``ref_points`` in a set of
+      ``points`` using the haversine distance formula.
 
     Parameters
     ----------
     ref_points: pair of array-like
         Latitude and longitude coordinates of the reference point (degrees)
     points: pair of array-like
         Locations of the set of points from which the nearest to
         ``ref_points`` is to be found. The first item specifies the latitudes,
         the second the longitudes (degrees)
+    figure: :class:`geo.figure.Figure`, optional
+        Figure of the spheroid the returned
+        distances are computed on (default: :obj:`geo.figure.IFS_SPHERE`)
 
     Returns
     -------
     ndarray
-        Indices of the nearest points to ``ref_points`.
+        Indices of the nearest points to ``ref_points``.
     ndarray
         The distance (m) between the ``ref_points`` and the corresponding nearest
-        point in ``points``.
+        point in ``points`` on the surface of the spheroid defined by ``figure``.
 
     Examples
     --------
     >>> from earthkit.geo import nearest_point_haversine
     >>> p_ref = (51.45, -0.97)
     >>> p_lat = [44.49, 50.73, 50.1]
     >>> p_lon = [11.34, 7.90, -8.1]
@@ -135,105 +140,136 @@
         raise ValueError(
             f"nearest_point_haversine: ref_point expected shape of (2,), got {ref_points.shape}"
         )
 
     res_index = []
     res_distance = []
     for lat, lon in ref_points.T:
-        distance = haversine_distance((lat, lon), points).flatten()
+        distance = haversine_distance((lat, lon), points, figure=UNIT_SPHERE).flatten()
         index = np.nanargmin(distance)
         index = index[0] if isinstance(index, np.ndarray) else index
         res_index.append(index)
         res_distance.append(distance[index])
-    return (np.array(res_index), np.array(res_distance))
+    return (np.array(res_index), figure.scale(np.array(res_distance)))
 
 
-def ll_to_xyz(lat, lon):
+def _latlon_to_xyz(lat, lon):
+    """Works on the unit sphere."""
     lat = np.asarray(lat)
     lon = np.asarray(lon)
     lat = np.radians(lat)
     lon = np.radians(lon)
-    x = constants.R_earth * np.cos(lat) * np.cos(lon)
-    y = constants.R_earth * np.cos(lat) * np.sin(lon)
-    z = constants.R_earth * np.sin(lat)
+    x = np.cos(lat) * np.cos(lon)
+    y = np.cos(lat) * np.sin(lon)
+    z = np.sin(lat)
+
     return x, y, z
 
 
-def cordlength_to_arclength(chord_length):
+def _chordlength_to_arclength(chord_length):
     """
     Convert 3D (Euclidean) distance to great circle arc length
     https://en.wikipedia.org/wiki/Great-circle_distance
+    Works on the unit sphere.
     """
-    central_angle = 2.0 * np.arcsin(chord_length / (2.0 * constants.R_earth))
-    return constants.R_earth * central_angle
+    central_angle = 2.0 * np.arcsin(chord_length / 2.0)
+    return central_angle
 
 
-def arclength_to_cordlenght(arc_length):
+def _arclength_to_chordlength(arc_length):
     """
     Convert great circle arc length to 3D (Euclidean) distance
     https://en.wikipedia.org/wiki/Great-circle_distance
+    Works on the unit sphere.
     """
-    central_angle = arc_length / constants.R_earth
-    return np.sin(central_angle / 2) * 2.0 * constants.R_earth
+    central_angle = arc_length
+    return np.sin(central_angle / 2) * 2.0
 
 
 class GeoKDTree:
     def __init__(self, lats, lons):
+        """KDTree built from ``lats`` and ``lons``."""
+        from scipy.spatial import KDTree
+
         lats = np.asarray(lats).flatten()
         lons = np.asarray(lons).flatten()
 
         # kdtree cannot contain nans
         if np.isnan(lats.max()) or np.isnan(lons.max()):
             mask = ~np.isnan(lats) & ~np.isnan(lons)
             lats = lats[mask]
             lons = lons[mask]
 
-        x, y, z = ll_to_xyz(lats, lons)
+        x, y, z = _latlon_to_xyz(lats, lons)
         v = np.column_stack((x, y, z))
         self.tree = KDTree(v)
 
         # TODO: allow user to specify max distance
-        self.max_distance_arc = 10000 * 1000  # m
-        if self.max_distance_arc <= np.pi * constants.R_earth:
-            self.max_distance_cord = arclength_to_cordlenght(self.max_distance_arc)
+        self.max_distance_arc = np.pi / 4
+        if self.max_distance_arc <= np.pi:
+            self.max_distance_chord = _arclength_to_chordlength(self.max_distance_arc)
         else:
-            self.max_distance_cord = np.inf
+            self.max_distance_chord = np.inf
+
+    def nearest_point(self, ref_points, figure=IFS_SPHERE):
+        """Find the index of the nearest point to all ``ref_points``.
 
-    def nearest_point(self, points):
-        lat, lon = points
-        x, y, z = ll_to_xyz(lat, lon)
+        Parameters
+        ----------
+        ref_points: pair of array-like
+            Latitude and longitude coordinates of the reference point (degrees)
+        figure: :class:`geo.figure.Figure`, optional
+            Figure of the spheroid the returned
+            distances are computed on (default: :obj:`geo.figure.IFS_SPHERE`)
+
+        Returns
+        -------
+        ndarray
+            Indices of the nearest points to ``ref_points``.
+        ndarray
+            The distance (m) between the ``ref_points`` and the corresponding nearest
+            point in ``points``. Computed on the surface of the spheroid defined
+            by ``figure``.
+
+        """
+        lat, lon = ref_points
+        x, y, z = _latlon_to_xyz(lat, lon)
         points = np.column_stack((x, y, z))
 
         # find the nearest point
         distance, index = self.tree.query(
             points, distance_upper_bound=self.max_distance_arc
         )
 
-        return index, cordlength_to_arclength(distance)
+        return index, figure.scale(_chordlength_to_arclength(distance))
 
 
-def nearest_point_kdtree(ref_points, points):
+def nearest_point_kdtree(ref_points, points, figure=IFS_SPHERE):
     """Find the index of the nearest point to all ``ref_points`` in a set of ``points`` using a KDTree.
 
     Parameters
     ----------
     ref_points: pair of array-like
         Latitude and longitude coordinates of the reference point (degrees)
     points: pair of array-like
         Locations of the set of points from which the nearest to
         ``ref_points`` is to be found. The first item specifies the latitudes,
         the second the longitudes (degrees)
+    figure: :class:`geo.figure.Figure`, optional
+        Figure of the spheroid the returned
+        distances are computed on (default: :obj:`geo.figure.IFS_SPHERE`)
 
     Returns
     -------
     ndarray
-        Indices of the nearest points to ``ref_points`.
+        Indices of the nearest points to ``ref_points``.
     ndarray
         The distance (m) between the ``ref_points`` and the corresponding nearest
-        point in ``points``.
+        point in ``points``. Computed on the surface of the spheroid defined
+        by ``figure``.
 
     Examples
     --------
     >>> from earthkit.geo import nearest_point_kdtree
     >>> p_ref = (51.45, -0.97)
     >>> p_lat = [44.49, 50.73, 50.1]
     >>> p_lon = [11.34, 7.90, -8.1]
@@ -246,9 +282,9 @@
     >>> p_lon = [11.34, 7.90, -8.1]
     >>> nearest_point_kdtree(p_ref, (p_lat, p_lon))
     (array([2, 0, 2]), array([ 523115.83147777,  659558.55282001, 4283987.17429322]))
 
     """
     lats, lons = points
     tree = GeoKDTree(lats, lons)
-    index, distance = tree.nearest_point(ref_points)
+    index, distance = tree.nearest_point(ref_points, figure=figure)
     return index, distance
```

### Comparing `earthkit-geo-0.0.1/earthkit_geo.egg-info/PKG-INFO` & `earthkit_geo-0.1.0/earthkit_geo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-geo
-Version: 0.0.1
+Version: 0.1.0
 Summary: A format-agnostic Python interface for geospatial data
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `earthkit-geo-0.0.1/earthkit_geo.egg-info/SOURCES.txt` & `earthkit_geo-0.1.0/earthkit_geo.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 docs/references.rst
 docs/requirements.txt
 docs/_static/.gitkeep
 docs/_static/style.css
 earthkit/geo/__init__.py
 earthkit/geo/constants.py
 earthkit/geo/distance.py
+earthkit/geo/figure.py
 earthkit/geo/version.py
 earthkit_geo.egg-info/PKG-INFO
 earthkit_geo.egg-info/SOURCES.txt
 earthkit_geo.egg-info/dependency_links.txt
 earthkit_geo.egg-info/requires.txt
 earthkit_geo.egg-info/top_level.txt
 tests/downstream-ci-requirements.txt
```

### Comparing `earthkit-geo-0.0.1/setup.cfg` & `earthkit_geo-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `earthkit-geo-0.0.1/tests/distance/test_distance.py` & `earthkit_geo-0.1.0/tests/distance/test_distance.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # nor does it submit to any jurisdiction.
 #
 
 import numpy as np
 import pytest
 
 from earthkit.geo import (
+    UNIT_SPHERE,
     haversine_distance,
     nearest_point_haversine,
     nearest_point_kdtree,
 )
 
 
 def get_nearest_method(mode):
@@ -99,14 +100,23 @@
 
     d = haversine_distance(p_ref, (lats, lons))
     assert np.allclose(
         d[:-1], d_ref[:-1]
     ), f"p_ref={p_ref},dlon_ref={dlon_ref},dlon_p={dlon_p}"
 
 
+def test_haversine_distance_with_radius():
+    p = (0, 90)
+    p_ref = (48.0, 20)
+    d_ref = 1.33989384590445
+
+    d = haversine_distance(p_ref, p, figure=UNIT_SPHERE)
+    assert np.allclose(d, d_ref)
+
+
 # lat is out of range
 @pytest.mark.parametrize("p_ref", [((90.00001, 0)), (((-90.00001, 0)))])
 def test_haversine_distance_invalid(p_ref):
     p = (-48, 12)
     d = haversine_distance(p_ref, p)
     assert np.isnan(d)
 
@@ -131,14 +141,33 @@
     meth = get_nearest_method(mode)
     index, distance = meth(p_ref, (lats, lons))
     assert np.allclose(index_ref, index)
     assert np.allclose(distance, dist_ref)
 
 
 @pytest.mark.parametrize("mode", ["haversine", "kdtree"])
+@pytest.mark.parametrize(
+    "p_ref,index_ref,dist_ref",
+    [
+        ((0, 0), 0, 0),
+        ((15, 22), 0, 0.46103882),
+        ((-50, -18), 8, 0.04174471),
+    ],
+)
+def test_nearest_single_ref_with_radius(mode, p_ref, index_ref, dist_ref):
+    lats = np.array([0.0, 0, 0, 0, 90, -90, 48, 48, -48, -48, np.nan])
+    lons = np.array([0, 90, -90, 180, 0, 0, 20, -20, -20, 20, 1.0])
+
+    meth = get_nearest_method(mode)
+    index, distance = meth(p_ref, (lats, lons), figure=UNIT_SPHERE)
+    assert np.allclose(index_ref, index)
+    assert np.allclose(distance, dist_ref)
+
+
+@pytest.mark.parametrize("mode", ["haversine", "kdtree"])
 def test_nearest_multi_ref_single_point(mode):
     p_ref = [(15, 44, 44), (22, 10, -10)]
 
     index_ref = np.array([0, 0, 0])
     dist_ref = np.array([3669564.47380201, 1026629.42232992, 2492883.80828643])
 
     lats = 48
@@ -163,15 +192,15 @@
     meth = get_nearest_method(mode)
     index, distance = meth(p_ref, (lats, lons))
     assert np.allclose(index, index_ref)
     assert np.allclose(distance, dist_ref)
 
 
 @pytest.mark.parametrize("mode", ["haversine", "kdtree"])
-def test_haversine_nearest_invalid(mode):
+def test_nearest_invalid(mode):
     # checks: p_ref must have a (2,) shape
     p_ref = ([15, 21], [22, 7], [44, 12])
     p = ([0.0, 0], [0, 90])
 
     with pytest.raises(ValueError):
         meth = get_nearest_method(mode)
         meth(p_ref, p)
```

