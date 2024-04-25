# Comparing `tmp/lghorizon-0.6.8.tar.gz` & `tmp/lghorizon-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lghorizon-0.6.8.tar", last modified: Mon Jan 22 21:12:30 2024, max compression
+gzip compressed data, was "lghorizon-0.6.9.tar", last modified: Mon Jan 22 22:01:36 2024, max compression
```

## Comparing `lghorizon-0.6.8.tar` & `lghorizon-0.6.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:12:30.533208 lghorizon-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-01-22 21:12:22.000000 lghorizon-0.6.8/.coverage
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-22 21:12:22.000000 lghorizon-0.6.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:12:30.525208 lghorizon-0.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:12:30.529208 lghorizon-0.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-22 21:12:22.000000 lghorizon-0.6.8/.github/workflows/build-on-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-01-22 21:12:22.000000 lghorizon-0.6.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-22 21:12:22.000000 lghorizon-0.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-22 21:12:22.000000 lghorizon-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-22 21:12:30.529208 lghorizon-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-22 21:12:22.000000 lghorizon-0.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-22 21:12:22.000000 lghorizon-0.6.8/instructions.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:12:30.529208 lghorizon-0.6.8/lghorizon/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-22 21:12:22.000000 lghorizon-0.6.8/lghorizon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-01-22 21:12:22.000000 lghorizon-0.6.8/lghorizon/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-22 21:12:22.000000 lghorizon-0.6.8/lghorizon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-22 21:12:22.000000 lghorizon-0.6.8/lghorizon/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    23752 2024-01-22 21:12:22.000000 lghorizon-0.6.8/lghorizon/lghorizon_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23678 2024-01-22 21:12:22.000000 lghorizon-0.6.8/lghorizon/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 21:12:22.000000 lghorizon-0.6.8/lghorizon/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:12:30.529208 lghorizon-0.6.8/lghorizon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-22 21:12:30.000000 lghorizon-0.6.8/lghorizon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-01-22 21:12:30.000000 lghorizon-0.6.8/lghorizon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 21:12:30.000000 lghorizon-0.6.8/lghorizon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 21:12:30.000000 lghorizon-0.6.8/lghorizon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-22 21:12:30.000000 lghorizon-0.6.8/lghorizon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-22 21:12:30.000000 lghorizon-0.6.8/lghorizon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-01-22 21:12:22.000000 lghorizon-0.6.8/lib64
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-22 21:12:22.000000 lghorizon-0.6.8/pyvenv.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-22 21:12:22.000000 lghorizon-0.6.8/secrets_stub.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 21:12:30.533208 lghorizon-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-01-22 21:12:22.000000 lghorizon-0.6.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-01-22 21:12:22.000000 lghorizon-0.6.8/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:36.739941 lghorizon-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-01-22 22:01:28.000000 lghorizon-0.6.9/.coverage
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-22 22:01:28.000000 lghorizon-0.6.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:36.735941 lghorizon-0.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:36.739941 lghorizon-0.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-22 22:01:28.000000 lghorizon-0.6.9/.github/workflows/build-on-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-01-22 22:01:28.000000 lghorizon-0.6.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-22 22:01:28.000000 lghorizon-0.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-22 22:01:28.000000 lghorizon-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-22 22:01:36.739941 lghorizon-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-22 22:01:28.000000 lghorizon-0.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-22 22:01:28.000000 lghorizon-0.6.9/instructions.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:36.739941 lghorizon-0.6.9/lghorizon/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-22 22:01:28.000000 lghorizon-0.6.9/lghorizon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-01-22 22:01:28.000000 lghorizon-0.6.9/lghorizon/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-22 22:01:28.000000 lghorizon-0.6.9/lghorizon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-22 22:01:28.000000 lghorizon-0.6.9/lghorizon/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23770 2024-01-22 22:01:28.000000 lghorizon-0.6.9/lghorizon/lghorizon_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23678 2024-01-22 22:01:28.000000 lghorizon-0.6.9/lghorizon/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:28.000000 lghorizon-0.6.9/lghorizon/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:36.739941 lghorizon-0.6.9/lghorizon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-22 22:01:36.000000 lghorizon-0.6.9/lghorizon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-01-22 22:01:36.000000 lghorizon-0.6.9/lghorizon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 22:01:36.000000 lghorizon-0.6.9/lghorizon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 22:01:36.000000 lghorizon-0.6.9/lghorizon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-22 22:01:36.000000 lghorizon-0.6.9/lghorizon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-22 22:01:36.000000 lghorizon-0.6.9/lghorizon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-01-22 22:01:28.000000 lghorizon-0.6.9/lib64
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-22 22:01:28.000000 lghorizon-0.6.9/pyvenv.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-22 22:01:28.000000 lghorizon-0.6.9/secrets_stub.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 22:01:36.739941 lghorizon-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-01-22 22:01:28.000000 lghorizon-0.6.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-01-22 22:01:28.000000 lghorizon-0.6.9/test.py
```

### Comparing `lghorizon-0.6.8/.coverage` & `lghorizon-0.6.9/.coverage`

 * *Files identical despite different names*

### Comparing `lghorizon-0.6.8/.github/workflows/build-on-pr.yml` & `lghorizon-0.6.9/.github/workflows/build-on-pr.yml`

 * *Files identical despite different names*

### Comparing `lghorizon-0.6.8/.github/workflows/publish-to-pypi.yml` & `lghorizon-0.6.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lghorizon-0.6.8/LICENSE` & `lghorizon-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lghorizon-0.6.8/PKG-INFO` & `lghorizon-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lghorizon
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python client for Liberty Global Horizon settop boxes
 Home-page: https://github.com/sholofly/LGHorizon-python
 Author: Rudolf Offereins
 Author-email: r.offereins@gmail.com
 License: MIT license
 Keywords: LG,Horizon,API,Settop box
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lghorizon-0.6.8/lghorizon/const.py` & `lghorizon-0.6.9/lghorizon/const.py`

 * *Files identical despite different names*

### Comparing `lghorizon-0.6.8/lghorizon/lghorizon_api.py` & `lghorizon-0.6.9/lghorizon/lghorizon_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         except Exception as ex:
             pass
 
     def _obtain_mqtt_token(self):
         _logger.debug("Obtain mqtt token...")
         mqtt_auth_url = self._config["authorizationService"]["URL"]
         if self._country_settings["use_legacy_auth"]:
