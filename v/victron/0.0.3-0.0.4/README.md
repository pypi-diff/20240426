# Comparing `tmp/victron-0.0.3.tar.gz` & `tmp/victron-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "victron-0.0.3.tar", last modified: Tue Apr 23 20:55:28 2024, max compression
+gzip compressed data, was "victron-0.0.4.tar", last modified: Fri Apr 26 15:16:04 2024, max compression
```

## Comparing `victron-0.0.3.tar` & `victron-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:55:28.347638 victron-0.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-23 20:55:22.000000 victron-0.0.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-23 20:55:22.000000 victron-0.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1755 2024-04-23 20:55:28.347638 victron-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1548 2024-04-23 20:55:22.000000 victron-0.0.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-23 20:55:28.348638 victron-0.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-23 20:55:22.000000 victron-0.0.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-04-23 20:55:22.000000 victron-0.0.3/versioneer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:55:28.346638 victron-0.0.3/victron/
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-23 20:55:22.000000 victron-0.0.3/victron/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-23 20:55:28.348638 victron-0.0.3/victron/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-04-23 20:55:22.000000 victron-0.0.3/victron/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-04-23 20:55:22.000000 victron-0.0.3/victron/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8112 2024-04-23 20:55:22.000000 victron-0.0.3/victron/victron.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:55:28.347638 victron-0.0.3/victron.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1755 2024-04-23 20:55:28.000000 victron-0.0.3/victron.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2024-04-23 20:55:28.000000 victron-0.0.3/victron.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 20:55:28.000000 victron-0.0.3/victron.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-23 20:55:28.000000 victron-0.0.3/victron.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-23 20:55:28.000000 victron-0.0.3/victron.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:16:04.421235 victron-0.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-26 15:15:58.000000 victron-0.0.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-26 15:15:58.000000 victron-0.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-04-26 15:16:04.421235 victron-0.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2024-04-26 15:15:58.000000 victron-0.0.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-26 15:16:04.421235 victron-0.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-26 15:15:58.000000 victron-0.0.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-04-26 15:15:58.000000 victron-0.0.4/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:16:04.420235 victron-0.0.4/victron/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-26 15:15:58.000000 victron-0.0.4/victron/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-26 15:16:04.422235 victron-0.0.4/victron/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-04-26 15:15:58.000000 victron-0.0.4/victron/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-04-26 15:15:58.000000 victron-0.0.4/victron/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8192 2024-04-26 15:15:58.000000 victron-0.0.4/victron/victron.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:16:04.421235 victron-0.0.4/victron.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-04-26 15:16:04.000000 victron-0.0.4/victron.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2024-04-26 15:16:04.000000 victron-0.0.4/victron.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 15:16:04.000000 victron-0.0.4/victron.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-26 15:16:04.000000 victron-0.0.4/victron.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-26 15:16:04.000000 victron-0.0.4/victron.egg-info/top_level.txt
```

### Comparing `victron-0.0.3/LICENSE` & `victron-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `victron-0.0.3/PKG-INFO` & `victron-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: victron
-Version: 0.0.3
+Version: 0.0.4
 Summary: An SDK for Victron via Modbus TCP
 Home-page: https://gitlab.com/jfk344/python-victron-sdk
 Author: @jfk344
 Author-email: info@jfk-enterprise.com
 License: mit
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `victron-0.0.3/README.md` & `victron-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `victron-0.0.3/setup.cfg` & `victron-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `victron-0.0.3/versioneer.py` & `victron-0.0.4/versioneer.py`

 * *Files identical despite different names*

### Comparing `victron-0.0.3/victron/victron.py` & `victron-0.0.4/victron/victron.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from loguru import logger as log
 
 from . import constants as c
 from . import exceptions as vException
 from .exceptions import VictronException
 
 class Victron():
-    def __init__(self, host:str, port:int=502, unit_id:int=100, config:dict={}) -> None:
+    def __init__(self, host:str, port:int=502, unit_id:int=100, config:dict={}, timeout:int=10) -> None:
         self.host = host
         self.port = port
         self.unit_id = unit_id
+        self.timeout = timeout
         self.client = None
 
         self.gridLimit = config.get(c.CFG_GRID_LIMIT, 2000)
         self.essFeedLimit = config.get(c.CFG_ESS_FEED_LIMIT, 2000)
         self.essChargeLimit = config.get(c.CFG_ESS_CHARGE_LIMIT, 2000)
         self.socDischargeLimit = config.get(c.CFG_SOC_DISCHARGE_LIMIT, 0)
         self.socChargeLimit = config.get(c.CFG_SOC_CHARGE_LIMIT, 100)
@@ -27,14 +28,15 @@
         """
         self.client = ModbusClient(
             host=self.host,
             port=self.port,
             auto_open=True,
             auto_close=True,
             unit_id=self.unit_id,
+            timeout=self.timeout
         )
 
     def parseValue(self, value:int) -> int:
         """
         Parse the value to a signed integer.
         """
         if value is not None:
```

### Comparing `victron-0.0.3/victron.egg-info/PKG-INFO` & `victron-0.0.4/victron.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: victron
-Version: 0.0.3
+Version: 0.0.4
 Summary: An SDK for Victron via Modbus TCP
 Home-page: https://gitlab.com/jfk344/python-victron-sdk
 Author: @jfk344
 Author-email: info@jfk-enterprise.com
 License: mit
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

