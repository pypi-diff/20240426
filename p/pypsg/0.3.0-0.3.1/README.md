# Comparing `tmp/pypsg-0.3.0.tar.gz` & `tmp/pypsg-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypsg-0.3.0.tar", last modified: Wed Mar 27 18:04:52 2024, max compression
+gzip compressed data, was "pypsg-0.3.1.tar", last modified: Fri Apr 26 03:37:42 2024, max compression
```

## Comparing `pypsg-0.3.0.tar` & `pypsg-0.3.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.441531 pypsg-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-27 18:04:45.000000 pypsg-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-03-27 18:04:52.441531 pypsg-0.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.433531 pypsg-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-27 18:04:45.000000 pypsg-0.3.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-27 18:04:45.000000 pypsg-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.433531 pypsg-0.3.0/pypsg/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.433531 pypsg-0.3.0/pypsg/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64219 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/cfg/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/cfg/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/cfg/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.437531 pypsg-0.3.0/pypsg/globes/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/globes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/globes/decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.437531 pypsg-0.3.0/pypsg/globes/exocam/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/globes/exocam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12489 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/globes/exocam/exocam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.437531 pypsg-0.3.0/pypsg/globes/exoplasim/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/globes/exoplasim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12301 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/globes/exoplasim/exoplasim.py
--rw-r--r--   0 runner    (1001) docker     (127)    18786 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/globes/globes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/globes/molec.json
--rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/globes/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.437531 pypsg-0.3.0/pypsg/globes/waccm/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/globes/waccm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/globes/waccm/waccm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.437531 pypsg-0.3.0/pypsg/lyr/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/lyr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/lyr/lyr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.437531 pypsg-0.3.0/pypsg/rad/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/rad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/rad/rad.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-27 18:04:45.000000 pypsg-0.3.0/pypsg/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.437531 pypsg-0.3.0/pypsg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-03-27 18:04:52.000000 pypsg-0.3.0/pypsg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-27 18:04:52.000000 pypsg-0.3.0/pypsg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 18:04:52.000000 pypsg-0.3.0/pypsg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-27 18:04:52.000000 pypsg-0.3.0/pypsg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 18:04:52.000000 pypsg-0.3.0/pypsg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 18:04:52.441531 pypsg-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:04:52.437531 pypsg-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-03-27 18:04:45.000000 pypsg-0.3.0/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-27 18:04:45.000000 pypsg-0.3.0/test/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-27 18:04:45.000000 pypsg-0.3.0/test/test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-27 18:04:45.000000 pypsg-0.3.0/test/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.014276 pypsg-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 03:37:37.000000 pypsg-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-26 03:37:42.014276 pypsg-0.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.006276 pypsg-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-26 03:37:37.000000 pypsg-0.3.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-26 03:37:37.000000 pypsg-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.006276 pypsg-0.3.1/pypsg/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.010276 pypsg-0.3.1/pypsg/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64219 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/cfg/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/cfg/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/cfg/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.010276 pypsg-0.3.1/pypsg/globes/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/globes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/globes/decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.010276 pypsg-0.3.1/pypsg/globes/exocam/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/globes/exocam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12489 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/globes/exocam/exocam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.010276 pypsg-0.3.1/pypsg/globes/exoplasim/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/globes/exoplasim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12301 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/globes/exoplasim/exoplasim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18786 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/globes/globes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/globes/molec.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/globes/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.010276 pypsg-0.3.1/pypsg/globes/waccm/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/globes/waccm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/globes/waccm/waccm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.010276 pypsg-0.3.1/pypsg/lyr/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/lyr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/lyr/lyr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.010276 pypsg-0.3.1/pypsg/rad/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/rad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/rad/rad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-26 03:37:37.000000 pypsg-0.3.1/pypsg/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.014276 pypsg-0.3.1/pypsg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-26 03:37:41.000000 pypsg-0.3.1/pypsg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-26 03:37:42.000000 pypsg-0.3.1/pypsg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 03:37:41.000000 pypsg-0.3.1/pypsg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-26 03:37:41.000000 pypsg-0.3.1/pypsg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 03:37:41.000000 pypsg-0.3.1/pypsg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 03:37:42.014276 pypsg-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:37:42.010276 pypsg-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-04-26 03:37:37.000000 pypsg-0.3.1/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-26 03:37:37.000000 pypsg-0.3.1/test/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-26 03:37:37.000000 pypsg-0.3.1/test/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-26 03:37:37.000000 pypsg-0.3.1/test/test_units.py
```

### Comparing `pypsg-0.3.0/LICENSE` & `pypsg-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/PKG-INFO` & `pypsg-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypsg
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python package for accessing the Planetary System Generator.
 Author-email: Ted Johnson <ted.johnson@unlv.edu>
 Maintainer-email: Ted Johnson <ted.johnson@unlv.edu>
 License: MIT License
         
         Copyright (c) 2023 Ted Johnson
         