-            mqtt_auth_url = self._country_settings["api_url"]
+            mqtt_auth_url = self._country_settings["api_url"] + "/auth-service"
         mqtt_response = self._do_api_call(f"{mqtt_auth_url}/v1/mqtt/token")
         self._auth.mqttToken = mqtt_response["token"]
         _logger.debug(f"MQTT token: {self._auth.mqttToken}")
 
     def _obtain_mqtt_token_gb(self):
         _logger.debug("Obtain Virgin GB mqtt token...")
         self._session.headers["x-oesp-token"] = self._auth.accessToken
```

### Comparing `lghorizon-0.6.8/lghorizon/models.py` & `lghorizon-0.6.9/lghorizon/models.py`

 * *Files identical despite different names*

### Comparing `lghorizon-0.6.8/lghorizon.egg-info/PKG-INFO` & `lghorizon-0.6.9/lghorizon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lghorizon
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python client for Liberty Global Horizon settop boxes
 Home-page: https://github.com/sholofly/LGHorizon-python
 Author: Rudolf Offereins
 Author-email: r.offereins@gmail.com
 License: MIT license
 Keywords: LG,Horizon,API,Settop box
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lghorizon-0.6.8/lghorizon.egg-info/SOURCES.txt` & `lghorizon-0.6.9/lghorizon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lghorizon-0.6.8/setup.py` & `lghorizon-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `lghorizon-0.6.8/test.py` & `lghorizon-0.6.9/test.py`

 * *Files identical despite different names*

