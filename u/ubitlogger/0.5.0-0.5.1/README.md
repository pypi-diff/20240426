# Comparing `tmp/ubitlogger-0.5.0.tar.gz` & `tmp/ubitlogger-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubitlogger-0.5.0.tar", last modified: Wed Apr 24 07:56:07 2024, max compression
+gzip compressed data, was "ubitlogger-0.5.1.tar", last modified: Fri Apr 26 08:43:54 2024, max compression
```

## Comparing `ubitlogger-0.5.0.tar` & `ubitlogger-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-24 07:56:07.298027 ubitlogger-0.5.0/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     1062 2024-04-15 23:12:06.000000 ubitlogger-0.5.0/LICENSE
--rw-r--r--   0 pairin    (1000) pairin    (1000)       42 2024-04-22 11:27:36.000000 ubitlogger-0.5.0/MANIFEST.in
--rw-r--r--   0 pairin    (1000) pairin    (1000)     8380 2024-04-24 07:56:07.288027 ubitlogger-0.5.0/PKG-INFO
--rw-r--r--   0 pairin    (1000) pairin    (1000)     6916 2024-04-24 07:47:37.000000 ubitlogger-0.5.0/README.md
--rw-r--r--   0 pairin    (1000) pairin    (1000)     1998 2024-04-24 07:49:37.000000 ubitlogger-0.5.0/pyproject.toml
--rw-r--r--   0 pairin    (1000) pairin    (1000)       38 2024-04-24 07:56:07.298027 ubitlogger-0.5.0/setup.cfg
--rw-r--r--   0 pairin    (1000) pairin    (1000)      529 2024-04-15 21:47:43.000000 ubitlogger-0.5.0/setup.py
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-24 07:56:07.288027 ubitlogger-0.5.0/src/
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-24 07:56:07.288027 ubitlogger-0.5.0/src/ubitlogger/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     3347 2024-04-24 07:49:37.000000 ubitlogger-0.5.0/src/ubitlogger/__init__.py
--rw-r--r--   0 pairin    (1000) pairin    (1000)     4373 2024-04-24 07:47:37.000000 ubitlogger-0.5.0/src/ubitlogger/cli.py
--rw-r--r--   0 pairin    (1000) pairin    (1000)      599 2024-04-24 07:47:37.000000 ubitlogger-0.5.0/src/ubitlogger/data_receiver.py
--rw-r--r--   0 pairin    (1000) pairin    (1000)      429 2024-04-22 11:41:11.000000 ubitlogger-0.5.0/src/ubitlogger/read_sensor.py
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-24 07:56:07.288027 ubitlogger-0.5.0/src/ubitlogger.egg-info/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     8380 2024-04-24 07:56:07.000000 ubitlogger-0.5.0/src/ubitlogger.egg-info/PKG-INFO
--rw-r--r--   0 pairin    (1000) pairin    (1000)      409 2024-04-24 07:56:07.000000 ubitlogger-0.5.0/src/ubitlogger.egg-info/SOURCES.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)        1 2024-04-24 07:56:07.000000 ubitlogger-0.5.0/src/ubitlogger.egg-info/dependency_links.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)       50 2024-04-24 07:56:07.000000 ubitlogger-0.5.0/src/ubitlogger.egg-info/entry_points.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)      218 2024-04-24 07:56:07.000000 ubitlogger-0.5.0/src/ubitlogger.egg-info/requires.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)       11 2024-04-24 07:56:07.000000 ubitlogger-0.5.0/src/ubitlogger.egg-info/top_level.txt
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-24 07:56:07.288027 ubitlogger-0.5.0/tests/
--rw-r--r--   0 pairin    (1000) pairin    (1000)        0 2024-04-17 14:44:36.000000 ubitlogger-0.5.0/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:43:54.535152 ubitlogger-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-26 08:43:48.000000 ubitlogger-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-26 08:43:48.000000 ubitlogger-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-26 08:43:54.535152 ubitlogger-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-26 08:43:48.000000 ubitlogger-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-26 08:43:48.000000 ubitlogger-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:43:54.535152 ubitlogger-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-26 08:43:48.000000 ubitlogger-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:43:54.531151 ubitlogger-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:43:54.531151 ubitlogger-0.5.1/src/ubitlogger/
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-26 08:43:48.000000 ubitlogger-0.5.1/src/ubitlogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-26 08:43:48.000000 ubitlogger-0.5.1/src/ubitlogger/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-26 08:43:48.000000 ubitlogger-0.5.1/src/ubitlogger/data_receiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-26 08:43:48.000000 ubitlogger-0.5.1/src/ubitlogger/read_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:43:54.535152 ubitlogger-0.5.1/src/ubitlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-26 08:43:54.000000 ubitlogger-0.5.1/src/ubitlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-26 08:43:54.000000 ubitlogger-0.5.1/src/ubitlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:43:54.000000 ubitlogger-0.5.1/src/ubitlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 08:43:54.000000 ubitlogger-0.5.1/src/ubitlogger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-26 08:43:54.000000 ubitlogger-0.5.1/src/ubitlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 08:43:54.000000 ubitlogger-0.5.1/src/ubitlogger.egg-info/top_level.txt
```

### Comparing `ubitlogger-0.5.0/LICENSE` & `ubitlogger-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ubitlogger-0.5.0/PKG-INFO` & `ubitlogger-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubitlogger
-Version: 0.5.0
+Version: 0.5.1
 Summary: A micro:bit serial port logger
 Author-email: p4irin <p4irin.github.io@gmail.com>
 Project-URL: Homepage, https://github.com/p4irin/ubitlogger
 Project-URL: Bug Tracker, https://github.com/p4irin/ubitlogger/issues
 Keywords: microbit,microbit-v1,data-logger,serial-port-listener
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -30,14 +30,15 @@
 Requires-Dist: twine>=4.0.2; extra == "package"
 Provides-Extra: dev
 Requires-Dist: bumpver>=2023.1126; extra == "dev"
 Requires-Dist: ubitlogger[lint]; extra == "dev"
 Requires-Dist: ubitlogger[test]; extra == "dev"
 Requires-Dist: ubitlogger[package]; extra == "dev"
 
