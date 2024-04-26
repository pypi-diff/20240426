# Comparing `tmp/rws-ddlpy-0.4.0.tar.gz` & `tmp/rws_ddlpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rws-ddlpy-0.4.0.tar", last modified: Mon Apr  8 15:52:10 2024, max compression
+gzip compressed data, was "rws_ddlpy-0.5.0.tar", last modified: Fri Apr 26 12:00:01 2024, max compression
```

## Comparing `rws-ddlpy-0.4.0.tar` & `rws_ddlpy-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:52:10.412506 rws-ddlpy-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35598 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-08 15:52:10.412506 rws-ddlpy-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:52:10.408506 rws-ddlpy-0.4.0/ddlpy/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/ddlpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/ddlpy/waterinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:52:10.408506 rws-ddlpy-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     5676 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:52:10.408506 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 15:52:10.000000 rws-ddlpy-0.4.0/rws_ddlpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:52:10.412506 rws-ddlpy-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:52:10.408506 rws-ddlpy-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    94497 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/20200608_069_20200507.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17635 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/NVT_WATHTE_SCHE_20200507.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/bulk.json
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/test_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8712 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/test_ddlpy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2230 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/test_endpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1198 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-08 15:51:47.000000 rws-ddlpy-0.4.0/tests/test_waterinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:00:01.450043 rws_ddlpy-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35598 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-26 12:00:01.450043 rws_ddlpy-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:00:01.442043 rws_ddlpy-0.5.0/ddlpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/ddlpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/ddlpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14990 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/ddlpy/ddlpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/ddlpy/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/ddlpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/ddlpy/waterinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:00:01.446043 rws_ddlpy-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5676 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:00:01.446043 rws_ddlpy-0.5.0/rws_ddlpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-26 12:00:01.000000 rws_ddlpy-0.5.0/rws_ddlpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-26 12:00:01.000000 rws_ddlpy-0.5.0/rws_ddlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:00:01.000000 rws_ddlpy-0.5.0/rws_ddlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-26 12:00:01.000000 rws_ddlpy-0.5.0/rws_ddlpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-26 12:00:01.000000 rws_ddlpy-0.5.0/rws_ddlpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 12:00:01.000000 rws_ddlpy-0.5.0/rws_ddlpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 12:00:01.450043 rws_ddlpy-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:00:01.446043 rws_ddlpy-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    94497 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/tests/20200608_069_20200507.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17635 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/tests/NVT_WATHTE_SCHE_20200507.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/tests/bulk.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/tests/test_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12261 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/tests/test_ddlpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2230 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/tests/test_endpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1198 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-26 11:59:39.000000 rws_ddlpy-0.5.0/tests/test_waterinfo.py
```

### Comparing `rws-ddlpy-0.4.0/CONTRIBUTING.rst` & `rws_ddlpy-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/HISTORY.rst` & `rws_ddlpy-0.5.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 =======
 History
 =======
 
+0.5.0 (2024-04-26)
+------------------
+* avoid duplicated periods in dataframe returned by `ddlpy.measurements_amount()` in https://github.com/Deltares/ddlpy/pull/93
+* allow for different retrieval frequencies (including None) in `ddlpy.measurements()` in https://github.com/Deltares/ddlpy/pull/95
+* only catch "Geen gegevens gevonden!" error message and raise all others (for instance for a too large request) in https://github.com/Deltares/ddlpy/pull/97
+* support for timezones in start_date/end_date in https://github.com/Deltares/ddlpy/pull/98
+
 0.4.0 (2024-04-08)
 ------------------
 * added `catalog_filter` argument to `ddlpy.locations()` to enabling retrieving the extended catalog in https://github.com/Deltares/ddlpy/pull/87
 * pass all Code parameters to measurements request instead of only four in https://github.com/Deltares/ddlpy/pull/88
