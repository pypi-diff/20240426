# Comparing `tmp/tcp_modbus_aio-0.2.0.tar.gz` & `tmp/tcp_modbus_aio-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcp_modbus_aio-0.2.0.tar", max compression
+gzip compressed data, was "tcp_modbus_aio-0.2.1.tar", max compression
```

## Comparing `tcp_modbus_aio-0.2.0.tar` & `tcp_modbus_aio-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/LICENSE
--rw-r--r--   0        0        0     1649 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/README.md
--rw-r--r--   0        0        0      857 2024-04-21 22:14:56.874465 tcp_modbus_aio-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-21 22:14:56.882465 tcp_modbus_aio-0.2.0/tcp_modbus_aio/__init__.py
--rw-r--r--   0        0        0    20152 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/tcp_modbus_aio/client.py
--rw-r--r--   0        0        0      267 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/tcp_modbus_aio/exceptions.py
--rw-r--r--   0        0        0     1140 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/tcp_modbus_aio/ping.py
--rw-r--r--   0        0        0        0 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/tcp_modbus_aio/py.typed
--rw-r--r--   0        0        0     2889 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/tcp_modbus_aio/typed_functions.py
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1649 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/README.md
+-rw-r--r--   0        0        0      857 2024-04-25 23:27:30.469780 tcp_modbus_aio-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-25 23:27:30.477780 tcp_modbus_aio-0.2.1/tcp_modbus_aio/__init__.py
+-rw-r--r--   0        0        0    20152 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/tcp_modbus_aio/client.py
+-rw-r--r--   0        0        0      267 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/tcp_modbus_aio/exceptions.py
+-rw-r--r--   0        0        0     1167 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/tcp_modbus_aio/ping.py
+-rw-r--r--   0        0        0        0 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/tcp_modbus_aio/py.typed
+-rw-r--r--   0        0        0     2889 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/tcp_modbus_aio/typed_functions.py
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.2.1/PKG-INFO
```

### Comparing `tcp_modbus_aio-0.2.0/LICENSE` & `tcp_modbus_aio-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.0/README.md` & `tcp_modbus_aio-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.0/pyproject.toml` & `tcp_modbus_aio-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tcp-modbus-aio"
-version = "0.2.0"
+version = "0.2.1"
 description = "asyncio client library for tcp modbus devices"
 authors = ["Josh Gruenstein <josh@tutorintelligence.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tcp_modbus_aio-0.2.0/tcp_modbus_aio/client.py` & `tcp_modbus_aio-0.2.1/tcp_modbus_aio/client.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.0/tcp_modbus_aio/ping.py` & `tcp_modbus_aio-0.2.1/tcp_modbus_aio/ping.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import subprocess
 
 
 async def ping_ip(ip: str, timeout: float = 0.5) -> float | None:
     """Return the latency in seconds of a ping to the given ip, or None if the ping failed"""
     ping_process = await asyncio.create_subprocess_shell(
-        f"ping -c 1 {ip}", stdout=subprocess.PIPE
+        f"ping -c 1 {ip}", stdout=subprocess.PIPE, stderr=subprocess.DEVNULL
     )
 
     try:
         # Wait for the subprocess to complete or timeout
         ping_output, stderr = await asyncio.wait_for(
             ping_process.communicate(), timeout=timeout
         )
```

### Comparing `tcp_modbus_aio-0.2.0/tcp_modbus_aio/typed_functions.py` & `tcp_modbus_aio-0.2.1/tcp_modbus_aio/typed_functions.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.0/PKG-INFO` & `tcp_modbus_aio-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcp-modbus-aio
-Version: 0.2.0
+Version: 0.2.1
 Summary: asyncio client library for tcp modbus devices
 License: MIT
 Author: Josh Gruenstein
 Author-email: josh@tutorintelligence.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

