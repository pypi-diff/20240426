# Comparing `tmp/earthkit-0.4.4.tar.gz` & `tmp/earthkit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit-0.4.4.tar", last modified: Thu Apr 18 12:01:03 2024, max compression
+gzip compressed data, was "earthkit-0.5.0.tar", last modified: Fri Apr 26 13:48:54 2024, max compression
```

## Comparing `earthkit-0.4.4.tar` & `earthkit-0.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:01:03.413932 earthkit-0.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:01:03.405932 earthkit-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:01:03.409932 earthkit-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-18 12:00:56.000000 earthkit-0.4.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-18 12:00:56.000000 earthkit-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-18 12:00:56.000000 earthkit-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-18 12:00:56.000000 earthkit-0.4.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-04-18 12:00:56.000000 earthkit-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 12:00:56.000000 earthkit-0.4.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-18 12:01:03.413932 earthkit-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-18 12:00:56.000000 earthkit-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:01:03.409932 earthkit-0.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:01:03.409932 earthkit-0.4.4/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/_ext/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:01:03.409932 earthkit-0.4.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    60639 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/_static/earthkit.png
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/components_overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:01:03.409932 earthkit-0.4.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    73703 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/examples/01_grib_file.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    52548 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/examples/02_grib_fdb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/licence.rst
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-18 12:00:56.000000 earthkit-0.4.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:01:03.409932 earthkit-0.4.4/earthkit/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-18 12:00:56.000000 earthkit-0.4.4/earthkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 12:01:03.000000 earthkit-0.4.4/earthkit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:01:03.413932 earthkit-0.4.4/earthkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-18 12:01:03.000000 earthkit-0.4.4/earthkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-18 12:01:03.000000 earthkit-0.4.4/earthkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:01:03.000000 earthkit-0.4.4/earthkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-18 12:01:03.000000 earthkit-0.4.4/earthkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 12:01:03.000000 earthkit-0.4.4/earthkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-18 12:00:56.000000 earthkit-0.4.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-18 12:00:56.000000 earthkit-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 12:00:56.000000 earthkit-0.4.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-18 12:01:03.413932 earthkit-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:01:03.413932 earthkit-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-18 12:00:56.000000 earthkit-0.4.4/tests/environment-docs-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-18 12:00:56.000000 earthkit-0.4.4/tests/environment-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-18 12:00:56.000000 earthkit-0.4.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.394324 earthkit-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.386324 earthkit-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-26 13:48:44.000000 earthkit-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-26 13:48:44.000000 earthkit-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-26 13:48:44.000000 earthkit-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 13:48:44.000000 earthkit-0.5.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-04-26 13:48:44.000000 earthkit-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-26 13:48:44.000000 earthkit-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-26 13:48:54.394324 earthkit-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-26 13:48:44.000000 earthkit-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/_ext/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    60639 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/_static/earthkit.png
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/components_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    73703 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/examples/01_grib_file.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    52548 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/examples/02_grib_fdb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/earthkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-26 13:48:44.000000 earthkit-0.5.0/earthkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.394324 earthkit-0.5.0/earthkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 13:48:44.000000 earthkit-0.5.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-26 13:48:44.000000 earthkit-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 13:48:44.000000 earthkit-0.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-26 13:48:54.394324 earthkit-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 13:48:44.000000 earthkit-0.5.0/tests/environment-docs-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-26 13:48:44.000000 earthkit-0.5.0/tests/environment-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-26 13:48:44.000000 earthkit-0.5.0/tests/test_version.py
```

### Comparing `earthkit-0.4.4/.github/workflows/ci.yml` & `earthkit-0.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/.gitignore` & `earthkit-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/.pre-commit-config.yaml` & `earthkit-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/LICENSE` & `earthkit-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/PKG-INFO` & `earthkit-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit
-Version: 0.4.4
+Version: 0.5.0
 Home-page: https://github.com/ecmwf/earthkit
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,16 +16,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: earthkit-data[all]>=0.7.0
+Requires-Dist: earthkit-geo>=0.1.0
 Requires-Dist: earthkit-maps>=0.0.18
-Requires-Dist: earthkit-meteo>=0.0.1
+Requires-Dist: earthkit-meteo>=0.1.0
 Requires-Dist: earthkit-plots>=0.0.6
 Requires-Dist: earthkit-regrid>=0.3.0
 
 # earthkit
 
 <img src="docs/_static/earthkit.png" width="120">