-* added ddlpy.dataframe_to_xarray()` function in https://github.com/Deltares/ddlpy/pull/86
+* added `ddlpy.dataframe_to_xarray()` function in https://github.com/Deltares/ddlpy/pull/86
 
 0.3.0 (2024-03-13)
 ------------------
 * improved nan filtering of measurements in https://github.com/deltares/ddlpy/pull/30
 * add `ddlpy.measurements_available()` check in https://github.com/deltares/ddlpy/pull/33 and https://github.com/deltares/ddlpy/pull/58
 * add `ddlpy.measurements_latest()` to retrieve latest measurements in https://github.com/deltares/ddlpy/pull/35
 * add optional time-sorting of returned measurements dataframe and made drop_duplicates optional in https://github.com/deltares/ddlpy/pull/37
```

### Comparing `rws-ddlpy-0.4.0/LICENSE` & `rws_ddlpy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/PKG-INFO` & `rws_ddlpy-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rws-ddlpy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Service from Rijkswaterstaat for distributing water quantity data.
 Maintainer-email: Fedor Baart <fedor.baart@deltares.nl>, Jelmer Veenstra <jelmer.veenstra@deltares.nl>
 License: GPLv3
 Project-URL: Home, https://github.com/deltares/ddlpy
 Project-URL: Code, https://github.com/deltares/ddlpy
 Project-URL: Issues, https://github.com/deltares/ddlpy/issues
 Keywords: ddlpy
```

### Comparing `rws-ddlpy-0.4.0/README.md` & `rws_ddlpy-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/ddlpy/__init__.py` & `rws_ddlpy-0.5.0/ddlpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for Data Distributie Laag. Service from Rijkswaterstaat for distributing water quantity data.."""
 
 __author__ = """Fedor Baart"""
 __email__ = 'fedor.baart@deltares.nl'
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 
 from ddlpy.ddlpy import locations
 from ddlpy.ddlpy import (measurements, 
                          measurements_latest, 
                          measurements_available, 
                          measurements_amount,
                          )
```

### Comparing `rws-ddlpy-0.4.0/ddlpy/cli.py` & `rws_ddlpy-0.5.0/ddlpy/cli.py`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/ddlpy/ddlpy.py` & `rws_ddlpy-0.5.0/ddlpy/ddlpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,43 +17,63 @@
 BASE_URL = "https://waterwebservices.rijkswaterstaat.nl/"
 ENDPOINTS_PATH = pathlib.Path(__file__).with_name("endpoints.json")
 
 with ENDPOINTS_PATH.open() as f:
     ENDPOINTS = json.load(f)
 
 
-class NoDataException(ValueError):
+class NoDataError(ValueError):
+    pass
+
+
+class UnsuccessfulRequestError(ValueError):
     pass
 
 
 # Web Feature Service
 # Web Mapping Service
 logger = logging.getLogger(__name__)
 
 
+def _send_post_request(url, request, timeout=None):
+    logger.debug("Requesting at {} with request: {}".format(url, json.dumps(request)))
+    resp = requests.post(url, json=request, timeout=timeout)
+    if not resp.ok:
+        raise IOError("Request failed: {}".format(resp.text))
+    
+    result = resp.json()
+    if not result['Succesvol']:
+        logger.debug('Response result is unsuccessful: {}'.format(result))
+        error_message = result.get('Foutmelding', 'No error returned')
+        if error_message == "Geen gegevens gevonden!":
+            # Foutmelding: "Geen gegevens gevonden!"
+            # this is a valid response for periods where there is no data
+            # this error is raised here, but catched in ddlpy.ddlpy.measurements() so the process can continue.
+            raise NoDataError(error_message)
+        else:
+            # Foutmelding: "Het max aantal waarnemingen (157681) is overschreven, beperk uw request."
+            # or any other possible error message are raised here
+            raise UnsuccessfulRequestError(error_message)
+    
+    # continue if request was successful
+    return result
+
+
 def catalog(catalog_filter=None):
     endpoint = ENDPOINTS["collect_catalogue"]
     
     if catalog_filter is None:
         # use the default request from endpoints.json
-        catalog_request = endpoint["request"]
+        request = endpoint["request"]
     else:
         assert isinstance(catalog_filter, list)
-        catalog_request = {"CatalogusFilter": {x:True for x in catalog_filter}}
+        request = {"CatalogusFilter": {x:True for x in catalog_filter}}
+    
+    result = _send_post_request(endpoint["url"], request, timeout=None)
     
-    msg = "{} with {}".format(endpoint["url"], json.dumps(catalog_request))
-    logger.debug("requesting: {}".format(msg))
-
-    resp = requests.post(endpoint["url"], json=catalog_request)
-    if not resp.ok:
-        raise IOError("Failed to request {}: {}".format(msg, resp.text))
-    result = resp.json()
-    if not result["Succesvol"]:
-        logger.exception(str(result))
-        raise ValueError(result.get("Foutmelding", "No error returned"))
     return result
 
 
 def locations(catalog_filter=None):
     """
     get station information from DDL (metadata from Catalogue). All metadata regarding stations.
     The response (result) retrieves more keys
