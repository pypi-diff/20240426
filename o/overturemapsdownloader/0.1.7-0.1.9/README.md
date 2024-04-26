# Comparing `tmp/overturemapsdownloader-0.1.7.tar.gz` & `tmp/overturemapsdownloader-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overturemapsdownloader-0.1.7.tar", max compression
+gzip compressed data, was "overturemapsdownloader-0.1.9.tar", max compression
```

## Comparing `overturemapsdownloader-0.1.7.tar` & `overturemapsdownloader-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      585 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/LICENSE
--rw-r--r--   0        0        0    11468 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/README.md
--rw-r--r--   0        0        0     1032 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/config.yml
--rw-r--r--   0        0        0      314 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/overturemapsdownloader/__init__.py
--rw-r--r--   0        0        0     4123 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/overturemapsdownloader/config.py
--rw-r--r--   0        0        0     2436 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/overturemapsdownloader/dask_qrys.py
--rw-r--r--   0        0        0     2050 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/overturemapsdownloader/main.py
--rw-r--r--   0        0        0     1580 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/overturemapsdownloader/om_logic.py
--rw-r--r--   0        0        0      879 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/overturemapsdownloader/read_om_schemas.py
--rw-r--r--   0        0        0     6444 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/overturemapsdownloader/utils_helper.py
--rw-r--r--   0        0        0      746 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/overturemapsdownloader/yaml_helper.py
--rw-r--r--   0        0        0      888 2024-02-23 16:43:44.000000 overturemapsdownloader-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    12503 1970-01-01 00:00:00.000000 overturemapsdownloader-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      585 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/LICENSE
+-rw-r--r--   0        0        0    11468 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/README.md
+-rw-r--r--   0        0        0     1031 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/config.yml
+-rw-r--r--   0        0        0      314 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/overturemapsdownloader/__init__.py
+-rw-r--r--   0        0        0     4123 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/overturemapsdownloader/config.py
+-rw-r--r--   0        0        0     3112 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/overturemapsdownloader/dask_qrys.py
+-rw-r--r--   0        0        0     2050 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/overturemapsdownloader/main.py
+-rw-r--r--   0        0        0     1580 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/overturemapsdownloader/om_logic.py
+-rw-r--r--   0        0        0      879 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/overturemapsdownloader/read_om_schemas.py
+-rw-r--r--   0        0        0     6444 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/overturemapsdownloader/utils_helper.py
+-rw-r--r--   0        0        0      746 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/overturemapsdownloader/yaml_helper.py
+-rw-r--r--   0        0        0      890 2024-04-26 09:39:31.000000 overturemapsdownloader-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    12546 1970-01-01 00:00:00.000000 overturemapsdownloader-0.1.9/PKG-INFO
```

### Comparing `overturemapsdownloader-0.1.7/LICENSE` & `overturemapsdownloader-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `overturemapsdownloader-0.1.7/README.md` & `overturemapsdownloader-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `overturemapsdownloader-0.1.7/config.yml` & `overturemapsdownloader-0.1.9/config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 global_variables:
-  release: "2024-02-15-alpha.0"
+  release: "2024-04-16-beta.0"
   s3_region: "us-west-2"
   default_theme: "places"
   default_type: "*"
   filter_by_bbox: true
   filter_by_country: false
   bbox_file_path: "examples/bbox.geojson"
   country_iso_code: "EG"
