# Comparing `tmp/pydolarvenezuela-1.4.3.tar.gz` & `tmp/pydolarvenezuela-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.4.3.tar", last modified: Thu Apr 25 23:19:00 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.4.4.tar", last modified: Thu Apr 25 23:38:40 2024, max compression
```

## Comparing `pydolarvenezuela-1.4.3.tar` & `pydolarvenezuela-1.4.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 23:19:00.245956 pydolarvenezuela-1.4.3/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.4.3/LICENSE
--rw-rw-rw-   0        0        0     7276 2024-04-25 23:19:00.229489 pydolarvenezuela-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     4885 2024-04-25 23:08:28.000000 pydolarvenezuela-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 23:18:59.946504 pydolarvenezuela-1.4.3/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2562 2024-04-25 21:35:52.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:18:59.979889 pydolarvenezuela-1.4.3/pyDolarVenezuela/assets/
--rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:18:59.979889 pydolarvenezuela-1.4.3/pyDolarVenezuela/assets/icons/
--rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/assets/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:18:59.996426 pydolarvenezuela-1.4.3/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      612 2024-04-25 22:15:03.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:19:00.013061 pydolarvenezuela-1.4.3/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      159 2024-04-25 21:35:09.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      802 2023-11-22 00:44:52.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      453 2023-11-23 16:38:28.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/network.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:19:00.196006 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     3516 2024-04-25 22:29:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2159 2024-04-02 19:39:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     2529 2024-04-02 19:27:15.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     1842 2024-04-02 19:27:50.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/dpedidos.py
--rw-rw-rw-   0        0        0     3002 2024-04-02 19:28:10.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     4136 2024-04-02 19:28:30.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/ivenezuela.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:19:00.213218 pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0     1201 2023-10-17 03:57:15.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:19:00.229489 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     7276 2024-04-25 23:18:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      909 2024-04-25 23:18:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 23:18:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-25 23:18:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-25 23:18:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-25 23:09:11.000000 pydolarvenezuela-1.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-25 23:19:00.245956 pydolarvenezuela-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-04-25 23:09:18.000000 pydolarvenezuela-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:38:40.388510 pydolarvenezuela-1.4.4/
+-rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0     7276 2024-04-25 23:38:40.376511 pydolarvenezuela-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4885 2024-04-25 23:08:28.000000 pydolarvenezuela-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 23:38:40.222529 pydolarvenezuela-1.4.4/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2589 2024-04-25 23:37:29.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:38:40.262379 pydolarvenezuela-1.4.4/pyDolarVenezuela/assets/
+-rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:38:40.266377 pydolarvenezuela-1.4.4/pyDolarVenezuela/assets/icons/
+-rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/assets/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:38:40.277194 pydolarvenezuela-1.4.4/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      612 2024-04-25 22:15:03.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:38:40.293249 pydolarvenezuela-1.4.4/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      159 2024-04-25 21:35:09.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      802 2023-11-22 00:44:52.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      453 2023-11-23 16:38:28.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/network.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:38:40.331336 pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     3516 2024-04-25 22:29:59.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2159 2024-04-02 19:39:59.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     2529 2024-04-02 19:27:15.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     1842 2024-04-02 19:27:50.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/dpedidos.py
+-rw-rw-rw-   0        0        0     3002 2024-04-02 19:28:10.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     4136 2024-04-02 19:28:30.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/ivenezuela.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:38:40.347338 pydolarvenezuela-1.4.4/pyDolarVenezuela/tools/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/tools/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/tools/calculator.py
+-rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/tools/time.py
+-rw-rw-rw-   0        0        0     1201 2023-10-17 03:57:15.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:38:40.353337 pydolarvenezuela-1.4.4/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0     7276 2024-04-25 23:38:39.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      909 2024-04-25 23:38:39.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 23:38:39.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-25 23:38:39.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-25 23:38:39.000000 pydolarvenezuela-1.4.4/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-25 23:38:04.000000 pydolarvenezuela-1.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 23:38:40.397513 pydolarvenezuela-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-04-25 23:38:07.000000 pydolarvenezuela-1.4.4/setup.py
```

### Comparing `pydolarvenezuela-1.4.3/LICENSE` & `pydolarvenezuela-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/PKG-INFO` & `pydolarvenezuela-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.4.3
+Version: 1.4.4
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.4.3/README.md` & `pydolarvenezuela-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 from typing import Literal
 from colorama import Fore
 
 from . import network
+from .models import pages
 from .models.pages import Monitor as Page
 from .data.redis import Redis
 from .tools import get_time_zone as getdate, currency_converter
 from .provider import select_monitor
 
-version = '1.4.2'
+version = '1.4.3'
 
 class CheckVersion:
     check = True
 
     @classmethod
     def _check_dependence_version(self):
             response = network.get("https://pypi.org/pypi/pydolarvenezuela/json")
```

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/assets/icons/__init__.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/assets/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/models/pages.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/models/pages.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/bcv.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/criptodolar.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/dpedidos.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/dpedidos.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/ivenezuela.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/provider/ivenezuela.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/calculator.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/time.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/tools/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela/utils.py` & `pydolarvenezuela-1.4.4/pyDolarVenezuela/utils.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.4.4/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.4.3
+Version: 1.4.4
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.4.4/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.3/pyproject.toml` & `pydolarvenezuela-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.4.3"
+version = "1.4.4"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.4.3/setup.py` & `pydolarvenezuela-1.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.4.3'
+VERSION = '1.4.4'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```

