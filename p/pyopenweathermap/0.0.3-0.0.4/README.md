# Comparing `tmp/pyopenweathermap-0.0.3.tar.gz` & `tmp/pyopenweathermap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenweathermap-0.0.3.tar", max compression
+gzip compressed data, was "pyopenweathermap-0.0.4.tar", max compression
```

## Comparing `pyopenweathermap-0.0.3.tar` & `pyopenweathermap-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.3/LICENSE
--rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.3/README.md
--rw-r--r--   0        0        0      567 2024-04-26 14:38:51.234560 pyopenweathermap-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      232 2024-04-26 09:04:44.323164 pyopenweathermap-0.0.3/src/pyopenweathermap/__init__.py
--rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.3/src/pyopenweathermap/exception.py
--rw-r--r--   0        0        0     2721 2024-04-26 14:38:45.810524 pyopenweathermap-0.0.3/src/pyopenweathermap/owm_client.py
--rw-r--r--   0        0        0     2534 2024-04-26 13:33:43.405295 pyopenweathermap-0.0.3/src/pyopenweathermap/weather.py
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.4/LICENSE
+-rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.4/README.md
+-rw-r--r--   0        0        0      569 2024-04-26 18:15:02.825861 pyopenweathermap-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      232 2024-04-26 09:04:44.323164 pyopenweathermap-0.0.4/src/pyopenweathermap/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.4/src/pyopenweathermap/exception.py
+-rw-r--r--   0        0        0     2721 2024-04-26 14:38:45.810524 pyopenweathermap-0.0.4/src/pyopenweathermap/owm_client.py
+-rw-r--r--   0        0        0     2534 2024-04-26 13:33:43.405295 pyopenweathermap-0.0.4/src/pyopenweathermap/weather.py
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.4/PKG-INFO
```

### Comparing `pyopenweathermap-0.0.3/LICENSE` & `pyopenweathermap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.3/pyproject.toml` & `pyopenweathermap-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "pyopenweathermap"
-version = "0.0.3"
+version = "0.0.4"
 description = "lib for OpenWeatherMap for Home Assistant"
 authors = ["Evgeny <iam@freekode.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["homeassistant", "owm", "openweathermap"]
 packages = [
     { include = "pyopenweathermap", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "^3.9.5"
-pydantic = "^2.7.1"
+pydantic = "^1.10.15"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
 
 [build-system]
```

### Comparing `pyopenweathermap-0.0.3/src/pyopenweathermap/owm_client.py` & `pyopenweathermap-0.0.4/src/pyopenweathermap/owm_client.py`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.3/src/pyopenweathermap/weather.py` & `pyopenweathermap-0.0.4/src/pyopenweathermap/weather.py`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.3/PKG-INFO` & `pyopenweathermap-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pyopenweathermap
-Version: 0.0.3
+Version: 0.0.4
 Summary: lib for OpenWeatherMap for Home Assistant
 License: MIT
 Keywords: homeassistant,owm,openweathermap
 Author: Evgeny
 Author-email: iam@freekode.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
-Requires-Dist: pydantic (>=2.7.1,<3.0.0)
+Requires-Dist: pydantic (>=1.10.15,<2.0.0)
 Description-Content-Type: text/markdown
 
 # pyopenweathermap
 
 Python library for OpenWeatherMap API for Home Assistant
```