@@ -40,15 +40,14 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: astropy
 Requires-Dist: numpy
 Requires-Dist: requests
-Requires-Dist: docker
 Requires-Dist: python-dateutil
 Requires-Dist: netCDF4
 Provides-Extra: plot
 Requires-Dist: matplotlib; extra == "plot"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pep8; extra == "dev"
```

### Comparing `pypsg-0.3.0/docs/readme.rst` & `pypsg-0.3.1/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pyproject.toml` & `pypsg-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 # Minimum requirements for the build system to execute.
 requires = ["setuptools", "wheel"]  # PEP 508 specifications.
 
 [project]
-version = "0.3.0"
+version = "0.3.1"
 name = "pypsg"
 authors = [
     {name = "Ted Johnson", email = "ted.johnson@unlv.edu"},
 ]
 maintainers = [ { name = "Ted Johnson", email = "ted.johnson@unlv.edu" } ]
 description = "A Python package for accessing the Planetary System Generator."
 readme = "docs/readme.rst"
@@ -25,15 +25,14 @@
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "astropy",
     "numpy",
     "requests",
-    "docker",
     "python-dateutil",
     "netCDF4",
 ]
 [project.optional-dependencies]
 plot = [
     "matplotlib",
 ]
```

### Comparing `pypsg-0.3.0/pypsg/cfg/__init__.py` & `pypsg-0.3.1/pypsg/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/cfg/base.py` & `pypsg-0.3.1/pypsg/cfg/base.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/cfg/config.py` & `pypsg-0.3.1/pypsg/cfg/config.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/cfg/models.py` & `pypsg-0.3.1/pypsg/cfg/models.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/exceptions.py` & `pypsg-0.3.1/pypsg/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/globes/decoder.py` & `pypsg-0.3.1/pypsg/globes/decoder.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/globes/exocam/exocam.py` & `pypsg-0.3.1/pypsg/globes/exocam/exocam.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/globes/exoplasim/exoplasim.py` & `pypsg-0.3.1/pypsg/globes/exoplasim/exoplasim.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/globes/globes.py` & `pypsg-0.3.1/pypsg/globes/globes.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/globes/molec.json` & `pypsg-0.3.1/pypsg/globes/molec.json`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/globes/structure.py` & `pypsg-0.3.1/pypsg/globes/structure.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/globes/waccm/waccm.py` & `pypsg-0.3.1/pypsg/globes/waccm/waccm.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/lyr/lyr.py` & `pypsg-0.3.1/pypsg/lyr/lyr.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/rad/rad.py` & `pypsg-0.3.1/pypsg/rad/rad.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/request.py` & `pypsg-0.3.1/pypsg/request.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/settings.py` & `pypsg-0.3.1/pypsg/settings.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg/units.py` & `pypsg-0.3.1/pypsg/units.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/pypsg.egg-info/PKG-INFO` & `pypsg-0.3.1/pypsg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypsg
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python package for accessing the Planetary System Generator.
 Author-email: Ted Johnson <ted.johnson@unlv.edu>
 Maintainer-email: Ted Johnson <ted.johnson@unlv.edu>
 License: MIT License
         
         Copyright (c) 2023 Ted Johnson
         
@@ -40,15 +40,14 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: astropy
 Requires-Dist: numpy
 Requires-Dist: requests
-Requires-Dist: docker
 Requires-Dist: python-dateutil
 Requires-Dist: netCDF4
 Provides-Extra: plot
 Requires-Dist: matplotlib; extra == "plot"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pep8; extra == "dev"
```

### Comparing `pypsg-0.3.0/pypsg.egg-info/SOURCES.txt` & `pypsg-0.3.1/pypsg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/test/test_api.py` & `pypsg-0.3.1/test/test_api.py`

 * *Files identical despite different names*

### Comparing `pypsg-0.3.0/test/test_docker.py` & `pypsg-0.3.1/test/test_docker.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,8 +39,8 @@
     if not started_out_running:
         psgdocker.stop_psg()
     assert started_out_running == psgdocker.is_psg_running()
     # give the container time to setup. This is important for other tests
     time.sleep(1)
 
 if __name__ in '__main__':
-    pytest.main(args=[__file__])
+    pytest.main(args=[__file__, '--local'])
```

### Comparing `pypsg-0.3.0/test/test_request.py` & `pypsg-0.3.1/test/test_request.py`

 * *Files identical despite different names*