@@ -80,20 +100,29 @@
     return merged.set_index("Code")
 
 
 def _check_convert_dates(start_date, end_date, return_str=True):
     start_date = pd.Timestamp(start_date)
     end_date = pd.Timestamp(end_date)
     
+    # check if timezones are the same
+    assert start_date.tz == end_date.tz
+    
+    # set UTC timezone if tz is None
+    if start_date.tz is None:
+        start_date = pytz.UTC.localize(start_date)
+    if end_date.tz is None:
+        end_date = pytz.UTC.localize(end_date)
+    
     if start_date > end_date:
-        raise ValueError("start_date is larger than end_date")
+        raise ValueError(f"start_date {start_date} is larger than end_date {end_date}")
     
     if return_str:
-        start_date_str = pytz.UTC.localize(start_date).isoformat(timespec='milliseconds')
-        end_date_str = pytz.UTC.localize(end_date).isoformat(timespec='milliseconds')
+        start_date_str = start_date.isoformat(timespec='milliseconds')
+        end_date_str = end_date.isoformat(timespec='milliseconds')
         return start_date_str, end_date_str
     else:
         return start_date, end_date
 
 
 def _get_request_dicts(location):
     
@@ -131,30 +160,22 @@
         "LocatieLijst": [request_dicts["Locatie"]],
         "Periode": {
             "Begindatumtijd": start_date_str,
             "Einddatumtijd": end_date_str
         }
     }
 
-    try:
-        logger.debug('requesting:  {}'.format(request))
-        resp = requests.post(endpoint['url'], json=request, timeout=5)
-        result = resp.json()
-        if not result['Succesvol']:
-            logger.debug('Got  invalid response: {}'.format(result))
-            raise NoDataException(result.get('Foutmelding', 'No error returned'))
-    except NoDataException as e:
-        logger.debug('No data availble for {} {}'.format(start_date, end_date))
-        raise e
-
-    if result['Succesvol']:
-        if result['WaarnemingenAanwezig'] == 'true' :
-            return True
-        else:
-            return False  
+    result = _send_post_request(endpoint["url"], request, timeout=5)
+    
+    # continue if request was successful
+    logger.debug('Got response: {}'.format(result))
+    if result['WaarnemingenAanwezig'] == 'true' :
+        return True
+    else:
+        return False  
 
 
 def measurements_amount(location, start_date, end_date, period="Jaar"):
     """checks how much measurements are available for a location, for the period start_date, end_date
     returns a DataFrame with columns Groeperingsperiode and AantalMetingen
     possible for Jaar/Maand/Dag
     """
@@ -175,45 +196,38 @@
         "Groeperingsperiode": period,
         "Periode": {
             "Begindatumtijd": start_date_str,
             "Einddatumtijd": end_date_str
         }
     }
 
