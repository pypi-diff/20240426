# Comparing `tmp/descarteslabs_dynamic_compute-1.1.2.tar.gz` & `tmp/descarteslabs_dynamic_compute-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descarteslabs_dynamic_compute-1.1.2.tar", max compression
+gzip compressed data, was "descarteslabs_dynamic_compute-1.1.4.tar", max compression
```

## Comparing `descarteslabs_dynamic_compute-1.1.2.tar` & `descarteslabs_dynamic_compute-1.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      561 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/LICENSE
--rw-r--r--   0        0        0     1786 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/README.md
--rw-r--r--   0        0        0      945 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/__init__.py
--rw-r--r--   0        0        0      308 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/catalog/__init__.py
--rw-r--r--   0        0        0     9728 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/catalog/blob.py
--rw-r--r--   0        0        0    21555 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/compute_map.py
--rw-r--r--   0        0        0     1467 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/datetime_utils.py
--rw-r--r--   0        0        0      648 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dl_utils.py
--rw-r--r--   0        0        0     3890 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dot.py
--rw-r--r--   0        0        0     1007 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dynamic_compute.py
--rw-r--r--   0        0        0        0 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/__init__.py
--rw-r--r--   0        0        0      541 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/client/__init__.py
--rw-r--r--   0        0        0    27769 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/client/client.py
--rw-r--r--   0        0        0      160 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/__init__.py
--rw-r--r--   0        0        0      223 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/exceptions.py
--rw-r--r--   0        0        0     5705 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py
--rw-r--r--   0        0        0      848 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py
--rw-r--r--   0        0        0     5217 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/spec.md
--rw-r--r--   0        0        0      465 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/syntax/__init__.py
--rw-r--r--   0        0        0     3620 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/syntax/syntax.py
--rw-r--r--   0        0        0    11234 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/groupby.py
--rw-r--r--   0        0        0    19407 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/image_stack.py
--rw-r--r--   0        0        0       41 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/__init__.py
--rw-r--r--   0        0        0     1573 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/clearable.py
--rw-r--r--   0        0        0     1179 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/colormaps.py
--rw-r--r--   0        0        0    13247 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/inspector.py
--rw-r--r--   0        0        0    22779 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer.py
--rw-r--r--   0        0        0     3752 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer_controller.py
--rw-r--r--   0        0        0    17054 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer_controller_row.py
--rw-r--r--   0        0        0     1333 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/lonlat.py
--rw-r--r--   0        0        0    18499 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/map_.py
--rw-r--r--   0        0        0    23843 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/parameters.py
--rw-r--r--   0        0        0     3572 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/tile_url.py
--rw-r--r--   0        0        0     1543 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/utils.py
--rw-r--r--   0        0        0    17999 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/mosaic.py
--rw-r--r--   0        0        0    39359 2024-04-13 00:40:32.901564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/operations.py
--rw-r--r--   0        0        0     3133 2024-04-13 00:40:32.901564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/pyversions.py
--rw-r--r--   0        0        0     1453 2024-04-13 00:40:32.901564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/reductions.py
--rw-r--r--   0        0        0      801 2024-04-13 00:40:32.901564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/serialization.py
--rw-r--r--   0        0        0      625 2024-04-13 00:40:32.901564 descarteslabs_dynamic_compute-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2738 1970-01-01 00:00:00.000000 descarteslabs_dynamic_compute-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      561 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/LICENSE
+-rw-r--r--   0        0        0     1786 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/README.md
+-rw-r--r--   0        0        0      945 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/__init__.py
+-rw-r--r--   0        0        0      308 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/catalog/__init__.py
+-rw-r--r--   0        0        0     9728 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/catalog/blob.py
+-rw-r--r--   0        0        0    21555 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/compute_map.py
+-rw-r--r--   0        0        0     1467 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/datetime_utils.py
+-rw-r--r--   0        0        0      648 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/dl_utils.py
+-rw-r--r--   0        0        0     3890 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/dot.py
+-rw-r--r--   0        0        0     1007 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/dynamic_compute.py
+-rw-r--r--   0        0        0        0 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/__init__.py
+-rw-r--r--   0        0        0      541 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/client/__init__.py
+-rw-r--r--   0        0        0    27769 2024-04-25 23:22:01.528020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/client/client.py
+-rw-r--r--   0        0        0      160 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/interpreter/__init__.py
+-rw-r--r--   0        0        0      223 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/interpreter/exceptions.py
+-rw-r--r--   0        0        0     5705 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py
+-rw-r--r--   0        0        0      848 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py
+-rw-r--r--   0        0        0     5217 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/spec.md
+-rw-r--r--   0        0        0      465 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/syntax/__init__.py
+-rw-r--r--   0        0        0     3620 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/syntax/syntax.py
+-rw-r--r--   0        0        0    11234 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/groupby.py
+-rw-r--r--   0        0        0    19407 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/image_stack.py
+-rw-r--r--   0        0        0       41 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/__init__.py
+-rw-r--r--   0        0        0     1573 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/clearable.py
+-rw-r--r--   0        0        0     1179 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/colormaps.py
+-rw-r--r--   0        0        0    13247 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/inspector.py
+-rw-r--r--   0        0        0    22779 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/layer.py
+-rw-r--r--   0        0        0     3752 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/layer_controller.py
+-rw-r--r--   0        0        0    17054 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/layer_controller_row.py
+-rw-r--r--   0        0        0     1333 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/lonlat.py
+-rw-r--r--   0        0        0    18499 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/map_.py
+-rw-r--r--   0        0        0    23843 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/parameters.py
+-rw-r--r--   0        0        0     3572 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/tile_url.py
+-rw-r--r--   0        0        0     1543 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/utils.py
+-rw-r--r--   0        0        0    17999 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/mosaic.py
+-rw-r--r--   0        0        0    39359 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/operations.py
+-rw-r--r--   0        0        0     3133 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/pyversions.py
+-rw-r--r--   0        0        0     1453 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/reductions.py
+-rw-r--r--   0        0        0      801 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/serialization.py
+-rw-r--r--   0        0        0      623 2024-04-25 23:22:01.532020 descarteslabs_dynamic_compute-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 descarteslabs_dynamic_compute-1.1.4/PKG-INFO
```

### Comparing `descarteslabs_dynamic_compute-1.1.2/LICENSE` & `descarteslabs_dynamic_compute-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/README.md` & `descarteslabs_dynamic_compute-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/__init__.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/catalog/blob.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/catalog/blob.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/compute_map.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/compute_map.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/datetime_utils.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dl_utils.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/dl_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dot.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/dot.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dynamic_compute.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/dynamic_compute.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/client/__init__.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/client/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/client/client.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/client/client.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/spec.md` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/spec.md`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/syntax/syntax.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/graft/syntax/syntax.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/groupby.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/groupby.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/image_stack.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/image_stack.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/clearable.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/clearable.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/colormaps.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/colormaps.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/inspector.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/inspector.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/layer.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer_controller.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/layer_controller.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer_controller_row.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/layer_controller_row.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/lonlat.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/lonlat.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/map_.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/map_.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/parameters.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/parameters.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/tile_url.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/tile_url.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/utils.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/interactive/utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/mosaic.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/mosaic.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/operations.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/operations.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/pyversions.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/pyversions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/reductions.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/reductions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/serialization.py` & `descarteslabs_dynamic_compute-1.1.4/descarteslabs/dynamic_compute/serialization.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.2/pyproject.toml` & `descarteslabs_dynamic_compute-1.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "descarteslabs-dynamic-compute"
-version = "1.1.2"
+version = "1.1.4"
 description = ""
 license = "Apache-2.0"
 authors = ["Descartes Labs"]
 readme = "README.md"
 packages = [
     { include = "descarteslabs" },
 ]
