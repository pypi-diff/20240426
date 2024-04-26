# Comparing `tmp/uom-0.6.3.tar.gz` & `tmp/uom-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uom-0.6.3.tar", last modified: Thu Sep 21 13:38:58 2023, max compression
+gzip compressed data, was "uom-0.6.7.tar", last modified: Fri Apr 26 20:01:47 2024, max compression
```

## Comparing `uom-0.6.3.tar` & `uom-0.6.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 13:38:58.421069 uom-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2023-09-21 13:38:45.000000 uom-0.6.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-09-21 13:38:45.000000 uom-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2023-09-21 13:38:58.421069 uom-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2023-09-21 13:38:45.000000 uom-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-21 13:38:45.000000 uom-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-21 13:38:58.421069 uom-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2023-09-21 13:38:45.000000 uom-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 13:38:58.421069 uom-0.6.3/uom/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-09-21 13:38:45.000000 uom-0.6.3/uom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-09-21 13:38:45.000000 uom-0.6.3/uom/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2023-09-21 13:38:45.000000 uom-0.6.3/uom/unit_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)   144435 2023-09-21 13:38:45.000000 uom-0.6.3/uom/uom.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2023-09-21 13:38:45.000000 uom-0.6.3/uom/uom.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-09-21 13:38:45.000000 uom-0.6.3/uom/uomdata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 13:38:58.421069 uom-0.6.3/uom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2023-09-21 13:38:58.000000 uom-0.6.3/uom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-09-21 13:38:58.000000 uom-0.6.3/uom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 13:38:58.000000 uom-0.6.3/uom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-09-21 13:38:58.000000 uom-0.6.3/uom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 13:38:58.000000 uom-0.6.3/uom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-21 13:38:58.000000 uom-0.6.3/uom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-09-21 13:38:58.000000 uom-0.6.3/uom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:01:47.101849 uom-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-26 20:00:46.000000 uom-0.6.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 20:00:46.000000 uom-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-26 20:01:47.101849 uom-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-26 20:00:46.000000 uom-0.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 20:00:46.000000 uom-0.6.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-26 20:01:47.101849 uom-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-26 20:00:46.000000 uom-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:01:47.101849 uom-0.6.7/uom/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-26 20:00:46.000000 uom-0.6.7/uom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-26 20:00:46.000000 uom-0.6.7/uom/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-26 20:00:46.000000 uom-0.6.7/uom/unit_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144435 2024-04-26 20:00:46.000000 uom-0.6.7/uom/uom.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-26 20:00:46.000000 uom-0.6.7/uom/uom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-26 20:00:46.000000 uom-0.6.7/uom/uomdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:01:47.101849 uom-0.6.7/uom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-26 20:01:47.000000 uom-0.6.7/uom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-26 20:01:47.000000 uom-0.6.7/uom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:01:47.000000 uom-0.6.7/uom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-26 20:01:47.000000 uom-0.6.7/uom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:01:46.000000 uom-0.6.7/uom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 20:01:47.000000 uom-0.6.7/uom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-26 20:01:47.000000 uom-0.6.7/uom.egg-info/top_level.txt
```

### Comparing `uom-0.6.3/LICENSE.md` & `uom-0.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uom-0.6.3/PKG-INFO` & `uom-0.6.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uom
-Version: 0.6.3
+Version: 0.6.7
 Summary: Unit of Measure conversion tool
 Home-page: http://github.com/schlumberger/UOM
 Author: Velizar VESSELINOV
 Author-email: vvesselinov@slb.com
 License: BSD 2-Clause “Simplified” License
 Keywords: uom unit measurement measure Energistics oilfield
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,20 +14,23 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pandas
+Requires-Dist: colorlog
 
 # UOM
 
 ## Static code analysis
 
 | Tools | Badges |
 | --- | --------------------------- |