-    try:
-        logger.debug('requesting:  {}'.format(request))
-        resp = requests.post(endpoint['url'], json=request)
-        result = resp.json()
-        if not result['Succesvol']:
-            logger.debug('Got  invalid response: {}'.format(result))
-            raise NoDataException(result.get('Foutmelding', 'No error returned'))
-    except NoDataException as e:
-        logger.debug('No data availble for {} {}'.format(start_date, end_date))
-        raise e
-
-    if result['Succesvol']:
-        df_list = []
-        for one in result['AantalWaarnemingenPerPeriodeLijst']:
-            df = pd.json_normalize(one['AantalMetingenPerPeriodeLijst'])
-            
-            # combine columns to a period string
-            df["Groeperingsperiode"] = df["Groeperingsperiode.Jaarnummer"].apply(lambda x: f"{x:04d}")
-            if period in ["Maand", "Dag"]:
-                df["Groeperingsperiode"] = (df["Groeperingsperiode"] + "-" + 
-                                            df["Groeperingsperiode.Maandnummer"].apply(lambda x: f"{x:02d}"))
-            if period in ["Dag"]:
-                df["Groeperingsperiode"] = (df["Groeperingsperiode"] + "-" + 
-                                            df["Groeperingsperiode.Dag"].apply(lambda x: f"{x:02d}"))
-            
-            # select columns from dataframe and append to list
-            df = df[["Groeperingsperiode","AantalMetingen"]]
-            df_list.append(df)
+    result = _send_post_request(endpoint["url"], request, timeout=None)
+
+    # continue if request was successful
+    df_list = []
+    for one in result['AantalWaarnemingenPerPeriodeLijst']:
+        df = pd.json_normalize(one['AantalMetingenPerPeriodeLijst'])
+        
+        # combine columns to a period string
+        df["Groeperingsperiode"] = df["Groeperingsperiode.Jaarnummer"].apply(lambda x: f"{x:04d}")
+        if period in ["Maand", "Dag"]:
+            df["Groeperingsperiode"] = (df["Groeperingsperiode"] + "-" + 
+                                        df["Groeperingsperiode.Maandnummer"].apply(lambda x: f"{x:02d}"))
+        if period in ["Dag"]:
+            df["Groeperingsperiode"] = (df["Groeperingsperiode"] + "-" + 
+                                        df["Groeperingsperiode.Dag"].apply(lambda x: f"{x:02d}"))
         
-        # concatenate
-        amount_all = pd.concat(df_list).sort_values("Groeperingsperiode").reset_index(drop=True)
+        # select columns from dataframe and append to list
+        df = df.set_index("Groeperingsperiode")
+        df = df[["AantalMetingen"]]
+        df_list.append(df)
+        
+        # concatenate and sum duplicated index
+        amount_all = pd.concat(df_list).sort_index()
+        amount_all = amount_all.groupby(amount_all.index).sum()
         return amount_all
 
 
 def _combine_waarnemingenlijst(result, location):
     assert "WaarnemingenLijst" in result
     
     # flatten the datastructure
@@ -292,46 +306,59 @@
             "AquoMetadata": request_dicts["AquoMetadata"]
             },
         "Locatie": request_dicts["Locatie"],
         "Periode": {"Begindatumtijd": start_date_str, 
                     "Einddatumtijd": end_date_str},
     }
 
-    try:
-        logger.debug("requesting:  {}".format(request))
-        resp = requests.post(endpoint["url"], json=request)
-        result = resp.json()
-        if not result["Succesvol"]:
-            logger.debug("Got  invalid response: {}".format(result))
-            raise NoDataException(result.get("Foutmelding", "No error returned"))
-    except NoDataException as e:
-        logger.debug("No data availble for {} {}".format(start_date, end_date))
-        raise e
-    
+    result = _send_post_request(endpoint["url"], request, timeout=None)
+
     df = _combine_waarnemingenlijst(result, location)
     return df
 
 
 def _clean_dataframe(measurements):
     len_raw = len(measurements)
     # drop duplicate rows (preserves e.g. different Grootheden/Groeperingen at same timestep)
     measurements = measurements.drop_duplicates()
     
