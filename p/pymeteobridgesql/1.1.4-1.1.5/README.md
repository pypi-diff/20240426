# Comparing `tmp/pymeteobridgesql-1.1.4.tar.gz` & `tmp/pymeteobridgesql-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeteobridgesql-1.1.4.tar", last modified: Tue Mar  5 14:52:45 2024, max compression
+gzip compressed data, was "pymeteobridgesql-1.1.5.tar", last modified: Fri Apr 26 17:08:28 2024, max compression
```

## Comparing `pymeteobridgesql-1.1.4.tar` & `pymeteobridgesql-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:52:45.752097 pymeteobridgesql-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-05 14:52:35.000000 pymeteobridgesql-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-05 14:52:45.752097 pymeteobridgesql-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-05 14:52:35.000000 pymeteobridgesql-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:52:45.748098 pymeteobridgesql-1.1.4/pymeteobridgesql/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-05 14:52:35.000000 pymeteobridgesql-1.1.4/pymeteobridgesql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-05 14:52:35.000000 pymeteobridgesql-1.1.4/pymeteobridgesql/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-03-05 14:52:35.000000 pymeteobridgesql-1.1.4/pymeteobridgesql/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 14:52:45.752097 pymeteobridgesql-1.1.4/pymeteobridgesql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-05 14:52:45.000000 pymeteobridgesql-1.1.4/pymeteobridgesql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-05 14:52:45.000000 pymeteobridgesql-1.1.4/pymeteobridgesql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 14:52:45.000000 pymeteobridgesql-1.1.4/pymeteobridgesql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-05 14:52:45.000000 pymeteobridgesql-1.1.4/pymeteobridgesql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 14:52:45.752097 pymeteobridgesql-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-05 14:52:35.000000 pymeteobridgesql-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:08:28.287230 pymeteobridgesql-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-26 17:08:28.287230 pymeteobridgesql-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:08:28.283230 pymeteobridgesql-1.1.5/pymeteobridgesql/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/pymeteobridgesql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/pymeteobridgesql/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/pymeteobridgesql/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:08:28.283230 pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-26 17:08:28.000000 pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-26 17:08:28.000000 pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:08:28.000000 pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 17:08:28.000000 pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 17:08:28.287230 pymeteobridgesql-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/setup.py
```

### Comparing `pymeteobridgesql-1.1.4/LICENSE` & `pymeteobridgesql-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeteobridgesql-1.1.4/PKG-INFO` & `pymeteobridgesql-1.1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.1.4
+Version: 1.1.5
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.1.4/pymeteobridgesql/api.py` & `pymeteobridgesql-1.1.5/pymeteobridgesql/api.py`

 * *Files identical despite different names*

### Comparing `pymeteobridgesql-1.1.4/pymeteobridgesql/data.py` & `pymeteobridgesql-1.1.5/pymeteobridgesql/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """This module describes dataclasses used by pymeteobridgesql."""
 
 from __future__ import annotations
 
-import dataclasses
+from dataclasses import dataclass
 import datetime
 import math
 
-@dataclasses.dataclass
+@dataclass(frozen=True)
 class RealtimeData:
     ID: str
     temperature: float
     tempmax: float
     tempmin: float
     windchill: float
     pm1: float
@@ -173,15 +173,15 @@
         if self.windbearing is None:
             return None
 
         directions = ['N', 'NNE', 'NE', 'ENE', 'E', 'ESE', 'SE', 'SSE', 'S', 'SSW', 'SW', 'WSW', 'W', 'WNW', 'NW', 'NNW']
         index = round(self.windbearing / 22.5) % 16
         return directions[index].lower()
 
-@dataclasses.dataclass
+@dataclass(frozen=True)
 class ForecastHourly:
     hour_num: int
     datetime: datetime.datetime
     temperature: float
     apparent_temperature: float
     humidity: int
     description: str
@@ -190,30 +190,30 @@
     precipitation: float
     pressure: float
     wind_bearing: int
     wind_speed: float
     wind_gust: float
     uv_index: float
 
-@dataclasses.dataclass
+@dataclass(frozen=True)
 class ForecastDaily:
     day_num: int
     datetime: datetime.datetime
     temperature: float
     temp_low: float
     description: str
     icon: str
     precipitation_probability: int
     precipitation: float
     pressure: float
     wind_bearing: int
     wind_speed: float
     wind_gust: float
 
-@dataclasses.dataclass
+@dataclass(frozen=True)
 class StationData:
     ID: str
     mb_ip: str
     mb_swversion: str
     mb_buildnum: str
     mb_platform: str
     mb_station: str
```

### Comparing `pymeteobridgesql-1.1.4/pymeteobridgesql.egg-info/PKG-INFO` & `pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.1.4
+Version: 1.1.5
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.1.4/setup.py` & `pymeteobridgesql-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymeteobridgesql",
-    version="1.1.4",
+    version="1.1.5",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets weather data from a MySQL table",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pymeteobridgesql",
```