```

### Comparing `overturemapsdownloader-0.1.7/overturemapsdownloader/config.py` & `overturemapsdownloader-0.1.9/overturemapsdownloader/config.py`

 * *Files identical despite different names*

### Comparing `overturemapsdownloader-0.1.7/overturemapsdownloader/main.py` & `overturemapsdownloader-0.1.9/overturemapsdownloader/main.py`

 * *Files identical despite different names*

### Comparing `overturemapsdownloader-0.1.7/overturemapsdownloader/om_logic.py` & `overturemapsdownloader-0.1.9/overturemapsdownloader/om_logic.py`

 * *Files identical despite different names*

### Comparing `overturemapsdownloader-0.1.7/overturemapsdownloader/read_om_schemas.py` & `overturemapsdownloader-0.1.9/overturemapsdownloader/read_om_schemas.py`

 * *Files identical despite different names*

### Comparing `overturemapsdownloader-0.1.7/overturemapsdownloader/utils_helper.py` & `overturemapsdownloader-0.1.9/overturemapsdownloader/utils_helper.py`

 * *Files identical despite different names*

### Comparing `overturemapsdownloader-0.1.7/overturemapsdownloader/yaml_helper.py` & `overturemapsdownloader-0.1.9/overturemapsdownloader/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `overturemapsdownloader-0.1.7/pyproject.toml` & `overturemapsdownloader-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "overturemapsdownloader"
-version = "0.1.7"
+version = "0.1.9"
 description = "Overture Maps Downloader simplifies geospatial data manipulation"
 authors = ["Youssef-Harby <me@youssefharby.com>"]
 readme = "README.md"
 include = ["config.yml"]
 
 [tool.poetry.scripts]
 OMDownloader = "overturemapsdownloader.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-typer = {extras = ["all"], version = "^0.9.0"}
+typer = {extras = ["all"], version = "^0.12.3"}
 jupyter = "^1.0.0"
 dask-geopandas = "^0.3.1"
-pyarrow = "^15.0.0"
-adlfs = "^2024.2.0"
-duckdb = "^0.10.0"
+pyarrow = "^15.0.2"
+adlfs = "^2024.4.0"
+duckdb = "^0.10.1"
 geopandas = "^0.14.3"
-shapely = "^2.0.3"
-gdal = {version = "^3.8.4", optional = true}
-fiona = "^1.9.5"
+shapely = "^2.0.4"
+gdal = "3.8.5"
+fiona = "^1.9.6"
 fastparquet = "^2024.2.0"
-s3fs = "^2024.2.0"
-dask = {extras = ["complete"], version = "^2024.2.0"}
+s3fs = "^2024.3.1"
+dask = {extras = ["complete", "dataframe"], version = "^2024.4.1"}
+pyproj = "^3.6.1"
 
 [tool.poetry.extras]
 gdal_support = ["gdal"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `overturemapsdownloader-0.1.7/PKG-INFO` & `overturemapsdownloader-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: overturemapsdownloader
-Version: 0.1.7
+Version: 0.1.9
 Summary: Overture Maps Downloader simplifies geospatial data manipulation
 Author: Youssef-Harby
 Author-email: me@youssefharby.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gdal-support
-Requires-Dist: adlfs (>=2024.2.0,<2025.0.0)
+Requires-Dist: adlfs (>=2024.4.0,<2025.0.0)
 Requires-Dist: dask-geopandas (>=0.3.1,<0.4.0)
-Requires-Dist: dask[complete] (>=2024.2.0,<2025.0.0)
-Requires-Dist: duckdb (>=0.10.0,<0.11.0)
+Requires-Dist: dask[complete,dataframe] (>=2024.4.1,<2025.0.0)
+Requires-Dist: duckdb (>=0.10.1,<0.11.0)
 Requires-Dist: fastparquet (>=2024.2.0,<2025.0.0)
-Requires-Dist: fiona (>=1.9.5,<2.0.0)
-Requires-Dist: gdal (>=3.8.4,<4.0.0) ; extra == "gdal-support"
+Requires-Dist: fiona (>=1.9.6,<2.0.0)
+Requires-Dist: gdal (==3.8.5) ; extra == "gdal-support"
 Requires-Dist: geopandas (>=0.14.3,<0.15.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
-Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
-Requires-Dist: s3fs (>=2024.2.0,<2025.0.0)
-Requires-Dist: shapely (>=2.0.3,<3.0.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
+Requires-Dist: pyproj (>=3.6.1,<4.0.0)
+Requires-Dist: s3fs (>=2024.3.1,<2025.0.0)
+Requires-Dist: shapely (>=2.0.4,<3.0.0)
+Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
 # Overture Maps Downloader
 
 This repository is still under heavy development. Features may change, and documentation will be updated accordingly. Use at your own risk and feel free to contribute!
 
 [![Docker build and push](https://github.com/Youssef-Harby/OvertureMapsDownloader/actions/workflows/docker-build-push.yml/badge.svg)](https://github.com/Youssef-Harby/OvertureMapsDownloader/actions/workflows/docker-build-push.yml)
```