-    # remove Tijdstap column, has to be done after drop_duplicates to avoid too much to be dropped
+    # remove Tijdstip column, has to be done after drop_duplicates to avoid too much to be dropped
     measurements = measurements.drop("Tijdstip", axis=1, errors='ignore')
     
     # sort dataframe on time, ddl returns non-sorted data
     measurements = measurements.sort_index()
     ndropped = len_raw - len(measurements)
     logger.debug(f"{ndropped} duplicated values dropped")
     return measurements
 
 
-def measurements(location, start_date, end_date, clean_df=True):
-    """return measurements for the given location and time window (start_date, end_date)"""
+def measurements(location, start_date, end_date, freq=dateutil.rrule.MONTHLY, clean_df=True):
+    """
+    Return measurements for the given location and time window (start_date, end_date)
+
+    Parameters
+    ----------
+    location : pd.Series
+        Single row of the `ddlpy.locations()` DataFrame.
+    start_date : str, dt.datetime, pd.Timestamp
+        Start of the retrieval period.
+    end_date : str, dt.datetime, pd.Timestamp
+        End of the retrieval period.
+    freq : None, dateutil.rrule.MONTHLY, dateutil.rrule.YEARLY, etc., optional
+        The frequency in which to divide the requested period (e.g. yearly or monthly).
+        Can also be None, in which case the entire dataset will be retrieved at once.
+        Please note that 10-minute measurements can often not be downloaded in yearly (or larger) chunks 
+        since the DDL limits the responses to 157681 values and several stations have duplicated timesteps.
+        In that case the query will fail with an error or timeout or just return an empty result (as if there was no data).
+        In that case, the user should fallback to monthly chunks.
+        This is significantly slower but it is also much more robust. The default is dateutil.rrule.MONTHLY.
+    clean_df : bool, optional
+        Whether to sort the dataframe and remove duplicate rows. The default is True.
+    
+    """
     
     if isinstance(location, pd.DataFrame):
         raise TypeError("The provided location is a pandas.DataFrame, but should be a pandas.Series, "
                         "supply only one location/row instead, for instance by doing 'location.iloc[0]'")
     
     start_date, end_date = _check_convert_dates(start_date, end_date, return_str=False)
     
@@ -340,41 +367,40 @@
     # data_present = measurements_available(
     #         location, start_date=start_date, end_date=end_date)
     # if not data_present:
     #     # early return in case of no data
     #     logger.debug("no data found for this station and time extent")
     #     return
     
-    for (start_date_i, end_date_i) in tqdm.tqdm(
-        date_series(start_date, end_date, freq=dateutil.rrule.MONTHLY)
-    ):
-        """return measurements for station given by locations record \"location\", from start_date through end_date
-        IMPORTANT: measurements made every 10 minutes will not be downoladed if freq= YEAR.
-        For instance if many duplicate timesteps are present, it will fail or timeout.
-        Therefore, Please DO NOT CHANGE THE FREQUENCY TO YEAR. KEEP IT MONTHLY NO MATTER HOW SLOW THE CODE CAN BE!
-        """
-
+    if freq is None:
+        date_series_iterator = tqdm.tqdm([(start_date, end_date)])
+    else:
+        date_series_iterator = tqdm.tqdm(
+            date_series(start_date, end_date, freq=freq)
+        )
+    
+    for (start_date_i, end_date_i) in date_series_iterator:
         try:
             measurement = _measurements_slice(
                 location, start_date=start_date_i, end_date=end_date_i
             )
             measurements.append(measurement)
-        except NoDataException:
+        except NoDataError:
             continue
 
     if len(measurements) == 0:
         # return empty dataframe in case of no data
         logger.debug("no data found for this station and time extent")
         return pd.DataFrame()
     
     measurements = pd.concat(measurements)
 
     if clean_df:
         measurements = _clean_dataframe(measurements)
