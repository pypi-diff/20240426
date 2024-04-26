# Comparing `tmp/pyridy-1.0.3.tar.gz` & `tmp/pyridy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyridy-1.0.3.tar", max compression
+gzip compressed data, was "pyridy-1.0.4.tar", max compression
```

## Comparing `pyridy-1.0.3.tar` & `pyridy-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0    11583 2023-02-14 16:19:37.926633 pyridy-1.0.3/LICENSE
--rw-r--r--   0        0        0      971 2023-05-11 13:19:47.076041 pyridy-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       65 2023-02-14 16:19:37.951522 pyridy-1.0.3/pyridy/__init__.py
--rw-r--r--   0        0        0    22145 2023-03-09 12:44:02.621957 pyridy-1.0.3/pyridy/campaign.py
--rw-r--r--   0        0        0     2402 2023-02-14 16:19:37.954033 pyridy-1.0.3/pyridy/config.py
--rw-r--r--   0        0        0    62789 2023-03-09 12:44:02.626960 pyridy-1.0.3/pyridy/file.py
--rw-r--r--   0        0        0       22 2023-02-14 16:19:37.955033 pyridy-1.0.3/pyridy/osm/__init__.py
--rw-r--r--   0        0        0    30598 2023-04-27 12:36:22.469380 pyridy-1.0.3/pyridy/osm/osm.py
--rw-r--r--   0        0        0      121 2023-02-14 16:19:37.956033 pyridy-1.0.3/pyridy/osm/utils/__init__.py
--rw-r--r--   0        0        0    12461 2023-04-27 12:36:22.472382 pyridy-1.0.3/pyridy/osm/utils/elements.py
--rw-r--r--   0        0        0     6329 2023-03-09 12:44:02.642961 pyridy-1.0.3/pyridy/osm/utils/overpass.py
--rw-r--r--   0        0        0     1173 2023-03-09 12:44:02.647963 pyridy-1.0.3/pyridy/osm/utils/query.py
--rw-r--r--   0        0        0       60 2023-02-14 16:19:37.958033 pyridy-1.0.3/pyridy/osm/utils/relation.py
--rw-r--r--   0        0        0    14525 2023-03-09 16:42:58.451384 pyridy-1.0.3/pyridy/osm/utils/tools.py
--rw-r--r--   0        0        0      105 2023-02-14 16:19:37.959032 pyridy-1.0.3/pyridy/processing/__init__.py
--rw-r--r--   0        0        0    16957 2023-03-09 16:42:58.467625 pyridy-1.0.3/pyridy/processing/comfort.py
--rw-r--r--   0        0        0     6510 2023-03-09 12:44:02.659964 pyridy-1.0.3/pyridy/processing/condition.py
--rw-r--r--   0        0        0     8805 2023-03-09 16:42:58.476180 pyridy-1.0.3/pyridy/processing/excitation.py
--rw-r--r--   0        0        0      239 2023-02-14 16:19:37.961198 pyridy-1.0.3/pyridy/processing/processor.py
--rw-r--r--   0        0        0       57 2023-02-14 16:19:37.962255 pyridy-1.0.3/pyridy/utils/__init__.py
--rw-r--r--   0        0        0     3740 2023-02-14 16:19:37.962255 pyridy-1.0.3/pyridy/utils/device.py
--rw-r--r--   0        0        0     2000 2023-02-14 16:19:37.963205 pyridy-1.0.3/pyridy/utils/sensor.py
--rw-r--r--   0        0        0    46523 2023-03-09 16:42:58.434611 pyridy-1.0.3/pyridy/utils/timeseries.py
--rw-r--r--   0        0        0     3890 2023-03-09 16:42:58.443203 pyridy-1.0.3/pyridy/utils/tools.py
--rw-r--r--   0        0        0       18 2023-02-14 16:19:37.965205 pyridy-1.0.3/pyridy/widgets/__init__.py
--rw-r--r--   0        0        0    12800 2023-02-14 16:19:37.965205 pyridy-1.0.3/pyridy/widgets/map.py
--rw-r--r--   0        0        0     2332 2023-02-14 16:19:37.926633 pyridy-1.0.3/README.md
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 pyridy-1.0.3/setup.py
--rw-r--r--   0        0        0     3677 1970-01-01 00:00:00.000000 pyridy-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11583 2023-02-14 16:19:37.926633 pyridy-1.0.4/LICENSE
+-rw-r--r--   0        0        0      988 2024-04-26 13:35:31.503470 pyridy-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-02-14 16:19:37.951522 pyridy-1.0.4/pyridy/__init__.py
+-rw-r--r--   0        0        0    22145 2023-03-09 12:44:02.621957 pyridy-1.0.4/pyridy/campaign.py
+-rw-r--r--   0        0        0     2402 2023-02-14 16:19:37.954033 pyridy-1.0.4/pyridy/config.py
+-rw-r--r--   0        0        0    62635 2024-02-20 10:12:28.770803 pyridy-1.0.4/pyridy/file.py
+-rw-r--r--   0        0        0       22 2023-02-14 16:19:37.955033 pyridy-1.0.4/pyridy/osm/__init__.py
+-rw-r--r--   0        0        0    30598 2023-04-27 12:36:22.469380 pyridy-1.0.4/pyridy/osm/osm.py
+-rw-r--r--   0        0        0      121 2023-02-14 16:19:37.956033 pyridy-1.0.4/pyridy/osm/utils/__init__.py
+-rw-r--r--   0        0        0    12461 2023-04-27 12:36:22.472382 pyridy-1.0.4/pyridy/osm/utils/elements.py
+-rw-r--r--   0        0        0     6329 2023-03-09 12:44:02.642961 pyridy-1.0.4/pyridy/osm/utils/overpass.py
+-rw-r--r--   0        0        0     1173 2023-03-09 12:44:02.647963 pyridy-1.0.4/pyridy/osm/utils/query.py
+-rw-r--r--   0        0        0       60 2023-02-14 16:19:37.958033 pyridy-1.0.4/pyridy/osm/utils/relation.py
+-rw-r--r--   0        0        0    14525 2023-03-09 16:42:58.451384 pyridy-1.0.4/pyridy/osm/utils/tools.py
+-rw-r--r--   0        0        0      105 2023-02-14 16:19:37.959032 pyridy-1.0.4/pyridy/processing/__init__.py
+-rw-r--r--   0        0        0    16957 2023-03-09 16:42:58.467625 pyridy-1.0.4/pyridy/processing/comfort.py
+-rw-r--r--   0        0        0     6510 2023-03-09 12:44:02.659964 pyridy-1.0.4/pyridy/processing/condition.py
+-rw-r--r--   0        0        0     8805 2023-03-09 16:42:58.476180 pyridy-1.0.4/pyridy/processing/excitation.py
+-rw-r--r--   0        0        0      239 2023-02-14 16:19:37.961198 pyridy-1.0.4/pyridy/processing/processor.py
+-rw-r--r--   0        0        0       57 2023-02-14 16:19:37.962255 pyridy-1.0.4/pyridy/utils/__init__.py
+-rw-r--r--   0        0        0     3740 2023-02-14 16:19:37.962255 pyridy-1.0.4/pyridy/utils/device.py
+-rw-r--r--   0        0        0     2000 2023-02-14 16:19:37.963205 pyridy-1.0.4/pyridy/utils/sensor.py
+-rw-r--r--   0        0        0    46523 2023-03-09 16:42:58.434611 pyridy-1.0.4/pyridy/utils/timeseries.py
+-rw-r--r--   0        0        0     3890 2023-03-09 16:42:58.443203 pyridy-1.0.4/pyridy/utils/tools.py
+-rw-r--r--   0        0        0       18 2023-02-14 16:19:37.965205 pyridy-1.0.4/pyridy/widgets/__init__.py
+-rw-r--r--   0        0        0    12800 2023-02-14 16:19:37.965205 pyridy-1.0.4/pyridy/widgets/map.py
+-rw-r--r--   0        0        0     2332 2023-02-14 16:19:37.926633 pyridy-1.0.4/README.md
+-rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 pyridy-1.0.4/PKG-INFO
```

### Comparing `pyridy-1.0.3/LICENSE` & `pyridy-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/campaign.py` & `pyridy-1.0.4/pyridy/campaign.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/config.py` & `pyridy-1.0.4/pyridy/config.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/file.py` & `pyridy-1.0.4/pyridy/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,28 @@
 from sqlite3 import DatabaseError
 from typing import Optional, List, Dict, Tuple, Union, Type
 
 import networkx as nx
 import numpy as np
 import overpy
 import pandas as pd
