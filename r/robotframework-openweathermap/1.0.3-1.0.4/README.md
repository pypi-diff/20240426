# Comparing `tmp/robotframework-openweathermap-1.0.3.tar.gz` & `tmp/robotframework_openweathermap-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-openweathermap-1.0.3.tar", last modified: Tue Sep 20 15:00:48 2022, max compression
+gzip compressed data, was "robotframework_openweathermap-1.0.4.tar", last modified: Fri Apr 26 20:34:36 2024, max compression
```

## Comparing `robotframework-openweathermap-1.0.3.tar` & `robotframework_openweathermap-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 15:00:48.888800 robotframework-openweathermap-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-20 15:00:37.000000 robotframework-openweathermap-1.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 15:00:48.888800 robotframework-openweathermap-1.0.3/OpenWeatherMapLibrary/
--rw-r--r--   0 runner    (1001) docker     (121)    37143 2022-09-20 15:00:37.000000 robotframework-openweathermap-1.0.3/OpenWeatherMapLibrary/OpenWeatherMapLibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-20 15:00:37.000000 robotframework-openweathermap-1.0.3/OpenWeatherMapLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12767 2022-09-20 15:00:48.888800 robotframework-openweathermap-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11900 2022-09-20 15:00:37.000000 robotframework-openweathermap-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 15:00:48.888800 robotframework-openweathermap-1.0.3/robotframework_openweathermap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12767 2022-09-20 15:00:48.000000 robotframework-openweathermap-1.0.3/robotframework_openweathermap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-09-20 15:00:48.000000 robotframework-openweathermap-1.0.3/robotframework_openweathermap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-20 15:00:48.000000 robotframework-openweathermap-1.0.3/robotframework_openweathermap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-20 15:00:48.000000 robotframework-openweathermap-1.0.3/robotframework_openweathermap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-20 15:00:48.000000 robotframework-openweathermap-1.0.3/robotframework_openweathermap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-20 15:00:48.892799 robotframework-openweathermap-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-09-20 15:00:37.000000 robotframework-openweathermap-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:34:36.946726 robotframework_openweathermap-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-26 20:34:30.000000 robotframework_openweathermap-1.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:34:36.946726 robotframework_openweathermap-1.0.4/OpenWeatherMapLibrary/
+-rw-r--r--   0 runner    (1001) docker     (127)    37143 2024-04-26 20:34:30.000000 robotframework_openweathermap-1.0.4/OpenWeatherMapLibrary/OpenWeatherMapLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 20:34:30.000000 robotframework_openweathermap-1.0.4/OpenWeatherMapLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12834 2024-04-26 20:34:36.946726 robotframework_openweathermap-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-26 20:34:30.000000 robotframework_openweathermap-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:34:36.946726 robotframework_openweathermap-1.0.4/robotframework_openweathermap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12834 2024-04-26 20:34:36.000000 robotframework_openweathermap-1.0.4/robotframework_openweathermap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-26 20:34:36.000000 robotframework_openweathermap-1.0.4/robotframework_openweathermap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:34:36.000000 robotframework_openweathermap-1.0.4/robotframework_openweathermap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 20:34:36.000000 robotframework_openweathermap-1.0.4/robotframework_openweathermap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 20:34:36.000000 robotframework_openweathermap-1.0.4/robotframework_openweathermap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:34:36.946726 robotframework_openweathermap-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-26 20:34:30.000000 robotframework_openweathermap-1.0.4/setup.py
```

### Comparing `robotframework-openweathermap-1.0.3/LICENSE` & `robotframework_openweathermap-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-openweathermap-1.0.3/OpenWeatherMapLibrary/OpenWeatherMapLibrary.py` & `robotframework_openweathermap-1.0.4/OpenWeatherMapLibrary/OpenWeatherMapLibrary.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import logging
 
 logging.basicConfig(
     level=logging.DEBUG, format="%(asctime)s %(module)s -%(levelname)s- %(message)s"
 )
 logger = logging.getLogger(__name__)
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __author__ = "Joerg Schultze-Lutter"
 
 #
 # Various API types which are supported by the OpenWeatherMap API
 # Enum value is used for the construction of the future URL
 #
 class OpenWeatherMapApiType(Enum):
@@ -496,15 +496,15 @@
         language: str = None,
     ):
         # perform pre-sanity checks for the optional parameters
         exclude = self.__owm_exclude_check(owm_exclude=exclude)
         unit_format = self.__owm_unit_format_check(owm_unit_format=unit_format)
         language = self.__owm_language_check(owm_language=language)
 
-        __url_path = "/2.5/onecall"
+        __url_path = "/3.0/onecall"
         url = self.__get_base_api(api_type=OpenWeatherMapApiType.API) + __url_path
 
         # Add mandatory / optional fields whereas present
         # parameter payload dictionary
         payload = {}
 
         # fmt: off
```

### Comparing `robotframework-openweathermap-1.0.3/PKG-INFO` & `robotframework_openweathermap-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openweathermap
-Version: 1.0.3
+Version: 1.0.4
 Summary: Robot Framework keywords for the 'OpenWeatherMap' library
 Home-page: https://github.com/joergschultzelutter/robotframework-openweathermap
 Author: Joerg Schultze-Lutter
 Author-email: joerg.schultze.lutter@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: Robot Framework
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,16 @@
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: robotframework>=3.2
+Requires-Dist: requests>=2.26.0
 
 # robotframework-openweathermap
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CodeQL](https://github.com/joergschultzelutter/robotframework-openweathermap/actions/workflows/codeql.yml/badge.svg)](https://github.com/joergschultzelutter/robotframework-openweathermap/actions/workflows/codeql.yml) [![PyPi version](https://img.shields.io/pypi/v/robotframework-openweathermap.svg)](https://pypi.python.org/pypi/robotframework-openweathermap)
 
 ```robotframework-openweathermap``` is a [Robot Framework](https://www.robotframework.org) keyword collection for the [OpenWeatherMap](https://www.openweathermap.org/api) API.
```

### Comparing `robotframework-openweathermap-1.0.3/README.md` & `robotframework_openweathermap-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-openweathermap-1.0.3/robotframework_openweathermap.egg-info/PKG-INFO` & `robotframework_openweathermap-1.0.4/robotframework_openweathermap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openweathermap
-Version: 1.0.3
+Version: 1.0.4
 Summary: Robot Framework keywords for the 'OpenWeatherMap' library
 Home-page: https://github.com/joergschultzelutter/robotframework-openweathermap
 Author: Joerg Schultze-Lutter
 Author-email: joerg.schultze.lutter@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: Robot Framework
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,16 @@
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: robotframework>=3.2
+Requires-Dist: requests>=2.26.0
 
 # robotframework-openweathermap
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CodeQL](https://github.com/joergschultzelutter/robotframework-openweathermap/actions/workflows/codeql.yml/badge.svg)](https://github.com/joergschultzelutter/robotframework-openweathermap/actions/workflows/codeql.yml) [![PyPi version](https://img.shields.io/pypi/v/robotframework-openweathermap.svg)](https://pypi.python.org/pypi/robotframework-openweathermap)
 
 ```robotframework-openweathermap``` is a [Robot Framework](https://www.robotframework.org) keyword collection for the [OpenWeatherMap](https://www.openweathermap.org/api) API.
```

### Comparing `robotframework-openweathermap-1.0.3/setup.py` & `robotframework_openweathermap-1.0.4/setup.py`

 * *Files identical despite different names*