-
+    
     return measurements
 
 
 def measurements_latest(location):
     """checks if there are measurements for location, for the period start_date, end_date
     gives None if check was unsuccesfull
     gives True/False if there are / are no measurement available
@@ -383,21 +409,12 @@
 
     request_dicts = _get_request_dicts(location)
     
     request = {"AquoPlusWaarnemingMetadataLijst":[{"AquoMetadata":request_dicts["AquoMetadata"]}],
                "LocatieLijst":[request_dicts["Locatie"]]
                }
 
-    try:
-        logger.debug('requesting:  {}'.format(request))
-        resp = requests.post(endpoint['url'], json=request, timeout=5)
-        result = resp.json()
-        if not result['Succesvol']:
-            logger.debug('Got  invalid response: {}'.format(result))
-            raise NoDataException(result.get('Foutmelding', 'No error returned'))
-    except NoDataException as e:
-        logger.debug('No data availble')
-        raise e
-
-    if result['Succesvol']:
-        df = _combine_waarnemingenlijst(result, location)
-        return df
+    result = _send_post_request(endpoint["url"], request, timeout=5)
+    
+    # continue if request was successful
+    df = _combine_waarnemingenlijst(result, location)
+    return df
```

### Comparing `rws-ddlpy-0.4.0/ddlpy/endpoints.json` & `rws_ddlpy-0.5.0/ddlpy/endpoints.json`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/ddlpy/utils.py` & `rws_ddlpy-0.5.0/ddlpy/utils.py`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/ddlpy/waterinfo.py` & `rws_ddlpy-0.5.0/ddlpy/waterinfo.py`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/docs/Makefile` & `rws_ddlpy-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/docs/conf.py` & `rws_ddlpy-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/docs/make.bat` & `rws_ddlpy-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/pyproject.toml` & `rws_ddlpy-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rws-ddlpy"
-version = "0.4.0"
+version = "0.5.0"
 maintainers = [
 	{ name = "Fedor Baart", email = "fedor.baart@deltares.nl"},
 	{ name = "Jelmer Veenstra", email = "jelmer.veenstra@deltares.nl"},
 ]
 description = "Service from Rijkswaterstaat for distributing water quantity data."
 readme = "README.md"
 keywords = ["ddlpy"]
```

### Comparing `rws-ddlpy-0.4.0/rws_ddlpy.egg-info/PKG-INFO` & `rws_ddlpy-0.5.0/rws_ddlpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rws-ddlpy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Service from Rijkswaterstaat for distributing water quantity data.
 Maintainer-email: Fedor Baart <fedor.baart@deltares.nl>, Jelmer Veenstra <jelmer.veenstra@deltares.nl>
 License: GPLv3
 Project-URL: Home, https://github.com/deltares/ddlpy
 Project-URL: Code, https://github.com/deltares/ddlpy
 Project-URL: Issues, https://github.com/deltares/ddlpy/issues
 Keywords: ddlpy
```

### Comparing `rws-ddlpy-0.4.0/rws_ddlpy.egg-info/SOURCES.txt` & `rws_ddlpy-0.5.0/rws_ddlpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/tests/20200608_069_20200507.csv` & `rws_ddlpy-0.5.0/tests/20200608_069_20200507.csv`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/tests/NVT_WATHTE_SCHE_20200507.csv` & `rws_ddlpy-0.5.0/tests/NVT_WATHTE_SCHE_20200507.csv`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/tests/bulk.json` & `rws_ddlpy-0.5.0/tests/bulk.json`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/tests/test_cli.py` & `rws_ddlpy-0.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/tests/test_endpoints.py` & `rws_ddlpy-0.5.0/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/tests/test_utils.py` & `rws_ddlpy-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rws-ddlpy-0.4.0/tests/test_waterinfo.py` & `rws_ddlpy-0.5.0/tests/test_waterinfo.py`

 * *Files identical despite different names*