+[![ubitlogger CI](https://github.com/p4irin/ubitlogger/actions/workflows/ci.yml/badge.svg)](https://github.com/p4irin/ubitlogger/actions/workflows/ci.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/ubitlogger)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ubitlogger)
 ![PyPI - License](https://img.shields.io/pypi/l/ubitlogger)
 [![Static Badge](https://img.shields.io/badge/microbit-v1.3x-blue?logo=microbit&link=https%3A%2F%2Ftech.microbit.org%2Fhardware%2F1-3-revision%2F)](https://tech.microbit.org/hardware/1-3-revision/)
 [![Static Badge](https://img.shields.io/badge/Ubuntu-22.04_LTS_jammy-orange?logo=ubuntu)](https://ubuntu.com/download/server)
 [![Static Badge](https://img.shields.io/badge/Raspberry_Pi-4B_8GB-red?logo=raspberrypi&logoColor=red)](https://www.raspberrypi.com/products/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

### Comparing `ubitlogger-0.5.0/README.md` & `ubitlogger-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[![ubitlogger CI](https://github.com/p4irin/ubitlogger/actions/workflows/ci.yml/badge.svg)](https://github.com/p4irin/ubitlogger/actions/workflows/ci.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/ubitlogger)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ubitlogger)
 ![PyPI - License](https://img.shields.io/pypi/l/ubitlogger)
 [![Static Badge](https://img.shields.io/badge/microbit-v1.3x-blue?logo=microbit&link=https%3A%2F%2Ftech.microbit.org%2Fhardware%2F1-3-revision%2F)](https://tech.microbit.org/hardware/1-3-revision/)
 [![Static Badge](https://img.shields.io/badge/Ubuntu-22.04_LTS_jammy-orange?logo=ubuntu)](https://ubuntu.com/download/server)
 [![Static Badge](https://img.shields.io/badge/Raspberry_Pi-4B_8GB-red?logo=raspberrypi&logoColor=red)](https://www.raspberrypi.com/products/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

### Comparing `ubitlogger-0.5.0/pyproject.toml` & `ubitlogger-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ubitlogger"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="p4irin", email="p4irin.github.io@gmail.com" },
 ]
 description = "A micro:bit serial port logger"
 readme = "README.md"
 requires-python = ">=3.8.10"
 keywords = [
@@ -60,15 +60,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 
 [tool.bumpver]
-current_version = "0.5.0"
+current_version = "0.5.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
 
@@ -81,20 +81,22 @@
   "^__version__ = '{version}'$",
 ]
 
 
 [tool.ruff]
 exclude = [
   "read_sensor*.py",
+  "data_receiver*.py",
 ]
 
 
 [tool.mypy]
 exclude = [
   "read_sensor",
+  "data_receiver",
 ]
 
 [[tool.mypy.overrides]]
 module = [
   "serial.*", "uflash",
 ]
 ignore_missing_imports = true
```

### Comparing `ubitlogger-0.5.0/setup.py` & `ubitlogger-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `ubitlogger-0.5.0/src/ubitlogger/__init__.py` & `ubitlogger-0.5.1/src/ubitlogger/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 """
 
 __author__ = 'p4irin'
 __email__ = 'p4irin.github.io@gmail.com'
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 
 
 from threading import Thread, Event, enumerate
 from signal import signal, SIGINT, SIGTERM
 from time import sleep
 from serial import Serial
 from serial.tools.list_ports import comports
 
 
-def _exit_gracefully(signum, frame):
+def _exit_gracefully(signum: int, frame) -> None:
     if signum in [2, 15]:
         if signum == 2:
             msg = "\nExited by CTRL-C\n"
         if signum == 15:
             msg = "Exited by SIGTERM\n"
         msg += "Cleaning up thread\n"
         _stop_event.set()
@@ -27,31 +27,32 @@
                 thread.join()
     else:
         msg = f"Received signal: {signum}"
     print(msg)
     print(f"frame: {frame}")
     exit(1)
 
-signal(SIGINT, handler=_exit_gracefully)
-signal(SIGTERM, handler=_exit_gracefully)
+signal(SIGINT, _exit_gracefully)
+signal(SIGTERM, _exit_gracefully)
 
 _stop_event = Event()
 
 
 class NoUBitFound(Exception):
     pass
 
 
 class UBitLogger(object):
 
-    _product_id = 516
-    _vendor_id = 3368
+    _product_id: int = 516
+    _vendor_id: int = 3368
 
     def __init__(
-            self, handler = None,
+            self,
+            handler = None,
             baudrate: int = 115200,
             timeout: float = 0.1,
             interval: int = 1,
             debug: bool = False,
             block: bool = True
             ) -> None:
         
@@ -59,15 +60,15 @@
         self.handler = handler or self._default_handler
         self._baudrate = baudrate
         self._timeout = timeout
         self._interval = interval
         self._block = block
         self._serial_port = self._scan()
 
-    def _default_handler(self, line:str):
+    def _default_handler(self, line: str) -> None:
         print(line)
 
     def _scan(self) -> Serial:
         ports = comports()
         if len(ports) > 0:
             for port in ports:
                 try:
@@ -81,24 +82,24 @@
                             baudrate=self._baudrate
                             )
                         return connection
                 except AttributeError:
                     continue
         raise NoUBitFound
     
-    def _listen(self):
+    def _listen(self) -> None:
         self._serial_port.reset_input_buffer()
         while not _stop_event.is_set():
             if self._serial_port.in_waiting > 0:
                 line = self._serial_port.readline().decode('utf-8').strip()
                 self.handler(line)
             sleep(self._interval)
         self._serial_port.close()
 
-    def start(self):
+    def start(self) -> None:
         if self._debug:
             connection = self._serial_port
             print(f"Listening on port {connection.port}")
             print(f"Baudrate: {connection.baudrate}")
             print(f"Data bits: {connection.bytesize}")
             print(f"Stop bits: {connection.stopbits}")
             print(f"Parity: {connection.parity}")
@@ -107,9 +108,9 @@
 
         thread = Thread(target=self._listen, name="listening_thread")
         self._thread = thread
         self._thread.start()
         if self._block:
             self._thread.join()
     
-    def stop(self):
+    def stop(self) -> None:
         _stop_event.set()
```

### Comparing `ubitlogger-0.5.0/src/ubitlogger/cli.py` & `ubitlogger-0.5.1/src/ubitlogger/cli.py`

 * *Files identical despite different names*

### Comparing `ubitlogger-0.5.0/src/ubitlogger/data_receiver.py` & `ubitlogger-0.5.1/src/ubitlogger/data_receiver.py`

 * *Files identical despite different names*

### Comparing `ubitlogger-0.5.0/src/ubitlogger.egg-info/PKG-INFO` & `ubitlogger-0.5.1/src/ubitlogger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubitlogger
-Version: 0.5.0
+Version: 0.5.1
 Summary: A micro:bit serial port logger
 Author-email: p4irin <p4irin.github.io@gmail.com>
 Project-URL: Homepage, https://github.com/p4irin/ubitlogger
 Project-URL: Bug Tracker, https://github.com/p4irin/ubitlogger/issues
 Keywords: microbit,microbit-v1,data-logger,serial-port-listener
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -30,14 +30,15 @@
 Requires-Dist: twine>=4.0.2; extra == "package"
 Provides-Extra: dev
 Requires-Dist: bumpver>=2023.1126; extra == "dev"
 Requires-Dist: ubitlogger[lint]; extra == "dev"
 Requires-Dist: ubitlogger[test]; extra == "dev"
 Requires-Dist: ubitlogger[package]; extra == "dev"
 
+[![ubitlogger CI](https://github.com/p4irin/ubitlogger/actions/workflows/ci.yml/badge.svg)](https://github.com/p4irin/ubitlogger/actions/workflows/ci.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/ubitlogger)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ubitlogger)
 ![PyPI - License](https://img.shields.io/pypi/l/ubitlogger)
 [![Static Badge](https://img.shields.io/badge/microbit-v1.3x-blue?logo=microbit&link=https%3A%2F%2Ftech.microbit.org%2Fhardware%2F1-3-revision%2F)](https://tech.microbit.org/hardware/1-3-revision/)
 [![Static Badge](https://img.shields.io/badge/Ubuntu-22.04_LTS_jammy-orange?logo=ubuntu)](https://ubuntu.com/download/server)
 [![Static Badge](https://img.shields.io/badge/Raspberry_Pi-4B_8GB-red?logo=raspberrypi&logoColor=red)](https://www.raspberrypi.com/products/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