-from ipyleaflet import Map, ScaleControl, FullScreenControl, Polyline, Marker, Circle, LayerGroup
-from ipywidgets import HTML
+from ipyleaflet import Map
 from pandas.io.sql import DatabaseError as PandasDatabaseError
 from scipy.spatial import KDTree
 from scipy.stats import norm
 
 from pyridy import config
 from pyridy.config import cm, options
 from pyridy.osm import OSM, OSMRailwayLine
 from pyridy.osm.utils import is_point_within_line_projection, project_point_onto_line
 from pyridy.utils import Sensor, AccelerationSeries, LinearAccelerationSeries, MagnetometerSeries, OrientationSeries, \
     GyroSeries, RotationSeries, GPSSeries, PressureSeries, HumiditySeries, TemperatureSeries, WzSeries, LightSeries, \
     SubjectiveComfortSeries, AccelerationUncalibratedSeries, MagnetometerUncalibratedSeries, GyroUncalibratedSeries, \
     GNSSClockMeasurementSeries, GNSSMeasurementSeries, NMEAMessageSeries, TimeSeries, NTPDatetimeSeries
 from pyridy.utils.device import Device
-from pyridy.utils.tools import generate_random_color
 
 logger = logging.getLogger(__name__)
 
 
 class RDYFile:
     c_cycler = itertools.cycle(cm.rwth_color_cycle)
 
