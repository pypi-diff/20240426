# Comparing `tmp/pyopenweathermap-0.0.1.tar.gz` & `tmp/pyopenweathermap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenweathermap-0.0.1.tar", max compression
+gzip compressed data, was "pyopenweathermap-0.0.2.tar", max compression
```

## Comparing `pyopenweathermap-0.0.1.tar` & `pyopenweathermap-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.1/LICENSE
--rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.1/README.md
--rw-r--r--   0        0        0      567 2024-04-25 17:47:01.871077 pyopenweathermap-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      232 2024-04-26 09:04:44.323164 pyopenweathermap-0.0.1/src/pyopenweathermap/__init__.py
--rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.1/src/pyopenweathermap/exception.py
--rw-r--r--   0        0        0     2740 2024-04-26 09:04:44.327165 pyopenweathermap-0.0.1/src/pyopenweathermap/owm_client.py
--rw-r--r--   0        0        0     2534 2024-04-26 13:33:43.405295 pyopenweathermap-0.0.1/src/pyopenweathermap/weather.py
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.2/LICENSE
+-rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.2/README.md
+-rw-r--r--   0        0        0      567 2024-04-26 14:34:18.257076 pyopenweathermap-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      232 2024-04-26 09:04:44.323164 pyopenweathermap-0.0.2/src/pyopenweathermap/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.2/src/pyopenweathermap/exception.py
+-rw-r--r--   0        0        0     2740 2024-04-26 09:04:44.327165 pyopenweathermap-0.0.2/src/pyopenweathermap/owm_client.py
+-rw-r--r--   0        0        0     2534 2024-04-26 13:33:43.405295 pyopenweathermap-0.0.2/src/pyopenweathermap/weather.py
+-rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.2/PKG-INFO
```

### Comparing `pyopenweathermap-0.0.1/LICENSE` & `pyopenweathermap-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.1/pyproject.toml` & `pyopenweathermap-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pyopenweathermap"
-version = "0.0.1"
+version = "0.0.2"
 description = "lib for OpenWeatherMap for Home Assistant"
 authors = ["Evgeny <iam@freekode.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["homeassistant", "owm", "openweathermap"]
 packages = [
     { include = "pyopenweathermap", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 aiohttp = "^3.9.5"
 pydantic = "^2.7.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
```

### Comparing `pyopenweathermap-0.0.1/src/pyopenweathermap/owm_client.py` & `pyopenweathermap-0.0.2/src/pyopenweathermap/owm_client.py`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.1/src/pyopenweathermap/weather.py` & `pyopenweathermap-0.0.2/src/pyopenweathermap/weather.py`

 * *Files identical despite different names*

