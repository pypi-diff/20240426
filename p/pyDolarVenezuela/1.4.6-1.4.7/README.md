# Comparing `tmp/pydolarvenezuela-1.4.6.tar.gz` & `tmp/pydolarvenezuela-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.4.6.tar", last modified: Thu Apr 25 23:49:42 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.4.7.tar", last modified: Fri Apr 26 00:29:48 2024, max compression
```

## Comparing `pydolarvenezuela-1.4.6.tar` & `pydolarvenezuela-1.4.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 23:49:42.496463 pydolarvenezuela-1.4.6/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.4.6/LICENSE
--rw-rw-rw-   0        0        0     7276 2024-04-25 23:49:42.490462 pydolarvenezuela-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     4885 2024-04-25 23:08:28.000000 pydolarvenezuela-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 23:49:42.396596 pydolarvenezuela-1.4.6/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2562 2024-04-25 23:48:34.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:49:42.421232 pydolarvenezuela-1.4.6/pyDolarVenezuela/assets/
--rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:49:42.424332 pydolarvenezuela-1.4.6/pyDolarVenezuela/assets/icons/
--rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/assets/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:49:42.433336 pydolarvenezuela-1.4.6/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      612 2024-04-25 22:15:03.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:49:42.443627 pydolarvenezuela-1.4.6/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      159 2024-04-25 21:35:09.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      119 2024-04-25 23:42:45.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      453 2023-11-23 16:38:28.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      716 2024-04-25 23:43:03.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:49:42.469798 pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     3509 2024-04-25 23:46:28.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2159 2024-04-02 19:39:59.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     2529 2024-04-02 19:27:15.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     1842 2024-04-02 19:27:50.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/dpedidos.py
--rw-rw-rw-   0        0        0     3002 2024-04-02 19:28:10.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     4136 2024-04-02 19:28:30.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/ivenezuela.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:49:42.483462 pydolarvenezuela-1.4.6/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0     1201 2023-10-17 03:57:15.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:49:42.487463 pydolarvenezuela-1.4.6/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     7276 2024-04-25 23:49:42.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      935 2024-04-25 23:49:42.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 23:49:42.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-25 23:49:42.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-25 23:49:42.000000 pydolarvenezuela-1.4.6/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-25 23:48:40.000000 pydolarvenezuela-1.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-25 23:49:42.497462 pydolarvenezuela-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-04-25 23:48:44.000000 pydolarvenezuela-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:29:48.104844 pydolarvenezuela-1.4.7/
+-rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.4.7/LICENSE
+-rw-rw-rw-   0        0        0     7276 2024-04-26 00:29:48.092364 pydolarvenezuela-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4885 2024-04-25 23:08:28.000000 pydolarvenezuela-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 00:29:47.952560 pydolarvenezuela-1.4.7/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2562 2024-04-26 00:28:57.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:29:47.985792 pydolarvenezuela-1.4.7/pyDolarVenezuela/assets/
+-rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:29:48.002384 pydolarvenezuela-1.4.7/pyDolarVenezuela/assets/icons/
+-rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/assets/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:29:48.002384 pydolarvenezuela-1.4.7/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      612 2024-04-25 22:15:03.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:29:48.019573 pydolarvenezuela-1.4.7/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      159 2024-04-25 21:35:09.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      119 2024-04-25 23:42:45.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      453 2023-11-23 16:38:28.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      716 2024-04-25 23:43:03.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:29:48.053857 pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     3543 2024-04-26 00:28:13.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2159 2024-04-02 19:39:59.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     2529 2024-04-02 19:27:15.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     1842 2024-04-02 19:27:50.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/dpedidos.py
+-rw-rw-rw-   0        0        0     3002 2024-04-02 19:28:10.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     4136 2024-04-02 19:28:30.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/ivenezuela.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:29:48.075666 pydolarvenezuela-1.4.7/pyDolarVenezuela/tools/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/tools/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/tools/calculator.py
+-rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/tools/time.py
+-rw-rw-rw-   0        0        0     1201 2023-10-17 03:57:15.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:29:48.088216 pydolarvenezuela-1.4.7/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0     7276 2024-04-26 00:29:47.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2024-04-26 00:29:47.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 00:29:47.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-26 00:29:47.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-26 00:29:47.000000 pydolarvenezuela-1.4.7/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-26 00:28:51.000000 pydolarvenezuela-1.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 00:29:48.105843 pydolarvenezuela-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-04-26 00:28:48.000000 pydolarvenezuela-1.4.7/setup.py
```

### Comparing `pydolarvenezuela-1.4.6/LICENSE` & `pydolarvenezuela-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/PKG-INFO` & `pydolarvenezuela-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.4.6
+Version: 1.4.7
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.4.6/README.md` & `pydolarvenezuela-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from . import network
 from .models.pages import Monitor as Page
 from .data.redis import Redis
 from .tools import get_time_zone as getdate, currency_converter
 from .provider import select_monitor
 
-version = '1.4.6'
+version = '1.4.7'
 
 class CheckVersion:
     check = True
 
     @classmethod
     def _check_dependence_version(self):
             response = network.get("https://pypi.org/pypi/pydolarvenezuela/json")
```

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/assets/icons/__init__.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/assets/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/pages.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,16 +46,16 @@
                 if not cache.get_data(key):
                     cache.set_data(key, json.dumps(response), db.ttl)
                 
                 get_data = dict(json.loads(cache.get_data(key)))
                 for name in get_data:
                     if not name == 'last_update':
                         price   = get_data[name]['price']
-                        change  = price - response[name]['price']
-                        percent = f'{(change / price) * 100 if price != 0 else 0}%'
+                        change  = round(float(price - response[name]['price']), 2)
+                        percent = f'{round(float((change / price) * 100 if price != 0 else 0), 2)}%'
                         symbol  = "" if change == 0 else "▲" if change >= 0 else "▼"
                         color   = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
                         
                         get_data[name].update({
                             'price': price,
                             'change': change,
                             'percent': percent,
```

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/bcv.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/criptodolar.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/dpedidos.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/dpedidos.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/provider/ivenezuela.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/provider/ivenezuela.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/tools/calculator.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/tools/time.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/tools/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela/utils.py` & `pydolarvenezuela-1.4.7/pyDolarVenezuela/utils.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.4.7/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.4.6
+Version: 1.4.7
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.4.6/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.4.7/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.4.6/pyproject.toml` & `pydolarvenezuela-1.4.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.4.6"
+version = "1.4.7"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.4.6/setup.py` & `pydolarvenezuela-1.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.4.6'
+VERSION = '1.4.7'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```