@@ -15,15 +15,15 @@
 shapely = ">2,<3"
 utm = "^0.7.0"
 pyproj = "^3.4.1"
 geojson = ">=2.5.0"
 numpy = "<=1.24.2"
 descarteslabs = ">=2.0.3,<4"
 cloudpickle = [
-    {version = "1.6.0", python = ">=3.8,<3.11"},
-    {version = "3.0.0", python = ">=3.11"}
+    {version = "1.6.0", python = ">=3.8,<3.9"},
+    {version = "3.0.0", python = ">=3.9"}
 ]
 certifi = ">=2023.7.22"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `descarteslabs_dynamic_compute-1.1.2/PKG-INFO` & `descarteslabs_dynamic_compute-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: descarteslabs-dynamic-compute
-Version: 1.1.2
+Version: 1.1.4
 Summary: 
 License: Apache-2.0
 Author: Descartes Labs
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi (>=2023.7.22)
-Requires-Dist: cloudpickle (==1.6.0) ; python_version >= "3.8" and python_version < "3.11"
-Requires-Dist: cloudpickle (==3.0.0) ; python_version >= "3.11"
+Requires-Dist: cloudpickle (==1.6.0) ; python_version >= "3.8" and python_version < "3.9"
+Requires-Dist: cloudpickle (==3.0.0) ; python_version >= "3.9"
 Requires-Dist: descarteslabs (>=2.0.3,<4)
 Requires-Dist: geojson (>=2.5.0)
 Requires-Dist: ipyleaflet (>=0.15.0)
 Requires-Dist: numpy (<=1.24.2)
 Requires-Dist: pyproj (>=3.4.1,<4.0.0)
 Requires-Dist: shapely (>2,<3)
 Requires-Dist: utm (>=0.7.0,<0.8.0)
```

