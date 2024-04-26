# Comparing `tmp/pyopenweathermap-0.0.2.tar.gz` & `tmp/pyopenweathermap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenweathermap-0.0.2.tar", max compression
+gzip compressed data, was "pyopenweathermap-0.0.3.tar", max compression
```

## Comparing `pyopenweathermap-0.0.2.tar` & `pyopenweathermap-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.2/LICENSE
--rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.2/README.md
--rw-r--r--   0        0        0      567 2024-04-26 14:34:18.257076 pyopenweathermap-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      232 2024-04-26 09:04:44.323164 pyopenweathermap-0.0.2/src/pyopenweathermap/__init__.py
--rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.2/src/pyopenweathermap/exception.py
--rw-r--r--   0        0        0     2740 2024-04-26 09:04:44.327165 pyopenweathermap-0.0.2/src/pyopenweathermap/owm_client.py
--rw-r--r--   0        0        0     2534 2024-04-26 13:33:43.405295 pyopenweathermap-0.0.2/src/pyopenweathermap/weather.py
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.3/LICENSE
+-rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.3/README.md
+-rw-r--r--   0        0        0      567 2024-04-26 14:38:51.234560 pyopenweathermap-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      232 2024-04-26 09:04:44.323164 pyopenweathermap-0.0.3/src/pyopenweathermap/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.3/src/pyopenweathermap/exception.py
+-rw-r--r--   0        0        0     2721 2024-04-26 14:38:45.810524 pyopenweathermap-0.0.3/src/pyopenweathermap/owm_client.py
+-rw-r--r--   0        0        0     2534 2024-04-26 13:33:43.405295 pyopenweathermap-0.0.3/src/pyopenweathermap/weather.py
+-rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.3/PKG-INFO
```

### Comparing `pyopenweathermap-0.0.2/LICENSE` & `pyopenweathermap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.2/pyproject.toml` & `pyopenweathermap-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyopenweathermap"
-version = "0.0.2"
+version = "0.0.3"
 description = "lib for OpenWeatherMap for Home Assistant"
 authors = ["Evgeny <iam@freekode.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["homeassistant", "owm", "openweathermap"]
 packages = [
     { include = "pyopenweathermap", from = "src" },
```

### Comparing `pyopenweathermap-0.0.2/src/pyopenweathermap/owm_client.py` & `pyopenweathermap-0.0.3/src/pyopenweathermap/owm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         try:
             await self._request(url)
             return True
         except UnauthorizedError:
             return False
 
     async def _request(self, url):
-        print(url)
         async with ClientSession() as session:
             try:
                 async with session.get(url=url, timeout=self.request_timeout) as response:
                     if response.status == 200:
                         return await response.json()
                     elif response.status == 401:
                         raise UnauthorizedError
```

### Comparing `pyopenweathermap-0.0.2/src/pyopenweathermap/weather.py` & `pyopenweathermap-0.0.3/src/pyopenweathermap/weather.py`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.2/PKG-INFO` & `pyopenweathermap-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopenweathermap
-Version: 0.0.2
+Version: 0.0.3
 Summary: lib for OpenWeatherMap for Home Assistant
 License: MIT
 Keywords: homeassistant,owm,openweathermap
 Author: Evgeny
 Author-email: iam@freekode.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

