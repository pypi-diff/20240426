# Comparing `tmp/felicien-0.3.0.tar.gz` & `tmp/felicien-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felicien-0.3.0.tar", max compression
+gzip compressed data, was "felicien-0.4.0.tar", max compression
```

## Comparing `felicien-0.3.0.tar` & `felicien-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2024-04-22 13:01:40.260774 felicien-0.3.0/LICENSE
--rw-r--r--   0        0        0     2558 2024-04-22 13:01:40.260774 felicien-0.3.0/README.md
--rw-r--r--   0        0        0      142 2024-04-22 13:01:40.265774 felicien-0.3.0/felicien/__init__.py
--rw-r--r--   0        0        0     6372 2024-04-22 13:01:40.265774 felicien-0.3.0/felicien/feliconnector.py
--rw-r--r--   0        0        0     9812 2024-04-22 13:01:40.266774 felicien-0.3.0/felicien/felits.py
--rw-r--r--   0        0        0      999 2024-04-22 13:01:40.266774 felicien-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 felicien-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-04-25 22:03:26.094113 felicien-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2558 2024-04-25 22:03:26.094113 felicien-0.4.0/README.md
+-rw-r--r--   0        0        0      142 2024-04-25 22:03:26.099113 felicien-0.4.0/felicien/__init__.py
+-rw-r--r--   0        0        0     6409 2024-04-25 22:03:26.099113 felicien-0.4.0/felicien/feliconnector.py
+-rw-r--r--   0        0        0    10153 2024-04-25 22:03:26.099113 felicien-0.4.0/felicien/felits.py
+-rw-r--r--   0        0        0      999 2024-04-25 22:03:26.100113 felicien-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 felicien-0.4.0/PKG-INFO
```

### Comparing `felicien-0.3.0/LICENSE` & `felicien-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `felicien-0.3.0/README.md` & `felicien-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `felicien-0.3.0/felicien/feliconnector.py` & `felicien-0.4.0/felicien/feliconnector.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import requests
 from felicien.felits import FeliTS
 
 REQUESTS_OPTIONS = {
     "auth": (tuple, HTTPBasicAuth),
     "verify": (bool, str),
     "cert": (tuple, str),
+    "headers": (dict),
 }
 TSDB_TYPES = ["prometheus", "victoriametrics"]
 API_TSDB_HEALTH = {
     "prometheus": "api/v1/status/tsdb",
     "victoriametrics": "api/v1/status/tsdb",
 }
 API_TSDB_QUERY = {
@@ -57,15 +58,15 @@
         Args:
             url (str, optional): Base URL of the TSDB.
                 Defaults to None.
             tsdb (str, optional): Type of TSDB. Can be "prometheus",
                 "victoriametrics".
                 Defaults to "prometheus"
             options (dict, optional): Options to use with requests, such as
-                auth, TLS verification, client certificate, ...
+                auth, TLS verification, client certificate, headers...
 
         Raises:
             ValueError if the url is not valid
 
             ValueError if tsdb is not a valid type
 
             ConnectionError if TSDB API is not reachable
@@ -196,13 +197,13 @@
         payload = ts.as_prometheus()
 
         r = requests.post(
             url=f"{self.base_url}/{API_TSDB_IMPORT[self.tsdb]}",
             data=payload,
             **self._options,  # type: ignore
         )
-        if not r.status_code == 200:
+        if r.status_code not in [200, 204]:
             raise ConnectionError(
                 f"unable to import timeserie: {r.status_code}"
             )
 
         return True
```

### Comparing `felicien-0.3.0/felicien/felits.py` & `felicien-0.4.0/felicien/felits.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
 
 import pandas as pd
 import datetime as dt
 import matplotlib.pyplot as plt
+import json
+
+
+# Smallest frequency should be seen at least 10% of the Serie to be considered
+# as the Serie frequency
+MIN_FREQUENCY_REPRESENTATION = 0.1
 
 
 class FeliTS:
     """A Timeserie of a Prometheus metric
 
     This is a metric representation as returned by the Prometheus API. It
     includes the metric definition, and the data as a pandas Series.
@@ -154,35 +160,40 @@
             self.data.index.floor("s").diff().value_counts()  # type: ignore
         )
 
         if frequencies.size == 1:
             # only one frequency: return it
             return frequencies.idxmax()
         elif frequencies.size > 1:
-            # multiple frequencies: return the most occuring (if several values
-            # are the most occuring, returning the smallest)
-            return frequencies[frequencies == frequencies.max()].idxmin()
+            # multiple frequencies: return the lowest one that is occuring
+            # more than 10% of the time
+            for i in range(frequencies.size):
+                if (frequencies / self.data.size).sort_index().iloc[
+                    i
+                ] > MIN_FREQUENCY_REPRESENTATION:
+                    return frequencies[i:].idxmax()
 
         # all other cases seem wrong
         return dt.timedelta()
 
     @property
     def size(self) -> int:
         """Expose the size to the timeseries
 
         Returns:
             int: Size of the timeseries
         """
         return self.data.size
 
-    def as_prometheus(self) -> dict:
+    def as_prometheus(self) -> str:
         """Object representation based on Prometheus API format
 
         Returns:
-            dict: The object, as you could push it to Prometheus
+            str: JSON representation of the object, as you could push it
+                to Prometheus
         """
         result = dict()
 
         result["metric"] = {"__name__": self.name}
 
         for k, v in self.labels.items():
             result["metric"][k] = v
@@ -192,15 +203,15 @@
             (pd.Series(data=self.data.index) - dt.datetime(1970, 1, 1))
             .dt.total_seconds()
             .apply(lambda x: x * 1000)
             .astype(int)
             .to_list()
         )
 
-        return result
+        return json.dumps(result)
 
     def as_dataframe(self, name: str = "") -> pd.DataFrame:
         """self.data representation as a pandas.DataFrame
 
         Args:
             name (str, optional): Name of the column for the Serie in the
                 resulting DataFrame. Defaults to self.name.
```

### Comparing `felicien-0.3.0/pyproject.toml` & `felicien-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "felicien"
-version = "0.3.0"
+version = "0.4.0"
 description = "Felicien is you companion to retrieve timeseries from a TSDB, to transform it in various format and to push it to a TSDB."
 authors = ["Julien Andrieux <chilladx@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "felicien" },
 ]
```

### Comparing `felicien-0.3.0/PKG-INFO` & `felicien-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felicien
-Version: 0.3.0
+Version: 0.4.0
 Summary: Felicien is you companion to retrieve timeseries from a TSDB, to transform it in various format and to push it to a TSDB.
 License: MIT
 Author: Julien Andrieux
 Author-email: chilladx@pm.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