@@ -43,16 +46,16 @@
 | PePy | [![Downloads](https://pepy.tech/badge/uom)](https://pepy.tech/project/uom) [![Downloads](https://pepy.tech/badge/uom/month)](https://pepy.tech/project/uom) [![Downloads](https://pepy.tech/badge/uom/week)](https://pepy.tech/project/uom) |
 | Code formatting | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
 
 <!--
 ## Build package
 
 ```sh
-pip3 install wheel
-python3 setup.py bdist_wheel
+pip3 install test-requirements.txt
+python -m build
 ``` -->
 
 ## Description
 
 Python unit of measure (UOM) conversion tool
 
 Energistics UOM 1.0 (<https://www.energistics.org/energistics-unit-of-measure-standard/>)
```

### Comparing `uom-0.6.3/README.md` & `uom-0.6.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 | PePy | [![Downloads](https://pepy.tech/badge/uom)](https://pepy.tech/project/uom) [![Downloads](https://pepy.tech/badge/uom/month)](https://pepy.tech/project/uom) [![Downloads](https://pepy.tech/badge/uom/week)](https://pepy.tech/project/uom) |
 | Code formatting | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
 
 <!--
 ## Build package
 
 ```sh
-pip3 install wheel
-python3 setup.py bdist_wheel
+pip3 install test-requirements.txt
+python -m build
 ``` -->
 
 ## Description
 
 Python unit of measure (UOM) conversion tool
 
 Energistics UOM 1.0 (<https://www.energistics.org/energistics-unit-of-measure-standard/>)
```

### Comparing `uom-0.6.3/setup.py` & `uom-0.6.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Python Package setup."""
+
 from __future__ import absolute_import
 
 from setuptools import setup
 
 
 def requirements():
     """Requirement from source."""
@@ -14,15 +15,15 @@
     """Readme from source."""
     with open("README.md", "r", encoding="utf8") as fil:
         return fil.read()
 
 
 setup(
     name="uom",
-    version="0.6.3",
+    version="0.6.7",
     description="Unit of Measure conversion tool",
     long_description=readme(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Customer Service",
@@ -30,14 +31,16 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Information Analysis",
     ],
     keywords="uom unit measurement measure Energistics oilfield",
     url="http://github.com/schlumberger/UOM",
     author="Velizar VESSELINOV",
     author_email="vvesselinov@slb.com",
```

### Comparing `uom-0.6.3/uom/unit_alias.py` & `uom-0.6.7/uom/unit_alias.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     "PPA": "lbm/gal[US]",
     "PPG": "lbm/gal[US]",
     "PPGE": "lbm/gal[US]",
     "lb/U.S.gal": "lbm/gal[US]",
     "lbm/galUS": "lbm/gal[US]",
     "1000 kgf": "Mgf",
     "KKGF": "Mgf",
+    "tf": "Mgf",
     "v": "V",
     "VOLT": "V",
     "Volts": "V",
     "volts": "V",
     "В": "V",
     "Mv": "MV",
     "DEGC": "degC",
@@ -103,15 +104,15 @@
     "DEGF": "degF",
     "DegF": "degF",
     "deg F": "degF",
     "oF": "degF",
     "°F": "degF",
     "RPM": "rpm",
     "KLBF": "klbf",
-    "KFLB": "klbf",
+    "KFLB": "klbf.ft",  # WITS thousand foot-pounds (torque)
     "G": "gn",
     "G's": "gn",
     "hr": "h",
     "hour": "h",
     "HR": "h",
     "hrs": "h",
     "MINUTES": "min",
@@ -158,15 +159,15 @@
     "lbs": "lbf",
     "kg/(m.s2)": "Pa",
     "AHrs": "A.h",
     "amp-hours": "A.h",
     "degreesCelsius": "degC",
     "KNM": "kN.m",
     "KGM3": "kg/m3",
-    "KDN": "kdyne",
+    "KDN": "10 kN",  # WITS kilo deca Newton
     "RPG": "rev/gal[US]",
     "0.01 m3/m3": "0.01 bbl/bbl",
     "0.001/(ohm.m)": "mS",
     "MMSCFD": "1E6 ft3/d",
     "MMscfd": "1E6 ft3/d",
     "mmscfd": "1E6 ft3/d",
 }
```

### Comparing `uom-0.6.3/uom/uom.csv` & `uom-0.6.7/uom/uom.csv`

 * *Files identical despite different names*

### Comparing `uom-0.6.3/uom.egg-info/PKG-INFO` & `uom-0.6.7/uom.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uom
-Version: 0.6.3
+Version: 0.6.7
 Summary: Unit of Measure conversion tool
 Home-page: http://github.com/schlumberger/UOM
 Author: Velizar VESSELINOV
 Author-email: vvesselinov@slb.com
 License: BSD 2-Clause “Simplified” License
 Keywords: uom unit measurement measure Energistics oilfield
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,20 +14,23 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pandas
+Requires-Dist: colorlog
 
 # UOM
 
 ## Static code analysis
 
 | Tools | Badges |
 | --- | --------------------------- |
@@ -43,16 +46,16 @@
 | PePy | [![Downloads](https://pepy.tech/badge/uom)](https://pepy.tech/project/uom) [![Downloads](https://pepy.tech/badge/uom/month)](https://pepy.tech/project/uom) [![Downloads](https://pepy.tech/badge/uom/week)](https://pepy.tech/project/uom) |
 | Code formatting | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
 
 <!--
 ## Build package
 
 ```sh
-pip3 install wheel
-python3 setup.py bdist_wheel
+pip3 install test-requirements.txt
+python -m build
 ``` -->
 
 ## Description
 
 Python unit of measure (UOM) conversion tool
 
 Energistics UOM 1.0 (<https://www.energistics.org/energistics-unit-of-measure-standard/>)
```