@@ -1177,15 +1175,15 @@
         ----------
         interpolate : bool
             If true interpolates NaN values of concatenated measurement series
 
         Returns
         -------
         dataframe : pd.DataFrame
-            Dataframe containing the measurements
+            DataFrame containing the measurements
         """
         data_frames = [series.to_df() for series in self.measurements.values()]
 
         # Concatenate dataframes and resort them ascending
         df_merged = pd.concat(data_frames).sort_index()
 
         # Merge identical indices by taking mean of column values and then interpolate NaN values
```

### Comparing `pyridy-1.0.3/pyridy/osm/osm.py` & `pyridy-1.0.4/pyridy/osm/osm.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/osm/utils/elements.py` & `pyridy-1.0.4/pyridy/osm/utils/elements.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/osm/utils/overpass.py` & `pyridy-1.0.4/pyridy/osm/utils/overpass.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/osm/utils/query.py` & `pyridy-1.0.4/pyridy/osm/utils/query.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/osm/utils/tools.py` & `pyridy-1.0.4/pyridy/osm/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/processing/comfort.py` & `pyridy-1.0.4/pyridy/processing/comfort.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/processing/condition.py` & `pyridy-1.0.4/pyridy/processing/condition.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/processing/excitation.py` & `pyridy-1.0.4/pyridy/processing/excitation.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/utils/device.py` & `pyridy-1.0.4/pyridy/utils/device.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/utils/sensor.py` & `pyridy-1.0.4/pyridy/utils/sensor.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/utils/timeseries.py` & `pyridy-1.0.4/pyridy/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/utils/tools.py` & `pyridy-1.0.4/pyridy/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/pyridy/widgets/map.py` & `pyridy-1.0.4/pyridy/widgets/map.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/README.md` & `pyridy-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.3/PKG-INFO` & `pyridy-1.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: pyridy
-Version: 1.0.3
+Version: 1.0.4
 Summary: Support library for measurements made with the Ridy Android App
 License: Apache-2.0
 Keywords: signal processing,ridy,android
 Author: Philipp Simon Leibner
 Author-email: philipp.leibner@ifs.rwth-aachen.de
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Dist: HeapDict (>=1.0.1,<2.0.0)
-Requires-Dist: Shapely (>=1.8.1,<2.0.0)
-Requires-Dist: geopy (>=2.1.0,<3.0.0)
-Requires-Dist: ipyleaflet (>=0.17.0,<0.18.0)
-Requires-Dist: matplotlib (>=3.4.1,<4.0.0)
-Requires-Dist: networkx (>=3.1,<4.0)
-Requires-Dist: numpy (>=1.21.5,<2.0.0)
-Requires-Dist: overpy (>=0.6,<0.7)
-Requires-Dist: pandas (>=1.2.0,<2.0.0)
-Requires-Dist: pyproj (>=3.3.0,<4.0.0)
-Requires-Dist: pytest (>=7.1.1,<8.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
-Requires-Dist: rwthcolors (>=0.2.3,<0.3.0)
-Requires-Dist: scipy (>=1.6.3,<2.0.0)
-Requires-Dist: tqdm (>=4.60.0,<5.0.0)
+Requires-Dist: HeapDict (>=1.0.1)
+Requires-Dist: Shapely (>=1.8.1)
+Requires-Dist: geopy (>=2.1.0)
+Requires-Dist: ipyleaflet (>=0.19.0)
+Requires-Dist: matplotlib (>=3.8.1)
+Requires-Dist: networkx (>=3.1)
+Requires-Dist: numpy (>=1.26.4)
+Requires-Dist: overpy (>=0.6)
+Requires-Dist: pandas (>=2.2.0)
+Requires-Dist: pyproj (>=3.3.0)
+Requires-Dist: pytest (>=8.1.1)
+Requires-Dist: requests (>=2.28.1)
+Requires-Dist: requests-cache (>=1.0.1)
+Requires-Dist: rwthcolors (>=0.2.3)
+Requires-Dist: scipy (>=1.6.3)
+Requires-Dist: tqdm (>=4.60.0)
 Description-Content-Type: text/markdown
 
 # PyRidy
 
 ![alt text](assets/ic_launcher.png "PyRidy Logo")
 
 Python Support Library to import and process Ridy files
```

#### html2text {}

```diff
@@ -1,48 +1,46 @@
-Metadata-Version: 2.1 Name: pyridy Version: 1.0.3 Summary: Support library for
+Metadata-Version: 2.1 Name: pyridy Version: 1.0.4 Summary: Support library for
 measurements made with the Ridy Android App License: Apache-2.0 Keywords:
 signal processing,ridy,android Author: Philipp Simon Leibner Author-email:
-philipp.leibner@ifs.rwth-aachen.de Requires-Python: >=3.8,<3.12 Classifier:
+philipp.leibner@ifs.rwth-aachen.de Requires-Python: >=3.9,<3.13 Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Requires-Dist: HeapDict
-(>=1.0.1,<2.0.0) Requires-Dist: Shapely (>=1.8.1,<2.0.0) Requires-Dist: geopy
-(>=2.1.0,<3.0.0) Requires-Dist: ipyleaflet (>=0.17.0,<0.18.0) Requires-Dist:
-matplotlib (>=3.4.1,<4.0.0) Requires-Dist: networkx (>=3.1,<4.0) Requires-Dist:
-numpy (>=1.21.5,<2.0.0) Requires-Dist: overpy (>=0.6,<0.7) Requires-Dist:
-pandas (>=1.2.0,<2.0.0) Requires-Dist: pyproj (>=3.3.0,<4.0.0) Requires-Dist:
-pytest (>=7.1.1,<8.0.0) Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-
-Dist: requests-cache (>=1.0.1,<2.0.0) Requires-Dist: rwthcolors
-(>=0.2.3,<0.3.0) Requires-Dist: scipy (>=1.6.3,<2.0.0) Requires-Dist: tqdm
-(>=4.60.0,<5.0.0) Description-Content-Type: text/markdown # PyRidy ![alt text]
-(assets/ic_launcher.png "PyRidy Logo") Python Support Library to import and
-process Ridy files ### About Ridy Ridy is an Android App to record sensor data
-for uses in science and engineering. The app is currently actively being
-developed at the [Chair and Institute for Rail Vehicles and Transport Systems
-(IFS)](http://www.ifs.rwth-aachen.de/en/start/) [Ridy Screenshot]At the
-institute Ridy is e.g. used for condition monitoring of railway tracks and
-several more use-cases are currently researched upon. Among other, Ridy can
-record: * Acceleration * Linear Acceleration (i.e., without g-Force) * Magnetic
-Field * Gyroscope * Orientation * GNSS Location (+ Android Raw GNSS
-Measurements) * Pressure, Humidity, Temperature, Ambient Light Compared to
-other existing apps Ridy can perform long measurements even in the background
-when the phone is locked. The app supports two formats for data export, JSON
-and SQLITE. If you would like to use or try out the app please contact the
-developer (see below) to get access. ### About PyRidy PyRidy is the companion
-python library for the Ridy Android App. It provides easy access to the data no
-matter which recording format was used. If pyridy is used, one does no longer
-need to manually write code to import the files. In addition, pyridy provides
-several more features: * Automatic conversion of sensor data into objects and
-numpy arrays * Conversion of arrays to Pandas DataFrame objects * Time
-synchronization of individual files (e.g. from different phones) * Download of
-OSM Railway Data via the Overpass API * Plotting of GPS tracks onto a map using
-ipyleaflet ### Documentation [PyRidy Documentation](https://
+(>=1.0.1) Requires-Dist: Shapely (>=1.8.1) Requires-Dist: geopy (>=2.1.0)
+Requires-Dist: ipyleaflet (>=0.19.0) Requires-Dist: matplotlib (>=3.8.1)
+Requires-Dist: networkx (>=3.1) Requires-Dist: numpy (>=1.26.4) Requires-Dist:
+overpy (>=0.6) Requires-Dist: pandas (>=2.2.0) Requires-Dist: pyproj (>=3.3.0)
+Requires-Dist: pytest (>=8.1.1) Requires-Dist: requests (>=2.28.1) Requires-
+Dist: requests-cache (>=1.0.1) Requires-Dist: rwthcolors (>=0.2.3) Requires-
+Dist: scipy (>=1.6.3) Requires-Dist: tqdm (>=4.60.0) Description-Content-Type:
+text/markdown # PyRidy ![alt text](assets/ic_launcher.png "PyRidy Logo") Python
+Support Library to import and process Ridy files ### About Ridy Ridy is an
+Android App to record sensor data for uses in science and engineering. The app
+is currently actively being developed at the [Chair and Institute for Rail
+Vehicles and Transport Systems (IFS)](http://www.ifs.rwth-aachen.de/en/start/)
+[Ridy Screenshot]At the institute Ridy is e.g. used for condition monitoring of
+railway tracks and several more use-cases are currently researched upon. Among
+other, Ridy can record: * Acceleration * Linear Acceleration (i.e., without g-
+Force) * Magnetic Field * Gyroscope * Orientation * GNSS Location (+ Android
+Raw GNSS Measurements) * Pressure, Humidity, Temperature, Ambient Light
+Compared to other existing apps Ridy can perform long measurements even in the
+background when the phone is locked. The app supports two formats for data
+export, JSON and SQLITE. If you would like to use or try out the app please
+contact the developer (see below) to get access. ### About PyRidy PyRidy is the
+companion python library for the Ridy Android App. It provides easy access to
+the data no matter which recording format was used. If pyridy is used, one does
+no longer need to manually write code to import the files. In addition, pyridy
+provides several more features: * Automatic conversion of sensor data into
+objects and numpy arrays * Conversion of arrays to Pandas DataFrame objects *
+Time synchronization of individual files (e.g. from different phones) *
+Download of OSM Railway Data via the Overpass API * Plotting of GPS tracks onto
+a map using ipyleaflet ### Documentation [PyRidy Documentation](https://
 pyridy.readthedocs.io/) #### Installation Install using pip ```python pip
 install pyridy ``` #### Usage Information and examples on how to use the
 library can be found in the [PyRidy documentation](https://
 pyridy.readthedocs.io/) ### Creator Philipp Leibner - philipp.leibner@ifs.rwth-
 aachen.de ### Contributor Daniel Pujiula Buhl - daniel.pujiula@rwth-aachen.de
 Sarra Bouchkati - sarra.bouchkati@rwth-aachen.de
 [IFS Logo]
```