```

### Comparing `earthkit-0.4.4/README.md` & `earthkit-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/docs/Makefile` & `earthkit-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/docs/_ext/xref.py` & `earthkit-0.5.0/docs/_ext/xref.py`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/docs/_static/earthkit.png` & `earthkit-0.5.0/docs/_static/earthkit.png`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/docs/_static/style.css` & `earthkit-0.5.0/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/docs/components_overview.rst` & `earthkit-0.5.0/docs/components_overview.rst`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     * - Component
       - Description
       - Logo
     * - :xref:`earthkit-data`
       - Format-agnostic Python interface for geospatial data with a focus on meteorology and climate science.
       - .. image:: https://raw.githubusercontent.com/ecmwf/earthkit-data/main/docs/_static/earthkit-data.png
           :width: 120px
+    * - :xref:`earthkit-geo`
+      - Geospatial computations
+      -
     * - :xref:`earthkit-maps`
       - Geospatial visualisation tools and templates.
       - .. image:: https://raw.githubusercontent.com/ecmwf/earthkit-maps/develop/docs/_static/earthkit-maps.png
           :width: 120px
     * - :xref:`earthkit-meteo`
       - Meteorological computations.
       -
```

### Comparing `earthkit-0.4.4/docs/conf.py` & `earthkit-0.5.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,18 @@
 html_logo = "_static/earthkit.png"
 
 xref_links = {
     "earthkit-data": (
         "earthkit-data",
         "https://earthkit-data.readthedocs.io",
     ),
+    "earthkit-geo": (
+        "earthkit-geo",
+        "https://earthkit-geo.readthedocs.io",
+    ),
     "earthkit-maps": (
         "earthkit-maps",
         "https://earthkit-maps.readthedocs.io",
     ),
     "earthkit-meteo": (
         "earthkit-meteo",
         "https://earthkit-meteo.readthedocs.io",
```

### Comparing `earthkit-0.4.4/docs/examples/01_grib_file.ipynb` & `earthkit-0.5.0/docs/examples/01_grib_file.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/docs/examples/02_grib_fdb.ipynb` & `earthkit-0.5.0/docs/examples/02_grib_fdb.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/docs/index.rst` & `earthkit-0.5.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 .. toctree::
     :maxdepth: 1
     :caption: Components
     :titlesonly:
 
     components_overview
     earthkit-data <https://earthkit-data.readthedocs.io>
+    earthkit-geo <https://earthkit-geo.readthedocs.io>
     earthkit-maps <https://earthkit-maps.readthedocs.io>
     earthkit-meteo <https://earthkit-meteo.readthedocs.io>
     earthkit-plots <https://pypi.org/project/earthkit-plots>
     earthkit-regrid <https://earthkit-regrid.readthedocs.io>
 
 .. toctree::
    :maxdepth: 1
```

### Comparing `earthkit-0.4.4/docs/install.rst` & `earthkit-0.5.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/docs/licence.rst` & `earthkit-0.5.0/docs/licence.rst`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/earthkit/__init__.py` & `earthkit-0.5.0/earthkit/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/earthkit.egg-info/PKG-INFO` & `earthkit-0.5.0/earthkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit
-Version: 0.4.4
+Version: 0.5.0
 Home-page: https://github.com/ecmwf/earthkit
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,16 +16,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: earthkit-data[all]>=0.7.0
+Requires-Dist: earthkit-geo>=0.1.0
 Requires-Dist: earthkit-maps>=0.0.18
-Requires-Dist: earthkit-meteo>=0.0.1
+Requires-Dist: earthkit-meteo>=0.1.0
 Requires-Dist: earthkit-plots>=0.0.6
 Requires-Dist: earthkit-regrid>=0.3.0
 
 # earthkit
 
 <img src="docs/_static/earthkit.png" width="120">
```

### Comparing `earthkit-0.4.4/earthkit.egg-info/SOURCES.txt` & `earthkit-0.5.0/earthkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthkit-0.4.4/setup.cfg` & `earthkit-0.5.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 test_suite = tests
 
 [options]
 python-requires = >=3.8
 packages = find_namespace:
 install_requires = 
 	earthkit-data[all]>=0.7.0
+	earthkit-geo>=0.1.0
 	earthkit-maps>=0.0.18
-	earthkit-meteo>=0.0.1
+	earthkit-meteo>=0.1.0
 	earthkit-plots>=0.0.6
 	earthkit-regrid>=0.3.0
 
 [options.packages.find]
 include = earthkit, earthkit.*
 
 [flake8]
```

### Comparing `earthkit-0.4.4/tests/test_version.py` & `earthkit-0.5.0/tests/test_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,14 +29,26 @@
 
 def test_earthkit_data_version_2():
     from earthkit import data
 
     assert VERSION_RX.match(data.__version__) is not None
 
 
+def test_earthkit_geo_version_1():
+    import earthkit.geo  # noqa
+
+    assert VERSION_RX.match(earthkit.geo.__version__) is not None
+
+
+def test_earthkit_geo_version_2():
+    from earthkit import geo  # noqa
+
+    assert VERSION_RX.match(geo.__version__) is not None
+
+
 def test_earthkit_maps_version_1():
     import earthkit.maps  # noqa
 
     assert VERSION_RX.match(earthkit.maps.__version__) is not None
 
 
 def test_earthkit_maps_version_2():
```

