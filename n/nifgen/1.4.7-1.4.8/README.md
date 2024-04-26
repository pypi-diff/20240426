# Comparing `tmp/nifgen-1.4.7.tar.gz` & `tmp/nifgen-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifgen-1.4.7.tar", last modified: Fri Dec 15 19:31:01 2023, max compression
+gzip compressed data, was "nifgen-1.4.8.tar", last modified: Fri Apr 26 18:16:04 2024, max compression
```

## Comparing `nifgen-1.4.7.tar` & `nifgen-1.4.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:10.255455 nifgen-1.4.7/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8205 2023-12-15 19:31:10.248455 nifgen-1.4.7/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7020 2023-12-15 19:28:03.000000 nifgen-1.4.7/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:10.023429 nifgen-1.4.7/nifgen/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-12-15 19:27:48.000000 nifgen-1.4.7/nifgen/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3031 2023-12-15 19:27:46.000000 nifgen-1.4.7/nifgen/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5436 2023-12-15 19:27:38.000000 nifgen-1.4.7/nifgen/_attributes.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13871 2023-12-15 19:27:47.000000 nifgen-1.4.7/nifgen/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    23209 2023-12-15 19:27:49.000000 nifgen-1.4.7/nifgen/_grpc_stub_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    48679 2023-12-15 19:27:39.000000 nifgen-1.4.7/nifgen/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    54576 2023-12-15 19:27:40.000000 nifgen-1.4.7/nifgen/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1719 2023-12-15 19:27:41.000000 nifgen-1.4.7/nifgen/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-12-15 19:27:52.000000 nifgen-1.4.7/nifgen/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10347 2023-12-15 19:27:39.000000 nifgen-1.4.7/nifgen/enums.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4355 2023-12-15 19:27:43.000000 nifgen-1.4.7/nifgen/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3452 2023-12-15 19:27:50.000000 nifgen-1.4.7/nifgen/grpc_session_options.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-12-15 19:27:51.000000 nifgen-1.4.7/nifgen/nidevice_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-12-15 19:27:51.000000 nifgen-1.4.7/nifgen/nidevice_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   123775 2023-12-15 19:27:50.000000 nifgen-1.4.7/nifgen/nifgen_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   216324 2023-12-15 19:27:50.000000 nifgen-1.4.7/nifgen/nifgen_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   212642 2023-12-15 19:27:42.000000 nifgen-1.4.7/nifgen/session.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-12-15 19:27:52.000000 nifgen-1.4.7/nifgen/session_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-12-15 19:27:52.000000 nifgen-1.4.7/nifgen/session_pb2_grpc.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:10.238457 nifgen-1.4.7/nifgen.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8205 2023-12-15 19:31:09.000000 nifgen-1.4.7/nifgen.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      632 2023-12-15 19:31:09.000000 nifgen-1.4.7/nifgen.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:31:09.000000 nifgen-1.4.7/nifgen.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       71 2023-12-15 19:31:09.000000 nifgen-1.4.7/nifgen.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        7 2023-12-15 19:31:09.000000 nifgen-1.4.7/nifgen.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:31:09.000000 nifgen-1.4.7/nifgen.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-12-15 19:31:10.256456 nifgen-1.4.7/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2096 2023-12-15 19:28:04.000000 nifgen-1.4.7/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:16:04.151019 nifgen-1.4.8/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8258 2024-04-26 18:16:04.145016 nifgen-1.4.8/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7020 2024-04-26 18:09:57.000000 nifgen-1.4.8/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:16:04.049014 nifgen-1.4.8/nifgen/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2024-04-26 18:09:42.000000 nifgen-1.4.8/nifgen/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3550 2024-04-26 18:09:40.000000 nifgen-1.4.8/nifgen/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5436 2024-04-26 18:09:32.000000 nifgen-1.4.8/nifgen/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13871 2024-04-26 18:09:41.000000 nifgen-1.4.8/nifgen/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    23209 2024-04-26 18:09:43.000000 nifgen-1.4.8/nifgen/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    48679 2024-04-26 18:09:33.000000 nifgen-1.4.8/nifgen/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    54576 2024-04-26 18:09:35.000000 nifgen-1.4.8/nifgen/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1719 2024-04-26 18:09:35.000000 nifgen-1.4.8/nifgen/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      635 2024-04-26 18:09:46.000000 nifgen-1.4.8/nifgen/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10563 2024-04-26 18:09:33.000000 nifgen-1.4.8/nifgen/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4349 2024-04-26 18:09:37.000000 nifgen-1.4.8/nifgen/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3452 2024-04-26 18:09:43.000000 nifgen-1.4.8/nifgen/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2009 2024-04-26 18:09:45.000000 nifgen-1.4.8/nifgen/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2024-04-26 18:09:45.000000 nifgen-1.4.8/nifgen/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   129292 2024-04-26 18:09:44.000000 nifgen-1.4.8/nifgen/nifgen_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   212964 2024-04-26 18:09:44.000000 nifgen-1.4.8/nifgen/nifgen_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   214695 2024-04-26 18:09:37.000000 nifgen-1.4.8/nifgen/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4550 2024-04-26 18:09:46.000000 nifgen-1.4.8/nifgen/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2024-04-26 18:09:46.000000 nifgen-1.4.8/nifgen/session_pb2_grpc.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:16:04.137016 nifgen-1.4.8/nifgen.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8258 2024-04-26 18:16:03.000000 nifgen-1.4.8/nifgen.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      632 2024-04-26 18:16:03.000000 nifgen-1.4.8/nifgen.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:16:03.000000 nifgen-1.4.8/nifgen.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       73 2024-04-26 18:16:03.000000 nifgen-1.4.8/nifgen.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        7 2024-04-26 18:16:03.000000 nifgen-1.4.8/nifgen.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:16:03.000000 nifgen-1.4.8/nifgen.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2024-04-26 18:16:04.152017 nifgen-1.4.8/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2124 2024-04-26 18:09:57.000000 nifgen-1.4.8/setup.py
```

### Comparing `nifgen-1.4.7/PKG-INFO` & `nifgen-1.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifgen
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI-FGEN Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -17,22 +17,23 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Description-Content-Type: text/x-rst
 Requires-Dist: hightime>=0.2.0
 Requires-Dist: nitclk
 Provides-Extra: grpc
-Requires-Dist: grpcio<2.0,>=1.49.1; extra == "grpc"
-Requires-Dist: protobuf<5.0,>=4.21; extra == "grpc"
+Requires-Dist: grpcio<2.0,>=1.59.0; extra == "grpc"
+Requires-Dist: protobuf<5.0,>=4.21.6; extra == "grpc"
 
 Overall Status
 --------------
 
 +----------------------+------------------------------------------------------------------------------------------------------------------------------------+
 | master branch status | |BuildStatus| |MITLicense| |CoverageStatus|                                                                                        |
 +----------------------+------------------------------------------------------------------------------------------------------------------------------------+
@@ -81,15 +82,15 @@
 
 NI-FGEN Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-FGEN (nifgen)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 2023 Q1.1             |
+| Driver Version Tested Against | 2023 Q4               |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nifgenLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nifgenPythonVersion| |
 +-------------------------------+-----------------------+
 | Documentation                 | |nifgenDocs|          |
 +-------------------------------+-----------------------+
@@ -130,15 +131,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nifgen** module, you must install the NI-FGEN runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-FGEN**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nifgen~=1.4.7
+  $ python -m pip install nifgen~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nifgen-1.4.7/README.rst` & `nifgen-1.4.8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 NI-FGEN Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-FGEN (nifgen)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 2023 Q1.1             |
+| Driver Version Tested Against | 2023 Q4               |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nifgenLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nifgenPythonVersion| |
 +-------------------------------+-----------------------+
 | Documentation                 | |nifgenDocs|          |
 +-------------------------------+-----------------------+
@@ -98,15 +98,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nifgen** module, you must install the NI-FGEN runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-FGEN**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nifgen~=1.4.7
+  $ python -m pip install nifgen~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nifgen-1.4.7/nifgen/__init__.py` & `nifgen-1.4.8/nifgen/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.7'
+__version__ = '1.4.8'
 
 from nifgen.enums import *  # noqa: F403,F401,H303
 from nifgen.errors import DriverWarning  # noqa: F401
 from nifgen.errors import Error  # noqa: F401
 from nifgen.grpc_session_options import *  # noqa: F403,F401,H303
 from nifgen.session import Session  # noqa: F401
 
@@ -14,16 +14,16 @@
 def get_diagnostic_information():
     '''Get diagnostic information about the system state that is suitable for printing or logging
 
     returns: dict
 
     note: Python bitness may be incorrect when running in a virtual environment
     '''
+    import importlib.metadata
     import os
-    import pkg_resources
     import platform
     import struct
     import sys
 
     def is_python_64bit():
         return (struct.calcsize("P") == 8)
 
@@ -52,24 +52,37 @@
             driver_version = 'Unknown'
     elif platform.system() == 'Linux':
         os_name = 'Linux'
         driver_version = 'Unknown'
     else:
         raise SystemError('Unsupported platform: {}'.format(platform.system()))
 
-    installed_packages = pkg_resources.working_set
-    installed_packages_list = [{'name': i.key, 'version': i.version, } for i in installed_packages]
+    if sys.version_info[1] >= 10:
+        installed_packages_names = [
+            name
+            for name_list in importlib.metadata.packages_distributions().values()
+            for name in name_list
+        ]
+        installed_packages_names = set(installed_packages_names)
+        installed_packages_list = [
+            {'name': name, 'version': importlib.metadata.distribution(name).version}
+            for name in sorted(installed_packages_names)
+        ]
+    else:
+        import pkg_resources
+        installed_packages = pkg_resources.working_set
+        installed_packages_list = [{'name': i.key, 'version': i.version, } for i in installed_packages]
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-FGEN"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nifgen'
-    info['module']['version'] = "1.4.7"
+    info['module']['version'] = "1.4.8"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nifgen-1.4.7/nifgen/_attributes.py` & `nifgen-1.4.8/nifgen/_attributes.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.7/nifgen/_converters.py` & `nifgen-1.4.8/nifgen/_converters.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.7/nifgen/_grpc_stub_interpreter.py` & `nifgen-1.4.8/nifgen/_grpc_stub_interpreter.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.7/nifgen/_library.py` & `nifgen-1.4.8/nifgen/_library.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.7/nifgen/_library_interpreter.py` & `nifgen-1.4.8/nifgen/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.7/nifgen/_library_singleton.py` & `nifgen-1.4.8/nifgen/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.7/nifgen/_visatype.py` & `nifgen-1.4.8/nifgen/_visatype.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# -*- coding: utf-8 -*-
-import ctypes
-
-
-'''Definitions of the VISA types used by the C API of the driver runtime.
-These are aliased directly to ctypes types so can be used directly to call into the library.
-'''
-
-
-ViChar = ctypes.c_char
-ViInt8 = ctypes.c_int8
-ViUInt8 = ctypes.c_uint8
-ViInt16 = ctypes.c_int16
-ViUInt16 = ctypes.c_uint16
-ViInt32 = ctypes.c_int32
-ViUInt32 = ctypes.c_uint32
-ViInt64 = ctypes.c_int64
-ViString = ctypes.c_char_p
-ViReal32 = ctypes.c_float
-ViReal64 = ctypes.c_double
-
-# Types that are based on other visatypes
-ViBoolean = ViUInt16
-ViStatus = ViInt32
-ViSession = ViUInt32
-ViAttr = ViUInt32
-ViConstString = ViString
-ViRsrc = ViString
-
+import ctypes
+
+
+'''Definitions of the VISA types used by the C API of the driver runtime.
+These are aliased directly to ctypes types so can be used directly to call into the library.
+'''
+
+
+ViChar = ctypes.c_char
+ViInt8 = ctypes.c_int8
+ViUInt8 = ctypes.c_uint8
+ViInt16 = ctypes.c_int16
+ViUInt16 = ctypes.c_uint16
+ViInt32 = ctypes.c_int32
+ViUInt32 = ctypes.c_uint32
+ViInt64 = ctypes.c_int64
+ViString = ctypes.c_char_p
+ViReal32 = ctypes.c_float
+ViReal64 = ctypes.c_double
+
+# Types that are based on other visatypes
+ViBoolean = ViUInt16
+ViStatus = ViInt32
+ViSession = ViUInt32
+ViAttr = ViUInt32
+ViConstString = ViString
+ViRsrc = ViString
+
```

### Comparing `nifgen-1.4.7/nifgen/enums.py` & `nifgen-1.4.8/nifgen/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,25 @@
     '''
     LOW = 102
     r'''
     When the operation is ready to start, the Ready for Start  event level is low.
     '''
 
 
+class EventPulseWidthUnits(Enum):
+    SAMPLE_CLOCK_PERIODS = 101
+    r'''
+    Specifies the pulse width in Sample clock periods.
+    '''
+    SECONDS = 102
+    r'''
+    Specifies the pulse width in seconds.
+    '''
+
+
 class HardwareState(Enum):
     IDLE = 0
     WAITING_FOR_START_TRIGGER = 100
     RUNNING = 200
     DONE = 600
     HARDWARE_ERROR = 1000
```

### Comparing `nifgen-1.4.7/nifgen/errors.py` & `nifgen-1.4.8/nifgen/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-FGEN driver'''
 
     def __init__(self, code, description):
         assert _is_warning(code), "Should not create Warning if code is not positive."
-        super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
+        super(DriverWarning, self).__init__('Warning {} occurred.\n\n{}'.format(code, description))
 
 
 class RpcError(Error):
     '''An error specific to sessions to the NI gRPC Device Server'''
 
     def __init__(self, rpc_code, description):
         self.rpc_code = rpc_code
@@ -85,24 +85,24 @@
         super(DriverTooNewError, self).__init__('The NI-FGEN runtime returned an unexpected value. This can occur if it is too new for the nifgen Python module. Upgrade the nifgen Python module.')
 
 
 class InvalidRepeatedCapabilityError(Error):
     '''An error due to an invalid character in a repeated capability'''
 
     def __init__(self, invalid_character, invalid_string):
-        super(InvalidRepeatedCapabilityError, self).__init__('An invalid character ({0}) was found in repeated capability string ({1})'.format(invalid_character, invalid_string))
+        super(InvalidRepeatedCapabilityError, self).__init__('An invalid character ({}) was found in repeated capability string ({})'.format(invalid_character, invalid_string))
 
 
 class SelfTestError(Error):
     '''An error due to a failed self-test'''
 
     def __init__(self, code, msg):
         self.code = code
         self.message = msg
-        super(SelfTestError, self).__init__('Self-test failed with code {0}: {1}'.format(code, msg))
+        super(SelfTestError, self).__init__('Self-test failed with code {}: {}'.format(code, msg))
 
 
 def handle_error(library_interpreter, code, ignore_warnings, is_error_handling):
     '''handle_error
 
     Helper function for handling errors returned by nifgen.Library.
     It calls back into the LibraryInterpreter to get the corresponding error
```

### Comparing `nifgen-1.4.7/nifgen/grpc_session_options.py` & `nifgen-1.4.8/nifgen/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.7/nifgen/nidevice_pb2.py` & `nifgen-1.4.8/nifgen/nidevice_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: nidevice.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0enidevice.proto\x12\rnidevice_grpc\"2\n\x0fNIComplexNumber\x12\x0c\n\x04real\x18\x01 \x01(\x01\x12\x11\n\timaginary\x18\x02 \x01(\x01\"5\n\x12NIComplexNumberF32\x12\x0c\n\x04real\x18\x01 \x01(\x02\x12\x11\n\timaginary\x18\x02 \x01(\x02\"/\n\x0cNIComplexI16\x12\x0c\n\x04real\x18\x01 \x01(\x11\x12\x11\n\timaginary\x18\x02 \x01(\x11\"r\n\x0fSmtSpectrumInfo\x12\x15\n\rspectrum_type\x18\x01 \x01(\r\x12\x11\n\tlinear_db\x18\x02 \x01(\r\x12\x0e\n\x06window\x18\x03 \x01(\r\x12\x13\n\x0bwindow_size\x18\x04 \x01(\x11\x12\x10\n\x08\x66\x66t_size\x18\x05 \x01(\x11\x42\x42\n\x12\x63om.ni.grpc.deviceB\x08NiDeviceP\x01\xaa\x02\x1fNationalInstruments.Grpc.Deviceb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nidevice_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nidevice_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.ni.grpc.deviceB\010NiDeviceP\001\252\002\037NationalInstruments.Grpc.Device'
-  _NICOMPLEXNUMBER._serialized_start=33
-  _NICOMPLEXNUMBER._serialized_end=83
-  _NICOMPLEXNUMBERF32._serialized_start=85
-  _NICOMPLEXNUMBERF32._serialized_end=138
-  _NICOMPLEXI16._serialized_start=140
-  _NICOMPLEXI16._serialized_end=187
-  _SMTSPECTRUMINFO._serialized_start=189
-  _SMTSPECTRUMINFO._serialized_end=303
+  _globals['_NICOMPLEXNUMBER']._serialized_start=33
+  _globals['_NICOMPLEXNUMBER']._serialized_end=83
+  _globals['_NICOMPLEXNUMBERF32']._serialized_start=85
+  _globals['_NICOMPLEXNUMBERF32']._serialized_end=138
+  _globals['_NICOMPLEXI16']._serialized_start=140
+  _globals['_NICOMPLEXI16']._serialized_end=187
+  _globals['_SMTSPECTRUMINFO']._serialized_start=189
+  _globals['_SMTSPECTRUMINFO']._serialized_end=303
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nifgen-1.4.7/nifgen/nifgen_pb2.py` & `nifgen-1.4.8/nifgen/nifgen_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,600 +1,592 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: nifgen.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import nidevice_pb2 as nidevice__pb2
 from . import session_pb2 as session__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cnifgen.proto\x12\x0bnifgen_grpc\x1a\x0enidevice.proto\x1a\rsession.proto\"<\n\x16\x41\x62ortGenerationRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\")\n\x17\x41\x62ortGenerationResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"d\n%AdjustSampleClockRelativeDelayRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x17\n\x0f\x61\x64justment_time\x18\x02 \x01(\x01\"8\n&AdjustSampleClockRelativeDelayResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x86\x01\n\x1c\x41llocateNamedWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12\x15\n\rwaveform_size\x18\x04 \x01(\x11\"/\n\x1d\x41llocateNamedWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"j\n\x17\x41llocateWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_size\x18\x03 \x01(\x11\"C\n\x18\x41llocateWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"\xa7\x01\n\x1e\x43heckAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x17\n\x0f\x61ttribute_value\x18\x04 \x01(\x08\"1\n\x1f\x43heckAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x87\x02\n\x1c\x43heckAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x42\n\x0f\x61ttribute_value\x18\x04 \x01(\x0e\x32\'.nifgen_grpc.NiFgenInt32AttributeValuesH\x00\x12\x1d\n\x13\x61ttribute_value_raw\x18\x05 \x01(\x11H\x00\x42\x16\n\x14\x61ttribute_value_enum\"/\n\x1d\x43heckAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa9\x01\n\x1c\x43heckAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x1b\n\x13\x61ttribute_value_raw\x18\x04 \x01(\x03\"/\n\x1d\x43heckAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x89\x02\n\x1d\x43heckAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x43\n\x0f\x61ttribute_value\x18\x04 \x01(\x0e\x32(.nifgen_grpc.NiFgenReal64AttributeValuesH\x00\x12\x1d\n\x13\x61ttribute_value_raw\x18\x05 \x01(\x01H\x00\x42\x16\n\x14\x61ttribute_value_enum\"0\n\x1e\x43heckAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xbf\x01\n\x1e\x43heckAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12/\n\x0f\x61ttribute_value\x18\x04 \x01(\x0b\x32\x16.nidevice_grpc.Session\"1\n\x1f\x43heckAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x96\x02\n\x1d\x43heckAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x1d\n\x13\x61ttribute_value_raw\x18\x04 \x01(\tH\x00\x12P\n\x16\x61ttribute_value_mapped\x18\x05 \x01(\x0e\x32..nifgen_grpc.NiFgenStringAttributeValuesMappedH\x00\x42\x16\n\x14\x61ttribute_value_enum\"0\n\x1e\x43heckAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\";\n\x15\x43learArbMemoryRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"(\n\x16\x43learArbMemoryResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xac\x01\n\x17\x43learArbSequenceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x36\n\x0fsequence_handle\x18\x02 \x01(\x0e\x32\x1b.nifgen_grpc.SequenceHandleH\x00\x12\x1d\n\x13sequence_handle_raw\x18\x03 \x01(\x11H\x00\x42\x16\n\x14sequence_handle_enum\"*\n\x18\x43learArbSequenceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xac\x01\n\x17\x43learArbWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x36\n\x0fwaveform_handle\x18\x02 \x01(\x0e\x32\x1b.nifgen_grpc.WaveformHandleH\x00\x12\x1d\n\x13waveform_handle_raw\x18\x03 \x01(\x11H\x00\x42\x16\n\x14waveform_handle_enum\"*\n\x18\x43learArbWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"7\n\x11\x43learErrorRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"$\n\x12\x43learErrorResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xc1\x01\n\x14\x43learFreqListRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x42\n\x15\x66requency_list_handle\x18\x02 \x01(\x0e\x32!.nifgen_grpc.FrequencyListOptionsH\x00\x12#\n\x19\x66requency_list_handle_raw\x18\x03 \x01(\x11H\x00\x42\x1c\n\x1a\x66requency_list_handle_enum\"\'\n\x15\x43learFreqListResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"E\n\x1f\x43learInterchangeWarningsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"2\n ClearInterchangeWarningsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\\\n ClearUserStandardWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"3\n!ClearUserStandardWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"2\n\x0c\x43loseRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rCloseResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"3\n\rCommitRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\" \n\x0e\x43ommitResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"h\n\x19\x43onfigureAmplitudeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\tamplitude\x18\x03 \x01(\x01\",\n\x1a\x43onfigureAmplitudeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8e\x01\n\x1b\x43onfigureArbSequenceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fsequence_handle\x18\x03 \x01(\x11\x12\x0c\n\x04gain\x18\x04 \x01(\x01\x12\x0e\n\x06offset\x18\x05 \x01(\x01\".\n\x1c\x43onfigureArbSequenceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8e\x01\n\x1b\x43onfigureArbWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fwaveform_handle\x18\x03 \x01(\x11\x12\x0c\n\x04gain\x18\x04 \x01(\x01\x12\x0e\n\x06offset\x18\x05 \x01(\x01\".\n\x1c\x43onfigureArbWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"P\n\x18\x43onfigureChannelsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x10\n\x08\x63hannels\x18\x02 \x01(\t\"+\n\x19\x43onfigureChannelsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x9a\x01\n\x19\x43onfigureClockModeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12,\n\nclock_mode\x18\x02 \x01(\x0e\x32\x16.nifgen_grpc.ClockModeH\x00\x12\x18\n\x0e\x63lock_mode_raw\x18\x03 \x01(\x11H\x00\x42\x11\n\x0f\x63lock_mode_enum\",\n\x1a\x43onfigureClockModeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x83\x01\n+ConfigureCustomFIRFilterCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1a\n\x12\x63oefficients_array\x18\x03 \x03(\x01\">\n,ConfigureCustomFIRFilterCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x80\x01\n(ConfigureDigitalEdgeScriptTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\ntrigger_id\x18\x02 \x01(\t\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x0c\n\x04\x65\x64ge\x18\x04 \x01(\x11\";\n)ConfigureDigitalEdgeScriptTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"k\n\'ConfigureDigitalEdgeStartTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0c\n\x04\x65\x64ge\x18\x03 \x01(\x11\":\n(ConfigureDigitalEdgeStartTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xd6\x01\n)ConfigureDigitalLevelScriptTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\ntrigger_id\x18\x02 \x01(\t\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x30\n\x0ctrigger_when\x18\x04 \x01(\x0e\x32\x18.nifgen_grpc.TriggerWhenH\x00\x12\x1a\n\x10trigger_when_raw\x18\x05 \x01(\x11H\x00\x42\x13\n\x11trigger_when_enum\"<\n*ConfigureDigitalLevelScriptTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xae\x01\n\x18\x43onfigureFreqListRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1d\n\x15\x66requency_list_handle\x18\x03 \x01(\x11\x12\x11\n\tamplitude\x18\x04 \x01(\x01\x12\x11\n\tdc_offset\x18\x05 \x01(\x01\x12\x13\n\x0bstart_phase\x18\x06 \x01(\x01\"+\n\x19\x43onfigureFreqListResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"h\n\x19\x43onfigureFrequencyRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\tfrequency\x18\x03 \x01(\x01\",\n\x1a\x43onfigureFrequencyResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"q\n\x1d\x43onfigureOperationModeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x16\n\x0eoperation_mode\x18\x03 \x01(\x11\"0\n\x1e\x43onfigureOperationModeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"j\n\x1d\x43onfigureOutputEnabledRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x0f\n\x07\x65nabled\x18\x03 \x01(\x08\"0\n\x1e\x43onfigureOutputEnabledResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"n\n\x1f\x43onfigureOutputImpedanceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\timpedance\x18\x03 \x01(\x01\"2\n ConfigureOutputImpedanceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x9f\x01\n\x1a\x43onfigureOutputModeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12.\n\x0boutput_mode\x18\x02 \x01(\x0e\x32\x17.nifgen_grpc.OutputModeH\x00\x12\x19\n\x0foutput_mode_raw\x18\x03 \x01(\x11H\x00\x42\x12\n\x10output_mode_enum\"-\n\x1b\x43onfigureOutputModeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"z\n/ConfigureP2PEndpointFullnessStartTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12#\n\x1bp2p_endpoint_fullness_level\x18\x02 \x01(\x11\"B\n0ConfigureP2PEndpointFullnessStartTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x87\x01\n\x1e\x43onfigureReferenceClockRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x1e\n\x16reference_clock_source\x18\x02 \x01(\t\x12!\n\x19reference_clock_frequency\x18\x03 \x01(\x01\"1\n\x1f\x43onfigureReferenceClockResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"d\n!ConfigureSampleClockSourceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x1b\n\x13sample_clock_source\x18\x02 \x01(\t\"4\n\"ConfigureSampleClockSourceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"U\n\x1a\x43onfigureSampleRateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x13\n\x0bsample_rate\x18\x02 \x01(\x01\"-\n\x1b\x43onfigureSampleRateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"c\n)ConfigureSoftwareEdgeScriptTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\ntrigger_id\x18\x02 \x01(\t\"<\n*ConfigureSoftwareEdgeScriptTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"N\n(ConfigureSoftwareEdgeStartTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\";\n)ConfigureSoftwareEdgeStartTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xfe\x01\n ConfigureStandardWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12)\n\x08waveform\x18\x03 \x01(\x0e\x32\x15.nifgen_grpc.WaveformH\x00\x12\x16\n\x0cwaveform_raw\x18\x04 \x01(\x11H\x00\x12\x11\n\tamplitude\x18\x05 \x01(\x01\x12\x11\n\tdc_offset\x18\x06 \x01(\x01\x12\x11\n\tfrequency\x18\x07 \x01(\x01\x12\x13\n\x0bstart_phase\x18\x08 \x01(\x01\x42\x0f\n\rwaveform_enum\"3\n!ConfigureStandardWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"{\n\x1f\x43onfigureSynchronizationRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1e\n\x16synchronization_source\x18\x03 \x01(\x11\"2\n ConfigureSynchronizationResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xba\x01\n\x1b\x43onfigureTriggerModeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x30\n\x0ctrigger_mode\x18\x03 \x01(\x0e\x32\x18.nifgen_grpc.TriggerModeH\x00\x12\x1a\n\x10trigger_mode_raw\x18\x04 \x01(\x11H\x00\x42\x13\n\x11trigger_mode_enum\".\n\x1c\x43onfigureTriggerModeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xbd\x01\n CreateAdvancedArbSequenceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x1e\n\x16waveform_handles_array\x18\x02 \x03(\x11\x12\x19\n\x11loop_counts_array\x18\x03 \x03(\x11\x12\x1b\n\x13sample_counts_array\x18\x04 \x03(\x11\x12\x1d\n\x15marker_location_array\x18\x05 \x03(\x11\"k\n!CreateAdvancedArbSequenceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1d\n\x15\x63oerced_markers_array\x18\x02 \x03(\x11\x12\x17\n\x0fsequence_handle\x18\x03 \x01(\x11\"y\n\x18\x43reateArbSequenceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x1e\n\x16waveform_handles_array\x18\x02 \x03(\x11\x12\x19\n\x11loop_counts_array\x18\x03 \x03(\x11\"D\n\x19\x43reateArbSequenceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fsequence_handle\x18\x02 \x01(\x11\"\xc0\x01\n\x15\x43reateFreqListRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12)\n\x08waveform\x18\x02 \x01(\x0e\x32\x15.nifgen_grpc.WaveformH\x00\x12\x16\n\x0cwaveform_raw\x18\x03 \x01(\x11H\x00\x12\x17\n\x0f\x66requency_array\x18\x04 \x03(\x01\x12\x16\n\x0e\x64uration_array\x18\x05 \x03(\x01\x42\x0f\n\rwaveform_enum\"G\n\x16\x43reateFreqListResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1d\n\x15\x66requency_list_handle\x18\x02 \x01(\x11\"\x98\x01\n\x1f\x43reateWaveformComplexF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12;\n\x13waveform_data_array\x18\x03 \x03(\x0b\x32\x1e.nidevice_grpc.NIComplexNumber\"K\n CreateWaveformComplexF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"q\n\x18\x43reateWaveformF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1b\n\x13waveform_data_array\x18\x03 \x03(\x01\"D\n\x19\x43reateWaveformF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"\xca\x01\n CreateWaveformFromFileF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\tfile_name\x18\x03 \x01(\t\x12,\n\nbyte_order\x18\x04 \x01(\x0e\x32\x16.nifgen_grpc.ByteOrderH\x00\x12\x18\n\x0e\x62yte_order_raw\x18\x05 \x01(\x11H\x00\x42\x11\n\x0f\x62yte_order_enum\"L\n!CreateWaveformFromFileF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"\xba\x01\n CreateWaveformFromFileHWSRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\tfile_name\x18\x03 \x01(\t\x12\x1e\n\x16use_rate_from_waveform\x18\x04 \x01(\x08\x12)\n!use_gain_and_offset_from_waveform\x18\x05 \x01(\x08\"L\n!CreateWaveformFromFileHWSResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"\xca\x01\n CreateWaveformFromFileI16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\tfile_name\x18\x03 \x01(\t\x12,\n\nbyte_order\x18\x04 \x01(\x0e\x32\x16.nifgen_grpc.ByteOrderH\x00\x12\x18\n\x0e\x62yte_order_raw\x18\x05 \x01(\x11H\x00\x42\x11\n\x0f\x62yte_order_enum\"L\n!CreateWaveformFromFileI16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"q\n\x18\x43reateWaveformI16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1b\n\x13waveform_data_array\x18\x03 \x03(\x11\"D\n\x19\x43reateWaveformI16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"z\n!DefineUserStandardWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1b\n\x13waveform_data_array\x18\x03 \x03(\x01\"4\n\"DefineUserStandardWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"m\n\x1a\x44\x65leteNamedWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\"-\n\x1b\x44\x65leteNamedWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"d\n\x13\x44\x65leteScriptRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x13\n\x0bscript_name\x18\x03 \x01(\t\"&\n\x14\x44\x65leteScriptResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"4\n\x0e\x44isableRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"!\n\x0f\x44isableResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"V\n\x1a\x44isableAnalogFilterRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"-\n\x1b\x44isableAnalogFilterResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"W\n\x1b\x44isableDigitalFilterRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\".\n\x1c\x44isableDigitalFilterResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"[\n\x1f\x44isableDigitalPatterningRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"2\n DisableDigitalPatterningResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"U\n\x1b\x44isableScriptTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\ntrigger_id\x18\x02 \x01(\t\".\n\x1c\x44isableScriptTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"@\n\x1a\x44isableStartTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"-\n\x1b\x44isableStartTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"z\n\x19\x45nableAnalogFilterRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12#\n\x1b\x66ilter_correction_frequency\x18\x03 \x01(\x01\",\n\x1a\x45nableAnalogFilterResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"V\n\x1a\x45nableDigitalFilterRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"-\n\x1b\x45nableDigitalFilterResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"Z\n\x1e\x45nableDigitalPatterningRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"1\n\x1f\x45nableDigitalPatterningResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"M\n\x13\x45rrorHandlerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nerror_code\x18\x02 \x01(\x11\"=\n\x14\x45rrorHandlerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"M\n\x13\x45rrorMessageRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nerror_code\x18\x02 \x01(\x11\"=\n\x14\x45rrorMessageResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"7\n\x11\x45rrorQueryRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"O\n\x12\x45rrorQueryResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x12\n\nerror_code\x18\x02 \x01(\x11\x12\x15\n\rerror_message\x18\x03 \x01(\t\"O\n)ExportAttributeConfigurationBufferRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"S\n*ExportAttributeConfigurationBufferResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rconfiguration\x18\x02 \x01(\x0c\"`\n\'ExportAttributeConfigurationFileRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x11\n\tfile_path\x18\x02 \x01(\t\":\n(ExportAttributeConfigurationFileResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb9\x01\n\x13\x45xportSignalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12%\n\x06signal\x18\x02 \x01(\x0e\x32\x13.nifgen_grpc.SignalH\x00\x12\x14\n\nsignal_raw\x18\x03 \x01(\x11H\x00\x12\x19\n\x11signal_identifier\x18\x04 \x01(\t\x12\x17\n\x0foutput_terminal\x18\x05 \x01(\tB\r\n\x0bsignal_enum\"&\n\x14\x45xportSignalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8c\x01\n\x1cGetAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"H\n\x1dGetAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\x08\"\x8a\x01\n\x1aGetAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"F\n\x1bGetAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\x11\"\x8a\x01\n\x1aGetAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"F\n\x1bGetAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\x03\"\x8b\x01\n\x1bGetAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"G\n\x1cGetAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\x01\"\x8c\x01\n\x1cGetAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"`\n\x1dGetAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12/\n\x0f\x61ttribute_value\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x8b\x01\n\x1bGetAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"G\n\x1cGetAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\t\"J\n\x15GetChannelNameRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\r\n\x05index\x18\x02 \x01(\x11\"@\n\x16GetChannelNameResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x16\n\x0e\x63hannel_string\x18\x02 \x01(\t\"5\n\x0fGetErrorRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"Q\n\x10GetErrorResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x12\n\nerror_code\x18\x02 \x01(\x11\x12\x19\n\x11\x65rror_description\x18\x03 \x01(\t\"E\n\x1fGetExtCalLastDateAndTimeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"z\n GetExtCalLastDateAndTimeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04year\x18\x02 \x01(\x11\x12\r\n\x05month\x18\x03 \x01(\x11\x12\x0b\n\x03\x64\x61y\x18\x04 \x01(\x11\x12\x0c\n\x04hour\x18\x05 \x01(\x11\x12\x0e\n\x06minute\x18\x06 \x01(\x11\">\n\x18GetExtCalLastTempRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"@\n\x19GetExtCalLastTempResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"I\n#GetExtCalRecommendedIntervalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"F\n$GetExtCalRecommendedIntervalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06months\x18\x02 \x01(\x11\"[\n\x1fGetFIRFilterCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"s\n GetFIRFilterCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1a\n\x12\x63oefficients_array\x18\x02 \x03(\x01\x12#\n\x1bnumber_of_coefficients_read\x18\x03 \x01(\x11\"=\n\x17GetHardwareStateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"h\n\x18GetHardwareStateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12)\n\x05state\x18\x02 \x01(\x0e\x32\x1a.nifgen_grpc.HardwareState\x12\x11\n\tstate_raw\x18\x03 \x01(\x11\"B\n\x1cGetNextCoercionRecordRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"H\n\x1dGetNextCoercionRecordResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x63oercion_record\x18\x02 \x01(\t\"F\n GetNextInterchangeWarningRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"P\n!GetNextInterchangeWarningResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1b\n\x13interchange_warning\x18\x02 \x01(\t\"F\n GetSelfCalLastDateAndTimeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"{\n!GetSelfCalLastDateAndTimeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04year\x18\x02 \x01(\x11\x12\r\n\x05month\x18\x03 \x01(\x11\x12\x0b\n\x03\x64\x61y\x18\x04 \x01(\x11\x12\x0c\n\x04hour\x18\x05 \x01(\x11\x12\x0e\n\x06minute\x18\x06 \x01(\x11\"?\n\x19GetSelfCalLastTempRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"A\n\x1aGetSelfCalLastTempResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"@\n\x1aGetSelfCalSupportedRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"I\n\x1bGetSelfCalSupportedResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1a\n\x12self_cal_supported\x18\x02 \x01(\x08\"]\n\x1eGetStreamEndpointHandleRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x17\n\x0fstream_endpoint\x18\x02 \x01(\t\"H\n\x1fGetStreamEndpointHandleResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rreader_handle\x18\x02 \x01(\r\"f\n)ImportAttributeConfigurationBufferRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x15\n\rconfiguration\x18\x02 \x01(\x0c\"<\n*ImportAttributeConfigurationBufferResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"`\n\'ImportAttributeConfigurationFileRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x11\n\tfile_path\x18\x02 \x01(\t\":\n(ImportAttributeConfigurationFileResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb1\x01\n\x0bInitRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x10\n\x08id_query\x18\x03 \x01(\x08\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12M\n\x17initialization_behavior\x18\x05 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"~\n\x0cInitResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"\xd3\x01\n\x16InitWithOptionsRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x10\n\x08id_query\x18\x03 \x01(\x08\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12\x15\n\roption_string\x18\x05 \x01(\t\x12M\n\x17initialization_behavior\x18\x06 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"\x89\x01\n\x17InitWithOptionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"\xde\x01\n\x1dInitializeWithChannelsRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x14\n\x0c\x63hannel_name\x18\x03 \x01(\t\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12\x15\n\roption_string\x18\x05 \x01(\t\x12M\n\x17initialization_behavior\x18\x06 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"\x90\x01\n\x1eInitializeWithChannelsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"?\n\x19InitiateGenerationRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\",\n\x1aInitiateGenerationResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"D\n\x1eInvalidateAllAttributesRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"1\n\x1fInvalidateAllAttributesResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"3\n\rIsDoneRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\".\n\x0eIsDoneResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04\x64one\x18\x02 \x01(\x08\"Y\n\x1cManualEnableP2PStreamRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x15\n\rendpoint_name\x18\x02 \x01(\t\"/\n\x1dManualEnableP2PStreamResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"D\n\x1eQueryArbSeqCapabilitiesRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\xb4\x01\n\x1fQueryArbSeqCapabilitiesResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12#\n\x1bmaximum_number_of_sequences\x18\x02 \x01(\x11\x12\x1f\n\x17minimum_sequence_length\x18\x03 \x01(\x11\x12\x1f\n\x17maximum_sequence_length\x18\x04 \x01(\x11\x12\x1a\n\x12maximum_loop_count\x18\x05 \x01(\x11\"D\n\x1eQueryArbWfmCapabilitiesRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\xae\x01\n\x1fQueryArbWfmCapabilitiesResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12#\n\x1bmaximum_number_of_waveforms\x18\x02 \x01(\x11\x12\x18\n\x10waveform_quantum\x18\x03 \x01(\x11\x12\x1d\n\x15minimum_waveform_size\x18\x04 \x01(\x11\x12\x1d\n\x15maximum_waveform_size\x18\x05 \x01(\x11\"F\n QueryFreqListCapabilitiesRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\xa2\x02\n!QueryFreqListCapabilitiesResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12$\n\x1cmaximum_number_of_freq_lists\x18\x02 \x01(\x11\x12%\n\x1dminimum_frequency_list_length\x18\x03 \x01(\x11\x12%\n\x1dmaximum_frequency_list_length\x18\x04 \x01(\x11\x12\'\n\x1fminimum_frequency_list_duration\x18\x05 \x01(\x01\x12\'\n\x1fmaximum_frequency_list_duration\x18\x06 \x01(\x01\x12\'\n\x1f\x66requency_list_duration_quantum\x18\x07 \x01(\x01\"C\n\x1dReadCurrentTemperatureRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"E\n\x1eReadCurrentTemperatureResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"2\n\x0cResetRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rResetResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x85\x01\n\x15ResetAttributeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"(\n\x16ResetAttributeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"8\n\x12ResetDeviceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"%\n\x13ResetDeviceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"B\n\x1cResetInterchangeCheckRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"/\n\x1dResetInterchangeCheckResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\">\n\x18ResetWithDefaultsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"+\n\x19ResetWithDefaultsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\":\n\x14RevisionQueryRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"f\n\x15RevisionQueryResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x1ainstrument_driver_revision\x18\x02 \x01(\t\x12\x19\n\x11\x66irmware_revision\x18\x03 \x01(\t\"\xb5\x02\n\x15RouteSignalOutRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x39\n\x11route_signal_from\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.RouteSignalFromH\x00\x12\x1f\n\x15route_signal_from_raw\x18\x04 \x01(\x11H\x00\x12\x35\n\x0froute_signal_to\x18\x05 \x01(\x0e\x32\x1a.nifgen_grpc.RouteSignalToH\x01\x12\x1d\n\x13route_signal_to_raw\x18\x06 \x01(\x11H\x01\x42\x18\n\x16route_signal_from_enumB\x16\n\x14route_signal_to_enum\"(\n\x16RouteSignalOutResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"4\n\x0eSelfCalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"!\n\x0fSelfCalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"5\n\x0fSelfTestRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"W\n\x10SelfTestResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x18\n\x10self_test_result\x18\x02 \x01(\x11\x12\x19\n\x11self_test_message\x18\x03 \x01(\t\"\xa8\x01\n\x1eSendSoftwareEdgeTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\'\n\x07trigger\x18\x02 \x01(\x0e\x32\x14.nifgen_grpc.TriggerH\x00\x12\x15\n\x0btrigger_raw\x18\x03 \x01(\x11H\x00\x12\x12\n\ntrigger_id\x18\x04 \x01(\tB\x0e\n\x0ctrigger_enum\"1\n\x1fSendSoftwareEdgeTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa5\x01\n\x1cSetAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x17\n\x0f\x61ttribute_value\x18\x04 \x01(\x08\"/\n\x1dSetAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x85\x02\n\x1aSetAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x42\n\x0f\x61ttribute_value\x18\x04 \x01(\x0e\x32\'.nifgen_grpc.NiFgenInt32AttributeValuesH\x00\x12\x1d\n\x13\x61ttribute_value_raw\x18\x05 \x01(\x11H\x00\x42\x16\n\x14\x61ttribute_value_enum\"-\n\x1bSetAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa7\x01\n\x1aSetAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x1b\n\x13\x61ttribute_value_raw\x18\x04 \x01(\x03\"-\n\x1bSetAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x87\x02\n\x1bSetAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x43\n\x0f\x61ttribute_value\x18\x04 \x01(\x0e\x32(.nifgen_grpc.NiFgenReal64AttributeValuesH\x00\x12\x1d\n\x13\x61ttribute_value_raw\x18\x05 \x01(\x01H\x00\x42\x16\n\x14\x61ttribute_value_enum\".\n\x1cSetAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xbd\x01\n\x1cSetAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12/\n\x0f\x61ttribute_value\x18\x04 \x01(\x0b\x32\x16.nidevice_grpc.Session\"/\n\x1dSetAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x94\x02\n\x1bSetAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x1d\n\x13\x61ttribute_value_raw\x18\x04 \x01(\tH\x00\x12P\n\x16\x61ttribute_value_mapped\x18\x05 \x01(\x0e\x32..nifgen_grpc.NiFgenStringAttributeValuesMappedH\x00\x42\x16\n\x14\x61ttribute_value_enum\".\n\x1cSetAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xea\x01\n(SetNamedWaveformNextWritePositionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12.\n\x0brelative_to\x18\x04 \x01(\x0e\x32\x17.nifgen_grpc.RelativeToH\x00\x12\x19\n\x0frelative_to_raw\x18\x05 \x01(\x11H\x00\x12\x0e\n\x06offset\x18\x06 \x01(\x11\x42\x12\n\x10relative_to_enum\";\n)SetNamedWaveformNextWritePositionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xe7\x01\n#SetWaveformNextWritePositionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fwaveform_handle\x18\x03 \x01(\x11\x12.\n\x0brelative_to\x18\x04 \x01(\x0e\x32\x17.nifgen_grpc.RelativeToH\x00\x12\x19\n\x0frelative_to_raw\x18\x05 \x01(\x11H\x00\x12\x0e\n\x06offset\x18\x06 \x01(\x11\x42\x12\n\x10relative_to_enum\"6\n$SetWaveformNextWritePositionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"L\n\x14WaitUntilDoneRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x10\n\x08max_time\x18\x02 \x01(\x11\"\'\n\x15WaitUntilDoneResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x7f\n\x1cWriteBinary16WaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fwaveform_handle\x18\x03 \x01(\x11\x12\x0c\n\x04\x64\x61ta\x18\x04 \x03(\x11\"/\n\x1dWriteBinary16WaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa3\x01\n#WriteComplexBinary16WaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fwaveform_handle\x18\x03 \x01(\x11\x12)\n\x04\x64\x61ta\x18\x04 \x03(\x0b\x32\x1b.nidevice_grpc.NIComplexI16\"6\n$WriteComplexBinary16WaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa4\x01\n#WriteNamedWaveformComplexF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12,\n\x04\x64\x61ta\x18\x04 \x03(\x0b\x32\x1e.nidevice_grpc.NIComplexNumber\"6\n$WriteNamedWaveformComplexF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa1\x01\n#WriteNamedWaveformComplexI16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12)\n\x04\x64\x61ta\x18\x04 \x03(\x0b\x32\x1b.nidevice_grpc.NIComplexI16\"6\n$WriteNamedWaveformComplexI16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"}\n\x1cWriteNamedWaveformF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x03(\x01\"/\n\x1dWriteNamedWaveformF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"}\n\x1cWriteNamedWaveformI16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x03(\x11\"/\n\x1dWriteNamedWaveformI16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"n\n\x1aWriteP2PEndpointI16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x15\n\rendpoint_name\x18\x02 \x01(\t\x12\x15\n\rendpoint_data\x18\x03 \x03(\x11\"-\n\x1bWriteP2PEndpointI16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"^\n\x12WriteScriptRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x0e\n\x06script\x18\x03 \x01(\t\"%\n\x13WriteScriptResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"w\n\x14WriteWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fwaveform_handle\x18\x03 \x01(\x11\x12\x0c\n\x04\x64\x61ta\x18\x04 \x03(\x01\"\'\n\x15WriteWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa1\x01\n\x1eWriteWaveformComplexF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12,\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32\x1e.nidevice_grpc.NIComplexNumber\x12\x17\n\x0fwaveform_handle\x18\x04 \x01(\x11\"1\n\x1fWriteWaveformComplexF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05*\xa9S\n\x0fNiFgenAttribute\x12 \n\x1cNIFGEN_ATTRIBUTE_UNSPECIFIED\x10\x00\x12\"\n\x1cNIFGEN_ATTRIBUTE_RANGE_CHECK\x10\x92\x8b@\x12.\n(NIFGEN_ATTRIBUTE_QUERY_INSTRUMENT_STATUS\x10\x93\x8b@\x12\x1c\n\x16NIFGEN_ATTRIBUTE_CACHE\x10\x94\x8b@\x12\x1f\n\x19NIFGEN_ATTRIBUTE_SIMULATE\x10\x95\x8b@\x12\'\n!NIFGEN_ATTRIBUTE_RECORD_COERCIONS\x10\x96\x8b@\x12#\n\x1dNIFGEN_ATTRIBUTE_DRIVER_SETUP\x10\x97\x8b@\x12(\n\"NIFGEN_ATTRIBUTE_INTERCHANGE_CHECK\x10\xa5\x8b@\x12$\n\x1eNIFGEN_ATTRIBUTE_CHANNEL_COUNT\x10\xdb\x8c@\x12-\n\'NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_PREFIX\x10\xbe\x8d@\x12-\n\'NIFGEN_ATTRIBUTE_IO_RESOURCE_DESCRIPTOR\x10\xc0\x8d@\x12#\n\x1dNIFGEN_ATTRIBUTE_LOGICAL_NAME\x10\xc1\x8d@\x12\x32\n,NIFGEN_ATTRIBUTE_SUPPORTED_INSTRUMENT_MODELS\x10\xd7\x8d@\x12)\n#NIFGEN_ATTRIBUTE_GROUP_CAPABILITIES\x10\xa1\x8e@\x12\x34\n.NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_MAJOR_VERSION\x10\x87\x8f@\x12\x34\n.NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_MINOR_VERSION\x10\x88\x8f@\x12\x33\n-NIFGEN_ATTRIBUTE_INSTRUMENT_FIRMWARE_REVISION\x10\x8e\x8f@\x12.\n(NIFGEN_ATTRIBUTE_INSTRUMENT_MANUFACTURER\x10\x8f\x8f@\x12\'\n!NIFGEN_ATTRIBUTE_INSTRUMENT_MODEL\x10\x90\x8f@\x12-\n\'NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_VENDOR\x10\x91\x8f@\x12\x32\n,NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_DESCRIPTION\x10\x92\x8f@\x12?\n9NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_CLASS_SPEC_MAJOR_VERSION\x10\x93\x8f@\x12?\n9NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_CLASS_SPEC_MINOR_VERSION\x10\x94\x8f@\x12/\n)NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_REVISION\x10\xb7\x8f@\x12(\n\"NIFGEN_ATTRIBUTE_ID_QUERY_RESPONSE\x10\xb1\x98\x46\x12.\n(NIFGEN_ATTRIBUTE_DIGITAL_PATTERN_ENABLED\x10\x95\x99\x46\x12-\n\'NIFGEN_ATTRIBUTE_DIGITAL_FILTER_ENABLED\x10\x96\x99\x46\x12,\n&NIFGEN_ATTRIBUTE_ANALOG_FILTER_ENABLED\x10\x97\x99\x46\x12\x32\n,NIFGEN_ATTRIBUTE_FILTER_CORRECTION_FREQUENCY\x10\x98\x99\x46\x12+\n%NIFGEN_ATTRIBUTE_SYNC_DUTY_CYCLE_HIGH\x10\x99\x99\x46\x12*\n$NIFGEN_ATTRIBUTE_UPDATE_CLOCK_SOURCE\x10\x9a\x99\x46\x12*\n$NIFGEN_ATTRIBUTE_REF_CLOCK_FREQUENCY\x10\x9b\x99\x46\x12#\n\x1dNIFGEN_ATTRIBUTE_TRIGGER_MODE\x10\x9c\x99\x46\x12!\n\x1bNIFGEN_ATTRIBUTE_CLOCK_MODE\x10\x9e\x99\x46\x12&\n NIFGEN_ATTRIBUTE_SYNCHRONIZATION\x10\x9f\x99\x46\x12*\n$NIFGEN_ATTRIBUTE_SAMPLE_CLOCK_SOURCE\x10\xa0\x99\x46\x12-\n\'NIFGEN_ATTRIBUTE_REFERENCE_CLOCK_SOURCE\x10\xa1\x99\x46\x12\'\n!NIFGEN_ATTRIBUTE_FREQ_LIST_HANDLE\x10\x80\x9a\x46\x12)\n#NIFGEN_ATTRIBUTE_MAX_NUM_FREQ_LISTS\x10\x81\x9a\x46\x12+\n%NIFGEN_ATTRIBUTE_MIN_FREQ_LIST_LENGTH\x10\x82\x9a\x46\x12+\n%NIFGEN_ATTRIBUTE_MAX_FREQ_LIST_LENGTH\x10\x83\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_MIN_FREQ_LIST_DURATION\x10\x84\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_MAX_FREQ_LIST_DURATION\x10\x85\x9a\x46\x12\x31\n+NIFGEN_ATTRIBUTE_FREQ_LIST_DURATION_QUANTUM\x10\x86\x9a\x46\x12\x1f\n\x19NIFGEN_ATTRIBUTE_BUS_TYPE\x10\x87\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_VIDEO_WAVEFORM_TYPE\x10\x88\x9a\x46\x12:\n4NIFGEN_ATTRIBUTE_DIGITAL_FILTER_INTERPOLATION_FACTOR\x10\x8a\x9a\x46\x12\x34\n.NIFGEN_ATTRIBUTE_EXPORTED_SAMPLE_CLOCK_DIVISOR\x10\x8b\x9a\x46\x12%\n\x1fNIFGEN_ATTRIBUTE_LOAD_IMPEDANCE\x10\x8c\x9a\x46\x12\"\n\x1cNIFGEN_ATTRIBUTE_ANALOG_PATH\x10\x8e\x9a\x46\x12%\n\x1fNIFGEN_ATTRIBUTE_GAIN_DAC_VALUE\x10\x8f\x9a\x46\x12\'\n!NIFGEN_ATTRIBUTE_OFFSET_DAC_VALUE\x10\x90\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_OSCILLATOR_FREQ_DAC_VALUE\x10\x91\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_PRE_AMPLIFIER_ATTENUATION\x10\x94\x9a\x46\x12\x31\n+NIFGEN_ATTRIBUTE_POST_AMPLIFIER_ATTENUATION\x10\x95\x9a\x46\x12=\n7NIFGEN_ATTRIBUTE_EXPORTED_SAMPLE_CLOCK_TIMEBASE_DIVISOR\x10\x96\x9a\x46\x12\x32\n,NIFGEN_ATTRIBUTE_SAMPLE_CLOCK_ABSOLUTE_DELAY\x10\x97\x9a\x46\x12\x31\n+NIFGEN_ATTRIBUTE_OSCILLATOR_PHASE_DAC_VALUE\x10\x98\x9a\x46\x12\x38\n2NIFGEN_ATTRIBUTE_EXTERNAL_CLOCK_DELAY_BINARY_VALUE\x10\x99\x9a\x46\x12\'\n!NIFGEN_ATTRIBUTE_ANALOG_DATA_MASK\x10\x9a\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_ANALOG_STATIC_VALUE\x10\x9b\x9a\x46\x12(\n\"NIFGEN_ATTRIBUTE_DIGITAL_DATA_MASK\x10\x9c\x9a\x46\x12+\n%NIFGEN_ATTRIBUTE_DIGITAL_STATIC_VALUE\x10\x9d\x9a\x46\x12\'\n!NIFGEN_ATTRIBUTE_FUNC_BUFFER_SIZE\x10\x9e\x9a\x46\x12+\n%NIFGEN_ATTRIBUTE_FUNC_MAX_BUFFER_SIZE\x10\x9f\x9a\x46\x12/\n)NIFGEN_ATTRIBUTE_FILE_TRANSFER_BLOCK_SIZE\x10\xa0\x9a\x46\x12/\n)NIFGEN_ATTRIBUTE_DATA_TRANSFER_BLOCK_SIZE\x10\xa1\x9a\x46\x12\"\n\x1cNIFGEN_ATTRIBUTE_MEMORY_SIZE\x10\xa2\x9a\x46\x12$\n\x1eNIFGEN_ATTRIBUTE_SERIAL_NUMBER\x10\xa3\x9a\x46\x12)\n#NIFGEN_ATTRIBUTE_DIRECT_DMA_ENABLED\x10\xa4\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_DIRECT_DMA_WINDOW_SIZE\x10\xa5\x9a\x46\x12\"\n\x1cNIFGEN_ATTRIBUTE_OSP_ENABLED\x10\xa6\x9a\x46\x12/\n)NIFGEN_ATTRIBUTE_OSP_DATA_PROCESSING_MODE\x10\xa7\x9a\x46\x12\"\n\x1cNIFGEN_ATTRIBUTE_OSP_IQ_RATE\x10\xa8\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_CARRIER_ENABLED\x10\xa9\x9a\x46\x12,\n&NIFGEN_ATTRIBUTE_OSP_CARRIER_FREQUENCY\x10\xaa\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_CARRIER_PHASE_I\x10\xab\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_CARRIER_PHASE_Q\x10\xac\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_TYPE\x10\xad\x9a\x46\x12#\n\x1dNIFGEN_ATTRIBUTE_DIGITAL_GAIN\x10\xae\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_ENABLED\x10\xaf\x9a\x46\x12\x33\n-NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_INTERPOLATION\x10\xb0\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_OSP_CIC_FILTER_ENABLED\x10\xb1\x9a\x46\x12\x33\n-NIFGEN_ATTRIBUTE_OSP_CIC_FILTER_INTERPOLATION\x10\xb2\x9a\x46\x12>\n8NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_ROOT_RAISED_COSINE_ALPHA\x10\xb3\x9a\x46\x12\x39\n3NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_RAISED_COSINE_ALPHA\x10\xb4\x9a\x46\x12\x33\n-NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_FLAT_PASSBAND\x10\xb5\x9a\x46\x12\x31\n+NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_GAUSSIAN_BT\x10\xb6\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_CIC_FILTER_GAIN\x10\xb7\x9a\x46\x12,\n&NIFGEN_ATTRIBUTE_OSP_PRE_FILTER_GAIN_I\x10\xb8\x9a\x46\x12,\n&NIFGEN_ATTRIBUTE_OSP_PRE_FILTER_GAIN_Q\x10\xb9\x9a\x46\x12.\n(NIFGEN_ATTRIBUTE_OSP_PRE_FILTER_OFFSET_I\x10\xba\x9a\x46\x12.\n(NIFGEN_ATTRIBUTE_OSP_PRE_FILTER_OFFSET_Q\x10\xbb\x9a\x46\x12\x33\n-NIFGEN_ATTRIBUTE_OSP_OVERFLOW_ERROR_REPORTING\x10\xbc\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_OVERFLOW_STATUS\x10\xbd\x9a\x46\x12)\n#NIFGEN_ATTRIBUTE_SCRIPT_TO_GENERATE\x10\xbe\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_MARKER_EVENTS_COUNT\x10\xbf\x9a\x46\x12,\n&NIFGEN_ATTRIBUTE_SCRIPT_TRIGGERS_COUNT\x10\xc0\x9a\x46\x12/\n)NIFGEN_ATTRIBUTE_DATA_MARKER_EVENTS_COUNT\x10\xc1\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_DIRECT_DMA_WINDOW_ADDRESS\x10\xc2\x9a\x46\x12)\n#NIFGEN_ATTRIBUTE_START_TRIGGER_TYPE\x10\xc8\x9a\x46\x12\x38\n2NIFGEN_ATTRIBUTE_DIGITAL_EDGE_START_TRIGGER_SOURCE\x10\xc9\x9a\x46\x12\x36\n0NIFGEN_ATTRIBUTE_DIGITAL_EDGE_START_TRIGGER_EDGE\x10\xca\x9a\x46\x12=\n7NIFGEN_ATTRIBUTE_EXPORTED_START_TRIGGER_OUTPUT_TERMINAL\x10\xcb\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_SCRIPT_TRIGGER_TYPE\x10\xd2\x9a\x46\x12\x39\n3NIFGEN_ATTRIBUTE_DIGITAL_EDGE_SCRIPT_TRIGGER_SOURCE\x10\xd3\x9a\x46\x12\x37\n1NIFGEN_ATTRIBUTE_DIGITAL_EDGE_SCRIPT_TRIGGER_EDGE\x10\xd4\x9a\x46\x12:\n4NIFGEN_ATTRIBUTE_DIGITAL_LEVEL_SCRIPT_TRIGGER_SOURCE\x10\xd5\x9a\x46\x12@\n:NIFGEN_ATTRIBUTE_DIGITAL_LEVEL_SCRIPT_TRIGGER_ACTIVE_LEVEL\x10\xd6\x9a\x46\x12>\n8NIFGEN_ATTRIBUTE_EXPORTED_SCRIPT_TRIGGER_OUTPUT_TERMINAL\x10\xd7\x9a\x46\x12<\n6NIFGEN_ATTRIBUTE_READY_FOR_START_EVENT_OUTPUT_TERMINAL\x10\xe6\x9a\x46\x12?\n9NIFGEN_ATTRIBUTE_READY_FOR_START_EVENT_LEVEL_ACTIVE_LEVEL\x10\xe7\x9a\x46\x12\x33\n-NIFGEN_ATTRIBUTE_MARKER_EVENT_OUTPUT_TERMINAL\x10\xe8\x9a\x46\x12\x32\n,NIFGEN_ATTRIBUTE_MARKER_EVENT_PULSE_POLARITY\x10\xe9\x9a\x46\x12\x34\n.NIFGEN_ATTRIBUTE_STARTED_EVENT_OUTPUT_TERMINAL\x10\xea\x9a\x46\x12\x31\n+NIFGEN_ATTRIBUTE_DONE_EVENT_OUTPUT_TERMINAL\x10\xeb\x9a\x46\x12\x37\n1NIFGEN_ATTRIBUTE_STARTED_EVENT_LEVEL_ACTIVE_LEVEL\x10\xec\x9a\x46\x12\x34\n.NIFGEN_ATTRIBUTE_DONE_EVENT_LEVEL_ACTIVE_LEVEL\x10\xed\x9a\x46\x12\x33\n-NIFGEN_ATTRIBUTE_STARTED_EVENT_PULSE_POLARITY\x10\xee\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_DONE_EVENT_PULSE_POLARITY\x10\xef\x9a\x46\x12<\n6NIFGEN_ATTRIBUTE_EXPORTED_SAMPLE_CLOCK_OUTPUT_TERMINAL\x10\xf0\x9a\x46\x12?\n9NIFGEN_ATTRIBUTE_EXPORTED_REFERENCE_CLOCK_OUTPUT_TERMINAL\x10\xf1\x9a\x46\x12G\nANIFGEN_ATTRIBUTE_EXPORTED_ONBOARD_REFERENCE_CLOCK_OUTPUT_TERMINAL\x10\xf2\x9a\x46\x12\x32\n,NIFGEN_ATTRIBUTE_FLATNESS_CORRECTION_ENABLED\x10\xf3\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_STREAMING_WAVEFORM_HANDLE\x10\xf4\x9a\x46\x12<\n6NIFGEN_ATTRIBUTE_STREAMING_SPACE_AVAILABLE_IN_WAVEFORM\x10\xf5\x9a\x46\x12.\n(NIFGEN_ATTRIBUTE_STREAMING_WAVEFORM_NAME\x10\xf6\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_ARB_MARKER_POSITION\x10\xf7\x9a\x46\x12\'\n!NIFGEN_ATTRIBUTE_ARB_REPEAT_COUNT\x10\xf8\x9a\x46\x12\x45\n?NIFGEN_ATTRIBUTE_EXPORTED_SAMPLE_CLOCK_TIMEBASE_OUTPUT_TERMINAL\x10\xf9\x9a\x46\x12/\n)NIFGEN_ATTRIBUTE_SYNC_OUT_OUTPUT_TERMINAL\x10\xfa\x9a\x46\x12\x34\n.NIFGEN_ATTRIBUTE_STARTED_EVENT_OUTPUT_BEHAVIOR\x10\xfb\x9a\x46\x12\x31\n+NIFGEN_ATTRIBUTE_DONE_EVENT_OUTPUT_BEHAVIOR\x10\xfc\x9a\x46\x12\x36\n0NIFGEN_ATTRIBUTE_STARTED_EVENT_PULSE_WIDTH_UNITS\x10\xfd\x9a\x46\x12\x33\n-NIFGEN_ATTRIBUTE_DONE_EVENT_PULSE_WIDTH_UNITS\x10\xfe\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_STARTED_EVENT_PULSE_WIDTH\x10\xff\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_DONE_EVENT_PULSE_WIDTH\x10\x80\x9b\x46\x12\x38\n2NIFGEN_ATTRIBUTE_DATA_MARKER_EVENT_DATA_BIT_NUMBER\x10\x81\x9b\x46\x12\x37\n1NIFGEN_ATTRIBUTE_DATA_MARKER_EVENT_LEVEL_POLARITY\x10\x82\x9b\x46\x12\x38\n2NIFGEN_ATTRIBUTE_DATA_MARKER_EVENT_OUTPUT_TERMINAL\x10\x83\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_MARKER_EVENT_PULSE_WIDTH\x10\x84\x9b\x46\x12\x35\n/NIFGEN_ATTRIBUTE_MARKER_EVENT_PULSE_WIDTH_UNITS\x10\x85\x9b\x46\x12\x33\n-NIFGEN_ATTRIBUTE_MARKER_EVENT_OUTPUT_BEHAVIOR\x10\x86\x9b\x46\x12\x38\n2NIFGEN_ATTRIBUTE_MARKER_EVENT_TOGGLE_INITIAL_STATE\x10\x87\x9b\x46\x12\x34\n.NIFGEN_ATTRIBUTE_ALL_MARKER_EVENTS_LIVE_STATUS\x10\x88\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_MARKER_EVENT_LIVE_STATUS\x10\x89\x9b\x46\x12\x38\n2NIFGEN_ATTRIBUTE_READY_FOR_START_EVENT_LIVE_STATUS\x10\x8c\x9b\x46\x12\x37\n1NIFGEN_ATTRIBUTE_ALL_MARKER_EVENTS_LATCHED_STATUS\x10\x8d\x9b\x46\x12\x32\n,NIFGEN_ATTRIBUTE_MARKER_EVENT_LATCHED_STATUS\x10\x8e\x9b\x46\x12\x30\n*NIFGEN_ATTRIBUTE_DONE_EVENT_LATCHED_STATUS\x10\x8f\x9b\x46\x12\x33\n-NIFGEN_ATTRIBUTE_STARTED_EVENT_LATCHED_STATUS\x10\x90\x9b\x46\x12)\n#NIFGEN_ATTRIBUTE_MARKER_EVENT_DELAY\x10\x92\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_MARKER_EVENT_DELAY_UNITS\x10\x93\x9b\x46\x12*\n$NIFGEN_ATTRIBUTE_STARTED_EVENT_DELAY\x10\x94\x9b\x46\x12\x30\n*NIFGEN_ATTRIBUTE_STARTED_EVENT_DELAY_UNITS\x10\x95\x9b\x46\x12\'\n!NIFGEN_ATTRIBUTE_DONE_EVENT_DELAY\x10\x96\x9b\x46\x12-\n\'NIFGEN_ATTRIBUTE_DONE_EVENT_DELAY_UNITS\x10\x97\x9b\x46\x12\x34\n.NIFGEN_ATTRIBUTE_PCI_DMA_OPTIMIZATIONS_ENABLED\x10\x9a\x9b\x46\x12-\n\'NIFGEN_ATTRIBUTE_TERMINAL_CONFIGURATION\x10\x9d\x9b\x46\x12)\n#NIFGEN_ATTRIBUTE_COMMON_MODE_OFFSET\x10\x9e\x9b\x46\x12\x33\n-NIFGEN_ATTRIBUTE_SAMPLE_CLOCK_TIMEBASE_SOURCE\x10\x9f\x9b\x46\x12\x31\n+NIFGEN_ATTRIBUTE_SAMPLE_CLOCK_TIMEBASE_RATE\x10\xa0\x9b\x46\x12$\n\x1eNIFGEN_ATTRIBUTE_CHANNEL_DELAY\x10\xa1\x9b\x46\x12\x1f\n\x19NIFGEN_ATTRIBUTE_OSP_MODE\x10\xa2\x9b\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_FREQUENCY_SHIFT\x10\xa3\x9b\x46\x12\x36\n0NIFGEN_ATTRIBUTE_DATA_TRANSFER_MAXIMUM_BANDWIDTH\x10\xa5\x9b\x46\x12:\n4NIFGEN_ATTRIBUTE_DATA_TRANSFER_PREFERRED_PACKET_SIZE\x10\xa6\x9b\x46\x12<\n6NIFGEN_ATTRIBUTE_DATA_TRANSFER_MAXIMUM_IN_FLIGHT_READS\x10\xa7\x9b\x46\x12\x37\n1NIFGEN_ATTRIBUTE_EXTERNAL_SAMPLE_CLOCK_MULTIPLIER\x10\xa8\x9b\x46\x12$\n\x1eNIFGEN_ATTRIBUTE_IDLE_BEHAVIOR\x10\xa9\x9b\x46\x12!\n\x1bNIFGEN_ATTRIBUTE_IDLE_VALUE\x10\xaa\x9b\x46\x12$\n\x1eNIFGEN_ATTRIBUTE_WAIT_BEHAVIOR\x10\xab\x9b\x46\x12!\n\x1bNIFGEN_ATTRIBUTE_WAIT_VALUE\x10\xac\x9b\x46\x12<\n6NIFGEN_ATTRIBUTE_OSP_COMPENSATE_FOR_FILTER_GROUP_DELAY\x10\xb5\x9b\x46\x12&\n NIFGEN_ATTRIBUTE_MODULE_REVISION\x10\xb6\x9b\x46\x12\"\n\x1cNIFGEN_ATTRIBUTE_P2P_ENABLED\x10\xb7\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_P2P_DESTINATION_CHANNELS\x10\xb8\x9b\x46\x12(\n\"NIFGEN_ATTRIBUTE_P2P_ENDPOINT_SIZE\x10\xb9\x9b\x46\x12\x36\n0NIFGEN_ATTRIBUTE_P2P_SPACE_AVAILABLE_IN_ENDPOINT\x10\xba\x9b\x46\x12;\n5NIFGEN_ATTRIBUTE_P2P_MOST_SPACE_AVAILABLE_IN_ENDPOINT\x10\xbb\x9b\x46\x12)\n#NIFGEN_ATTRIBUTE_P2P_ENDPOINT_COUNT\x10\xbc\x9b\x46\x12\x37\n1NIFGEN_ATTRIBUTE_P2P_MANUAL_CONFIGURATION_ENABLED\x10\xbd\x9b\x46\x12;\n5NIFGEN_ATTRIBUTE_P2P_DATA_TRANSFER_PERMISSION_ADDRESS\x10\xbe\x9b\x46\x12@\n:NIFGEN_ATTRIBUTE_P2P_DATA_TRANSFER_PERMISSION_ADDRESS_TYPE\x10\xbf\x9b\x46\x12<\n6NIFGEN_ATTRIBUTE_P2P_DATA_TRANSFER_PERMISSION_INTERVAL\x10\xc0\x9b\x46\x12\x32\n,NIFGEN_ATTRIBUTE_P2P_ENDPOINT_WINDOW_ADDRESS\x10\xc1\x9b\x46\x12\x37\n1NIFGEN_ATTRIBUTE_P2P_ENDPOINT_WINDOW_ADDRESS_TYPE\x10\xc2\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_P2P_ENDPOINT_WINDOW_SIZE\x10\xc3\x9b\x46\x12\x34\n.NIFGEN_ATTRIBUTE_P2P_DONE_NOTIFICATION_ADDRESS\x10\xc5\x9b\x46\x12\x39\n3NIFGEN_ATTRIBUTE_P2P_DONE_NOTIFICATION_ADDRESS_TYPE\x10\xc6\x9b\x46\x12\x32\n,NIFGEN_ATTRIBUTE_P2P_DONE_NOTIFICATION_VALUE\x10\xc7\x9b\x46\x12\x43\n=NIFGEN_ATTRIBUTE_P2P_DATA_TRANSFER_PERMISSION_INITIAL_CREDITS\x10\xc8\x9b\x46\x12.\n(NIFGEN_ATTRIBUTE_STREAMING_WRITE_TIMEOUT\x10\xc9\x9b\x46\x12@\n:NIFGEN_ATTRIBUTE_P2P_ENDPOINT_FULLNESS_START_TRIGGER_LEVEL\x10\xca\x9b\x46\x12(\n\"NIFGEN_ATTRIBUTE_AUX_POWER_ENABLED\x10\xcb\x9b\x46\x12(\n\"NIFGEN_ATTRIBUTE_FPGA_BITFILE_PATH\x10\xcc\x9b\x46\x12%\n\x1fNIFGEN_ATTRIBUTE_ABSOLUTE_DELAY\x10\xcd\x9b\x46\x12\"\n\x1cNIFGEN_ATTRIBUTE_OUTPUT_MODE\x10\xd1\xa5L\x12%\n\x1fNIFGEN_ATTRIBUTE_OUTPUT_ENABLED\x10\xd3\xa5L\x12\'\n!NIFGEN_ATTRIBUTE_OUTPUT_IMPEDANCE\x10\xd4\xa5L\x12$\n\x1eNIFGEN_ATTRIBUTE_FUNC_WAVEFORM\x10\xb5\xa6L\x12%\n\x1fNIFGEN_ATTRIBUTE_FUNC_AMPLITUDE\x10\xb6\xa6L\x12%\n\x1fNIFGEN_ATTRIBUTE_FUNC_DC_OFFSET\x10\xb7\xa6L\x12%\n\x1fNIFGEN_ATTRIBUTE_FUNC_FREQUENCY\x10\xb8\xa6L\x12\'\n!NIFGEN_ATTRIBUTE_FUNC_START_PHASE\x10\xb9\xa6L\x12+\n%NIFGEN_ATTRIBUTE_FUNC_DUTY_CYCLE_HIGH\x10\xba\xa6L\x12*\n$NIFGEN_ATTRIBUTE_ARB_WAVEFORM_HANDLE\x10\x99\xa7L\x12\x1f\n\x19NIFGEN_ATTRIBUTE_ARB_GAIN\x10\x9a\xa7L\x12!\n\x1bNIFGEN_ATTRIBUTE_ARB_OFFSET\x10\x9b\xa7L\x12&\n NIFGEN_ATTRIBUTE_ARB_SAMPLE_RATE\x10\x9c\xa7L\x12(\n\"NIFGEN_ATTRIBUTE_MAX_NUM_WAVEFORMS\x10\x9d\xa7L\x12\'\n!NIFGEN_ATTRIBUTE_WAVEFORM_QUANTUM\x10\x9e\xa7L\x12(\n\"NIFGEN_ATTRIBUTE_MIN_WAVEFORM_SIZE\x10\x9f\xa7L\x12(\n\"NIFGEN_ATTRIBUTE_MAX_WAVEFORM_SIZE\x10\xa0\xa7L\x12*\n$NIFGEN_ATTRIBUTE_ARB_SEQUENCE_HANDLE\x10\xa3\xa7L\x12(\n\"NIFGEN_ATTRIBUTE_MAX_NUM_SEQUENCES\x10\xa4\xa7L\x12*\n$NIFGEN_ATTRIBUTE_MIN_SEQUENCE_LENGTH\x10\xa5\xa7L\x12*\n$NIFGEN_ATTRIBUTE_MAX_SEQUENCE_LENGTH\x10\xa6\xa7L\x12%\n\x1fNIFGEN_ATTRIBUTE_MAX_LOOP_COUNT\x10\xa7\xa7L\x12%\n\x1fNIFGEN_ATTRIBUTE_TRIGGER_SOURCE\x10\xfe\xa7L\x12\"\n\x1cNIFGEN_ATTRIBUTE_BURST_COUNT\x10\xae\xa8L*Z\n\tByteOrder\x12\'\n#BYTE_ORDER_NIFGEN_VAL_LITTLE_ENDIAN\x10\x00\x12$\n BYTE_ORDER_NIFGEN_VAL_BIG_ENDIAN\x10\x01*\x82\x01\n\tClockMode\x12)\n%CLOCK_MODE_NIFGEN_VAL_HIGH_RESOLUTION\x10\x00\x12%\n!CLOCK_MODE_NIFGEN_VAL_DIVIDE_DOWN\x10\x01\x12#\n\x1f\x43LOCK_MODE_NIFGEN_VAL_AUTOMATIC\x10\x02*y\n\x14\x46requencyListOptions\x12&\n\"FREQUENCY_LIST_OPTIONS_UNSPECIFIED\x10\x00\x12\x39\n,FREQUENCY_LIST_OPTIONS_NIFGEN_VAL_ALL_FLISTS\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01*\xe8\x01\n\rHardwareState\x12\"\n\x1eHARDWARE_STATE_NIFGEN_VAL_IDLE\x10\x00\x12\x37\n3HARDWARE_STATE_NIFGEN_VAL_WAITING_FOR_START_TRIGGER\x10\x64\x12&\n!HARDWARE_STATE_NIFGEN_VAL_RUNNING\x10\xc8\x01\x12#\n\x1eHARDWARE_STATE_NIFGEN_VAL_DONE\x10\xd8\x04\x12-\n(HARDWARE_STATE_NIFGEN_VAL_HARDWARE_ERROR\x10\xe8\x07*\xc1Q\n\x1aNiFgenInt32AttributeValues\x12\x1c\n\x18NIFGEN_INT32_UNSPECIFIED\x10\x00\x12/\n+NIFGEN_INT32_ADDRESS_TYPE_VAL_ADDR_PHYSICAL\x10\x00\x12.\n*NIFGEN_INT32_ADDRESS_TYPE_VAL_ADDR_VIRTUAL\x10\x01\x12\x31\n-NIFGEN_INT32_ANALOG_PATH_VAL_MAIN_ANALOG_PATH\x10\x00\x12\x33\n/NIFGEN_INT32_ANALOG_PATH_VAL_DIRECT_ANALOG_PATH\x10\x01\x12;\n7NIFGEN_INT32_ANALOG_PATH_VAL_FIXED_LOW_GAIN_ANALOG_PATH\x10\x02\x12<\n8NIFGEN_INT32_ANALOG_PATH_VAL_FIXED_HIGH_GAIN_ANALOG_PATH\x10\x03\x12\x46\n@NIFGEN_INT32_ARBITRARY_SEQUENCE_HANDLE_VAL_FIRST_SEQUENCE_HANDLE\x10\xa0\x8d\x06\x12\x45\n?NIFGEN_INT32_ARBITRARY_SEQUENCE_HANDLE_VAL_LAST_SEQUENCE_HANDLE\x10\xaf\xdb\x06\x12\x43\n6NIFGEN_INT32_ARBITRARY_SEQUENCE_HANDLE_VAL_NO_SEQUENCE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x45\n@NIFGEN_INT32_ARBITRARY_WAVEFORM_HANDLE_VAL_FIRST_WAVEFORM_HANDLE\x10\x90N\x12\x44\n?NIFGEN_INT32_ARBITRARY_WAVEFORM_HANDLE_VAL_LAST_WAVEFORM_HANDLE\x10\xf7U\x12\x43\n6NIFGEN_INT32_ARBITRARY_WAVEFORM_HANDLE_VAL_NO_WAVEFORM\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12=\n0NIFGEN_INT32_BURST_COUNT_VAL_GENERATE_CONTINUOUS\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12)\n%NIFGEN_INT32_BUS_TYPE_VAL_BUS_INVALID\x10\x00\x12$\n NIFGEN_INT32_BUS_TYPE_VAL_BUS_AT\x10\x01\x12%\n!NIFGEN_INT32_BUS_TYPE_VAL_BUS_PCI\x10\x02\x12%\n!NIFGEN_INT32_BUS_TYPE_VAL_BUS_PXI\x10\x03\x12%\n!NIFGEN_INT32_BUS_TYPE_VAL_BUS_VXI\x10\x04\x12(\n$NIFGEN_INT32_BUS_TYPE_VAL_BUS_PCMCIA\x10\x05\x12&\n\"NIFGEN_INT32_BUS_TYPE_VAL_BUS_PXIE\x10\x06\x12/\n+NIFGEN_INT32_CLOCK_MODE_VAL_HIGH_RESOLUTION\x10\x00\x12+\n\'NIFGEN_INT32_CLOCK_MODE_VAL_DIVIDE_DOWN\x10\x01\x12)\n%NIFGEN_INT32_CLOCK_MODE_VAL_AUTOMATIC\x10\x02\x12\x41\n=NIFGEN_INT32_DATA_MARKER_EVENT_LEVEL_POLARITY_VAL_ACTIVE_HIGH\x10\x65\x12@\n<NIFGEN_INT32_DATA_MARKER_EVENT_LEVEL_POLARITY_VAL_ACTIVE_LOW\x10\x66\x12\x32\n.NIFGEN_INT32_DATA_PROCESSING_MODE_VAL_OSP_REAL\x10\x00\x12\x35\n1NIFGEN_INT32_DATA_PROCESSING_MODE_VAL_OSP_COMPLEX\x10\x01\x12\x38\n4NIFGEN_INT32_DONE_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_HIGH\x10\x65\x12\x37\n3NIFGEN_INT32_DONE_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_LOW\x10\x66\x12@\n<NIFGEN_INT32_DONE_EVENT_DELAY_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12\x33\n/NIFGEN_INT32_DONE_EVENT_DELAY_UNITS_VAL_SECONDS\x10\x66\x12\x35\n1NIFGEN_INT32_DONE_EVENT_OUTPUT_BEHAVIOR_VAL_PULSE\x10\x65\x12\x35\n1NIFGEN_INT32_DONE_EVENT_OUTPUT_BEHAVIOR_VAL_LEVEL\x10\x66\x12:\n6NIFGEN_INT32_DONE_EVENT_PULSE_POLARITY_VAL_ACTIVE_HIGH\x10\x65\x12\x39\n5NIFGEN_INT32_DONE_EVENT_PULSE_POLARITY_VAL_ACTIVE_LOW\x10\x66\x12\x46\nBNIFGEN_INT32_DONE_EVENT_PULSE_WIDTH_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12\x39\n5NIFGEN_INT32_DONE_EVENT_PULSE_WIDTH_UNITS_VAL_SECONDS\x10\x66\x12)\n%NIFGEN_INT32_FILTER_TYPE_VAL_OSP_FLAT\x10\x00\x12\x32\n.NIFGEN_INT32_FILTER_TYPE_VAL_OSP_RAISED_COSINE\x10\x01\x12\x37\n3NIFGEN_INT32_FILTER_TYPE_VAL_OSP_ROOT_RAISED_COSINE\x10\x02\x12-\n)NIFGEN_INT32_FILTER_TYPE_VAL_OSP_GAUSSIAN\x10\x03\x12+\n\'NIFGEN_INT32_FILTER_TYPE_VAL_OSP_CUSTOM\x10\x04\x12\x43\n=NIFGEN_INT32_FREQUENCY_LIST_HANDLE_VAL_FIRST_FREQ_LIST_HANDLE\x10\xc0\x9a\x0c\x12\x42\n<NIFGEN_INT32_FREQUENCY_LIST_HANDLE_VAL_LAST_FREQ_LIST_HANDLE\x10\xcf\xe8\x0c\x12@\n3NIFGEN_INT32_FREQUENCY_LIST_HANDLE_VAL_NO_FREQ_LIST\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x33\n.NIFGEN_INT32_IDLE_BEHAVIOR_VAL_HOLD_LAST_VALUE\x10\x90\x03\x12\x31\n,NIFGEN_INT32_IDLE_BEHAVIOR_VAL_JUMP_TO_VALUE\x10\x91\x03\x12\x42\n>NIFGEN_INT32_MARKER_EVENT_DELAY_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12\x35\n1NIFGEN_INT32_MARKER_EVENT_DELAY_UNITS_VAL_SECONDS\x10\x66\x12\x37\n3NIFGEN_INT32_MARKER_EVENT_OUTPUT_BEHAVIOR_VAL_PULSE\x10\x65\x12\x37\n3NIFGEN_INT32_MARKER_EVENT_OUTPUT_BEHAVIOR_VAL_LEVEL\x10\x66\x12\x38\n4NIFGEN_INT32_MARKER_EVENT_OUTPUT_BEHAVIOR_VAL_TOGGLE\x10g\x12<\n8NIFGEN_INT32_MARKER_EVENT_PULSE_POLARITY_VAL_ACTIVE_HIGH\x10\x65\x12;\n7NIFGEN_INT32_MARKER_EVENT_PULSE_POLARITY_VAL_ACTIVE_LOW\x10\x66\x12H\nDNIFGEN_INT32_MARKER_EVENT_PULSE_WIDTH_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12;\n7NIFGEN_INT32_MARKER_EVENT_PULSE_WIDTH_UNITS_VAL_SECONDS\x10\x66\x12;\n7NIFGEN_INT32_MARKER_EVENT_TOGGLE_INITIAL_STATE_VAL_HIGH\x10\x65\x12:\n6NIFGEN_INT32_MARKER_EVENT_TOGGLE_INITIAL_STATE_VAL_LOW\x10\x66\x12$\n NIFGEN_INT32_OSP_MODE_VAL_OSP_IF\x10\x00\x12*\n&NIFGEN_INT32_OSP_MODE_VAL_OSP_BASEBAND\x10\x01\x12G\nCNIFGEN_INT32_OSP_OVERFLOW_ERROR_REPORTING_VAL_ERROR_REPORTING_ERROR\x10\x00\x12J\nFNIFGEN_INT32_OSP_OVERFLOW_ERROR_REPORTING_VAL_ERROR_REPORTING_DISABLED\x10\x02\x12:\n6NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_NONE\x10\x00\x12G\nCNIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PRE_FILTER_GAIN_I\x10\x01\x12G\nCNIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PRE_FILTER_GAIN_Q\x10\x02\x12I\nENIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PRE_FILTER_OFFSET_I\x10\x04\x12I\nENIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PRE_FILTER_OFFSET_Q\x10\x08\x12\x42\n>NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_FIR_FILTER_I\x10\x10\x12\x43\n?NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PFIR_FILTER_I\x10\x10\x12\x42\n>NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_FIR_FILTER_Q\x10 \x12\x43\n?NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PFIR_FILTER_Q\x10 \x12\x42\n>NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_CIC_FILTER_I\x10@\x12\x43\n>NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_CIC_FILTER_Q\x10\x80\x01\x12\x43\n>NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_COMPLEX_DATA\x10\x80\x02\x12\x44\n?NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_CFIR_FILTER_I\x10\x80\x04\x12\x44\n?NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_CFIR_FILTER_Q\x10\x80\x08\x12@\n;NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_EQUALIZER\x10\x80\x10\x12,\n(NIFGEN_INT32_OUTPUT_MODE_VAL_OUTPUT_FUNC\x10\x00\x12+\n\'NIFGEN_INT32_OUTPUT_MODE_VAL_OUTPUT_ARB\x10\x01\x12+\n\'NIFGEN_INT32_OUTPUT_MODE_VAL_OUTPUT_SEQ\x10\x02\x12\x31\n-NIFGEN_INT32_OUTPUT_MODE_VAL_OUTPUT_FREQ_LIST\x10\x65\x12.\n*NIFGEN_INT32_OUTPUT_MODE_VAL_OUTPUT_SCRIPT\x10\x66\x12\x43\n?NIFGEN_INT32_READY_FOR_START_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_HIGH\x10\x65\x12\x42\n>NIFGEN_INT32_READY_FOR_START_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_LOW\x10\x66\x12\x41\n=NIFGEN_INT32_SCRIPT_TRIGGER_DIGITAL_EDGE_EDGE_VAL_RISING_EDGE\x10\x65\x12\x42\n>NIFGEN_INT32_SCRIPT_TRIGGER_DIGITAL_EDGE_EDGE_VAL_FALLING_EDGE\x10\x66\x12J\nFNIFGEN_INT32_SCRIPT_TRIGGER_DIGITAL_LEVEL_ACTIVE_LEVEL_VAL_ACTIVE_HIGH\x10\x65\x12I\nENIFGEN_INT32_SCRIPT_TRIGGER_DIGITAL_LEVEL_ACTIVE_LEVEL_VAL_ACTIVE_LOW\x10\x66\x12\x32\n.NIFGEN_INT32_SCRIPT_TRIGGER_TYPE_VAL_TRIG_NONE\x10\x65\x12\x35\n1NIFGEN_INT32_SCRIPT_TRIGGER_TYPE_VAL_DIGITAL_EDGE\x10\x66\x12\x36\n2NIFGEN_INT32_SCRIPT_TRIGGER_TYPE_VAL_DIGITAL_LEVEL\x10g\x12\x36\n2NIFGEN_INT32_SCRIPT_TRIGGER_TYPE_VAL_SOFTWARE_EDGE\x10h\x12@\n<NIFGEN_INT32_START_TRIGGER_DIGITAL_EDGE_EDGE_VAL_RISING_EDGE\x10\x65\x12\x41\n=NIFGEN_INT32_START_TRIGGER_DIGITAL_EDGE_EDGE_VAL_FALLING_EDGE\x10\x66\x12\x31\n-NIFGEN_INT32_START_TRIGGER_TYPE_VAL_TRIG_NONE\x10\x65\x12\x34\n0NIFGEN_INT32_START_TRIGGER_TYPE_VAL_DIGITAL_EDGE\x10\x66\x12\x35\n1NIFGEN_INT32_START_TRIGGER_TYPE_VAL_SOFTWARE_EDGE\x10h\x12=\n9NIFGEN_INT32_START_TRIGGER_TYPE_VAL_P2P_ENDPOINT_FULLNESS\x10j\x12;\n7NIFGEN_INT32_STARTED_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_HIGH\x10\x65\x12:\n6NIFGEN_INT32_STARTED_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_LOW\x10\x66\x12\x43\n?NIFGEN_INT32_STARTED_EVENT_DELAY_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12\x36\n2NIFGEN_INT32_STARTED_EVENT_DELAY_UNITS_VAL_SECONDS\x10\x66\x12\x38\n4NIFGEN_INT32_STARTED_EVENT_OUTPUT_BEHAVIOR_VAL_PULSE\x10\x65\x12\x38\n4NIFGEN_INT32_STARTED_EVENT_OUTPUT_BEHAVIOR_VAL_LEVEL\x10\x66\x12=\n9NIFGEN_INT32_STARTED_EVENT_PULSE_POLARITY_VAL_ACTIVE_HIGH\x10\x65\x12<\n8NIFGEN_INT32_STARTED_EVENT_PULSE_POLARITY_VAL_ACTIVE_LOW\x10\x66\x12I\nENIFGEN_INT32_STARTED_EVENT_PULSE_WIDTH_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12<\n8NIFGEN_INT32_STARTED_EVENT_PULSE_WIDTH_UNITS_VAL_SECONDS\x10\x66\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL0\x10o\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL1\x10p\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL2\x10q\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL3\x10r\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL4\x10s\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL5\x10t\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL6\x10u\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_0\x10\x8d\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_1\x10\x8e\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_2\x10\x8f\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_3\x10\x90\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_4\x10\x91\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_5\x10\x92\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_6\x10\x93\x01\x12\x31\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_NONE\x10\xe8\x07\x12\x39\n4NIFGEN_INT32_TERMINAL_CONFIGURATION_VAL_SINGLE_ENDED\x10\xac\x02\x12\x39\n4NIFGEN_INT32_TERMINAL_CONFIGURATION_VAL_DIFFERENTIAL\x10\xad\x02\x12(\n$NIFGEN_INT32_TRIGGER_MODE_VAL_SINGLE\x10\x01\x12,\n(NIFGEN_INT32_TRIGGER_MODE_VAL_CONTINUOUS\x10\x02\x12)\n%NIFGEN_INT32_TRIGGER_MODE_VAL_STEPPED\x10\x03\x12\'\n#NIFGEN_INT32_TRIGGER_MODE_VAL_BURST\x10\x04\x12-\n)NIFGEN_INT32_TRIGGER_SOURCE_VAL_IMMEDIATE\x10\x00\x12,\n(NIFGEN_INT32_TRIGGER_SOURCE_VAL_EXTERNAL\x10\x01\x12\x31\n-NIFGEN_INT32_TRIGGER_SOURCE_VAL_SOFTWARE_TRIG\x10\x02\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL0\x10o\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL1\x10p\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL2\x10q\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL3\x10r\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL4\x10s\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL5\x10t\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL6\x10u\x12-\n(NIFGEN_INT32_TRIGGER_SOURCE_VAL_PXI_STAR\x10\x83\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_0\x10\x8d\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_1\x10\x8e\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_2\x10\x8f\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_3\x10\x90\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_4\x10\x91\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_5\x10\x92\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_6\x10\x93\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_7\x10\xf2\x07\x12*\n%NIFGEN_INT32_TRIGGER_SOURCE_VAL_PFI_0\x10\xf3\x07\x12*\n%NIFGEN_INT32_TRIGGER_SOURCE_VAL_PFI_1\x10\xf4\x07\x12*\n%NIFGEN_INT32_TRIGGER_SOURCE_VAL_PFI_2\x10\xf5\x07\x12*\n%NIFGEN_INT32_TRIGGER_SOURCE_VAL_PFI_3\x10\xf6\x07\x12\x33\n.NIFGEN_INT32_TRIGGER_SOURCE_VAL_OTHER_TERMINAL\x10\xfa\x07\x12\x31\n-NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_INTERNAL\x10\x00\x12\x31\n-NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_EXTERNAL\x10\x01\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL1\x10p\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL2\x10q\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL3\x10r\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL4\x10s\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL5\x10t\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL6\x10u\x12\x32\n-NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_PXI_STAR\x10\x83\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_0\x10\x8d\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_1\x10\x8e\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_2\x10\x8f\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_3\x10\x90\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_4\x10\x91\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_5\x10\x92\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_6\x10\x93\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_7\x10\xf2\x07\x12\x38\n3NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_OTHER_TERMINAL\x10\xfa\x07\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_CLK_IN\x10\xb2\t\x12\x34\n/NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_DDC_CLK_IN\x10\xb3\t\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_B\x10\x00\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_D\x10\x01\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_G\x10\x02\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_H\x10\x03\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_I\x10\x04\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_M\x10\x05\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_N\x10\x06\x12/\n+NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_NTSC_M\x10\x07\x12\x33\n.NIFGEN_INT32_WAIT_BEHAVIOR_VAL_HOLD_LAST_VALUE\x10\x90\x03\x12\x31\n,NIFGEN_INT32_WAIT_BEHAVIOR_VAL_JUMP_TO_VALUE\x10\x91\x03\x12&\n\"NIFGEN_INT32_WAVEFORM_VAL_WFM_SINE\x10\x01\x12(\n$NIFGEN_INT32_WAVEFORM_VAL_WFM_SQUARE\x10\x02\x12*\n&NIFGEN_INT32_WAVEFORM_VAL_WFM_TRIANGLE\x10\x03\x12)\n%NIFGEN_INT32_WAVEFORM_VAL_WFM_RAMP_UP\x10\x04\x12+\n\'NIFGEN_INT32_WAVEFORM_VAL_WFM_RAMP_DOWN\x10\x05\x12$\n NIFGEN_INT32_WAVEFORM_VAL_WFM_DC\x10\x06\x12\'\n#NIFGEN_INT32_WAVEFORM_VAL_WFM_NOISE\x10\x65\x12&\n\"NIFGEN_INT32_WAVEFORM_VAL_WFM_USER\x10\x66\x1a\x02\x10\x01*\xa7\x02\n\x1bNiFgenReal64AttributeValues\x12\x1d\n\x19NIFGEN_REAL64_UNSPECIFIED\x10\x00\x12\x44\n7NIFGEN_REAL64_LOAD_IMPEDANCE_VAL_MATCHED_LOAD_IMPEDANCE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12.\n*NIFGEN_REAL64_OUTPUT_IMPEDANCE_VAL_50_OHMS\x10\x32\x12.\n*NIFGEN_REAL64_OUTPUT_IMPEDANCE_VAL_75_OHMS\x10K\x12?\n2NIFGEN_REAL64_SAMPLE_RATE_VAL_EXTERNAL_SAMPLE_RATE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x1a\x02\x10\x01*\xcf\n\n!NiFgenStringAttributeValuesMapped\x12$\n NIFGEN_STRING_MAPPED_UNSPECIFIED\x10\x00\x12I\nENIFGEN_STRING_REFERENCE_CLOCK_SOURCE_VAL_CLOCK_IN_COLLISION_AVOIDANCE\x10\x01\x12\x45\nANIFGEN_STRING_REFERENCE_CLOCK_SOURCE_VAL_NONE_COLLISION_AVOIDANCE\x10\x02\x12X\nTNIFGEN_STRING_REFERENCE_CLOCK_SOURCE_VAL_ONBOARD_REFERENCE_CLOCK_COLLISION_AVOIDANCE\x10\x03\x12J\nFNIFGEN_STRING_REFERENCE_CLOCK_SOURCE_VAL_PXI_CLOCK_COLLISION_AVOIDANCE\x10\x04\x12G\nCNIFGEN_STRING_REFERENCE_CLOCK_SOURCE_VAL_RTSI_7_COLLISION_AVOIDANCE\x10\x05\x12\x32\n.NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_CLOCK_IN\x10\x06\x12\x36\n2NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_DDC_CLOCK_IN\x10\x07\x12\x37\n3NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_ONBOARD_CLOCK\x10\x08\x12\x37\n3NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_STAR_LINE\x10\t\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_0_RTSI_0\x10\n\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_1_RTSI_1\x10\x0b\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_2_RTSI_2\x10\x0c\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_3_RTSI_3\x10\r\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_4_RTSI_4\x10\x0e\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_5_RTSI_5\x10\x0f\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_6_RTSI_6\x10\x10\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_7_RTSI_7\x10\x11\x12;\n7NIFGEN_STRING_SAMPLE_CLOCK_TIMEBASE_SOURCE_VAL_CLOCK_IN\x10\x12\x12@\n<NIFGEN_STRING_SAMPLE_CLOCK_TIMEBASE_SOURCE_VAL_ONBOARD_CLOCK\x10\x13*\xd9\x01\n\nOutputMode\x12&\n\"OUTPUT_MODE_NIFGEN_VAL_OUTPUT_FUNC\x10\x00\x12%\n!OUTPUT_MODE_NIFGEN_VAL_OUTPUT_ARB\x10\x01\x12%\n!OUTPUT_MODE_NIFGEN_VAL_OUTPUT_SEQ\x10\x02\x12+\n\'OUTPUT_MODE_NIFGEN_VAL_OUTPUT_FREQ_LIST\x10\x65\x12(\n$OUTPUT_MODE_NIFGEN_VAL_OUTPUT_SCRIPT\x10\x66*v\n\nRelativeTo\x12\x32\n.RELATIVE_TO_NIFGEN_VAL_WAVEFORM_POSITION_START\x10\x00\x12\x34\n0RELATIVE_TO_NIFGEN_VAL_WAVEFORM_POSITION_CURRENT\x10\x01*\x89\x07\n\x0fRouteSignalFrom\x12!\n\x1dROUTE_SIGNAL_FROM_UNSPECIFIED\x10\x00\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_MARKER\x10\xe9\x07\x12*\n%ROUTE_SIGNAL_FROM_NIFGEN_VAL_SYNC_OUT\x10\xea\x07\x12\x33\n.ROUTE_SIGNAL_FROM_NIFGEN_VAL_OUT_START_TRIGGER\x10\xec\x07\x12-\n(ROUTE_SIGNAL_FROM_NIFGEN_VAL_BOARD_CLOCK\x10\xee\x07\x12\x31\n,ROUTE_SIGNAL_FROM_NIFGEN_VAL_SYNCHRONIZATION\x10\xef\x07\x12.\n*ROUTE_SIGNAL_FROM_NIFGEN_VAL_SOFTWARE_TRIG\x10\x02\x12)\n$ROUTE_SIGNAL_FROM_NIFGEN_VAL_REF_OUT\x10\xf0\x07\x12+\n&ROUTE_SIGNAL_FROM_NIFGEN_VAL_CLOCK_OUT\x10\xf1\x07\x12*\n%ROUTE_SIGNAL_FROM_NIFGEN_VAL_PXI_STAR\x10\x83\x01\x12\'\n\"ROUTE_SIGNAL_FROM_NIFGEN_VAL_PFI_0\x10\xf3\x07\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_0\x10\x8d\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_1\x10\x8e\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_2\x10\x8f\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_3\x10\x90\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_4\x10\x91\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_5\x10\x92\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_6\x10\x93\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_7\x10\xf2\x07\x12\x39\n4ROUTE_SIGNAL_FROM_NIFGEN_VAL_ONBOARD_REFERENCE_CLOCK\x10\xfb\x07*\x91\x04\n\rRouteSignalTo\x12\x1f\n\x1bROUTE_SIGNAL_TO_UNSPECIFIED\x10\x00\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_0\x10\x8d\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_1\x10\x8e\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_2\x10\x8f\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_3\x10\x90\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_4\x10\x91\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_5\x10\x92\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_6\x10\x93\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_7\x10\xf2\x07\x12\'\n\"ROUTE_SIGNAL_TO_NIFGEN_VAL_REF_OUT\x10\xf0\x07\x12%\n ROUTE_SIGNAL_TO_NIFGEN_VAL_PFI_0\x10\xf3\x07\x12%\n ROUTE_SIGNAL_TO_NIFGEN_VAL_PFI_1\x10\xf4\x07\x12(\n#ROUTE_SIGNAL_TO_NIFGEN_VAL_PXI_STAR\x10\x83\x01*h\n\x0eSequenceHandle\x12\x1f\n\x1bSEQUENCE_HANDLE_UNSPECIFIED\x10\x00\x12\x35\n(SEQUENCE_HANDLE_NIFGEN_VAL_ALL_SEQUENCES\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01*\xa0\x04\n\x06Signal\x12\x16\n\x12SIGNAL_UNSPECIFIED\x10\x00\x12.\n)SIGNAL_NIFGEN_VAL_ONBOARD_REFERENCE_CLOCK\x10\xfb\x07\x12\x1f\n\x1aSIGNAL_NIFGEN_VAL_SYNC_OUT\x10\xea\x07\x12$\n\x1fSIGNAL_NIFGEN_VAL_START_TRIGGER\x10\xec\x07\x12#\n\x1eSIGNAL_NIFGEN_VAL_MARKER_EVENT\x10\xe9\x07\x12,\n\'SIGNAL_NIFGEN_VAL_SAMPLE_CLOCK_TIMEBASE\x10\xee\x07\x12&\n!SIGNAL_NIFGEN_VAL_SYNCHRONIZATION\x10\xef\x07\x12\"\n\x1eSIGNAL_NIFGEN_VAL_SAMPLE_CLOCK\x10\x65\x12%\n!SIGNAL_NIFGEN_VAL_REFERENCE_CLOCK\x10\x66\x12$\n SIGNAL_NIFGEN_VAL_SCRIPT_TRIGGER\x10g\x12+\n\'SIGNAL_NIFGEN_VAL_READY_FOR_START_EVENT\x10i\x12#\n\x1fSIGNAL_NIFGEN_VAL_STARTED_EVENT\x10j\x12 \n\x1cSIGNAL_NIFGEN_VAL_DONE_EVENT\x10k\x12\'\n#SIGNAL_NIFGEN_VAL_DATA_MARKER_EVENT\x10l*p\n\x07Trigger\x12\x17\n\x13TRIGGER_UNSPECIFIED\x10\x00\x12%\n TRIGGER_NIFGEN_VAL_START_TRIGGER\x10\xec\x07\x12%\n!TRIGGER_NIFGEN_VAL_SCRIPT_TRIGGER\x10g*\xbf\x01\n\x0bTriggerMode\x12\x1c\n\x18TRIGGER_MODE_UNSPECIFIED\x10\x00\x12\"\n\x1eTRIGGER_MODE_NIFGEN_VAL_SINGLE\x10\x01\x12&\n\"TRIGGER_MODE_NIFGEN_VAL_CONTINUOUS\x10\x02\x12#\n\x1fTRIGGER_MODE_NIFGEN_VAL_STEPPED\x10\x03\x12!\n\x1dTRIGGER_MODE_NIFGEN_VAL_BURST\x10\x04*|\n\x0bTriggerWhen\x12\x1c\n\x18TRIGGER_WHEN_UNSPECIFIED\x10\x00\x12\'\n#TRIGGER_WHEN_NIFGEN_VAL_ACTIVE_HIGH\x10\x65\x12&\n\"TRIGGER_WHEN_NIFGEN_VAL_ACTIVE_LOW\x10\x66*\xc1\x02\n\x08Waveform\x12\x18\n\x14WAVEFORM_UNSPECIFIED\x10\x00\x12 \n\x1cWAVEFORM_NIFGEN_VAL_WFM_SINE\x10\x01\x12\"\n\x1eWAVEFORM_NIFGEN_VAL_WFM_SQUARE\x10\x02\x12$\n WAVEFORM_NIFGEN_VAL_WFM_TRIANGLE\x10\x03\x12#\n\x1fWAVEFORM_NIFGEN_VAL_WFM_RAMP_UP\x10\x04\x12%\n!WAVEFORM_NIFGEN_VAL_WFM_RAMP_DOWN\x10\x05\x12\x1e\n\x1aWAVEFORM_NIFGEN_VAL_WFM_DC\x10\x06\x12!\n\x1dWAVEFORM_NIFGEN_VAL_WFM_NOISE\x10\x65\x12 \n\x1cWAVEFORM_NIFGEN_VAL_WFM_USER\x10\x66*h\n\x0eWaveformHandle\x12\x1f\n\x1bWAVEFORM_HANDLE_UNSPECIFIED\x10\x00\x12\x35\n(WAVEFORM_HANDLE_NIFGEN_VAL_ALL_WAVEFORMS\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x32\xc7p\n\x06NiFgen\x12\\\n\x0f\x41\x62ortGeneration\x12#.nifgen_grpc.AbortGenerationRequest\x1a$.nifgen_grpc.AbortGenerationResponse\x12\x89\x01\n\x1e\x41\x64justSampleClockRelativeDelay\x12\x32.nifgen_grpc.AdjustSampleClockRelativeDelayRequest\x1a\x33.nifgen_grpc.AdjustSampleClockRelativeDelayResponse\x12n\n\x15\x41llocateNamedWaveform\x12).nifgen_grpc.AllocateNamedWaveformRequest\x1a*.nifgen_grpc.AllocateNamedWaveformResponse\x12_\n\x10\x41llocateWaveform\x12$.nifgen_grpc.AllocateWaveformRequest\x1a%.nifgen_grpc.AllocateWaveformResponse\x12t\n\x17\x43heckAttributeViBoolean\x12+.nifgen_grpc.CheckAttributeViBooleanRequest\x1a,.nifgen_grpc.CheckAttributeViBooleanResponse\x12n\n\x15\x43heckAttributeViInt32\x12).nifgen_grpc.CheckAttributeViInt32Request\x1a*.nifgen_grpc.CheckAttributeViInt32Response\x12n\n\x15\x43heckAttributeViInt64\x12).nifgen_grpc.CheckAttributeViInt64Request\x1a*.nifgen_grpc.CheckAttributeViInt64Response\x12q\n\x16\x43heckAttributeViReal64\x12*.nifgen_grpc.CheckAttributeViReal64Request\x1a+.nifgen_grpc.CheckAttributeViReal64Response\x12t\n\x17\x43heckAttributeViSession\x12+.nifgen_grpc.CheckAttributeViSessionRequest\x1a,.nifgen_grpc.CheckAttributeViSessionResponse\x12q\n\x16\x43heckAttributeViString\x12*.nifgen_grpc.CheckAttributeViStringRequest\x1a+.nifgen_grpc.CheckAttributeViStringResponse\x12Y\n\x0e\x43learArbMemory\x12\".nifgen_grpc.ClearArbMemoryRequest\x1a#.nifgen_grpc.ClearArbMemoryResponse\x12_\n\x10\x43learArbSequence\x12$.nifgen_grpc.ClearArbSequenceRequest\x1a%.nifgen_grpc.ClearArbSequenceResponse\x12_\n\x10\x43learArbWaveform\x12$.nifgen_grpc.ClearArbWaveformRequest\x1a%.nifgen_grpc.ClearArbWaveformResponse\x12M\n\nClearError\x12\x1e.nifgen_grpc.ClearErrorRequest\x1a\x1f.nifgen_grpc.ClearErrorResponse\x12V\n\rClearFreqList\x12!.nifgen_grpc.ClearFreqListRequest\x1a\".nifgen_grpc.ClearFreqListResponse\x12w\n\x18\x43learInterchangeWarnings\x12,.nifgen_grpc.ClearInterchangeWarningsRequest\x1a-.nifgen_grpc.ClearInterchangeWarningsResponse\x12z\n\x19\x43learUserStandardWaveform\x12-.nifgen_grpc.ClearUserStandardWaveformRequest\x1a..nifgen_grpc.ClearUserStandardWaveformResponse\x12>\n\x05\x43lose\x12\x19.nifgen_grpc.CloseRequest\x1a\x1a.nifgen_grpc.CloseResponse\x12\x41\n\x06\x43ommit\x12\x1a.nifgen_grpc.CommitRequest\x1a\x1b.nifgen_grpc.CommitResponse\x12\x65\n\x12\x43onfigureAmplitude\x12&.nifgen_grpc.ConfigureAmplitudeRequest\x1a\'.nifgen_grpc.ConfigureAmplitudeResponse\x12k\n\x14\x43onfigureArbSequence\x12(.nifgen_grpc.ConfigureArbSequenceRequest\x1a).nifgen_grpc.ConfigureArbSequenceResponse\x12k\n\x14\x43onfigureArbWaveform\x12(.nifgen_grpc.ConfigureArbWaveformRequest\x1a).nifgen_grpc.ConfigureArbWaveformResponse\x12\x62\n\x11\x43onfigureChannels\x12%.nifgen_grpc.ConfigureChannelsRequest\x1a&.nifgen_grpc.ConfigureChannelsResponse\x12\x65\n\x12\x43onfigureClockMode\x12&.nifgen_grpc.ConfigureClockModeRequest\x1a\'.nifgen_grpc.ConfigureClockModeResponse\x12\x9b\x01\n$ConfigureCustomFIRFilterCoefficients\x12\x38.nifgen_grpc.ConfigureCustomFIRFilterCoefficientsRequest\x1a\x39.nifgen_grpc.ConfigureCustomFIRFilterCoefficientsResponse\x12\x92\x01\n!ConfigureDigitalEdgeScriptTrigger\x12\x35.nifgen_grpc.ConfigureDigitalEdgeScriptTriggerRequest\x1a\x36.nifgen_grpc.ConfigureDigitalEdgeScriptTriggerResponse\x12\x8f\x01\n ConfigureDigitalEdgeStartTrigger\x12\x34.nifgen_grpc.ConfigureDigitalEdgeStartTriggerRequest\x1a\x35.nifgen_grpc.ConfigureDigitalEdgeStartTriggerResponse\x12\x95\x01\n\"ConfigureDigitalLevelScriptTrigger\x12\x36.nifgen_grpc.ConfigureDigitalLevelScriptTriggerRequest\x1a\x37.nifgen_grpc.ConfigureDigitalLevelScriptTriggerResponse\x12\x62\n\x11\x43onfigureFreqList\x12%.nifgen_grpc.ConfigureFreqListRequest\x1a&.nifgen_grpc.ConfigureFreqListResponse\x12\x65\n\x12\x43onfigureFrequency\x12&.nifgen_grpc.ConfigureFrequencyRequest\x1a\'.nifgen_grpc.ConfigureFrequencyResponse\x12q\n\x16\x43onfigureOperationMode\x12*.nifgen_grpc.ConfigureOperationModeRequest\x1a+.nifgen_grpc.ConfigureOperationModeResponse\x12q\n\x16\x43onfigureOutputEnabled\x12*.nifgen_grpc.ConfigureOutputEnabledRequest\x1a+.nifgen_grpc.ConfigureOutputEnabledResponse\x12w\n\x18\x43onfigureOutputImpedance\x12,.nifgen_grpc.ConfigureOutputImpedanceRequest\x1a-.nifgen_grpc.ConfigureOutputImpedanceResponse\x12h\n\x13\x43onfigureOutputMode\x12\'.nifgen_grpc.ConfigureOutputModeRequest\x1a(.nifgen_grpc.ConfigureOutputModeResponse\x12\xa7\x01\n(ConfigureP2PEndpointFullnessStartTrigger\x12<.nifgen_grpc.ConfigureP2PEndpointFullnessStartTriggerRequest\x1a=.nifgen_grpc.ConfigureP2PEndpointFullnessStartTriggerResponse\x12t\n\x17\x43onfigureReferenceClock\x12+.nifgen_grpc.ConfigureReferenceClockRequest\x1a,.nifgen_grpc.ConfigureReferenceClockResponse\x12}\n\x1a\x43onfigureSampleClockSource\x12..nifgen_grpc.ConfigureSampleClockSourceRequest\x1a/.nifgen_grpc.ConfigureSampleClockSourceResponse\x12h\n\x13\x43onfigureSampleRate\x12\'.nifgen_grpc.ConfigureSampleRateRequest\x1a(.nifgen_grpc.ConfigureSampleRateResponse\x12\x95\x01\n\"ConfigureSoftwareEdgeScriptTrigger\x12\x36.nifgen_grpc.ConfigureSoftwareEdgeScriptTriggerRequest\x1a\x37.nifgen_grpc.ConfigureSoftwareEdgeScriptTriggerResponse\x12\x92\x01\n!ConfigureSoftwareEdgeStartTrigger\x12\x35.nifgen_grpc.ConfigureSoftwareEdgeStartTriggerRequest\x1a\x36.nifgen_grpc.ConfigureSoftwareEdgeStartTriggerResponse\x12z\n\x19\x43onfigureStandardWaveform\x12-.nifgen_grpc.ConfigureStandardWaveformRequest\x1a..nifgen_grpc.ConfigureStandardWaveformResponse\x12w\n\x18\x43onfigureSynchronization\x12,.nifgen_grpc.ConfigureSynchronizationRequest\x1a-.nifgen_grpc.ConfigureSynchronizationResponse\x12k\n\x14\x43onfigureTriggerMode\x12(.nifgen_grpc.ConfigureTriggerModeRequest\x1a).nifgen_grpc.ConfigureTriggerModeResponse\x12z\n\x19\x43reateAdvancedArbSequence\x12-.nifgen_grpc.CreateAdvancedArbSequenceRequest\x1a..nifgen_grpc.CreateAdvancedArbSequenceResponse\x12\x62\n\x11\x43reateArbSequence\x12%.nifgen_grpc.CreateArbSequenceRequest\x1a&.nifgen_grpc.CreateArbSequenceResponse\x12Y\n\x0e\x43reateFreqList\x12\".nifgen_grpc.CreateFreqListRequest\x1a#.nifgen_grpc.CreateFreqListResponse\x12w\n\x18\x43reateWaveformComplexF64\x12,.nifgen_grpc.CreateWaveformComplexF64Request\x1a-.nifgen_grpc.CreateWaveformComplexF64Response\x12\x62\n\x11\x43reateWaveformF64\x12%.nifgen_grpc.CreateWaveformF64Request\x1a&.nifgen_grpc.CreateWaveformF64Response\x12z\n\x19\x43reateWaveformFromFileF64\x12-.nifgen_grpc.CreateWaveformFromFileF64Request\x1a..nifgen_grpc.CreateWaveformFromFileF64Response\x12z\n\x19\x43reateWaveformFromFileHWS\x12-.nifgen_grpc.CreateWaveformFromFileHWSRequest\x1a..nifgen_grpc.CreateWaveformFromFileHWSResponse\x12z\n\x19\x43reateWaveformFromFileI16\x12-.nifgen_grpc.CreateWaveformFromFileI16Request\x1a..nifgen_grpc.CreateWaveformFromFileI16Response\x12\x62\n\x11\x43reateWaveformI16\x12%.nifgen_grpc.CreateWaveformI16Request\x1a&.nifgen_grpc.CreateWaveformI16Response\x12}\n\x1a\x44\x65\x66ineUserStandardWaveform\x12..nifgen_grpc.DefineUserStandardWaveformRequest\x1a/.nifgen_grpc.DefineUserStandardWaveformResponse\x12h\n\x13\x44\x65leteNamedWaveform\x12\'.nifgen_grpc.DeleteNamedWaveformRequest\x1a(.nifgen_grpc.DeleteNamedWaveformResponse\x12S\n\x0c\x44\x65leteScript\x12 .nifgen_grpc.DeleteScriptRequest\x1a!.nifgen_grpc.DeleteScriptResponse\x12\x44\n\x07\x44isable\x12\x1b.nifgen_grpc.DisableRequest\x1a\x1c.nifgen_grpc.DisableResponse\x12h\n\x13\x44isableAnalogFilter\x12\'.nifgen_grpc.DisableAnalogFilterRequest\x1a(.nifgen_grpc.DisableAnalogFilterResponse\x12k\n\x14\x44isableDigitalFilter\x12(.nifgen_grpc.DisableDigitalFilterRequest\x1a).nifgen_grpc.DisableDigitalFilterResponse\x12w\n\x18\x44isableDigitalPatterning\x12,.nifgen_grpc.DisableDigitalPatterningRequest\x1a-.nifgen_grpc.DisableDigitalPatterningResponse\x12k\n\x14\x44isableScriptTrigger\x12(.nifgen_grpc.DisableScriptTriggerRequest\x1a).nifgen_grpc.DisableScriptTriggerResponse\x12h\n\x13\x44isableStartTrigger\x12\'.nifgen_grpc.DisableStartTriggerRequest\x1a(.nifgen_grpc.DisableStartTriggerResponse\x12\x65\n\x12\x45nableAnalogFilter\x12&.nifgen_grpc.EnableAnalogFilterRequest\x1a\'.nifgen_grpc.EnableAnalogFilterResponse\x12h\n\x13\x45nableDigitalFilter\x12\'.nifgen_grpc.EnableDigitalFilterRequest\x1a(.nifgen_grpc.EnableDigitalFilterResponse\x12t\n\x17\x45nableDigitalPatterning\x12+.nifgen_grpc.EnableDigitalPatterningRequest\x1a,.nifgen_grpc.EnableDigitalPatterningResponse\x12S\n\x0c\x45rrorHandler\x12 .nifgen_grpc.ErrorHandlerRequest\x1a!.nifgen_grpc.ErrorHandlerResponse\x12S\n\x0c\x45rrorMessage\x12 .nifgen_grpc.ErrorMessageRequest\x1a!.nifgen_grpc.ErrorMessageResponse\x12M\n\nErrorQuery\x12\x1e.nifgen_grpc.ErrorQueryRequest\x1a\x1f.nifgen_grpc.ErrorQueryResponse\x12\x95\x01\n\"ExportAttributeConfigurationBuffer\x12\x36.nifgen_grpc.ExportAttributeConfigurationBufferRequest\x1a\x37.nifgen_grpc.ExportAttributeConfigurationBufferResponse\x12\x8f\x01\n ExportAttributeConfigurationFile\x12\x34.nifgen_grpc.ExportAttributeConfigurationFileRequest\x1a\x35.nifgen_grpc.ExportAttributeConfigurationFileResponse\x12S\n\x0c\x45xportSignal\x12 .nifgen_grpc.ExportSignalRequest\x1a!.nifgen_grpc.ExportSignalResponse\x12n\n\x15GetAttributeViBoolean\x12).nifgen_grpc.GetAttributeViBooleanRequest\x1a*.nifgen_grpc.GetAttributeViBooleanResponse\x12h\n\x13GetAttributeViInt32\x12\'.nifgen_grpc.GetAttributeViInt32Request\x1a(.nifgen_grpc.GetAttributeViInt32Response\x12h\n\x13GetAttributeViInt64\x12\'.nifgen_grpc.GetAttributeViInt64Request\x1a(.nifgen_grpc.GetAttributeViInt64Response\x12k\n\x14GetAttributeViReal64\x12(.nifgen_grpc.GetAttributeViReal64Request\x1a).nifgen_grpc.GetAttributeViReal64Response\x12n\n\x15GetAttributeViSession\x12).nifgen_grpc.GetAttributeViSessionRequest\x1a*.nifgen_grpc.GetAttributeViSessionResponse\x12k\n\x14GetAttributeViString\x12(.nifgen_grpc.GetAttributeViStringRequest\x1a).nifgen_grpc.GetAttributeViStringResponse\x12Y\n\x0eGetChannelName\x12\".nifgen_grpc.GetChannelNameRequest\x1a#.nifgen_grpc.GetChannelNameResponse\x12G\n\x08GetError\x12\x1c.nifgen_grpc.GetErrorRequest\x1a\x1d.nifgen_grpc.GetErrorResponse\x12w\n\x18GetExtCalLastDateAndTime\x12,.nifgen_grpc.GetExtCalLastDateAndTimeRequest\x1a-.nifgen_grpc.GetExtCalLastDateAndTimeResponse\x12\x62\n\x11GetExtCalLastTemp\x12%.nifgen_grpc.GetExtCalLastTempRequest\x1a&.nifgen_grpc.GetExtCalLastTempResponse\x12\x83\x01\n\x1cGetExtCalRecommendedInterval\x12\x30.nifgen_grpc.GetExtCalRecommendedIntervalRequest\x1a\x31.nifgen_grpc.GetExtCalRecommendedIntervalResponse\x12w\n\x18GetFIRFilterCoefficients\x12,.nifgen_grpc.GetFIRFilterCoefficientsRequest\x1a-.nifgen_grpc.GetFIRFilterCoefficientsResponse\x12_\n\x10GetHardwareState\x12$.nifgen_grpc.GetHardwareStateRequest\x1a%.nifgen_grpc.GetHardwareStateResponse\x12n\n\x15GetNextCoercionRecord\x12).nifgen_grpc.GetNextCoercionRecordRequest\x1a*.nifgen_grpc.GetNextCoercionRecordResponse\x12z\n\x19GetNextInterchangeWarning\x12-.nifgen_grpc.GetNextInterchangeWarningRequest\x1a..nifgen_grpc.GetNextInterchangeWarningResponse\x12z\n\x19GetSelfCalLastDateAndTime\x12-.nifgen_grpc.GetSelfCalLastDateAndTimeRequest\x1a..nifgen_grpc.GetSelfCalLastDateAndTimeResponse\x12\x65\n\x12GetSelfCalLastTemp\x12&.nifgen_grpc.GetSelfCalLastTempRequest\x1a\'.nifgen_grpc.GetSelfCalLastTempResponse\x12h\n\x13GetSelfCalSupported\x12\'.nifgen_grpc.GetSelfCalSupportedRequest\x1a(.nifgen_grpc.GetSelfCalSupportedResponse\x12t\n\x17GetStreamEndpointHandle\x12+.nifgen_grpc.GetStreamEndpointHandleRequest\x1a,.nifgen_grpc.GetStreamEndpointHandleResponse\x12\x95\x01\n\"ImportAttributeConfigurationBuffer\x12\x36.nifgen_grpc.ImportAttributeConfigurationBufferRequest\x1a\x37.nifgen_grpc.ImportAttributeConfigurationBufferResponse\x12\x8f\x01\n ImportAttributeConfigurationFile\x12\x34.nifgen_grpc.ImportAttributeConfigurationFileRequest\x1a\x35.nifgen_grpc.ImportAttributeConfigurationFileResponse\x12;\n\x04Init\x12\x18.nifgen_grpc.InitRequest\x1a\x19.nifgen_grpc.InitResponse\x12\\\n\x0fInitWithOptions\x12#.nifgen_grpc.InitWithOptionsRequest\x1a$.nifgen_grpc.InitWithOptionsResponse\x12q\n\x16InitializeWithChannels\x12*.nifgen_grpc.InitializeWithChannelsRequest\x1a+.nifgen_grpc.InitializeWithChannelsResponse\x12\x65\n\x12InitiateGeneration\x12&.nifgen_grpc.InitiateGenerationRequest\x1a\'.nifgen_grpc.InitiateGenerationResponse\x12t\n\x17InvalidateAllAttributes\x12+.nifgen_grpc.InvalidateAllAttributesRequest\x1a,.nifgen_grpc.InvalidateAllAttributesResponse\x12\x41\n\x06IsDone\x12\x1a.nifgen_grpc.IsDoneRequest\x1a\x1b.nifgen_grpc.IsDoneResponse\x12n\n\x15ManualEnableP2PStream\x12).nifgen_grpc.ManualEnableP2PStreamRequest\x1a*.nifgen_grpc.ManualEnableP2PStreamResponse\x12t\n\x17QueryArbSeqCapabilities\x12+.nifgen_grpc.QueryArbSeqCapabilitiesRequest\x1a,.nifgen_grpc.QueryArbSeqCapabilitiesResponse\x12t\n\x17QueryArbWfmCapabilities\x12+.nifgen_grpc.QueryArbWfmCapabilitiesRequest\x1a,.nifgen_grpc.QueryArbWfmCapabilitiesResponse\x12z\n\x19QueryFreqListCapabilities\x12-.nifgen_grpc.QueryFreqListCapabilitiesRequest\x1a..nifgen_grpc.QueryFreqListCapabilitiesResponse\x12q\n\x16ReadCurrentTemperature\x12*.nifgen_grpc.ReadCurrentTemperatureRequest\x1a+.nifgen_grpc.ReadCurrentTemperatureResponse\x12>\n\x05Reset\x12\x19.nifgen_grpc.ResetRequest\x1a\x1a.nifgen_grpc.ResetResponse\x12Y\n\x0eResetAttribute\x12\".nifgen_grpc.ResetAttributeRequest\x1a#.nifgen_grpc.ResetAttributeResponse\x12P\n\x0bResetDevice\x12\x1f.nifgen_grpc.ResetDeviceRequest\x1a .nifgen_grpc.ResetDeviceResponse\x12n\n\x15ResetInterchangeCheck\x12).nifgen_grpc.ResetInterchangeCheckRequest\x1a*.nifgen_grpc.ResetInterchangeCheckResponse\x12\x62\n\x11ResetWithDefaults\x12%.nifgen_grpc.ResetWithDefaultsRequest\x1a&.nifgen_grpc.ResetWithDefaultsResponse\x12V\n\rRevisionQuery\x12!.nifgen_grpc.RevisionQueryRequest\x1a\".nifgen_grpc.RevisionQueryResponse\x12Y\n\x0eRouteSignalOut\x12\".nifgen_grpc.RouteSignalOutRequest\x1a#.nifgen_grpc.RouteSignalOutResponse\x12\x44\n\x07SelfCal\x12\x1b.nifgen_grpc.SelfCalRequest\x1a\x1c.nifgen_grpc.SelfCalResponse\x12G\n\x08SelfTest\x12\x1c.nifgen_grpc.SelfTestRequest\x1a\x1d.nifgen_grpc.SelfTestResponse\x12t\n\x17SendSoftwareEdgeTrigger\x12+.nifgen_grpc.SendSoftwareEdgeTriggerRequest\x1a,.nifgen_grpc.SendSoftwareEdgeTriggerResponse\x12n\n\x15SetAttributeViBoolean\x12).nifgen_grpc.SetAttributeViBooleanRequest\x1a*.nifgen_grpc.SetAttributeViBooleanResponse\x12h\n\x13SetAttributeViInt32\x12\'.nifgen_grpc.SetAttributeViInt32Request\x1a(.nifgen_grpc.SetAttributeViInt32Response\x12h\n\x13SetAttributeViInt64\x12\'.nifgen_grpc.SetAttributeViInt64Request\x1a(.nifgen_grpc.SetAttributeViInt64Response\x12k\n\x14SetAttributeViReal64\x12(.nifgen_grpc.SetAttributeViReal64Request\x1a).nifgen_grpc.SetAttributeViReal64Response\x12n\n\x15SetAttributeViSession\x12).nifgen_grpc.SetAttributeViSessionRequest\x1a*.nifgen_grpc.SetAttributeViSessionResponse\x12k\n\x14SetAttributeViString\x12(.nifgen_grpc.SetAttributeViStringRequest\x1a).nifgen_grpc.SetAttributeViStringResponse\x12\x92\x01\n!SetNamedWaveformNextWritePosition\x12\x35.nifgen_grpc.SetNamedWaveformNextWritePositionRequest\x1a\x36.nifgen_grpc.SetNamedWaveformNextWritePositionResponse\x12\x83\x01\n\x1cSetWaveformNextWritePosition\x12\x30.nifgen_grpc.SetWaveformNextWritePositionRequest\x1a\x31.nifgen_grpc.SetWaveformNextWritePositionResponse\x12V\n\rWaitUntilDone\x12!.nifgen_grpc.WaitUntilDoneRequest\x1a\".nifgen_grpc.WaitUntilDoneResponse\x12n\n\x15WriteBinary16Waveform\x12).nifgen_grpc.WriteBinary16WaveformRequest\x1a*.nifgen_grpc.WriteBinary16WaveformResponse\x12\x83\x01\n\x1cWriteComplexBinary16Waveform\x12\x30.nifgen_grpc.WriteComplexBinary16WaveformRequest\x1a\x31.nifgen_grpc.WriteComplexBinary16WaveformResponse\x12\x83\x01\n\x1cWriteNamedWaveformComplexF64\x12\x30.nifgen_grpc.WriteNamedWaveformComplexF64Request\x1a\x31.nifgen_grpc.WriteNamedWaveformComplexF64Response\x12\x83\x01\n\x1cWriteNamedWaveformComplexI16\x12\x30.nifgen_grpc.WriteNamedWaveformComplexI16Request\x1a\x31.nifgen_grpc.WriteNamedWaveformComplexI16Response\x12n\n\x15WriteNamedWaveformF64\x12).nifgen_grpc.WriteNamedWaveformF64Request\x1a*.nifgen_grpc.WriteNamedWaveformF64Response\x12n\n\x15WriteNamedWaveformI16\x12).nifgen_grpc.WriteNamedWaveformI16Request\x1a*.nifgen_grpc.WriteNamedWaveformI16Response\x12h\n\x13WriteP2PEndpointI16\x12\'.nifgen_grpc.WriteP2PEndpointI16Request\x1a(.nifgen_grpc.WriteP2PEndpointI16Response\x12P\n\x0bWriteScript\x12\x1f.nifgen_grpc.WriteScriptRequest\x1a .nifgen_grpc.WriteScriptResponse\x12V\n\rWriteWaveform\x12!.nifgen_grpc.WriteWaveformRequest\x1a\".nifgen_grpc.WriteWaveformResponse\x12t\n\x17WriteWaveformComplexF64\x12+.nifgen_grpc.WriteWaveformComplexF64Request\x1a,.nifgen_grpc.WriteWaveformComplexF64ResponseB<\n\x10\x63om.ni.grpc.fgenB\x06NiFgenP\x01\xaa\x02\x1dNationalInstruments.Grpc.Fgenb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cnifgen.proto\x12\x0bnifgen_grpc\x1a\x0enidevice.proto\x1a\rsession.proto\"<\n\x16\x41\x62ortGenerationRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\")\n\x17\x41\x62ortGenerationResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"d\n%AdjustSampleClockRelativeDelayRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x17\n\x0f\x61\x64justment_time\x18\x02 \x01(\x01\"8\n&AdjustSampleClockRelativeDelayResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x86\x01\n\x1c\x41llocateNamedWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12\x15\n\rwaveform_size\x18\x04 \x01(\x11\"/\n\x1d\x41llocateNamedWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"j\n\x17\x41llocateWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_size\x18\x03 \x01(\x11\"C\n\x18\x41llocateWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"\xa7\x01\n\x1e\x43heckAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x17\n\x0f\x61ttribute_value\x18\x04 \x01(\x08\"1\n\x1f\x43heckAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x87\x02\n\x1c\x43heckAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x42\n\x0f\x61ttribute_value\x18\x04 \x01(\x0e\x32\'.nifgen_grpc.NiFgenInt32AttributeValuesH\x00\x12\x1d\n\x13\x61ttribute_value_raw\x18\x05 \x01(\x11H\x00\x42\x16\n\x14\x61ttribute_value_enum\"/\n\x1d\x43heckAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa9\x01\n\x1c\x43heckAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x1b\n\x13\x61ttribute_value_raw\x18\x04 \x01(\x03\"/\n\x1d\x43heckAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x89\x02\n\x1d\x43heckAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x43\n\x0f\x61ttribute_value\x18\x04 \x01(\x0e\x32(.nifgen_grpc.NiFgenReal64AttributeValuesH\x00\x12\x1d\n\x13\x61ttribute_value_raw\x18\x05 \x01(\x01H\x00\x42\x16\n\x14\x61ttribute_value_enum\"0\n\x1e\x43heckAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xbf\x01\n\x1e\x43heckAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12/\n\x0f\x61ttribute_value\x18\x04 \x01(\x0b\x32\x16.nidevice_grpc.Session\"1\n\x1f\x43heckAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x96\x02\n\x1d\x43heckAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x1d\n\x13\x61ttribute_value_raw\x18\x04 \x01(\tH\x00\x12P\n\x16\x61ttribute_value_mapped\x18\x05 \x01(\x0e\x32..nifgen_grpc.NiFgenStringAttributeValuesMappedH\x00\x42\x16\n\x14\x61ttribute_value_enum\"0\n\x1e\x43heckAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\";\n\x15\x43learArbMemoryRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"(\n\x16\x43learArbMemoryResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xac\x01\n\x17\x43learArbSequenceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x36\n\x0fsequence_handle\x18\x02 \x01(\x0e\x32\x1b.nifgen_grpc.SequenceHandleH\x00\x12\x1d\n\x13sequence_handle_raw\x18\x03 \x01(\x11H\x00\x42\x16\n\x14sequence_handle_enum\"*\n\x18\x43learArbSequenceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xac\x01\n\x17\x43learArbWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x36\n\x0fwaveform_handle\x18\x02 \x01(\x0e\x32\x1b.nifgen_grpc.WaveformHandleH\x00\x12\x1d\n\x13waveform_handle_raw\x18\x03 \x01(\x11H\x00\x42\x16\n\x14waveform_handle_enum\"*\n\x18\x43learArbWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"7\n\x11\x43learErrorRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"$\n\x12\x43learErrorResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xc1\x01\n\x14\x43learFreqListRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x42\n\x15\x66requency_list_handle\x18\x02 \x01(\x0e\x32!.nifgen_grpc.FrequencyListOptionsH\x00\x12#\n\x19\x66requency_list_handle_raw\x18\x03 \x01(\x11H\x00\x42\x1c\n\x1a\x66requency_list_handle_enum\"\'\n\x15\x43learFreqListResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"E\n\x1f\x43learInterchangeWarningsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"2\n ClearInterchangeWarningsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\\\n ClearUserStandardWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"3\n!ClearUserStandardWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"2\n\x0c\x43loseRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rCloseResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"3\n\rCommitRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\" \n\x0e\x43ommitResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"h\n\x19\x43onfigureAmplitudeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\tamplitude\x18\x03 \x01(\x01\",\n\x1a\x43onfigureAmplitudeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8e\x01\n\x1b\x43onfigureArbSequenceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fsequence_handle\x18\x03 \x01(\x11\x12\x0c\n\x04gain\x18\x04 \x01(\x01\x12\x0e\n\x06offset\x18\x05 \x01(\x01\".\n\x1c\x43onfigureArbSequenceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8e\x01\n\x1b\x43onfigureArbWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fwaveform_handle\x18\x03 \x01(\x11\x12\x0c\n\x04gain\x18\x04 \x01(\x01\x12\x0e\n\x06offset\x18\x05 \x01(\x01\".\n\x1c\x43onfigureArbWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"P\n\x18\x43onfigureChannelsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x10\n\x08\x63hannels\x18\x02 \x01(\t\"+\n\x19\x43onfigureChannelsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x9a\x01\n\x19\x43onfigureClockModeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12,\n\nclock_mode\x18\x02 \x01(\x0e\x32\x16.nifgen_grpc.ClockModeH\x00\x12\x18\n\x0e\x63lock_mode_raw\x18\x03 \x01(\x11H\x00\x42\x11\n\x0f\x63lock_mode_enum\",\n\x1a\x43onfigureClockModeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x83\x01\n+ConfigureCustomFIRFilterCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1a\n\x12\x63oefficients_array\x18\x03 \x03(\x01\">\n,ConfigureCustomFIRFilterCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x80\x01\n(ConfigureDigitalEdgeScriptTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\ntrigger_id\x18\x02 \x01(\t\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x0c\n\x04\x65\x64ge\x18\x04 \x01(\x11\";\n)ConfigureDigitalEdgeScriptTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"k\n\'ConfigureDigitalEdgeStartTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0c\n\x04\x65\x64ge\x18\x03 \x01(\x11\":\n(ConfigureDigitalEdgeStartTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xd6\x01\n)ConfigureDigitalLevelScriptTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\ntrigger_id\x18\x02 \x01(\t\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x30\n\x0ctrigger_when\x18\x04 \x01(\x0e\x32\x18.nifgen_grpc.TriggerWhenH\x00\x12\x1a\n\x10trigger_when_raw\x18\x05 \x01(\x11H\x00\x42\x13\n\x11trigger_when_enum\"<\n*ConfigureDigitalLevelScriptTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xae\x01\n\x18\x43onfigureFreqListRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1d\n\x15\x66requency_list_handle\x18\x03 \x01(\x11\x12\x11\n\tamplitude\x18\x04 \x01(\x01\x12\x11\n\tdc_offset\x18\x05 \x01(\x01\x12\x13\n\x0bstart_phase\x18\x06 \x01(\x01\"+\n\x19\x43onfigureFreqListResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"h\n\x19\x43onfigureFrequencyRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\tfrequency\x18\x03 \x01(\x01\",\n\x1a\x43onfigureFrequencyResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"q\n\x1d\x43onfigureOperationModeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x16\n\x0eoperation_mode\x18\x03 \x01(\x11\"0\n\x1e\x43onfigureOperationModeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"j\n\x1d\x43onfigureOutputEnabledRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x0f\n\x07\x65nabled\x18\x03 \x01(\x08\"0\n\x1e\x43onfigureOutputEnabledResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"n\n\x1f\x43onfigureOutputImpedanceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\timpedance\x18\x03 \x01(\x01\"2\n ConfigureOutputImpedanceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x9f\x01\n\x1a\x43onfigureOutputModeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12.\n\x0boutput_mode\x18\x02 \x01(\x0e\x32\x17.nifgen_grpc.OutputModeH\x00\x12\x19\n\x0foutput_mode_raw\x18\x03 \x01(\x11H\x00\x42\x12\n\x10output_mode_enum\"-\n\x1b\x43onfigureOutputModeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"z\n/ConfigureP2PEndpointFullnessStartTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12#\n\x1bp2p_endpoint_fullness_level\x18\x02 \x01(\x11\"B\n0ConfigureP2PEndpointFullnessStartTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x87\x01\n\x1e\x43onfigureReferenceClockRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x1e\n\x16reference_clock_source\x18\x02 \x01(\t\x12!\n\x19reference_clock_frequency\x18\x03 \x01(\x01\"1\n\x1f\x43onfigureReferenceClockResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"d\n!ConfigureSampleClockSourceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x1b\n\x13sample_clock_source\x18\x02 \x01(\t\"4\n\"ConfigureSampleClockSourceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"U\n\x1a\x43onfigureSampleRateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x13\n\x0bsample_rate\x18\x02 \x01(\x01\"-\n\x1b\x43onfigureSampleRateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"c\n)ConfigureSoftwareEdgeScriptTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\ntrigger_id\x18\x02 \x01(\t\"<\n*ConfigureSoftwareEdgeScriptTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"N\n(ConfigureSoftwareEdgeStartTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\";\n)ConfigureSoftwareEdgeStartTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xfe\x01\n ConfigureStandardWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12)\n\x08waveform\x18\x03 \x01(\x0e\x32\x15.nifgen_grpc.WaveformH\x00\x12\x16\n\x0cwaveform_raw\x18\x04 \x01(\x11H\x00\x12\x11\n\tamplitude\x18\x05 \x01(\x01\x12\x11\n\tdc_offset\x18\x06 \x01(\x01\x12\x11\n\tfrequency\x18\x07 \x01(\x01\x12\x13\n\x0bstart_phase\x18\x08 \x01(\x01\x42\x0f\n\rwaveform_enum\"3\n!ConfigureStandardWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"{\n\x1f\x43onfigureSynchronizationRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1e\n\x16synchronization_source\x18\x03 \x01(\x11\"2\n ConfigureSynchronizationResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xba\x01\n\x1b\x43onfigureTriggerModeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x30\n\x0ctrigger_mode\x18\x03 \x01(\x0e\x32\x18.nifgen_grpc.TriggerModeH\x00\x12\x1a\n\x10trigger_mode_raw\x18\x04 \x01(\x11H\x00\x42\x13\n\x11trigger_mode_enum\".\n\x1c\x43onfigureTriggerModeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xbd\x01\n CreateAdvancedArbSequenceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x1e\n\x16waveform_handles_array\x18\x02 \x03(\x11\x12\x19\n\x11loop_counts_array\x18\x03 \x03(\x11\x12\x1b\n\x13sample_counts_array\x18\x04 \x03(\x11\x12\x1d\n\x15marker_location_array\x18\x05 \x03(\x11\"k\n!CreateAdvancedArbSequenceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1d\n\x15\x63oerced_markers_array\x18\x02 \x03(\x11\x12\x17\n\x0fsequence_handle\x18\x03 \x01(\x11\"y\n\x18\x43reateArbSequenceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x1e\n\x16waveform_handles_array\x18\x02 \x03(\x11\x12\x19\n\x11loop_counts_array\x18\x03 \x03(\x11\"D\n\x19\x43reateArbSequenceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fsequence_handle\x18\x02 \x01(\x11\"\xc0\x01\n\x15\x43reateFreqListRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12)\n\x08waveform\x18\x02 \x01(\x0e\x32\x15.nifgen_grpc.WaveformH\x00\x12\x16\n\x0cwaveform_raw\x18\x03 \x01(\x11H\x00\x12\x17\n\x0f\x66requency_array\x18\x04 \x03(\x01\x12\x16\n\x0e\x64uration_array\x18\x05 \x03(\x01\x42\x0f\n\rwaveform_enum\"G\n\x16\x43reateFreqListResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1d\n\x15\x66requency_list_handle\x18\x02 \x01(\x11\"\x98\x01\n\x1f\x43reateWaveformComplexF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12;\n\x13waveform_data_array\x18\x03 \x03(\x0b\x32\x1e.nidevice_grpc.NIComplexNumber\"K\n CreateWaveformComplexF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"q\n\x18\x43reateWaveformF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1b\n\x13waveform_data_array\x18\x03 \x03(\x01\"D\n\x19\x43reateWaveformF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"\xca\x01\n CreateWaveformFromFileF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\tfile_name\x18\x03 \x01(\t\x12,\n\nbyte_order\x18\x04 \x01(\x0e\x32\x16.nifgen_grpc.ByteOrderH\x00\x12\x18\n\x0e\x62yte_order_raw\x18\x05 \x01(\x11H\x00\x42\x11\n\x0f\x62yte_order_enum\"L\n!CreateWaveformFromFileF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"\xca\x01\n CreateWaveformFromFileI16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\tfile_name\x18\x03 \x01(\t\x12,\n\nbyte_order\x18\x04 \x01(\x0e\x32\x16.nifgen_grpc.ByteOrderH\x00\x12\x18\n\x0e\x62yte_order_raw\x18\x05 \x01(\x11H\x00\x42\x11\n\x0f\x62yte_order_enum\"L\n!CreateWaveformFromFileI16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"q\n\x18\x43reateWaveformI16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1b\n\x13waveform_data_array\x18\x03 \x03(\x11\"D\n\x19\x43reateWaveformI16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"z\n!DefineUserStandardWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x1b\n\x13waveform_data_array\x18\x03 \x03(\x01\"4\n\"DefineUserStandardWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"m\n\x1a\x44\x65leteNamedWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\"-\n\x1b\x44\x65leteNamedWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"d\n\x13\x44\x65leteScriptRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x13\n\x0bscript_name\x18\x03 \x01(\t\"&\n\x14\x44\x65leteScriptResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"4\n\x0e\x44isableRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"!\n\x0f\x44isableResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"V\n\x1a\x44isableAnalogFilterRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"-\n\x1b\x44isableAnalogFilterResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"W\n\x1b\x44isableDigitalFilterRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\".\n\x1c\x44isableDigitalFilterResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"[\n\x1f\x44isableDigitalPatterningRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"2\n DisableDigitalPatterningResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"U\n\x1b\x44isableScriptTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\ntrigger_id\x18\x02 \x01(\t\".\n\x1c\x44isableScriptTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"@\n\x1a\x44isableStartTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"-\n\x1b\x44isableStartTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"z\n\x19\x45nableAnalogFilterRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12#\n\x1b\x66ilter_correction_frequency\x18\x03 \x01(\x01\",\n\x1a\x45nableAnalogFilterResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"V\n\x1a\x45nableDigitalFilterRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"-\n\x1b\x45nableDigitalFilterResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"Z\n\x1e\x45nableDigitalPatterningRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"1\n\x1f\x45nableDigitalPatterningResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"M\n\x13\x45rrorHandlerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nerror_code\x18\x02 \x01(\x11\"=\n\x14\x45rrorHandlerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"M\n\x13\x45rrorMessageRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nerror_code\x18\x02 \x01(\x11\"=\n\x14\x45rrorMessageResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"7\n\x11\x45rrorQueryRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"O\n\x12\x45rrorQueryResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x12\n\nerror_code\x18\x02 \x01(\x11\x12\x15\n\rerror_message\x18\x03 \x01(\t\"O\n)ExportAttributeConfigurationBufferRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"S\n*ExportAttributeConfigurationBufferResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rconfiguration\x18\x02 \x01(\x0c\"`\n\'ExportAttributeConfigurationFileRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x11\n\tfile_path\x18\x02 \x01(\t\":\n(ExportAttributeConfigurationFileResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb9\x01\n\x13\x45xportSignalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12%\n\x06signal\x18\x02 \x01(\x0e\x32\x13.nifgen_grpc.SignalH\x00\x12\x14\n\nsignal_raw\x18\x03 \x01(\x11H\x00\x12\x19\n\x11signal_identifier\x18\x04 \x01(\t\x12\x17\n\x0foutput_terminal\x18\x05 \x01(\tB\r\n\x0bsignal_enum\"&\n\x14\x45xportSignalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8c\x01\n\x1cGetAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"H\n\x1dGetAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\x08\"\x8a\x01\n\x1aGetAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"F\n\x1bGetAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\x11\"\x8a\x01\n\x1aGetAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"F\n\x1bGetAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\x03\"\x8b\x01\n\x1bGetAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"G\n\x1cGetAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\x01\"\x8c\x01\n\x1cGetAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"`\n\x1dGetAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12/\n\x0f\x61ttribute_value\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x8b\x01\n\x1bGetAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"G\n\x1cGetAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\t\"J\n\x15GetChannelNameRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\r\n\x05index\x18\x02 \x01(\x11\"@\n\x16GetChannelNameResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x16\n\x0e\x63hannel_string\x18\x02 \x01(\t\"5\n\x0fGetErrorRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"Q\n\x10GetErrorResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x12\n\nerror_code\x18\x02 \x01(\x11\x12\x19\n\x11\x65rror_description\x18\x03 \x01(\t\"E\n\x1fGetExtCalLastDateAndTimeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"z\n GetExtCalLastDateAndTimeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04year\x18\x02 \x01(\x11\x12\r\n\x05month\x18\x03 \x01(\x11\x12\x0b\n\x03\x64\x61y\x18\x04 \x01(\x11\x12\x0c\n\x04hour\x18\x05 \x01(\x11\x12\x0e\n\x06minute\x18\x06 \x01(\x11\">\n\x18GetExtCalLastTempRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"@\n\x19GetExtCalLastTempResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"I\n#GetExtCalRecommendedIntervalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"F\n$GetExtCalRecommendedIntervalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06months\x18\x02 \x01(\x11\"[\n\x1fGetFIRFilterCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\"s\n GetFIRFilterCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1a\n\x12\x63oefficients_array\x18\x02 \x03(\x01\x12#\n\x1bnumber_of_coefficients_read\x18\x03 \x01(\x11\"=\n\x17GetHardwareStateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"h\n\x18GetHardwareStateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12)\n\x05state\x18\x02 \x01(\x0e\x32\x1a.nifgen_grpc.HardwareState\x12\x11\n\tstate_raw\x18\x03 \x01(\x11\"F\n GetSelfCalLastDateAndTimeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"{\n!GetSelfCalLastDateAndTimeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04year\x18\x02 \x01(\x11\x12\r\n\x05month\x18\x03 \x01(\x11\x12\x0b\n\x03\x64\x61y\x18\x04 \x01(\x11\x12\x0c\n\x04hour\x18\x05 \x01(\x11\x12\x0e\n\x06minute\x18\x06 \x01(\x11\"?\n\x19GetSelfCalLastTempRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"A\n\x1aGetSelfCalLastTempResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"@\n\x1aGetSelfCalSupportedRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"I\n\x1bGetSelfCalSupportedResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1a\n\x12self_cal_supported\x18\x02 \x01(\x08\"]\n\x1eGetStreamEndpointHandleRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x17\n\x0fstream_endpoint\x18\x02 \x01(\t\"H\n\x1fGetStreamEndpointHandleResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rreader_handle\x18\x02 \x01(\r\"f\n)ImportAttributeConfigurationBufferRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x15\n\rconfiguration\x18\x02 \x01(\x0c\"<\n*ImportAttributeConfigurationBufferResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"`\n\'ImportAttributeConfigurationFileRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x11\n\tfile_path\x18\x02 \x01(\t\":\n(ImportAttributeConfigurationFileResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb1\x01\n\x0bInitRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x10\n\x08id_query\x18\x03 \x01(\x08\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12M\n\x17initialization_behavior\x18\x05 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"~\n\x0cInitResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"\xd3\x01\n\x16InitWithOptionsRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x10\n\x08id_query\x18\x03 \x01(\x08\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12\x15\n\roption_string\x18\x05 \x01(\t\x12M\n\x17initialization_behavior\x18\x06 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"\x89\x01\n\x17InitWithOptionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"\xde\x01\n\x1dInitializeWithChannelsRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x14\n\x0c\x63hannel_name\x18\x03 \x01(\t\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12\x15\n\roption_string\x18\x05 \x01(\t\x12M\n\x17initialization_behavior\x18\x06 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"\x90\x01\n\x1eInitializeWithChannelsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"?\n\x19InitiateGenerationRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\",\n\x1aInitiateGenerationResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"D\n\x1eInvalidateAllAttributesRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"1\n\x1fInvalidateAllAttributesResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"3\n\rIsDoneRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\".\n\x0eIsDoneResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04\x64one\x18\x02 \x01(\x08\"D\n\x1eQueryArbSeqCapabilitiesRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\xb4\x01\n\x1fQueryArbSeqCapabilitiesResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12#\n\x1bmaximum_number_of_sequences\x18\x02 \x01(\x11\x12\x1f\n\x17minimum_sequence_length\x18\x03 \x01(\x11\x12\x1f\n\x17maximum_sequence_length\x18\x04 \x01(\x11\x12\x1a\n\x12maximum_loop_count\x18\x05 \x01(\x11\"D\n\x1eQueryArbWfmCapabilitiesRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\xae\x01\n\x1fQueryArbWfmCapabilitiesResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12#\n\x1bmaximum_number_of_waveforms\x18\x02 \x01(\x11\x12\x18\n\x10waveform_quantum\x18\x03 \x01(\x11\x12\x1d\n\x15minimum_waveform_size\x18\x04 \x01(\x11\x12\x1d\n\x15maximum_waveform_size\x18\x05 \x01(\x11\"F\n QueryFreqListCapabilitiesRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\xa2\x02\n!QueryFreqListCapabilitiesResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12$\n\x1cmaximum_number_of_freq_lists\x18\x02 \x01(\x11\x12%\n\x1dminimum_frequency_list_length\x18\x03 \x01(\x11\x12%\n\x1dmaximum_frequency_list_length\x18\x04 \x01(\x11\x12\'\n\x1fminimum_frequency_list_duration\x18\x05 \x01(\x01\x12\'\n\x1fmaximum_frequency_list_duration\x18\x06 \x01(\x01\x12\'\n\x1f\x66requency_list_duration_quantum\x18\x07 \x01(\x01\"C\n\x1dReadCurrentTemperatureRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"E\n\x1eReadCurrentTemperatureResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"2\n\x0cResetRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rResetResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x85\x01\n\x15ResetAttributeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\"(\n\x16ResetAttributeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"8\n\x12ResetDeviceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"%\n\x13ResetDeviceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"B\n\x1cResetInterchangeCheckRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"/\n\x1dResetInterchangeCheckResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\">\n\x18ResetWithDefaultsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"+\n\x19ResetWithDefaultsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\":\n\x14RevisionQueryRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"f\n\x15RevisionQueryResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x1ainstrument_driver_revision\x18\x02 \x01(\t\x12\x19\n\x11\x66irmware_revision\x18\x03 \x01(\t\"\xb5\x02\n\x15RouteSignalOutRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x39\n\x11route_signal_from\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.RouteSignalFromH\x00\x12\x1f\n\x15route_signal_from_raw\x18\x04 \x01(\x11H\x00\x12\x35\n\x0froute_signal_to\x18\x05 \x01(\x0e\x32\x1a.nifgen_grpc.RouteSignalToH\x01\x12\x1d\n\x13route_signal_to_raw\x18\x06 \x01(\x11H\x01\x42\x18\n\x16route_signal_from_enumB\x16\n\x14route_signal_to_enum\"(\n\x16RouteSignalOutResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"4\n\x0eSelfCalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"!\n\x0fSelfCalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"5\n\x0fSelfTestRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"W\n\x10SelfTestResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x18\n\x10self_test_result\x18\x02 \x01(\x11\x12\x19\n\x11self_test_message\x18\x03 \x01(\t\"\xa8\x01\n\x1eSendSoftwareEdgeTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\'\n\x07trigger\x18\x02 \x01(\x0e\x32\x14.nifgen_grpc.TriggerH\x00\x12\x15\n\x0btrigger_raw\x18\x03 \x01(\x11H\x00\x12\x12\n\ntrigger_id\x18\x04 \x01(\tB\x0e\n\x0ctrigger_enum\"1\n\x1fSendSoftwareEdgeTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa5\x01\n\x1cSetAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x17\n\x0f\x61ttribute_value\x18\x04 \x01(\x08\"/\n\x1dSetAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x85\x02\n\x1aSetAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x42\n\x0f\x61ttribute_value\x18\x04 \x01(\x0e\x32\'.nifgen_grpc.NiFgenInt32AttributeValuesH\x00\x12\x1d\n\x13\x61ttribute_value_raw\x18\x05 \x01(\x11H\x00\x42\x16\n\x14\x61ttribute_value_enum\"-\n\x1bSetAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa7\x01\n\x1aSetAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x1b\n\x13\x61ttribute_value_raw\x18\x04 \x01(\x03\"-\n\x1bSetAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x87\x02\n\x1bSetAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x43\n\x0f\x61ttribute_value\x18\x04 \x01(\x0e\x32(.nifgen_grpc.NiFgenReal64AttributeValuesH\x00\x12\x1d\n\x13\x61ttribute_value_raw\x18\x05 \x01(\x01H\x00\x42\x16\n\x14\x61ttribute_value_enum\".\n\x1cSetAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xbd\x01\n\x1cSetAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12/\n\x0f\x61ttribute_value\x18\x04 \x01(\x0b\x32\x16.nidevice_grpc.Session\"/\n\x1dSetAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x94\x02\n\x1bSetAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x32\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1c.nifgen_grpc.NiFgenAttribute\x12\x1d\n\x13\x61ttribute_value_raw\x18\x04 \x01(\tH\x00\x12P\n\x16\x61ttribute_value_mapped\x18\x05 \x01(\x0e\x32..nifgen_grpc.NiFgenStringAttributeValuesMappedH\x00\x42\x16\n\x14\x61ttribute_value_enum\".\n\x1cSetAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xea\x01\n(SetNamedWaveformNextWritePositionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12.\n\x0brelative_to\x18\x04 \x01(\x0e\x32\x17.nifgen_grpc.RelativeToH\x00\x12\x19\n\x0frelative_to_raw\x18\x05 \x01(\x11H\x00\x12\x0e\n\x06offset\x18\x06 \x01(\x11\x42\x12\n\x10relative_to_enum\";\n)SetNamedWaveformNextWritePositionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xe7\x01\n#SetWaveformNextWritePositionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fwaveform_handle\x18\x03 \x01(\x11\x12.\n\x0brelative_to\x18\x04 \x01(\x0e\x32\x17.nifgen_grpc.RelativeToH\x00\x12\x19\n\x0frelative_to_raw\x18\x05 \x01(\x11H\x00\x12\x0e\n\x06offset\x18\x06 \x01(\x11\x42\x12\n\x10relative_to_enum\"6\n$SetWaveformNextWritePositionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"L\n\x14WaitUntilDoneRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x10\n\x08max_time\x18\x02 \x01(\x11\"\'\n\x15WaitUntilDoneResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x7f\n\x1cWriteBinary16WaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fwaveform_handle\x18\x03 \x01(\x11\x12\x0c\n\x04\x64\x61ta\x18\x04 \x03(\x11\"/\n\x1dWriteBinary16WaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa3\x01\n#WriteComplexBinary16WaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fwaveform_handle\x18\x03 \x01(\x11\x12)\n\x04\x64\x61ta\x18\x04 \x03(\x0b\x32\x1b.nidevice_grpc.NIComplexI16\"6\n$WriteComplexBinary16WaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa4\x01\n#WriteNamedWaveformComplexF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12,\n\x04\x64\x61ta\x18\x04 \x03(\x0b\x32\x1e.nidevice_grpc.NIComplexNumber\"6\n$WriteNamedWaveformComplexF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa1\x01\n#WriteNamedWaveformComplexI16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12)\n\x04\x64\x61ta\x18\x04 \x03(\x0b\x32\x1b.nidevice_grpc.NIComplexI16\"6\n$WriteNamedWaveformComplexI16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"}\n\x1cWriteNamedWaveformF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x03(\x01\"/\n\x1dWriteNamedWaveformF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"}\n\x1cWriteNamedWaveformI16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x15\n\rwaveform_name\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x03(\x11\"/\n\x1dWriteNamedWaveformI16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"n\n\x1aWriteP2PEndpointI16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x15\n\rendpoint_name\x18\x02 \x01(\t\x12\x15\n\rendpoint_data\x18\x03 \x03(\x11\"-\n\x1bWriteP2PEndpointI16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"^\n\x12WriteScriptRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x0e\n\x06script\x18\x03 \x01(\t\"%\n\x13WriteScriptResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"w\n\x14WriteWaveformRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x17\n\x0fwaveform_handle\x18\x03 \x01(\x11\x12\x0c\n\x04\x64\x61ta\x18\x04 \x03(\x01\"\'\n\x15WriteWaveformResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa1\x01\n\x1eWriteWaveformComplexF64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12,\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32\x1e.nidevice_grpc.NIComplexNumber\x12\x17\n\x0fwaveform_handle\x18\x04 \x01(\x11\"1\n\x1fWriteWaveformComplexF64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xba\x01\n CreateWaveformFromFileHWSRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x11\n\tfile_name\x18\x03 \x01(\t\x12\x1e\n\x16use_rate_from_waveform\x18\x04 \x01(\x08\x12)\n!use_gain_and_offset_from_waveform\x18\x05 \x01(\x08\"L\n!CreateWaveformFromFileHWSResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0fwaveform_handle\x18\x02 \x01(\x11\"Y\n\x1cManualEnableP2PStreamRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x15\n\rendpoint_name\x18\x02 \x01(\t\"/\n\x1dManualEnableP2PStreamResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05*\xa9S\n\x0fNiFgenAttribute\x12 \n\x1cNIFGEN_ATTRIBUTE_UNSPECIFIED\x10\x00\x12%\n\x1fNIFGEN_ATTRIBUTE_ABSOLUTE_DELAY\x10\xcd\x9b\x46\x12\x37\n1NIFGEN_ATTRIBUTE_ALL_MARKER_EVENTS_LATCHED_STATUS\x10\x8d\x9b\x46\x12\x34\n.NIFGEN_ATTRIBUTE_ALL_MARKER_EVENTS_LIVE_STATUS\x10\x88\x9b\x46\x12\'\n!NIFGEN_ATTRIBUTE_ANALOG_DATA_MASK\x10\x9a\x9a\x46\x12,\n&NIFGEN_ATTRIBUTE_ANALOG_FILTER_ENABLED\x10\x97\x99\x46\x12\"\n\x1cNIFGEN_ATTRIBUTE_ANALOG_PATH\x10\x8e\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_ANALOG_STATIC_VALUE\x10\x9b\x9a\x46\x12\x1f\n\x19NIFGEN_ATTRIBUTE_ARB_GAIN\x10\x9a\xa7L\x12*\n$NIFGEN_ATTRIBUTE_ARB_MARKER_POSITION\x10\xf7\x9a\x46\x12!\n\x1bNIFGEN_ATTRIBUTE_ARB_OFFSET\x10\x9b\xa7L\x12\'\n!NIFGEN_ATTRIBUTE_ARB_REPEAT_COUNT\x10\xf8\x9a\x46\x12&\n NIFGEN_ATTRIBUTE_ARB_SAMPLE_RATE\x10\x9c\xa7L\x12*\n$NIFGEN_ATTRIBUTE_ARB_SEQUENCE_HANDLE\x10\xa3\xa7L\x12*\n$NIFGEN_ATTRIBUTE_ARB_WAVEFORM_HANDLE\x10\x99\xa7L\x12(\n\"NIFGEN_ATTRIBUTE_AUX_POWER_ENABLED\x10\xcb\x9b\x46\x12\"\n\x1cNIFGEN_ATTRIBUTE_BURST_COUNT\x10\xae\xa8L\x12\x1f\n\x19NIFGEN_ATTRIBUTE_BUS_TYPE\x10\x87\x9a\x46\x12\x1c\n\x16NIFGEN_ATTRIBUTE_CACHE\x10\x94\x8b@\x12$\n\x1eNIFGEN_ATTRIBUTE_CHANNEL_COUNT\x10\xdb\x8c@\x12$\n\x1eNIFGEN_ATTRIBUTE_CHANNEL_DELAY\x10\xa1\x9b\x46\x12!\n\x1bNIFGEN_ATTRIBUTE_CLOCK_MODE\x10\x9e\x99\x46\x12)\n#NIFGEN_ATTRIBUTE_COMMON_MODE_OFFSET\x10\x9e\x9b\x46\x12\x38\n2NIFGEN_ATTRIBUTE_DATA_MARKER_EVENT_DATA_BIT_NUMBER\x10\x81\x9b\x46\x12\x37\n1NIFGEN_ATTRIBUTE_DATA_MARKER_EVENT_LEVEL_POLARITY\x10\x82\x9b\x46\x12\x38\n2NIFGEN_ATTRIBUTE_DATA_MARKER_EVENT_OUTPUT_TERMINAL\x10\x83\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_DATA_MARKER_EVENTS_COUNT\x10\xc1\x9a\x46\x12/\n)NIFGEN_ATTRIBUTE_DATA_TRANSFER_BLOCK_SIZE\x10\xa1\x9a\x46\x12\x36\n0NIFGEN_ATTRIBUTE_DATA_TRANSFER_MAXIMUM_BANDWIDTH\x10\xa5\x9b\x46\x12<\n6NIFGEN_ATTRIBUTE_DATA_TRANSFER_MAXIMUM_IN_FLIGHT_READS\x10\xa7\x9b\x46\x12:\n4NIFGEN_ATTRIBUTE_DATA_TRANSFER_PREFERRED_PACKET_SIZE\x10\xa6\x9b\x46\x12(\n\"NIFGEN_ATTRIBUTE_DIGITAL_DATA_MASK\x10\x9c\x9a\x46\x12\x37\n1NIFGEN_ATTRIBUTE_DIGITAL_EDGE_SCRIPT_TRIGGER_EDGE\x10\xd4\x9a\x46\x12\x39\n3NIFGEN_ATTRIBUTE_DIGITAL_EDGE_SCRIPT_TRIGGER_SOURCE\x10\xd3\x9a\x46\x12\x36\n0NIFGEN_ATTRIBUTE_DIGITAL_EDGE_START_TRIGGER_EDGE\x10\xca\x9a\x46\x12\x38\n2NIFGEN_ATTRIBUTE_DIGITAL_EDGE_START_TRIGGER_SOURCE\x10\xc9\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_DIGITAL_FILTER_ENABLED\x10\x96\x99\x46\x12:\n4NIFGEN_ATTRIBUTE_DIGITAL_FILTER_INTERPOLATION_FACTOR\x10\x8a\x9a\x46\x12#\n\x1dNIFGEN_ATTRIBUTE_DIGITAL_GAIN\x10\xae\x9a\x46\x12@\n:NIFGEN_ATTRIBUTE_DIGITAL_LEVEL_SCRIPT_TRIGGER_ACTIVE_LEVEL\x10\xd6\x9a\x46\x12:\n4NIFGEN_ATTRIBUTE_DIGITAL_LEVEL_SCRIPT_TRIGGER_SOURCE\x10\xd5\x9a\x46\x12.\n(NIFGEN_ATTRIBUTE_DIGITAL_PATTERN_ENABLED\x10\x95\x99\x46\x12+\n%NIFGEN_ATTRIBUTE_DIGITAL_STATIC_VALUE\x10\x9d\x9a\x46\x12)\n#NIFGEN_ATTRIBUTE_DIRECT_DMA_ENABLED\x10\xa4\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_DIRECT_DMA_WINDOW_ADDRESS\x10\xc2\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_DIRECT_DMA_WINDOW_SIZE\x10\xa5\x9a\x46\x12\'\n!NIFGEN_ATTRIBUTE_DONE_EVENT_DELAY\x10\x96\x9b\x46\x12-\n\'NIFGEN_ATTRIBUTE_DONE_EVENT_DELAY_UNITS\x10\x97\x9b\x46\x12\x30\n*NIFGEN_ATTRIBUTE_DONE_EVENT_LATCHED_STATUS\x10\x8f\x9b\x46\x12\x34\n.NIFGEN_ATTRIBUTE_DONE_EVENT_LEVEL_ACTIVE_LEVEL\x10\xed\x9a\x46\x12\x31\n+NIFGEN_ATTRIBUTE_DONE_EVENT_OUTPUT_BEHAVIOR\x10\xfc\x9a\x46\x12\x31\n+NIFGEN_ATTRIBUTE_DONE_EVENT_OUTPUT_TERMINAL\x10\xeb\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_DONE_EVENT_PULSE_POLARITY\x10\xef\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_DONE_EVENT_PULSE_WIDTH\x10\x80\x9b\x46\x12\x33\n-NIFGEN_ATTRIBUTE_DONE_EVENT_PULSE_WIDTH_UNITS\x10\xfe\x9a\x46\x12#\n\x1dNIFGEN_ATTRIBUTE_DRIVER_SETUP\x10\x97\x8b@\x12G\nANIFGEN_ATTRIBUTE_EXPORTED_ONBOARD_REFERENCE_CLOCK_OUTPUT_TERMINAL\x10\xf2\x9a\x46\x12?\n9NIFGEN_ATTRIBUTE_EXPORTED_REFERENCE_CLOCK_OUTPUT_TERMINAL\x10\xf1\x9a\x46\x12\x34\n.NIFGEN_ATTRIBUTE_EXPORTED_SAMPLE_CLOCK_DIVISOR\x10\x8b\x9a\x46\x12<\n6NIFGEN_ATTRIBUTE_EXPORTED_SAMPLE_CLOCK_OUTPUT_TERMINAL\x10\xf0\x9a\x46\x12=\n7NIFGEN_ATTRIBUTE_EXPORTED_SAMPLE_CLOCK_TIMEBASE_DIVISOR\x10\x96\x9a\x46\x12\x45\n?NIFGEN_ATTRIBUTE_EXPORTED_SAMPLE_CLOCK_TIMEBASE_OUTPUT_TERMINAL\x10\xf9\x9a\x46\x12>\n8NIFGEN_ATTRIBUTE_EXPORTED_SCRIPT_TRIGGER_OUTPUT_TERMINAL\x10\xd7\x9a\x46\x12=\n7NIFGEN_ATTRIBUTE_EXPORTED_START_TRIGGER_OUTPUT_TERMINAL\x10\xcb\x9a\x46\x12\x38\n2NIFGEN_ATTRIBUTE_EXTERNAL_CLOCK_DELAY_BINARY_VALUE\x10\x99\x9a\x46\x12\x37\n1NIFGEN_ATTRIBUTE_EXTERNAL_SAMPLE_CLOCK_MULTIPLIER\x10\xa8\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_FILE_TRANSFER_BLOCK_SIZE\x10\xa0\x9a\x46\x12\x32\n,NIFGEN_ATTRIBUTE_FILTER_CORRECTION_FREQUENCY\x10\x98\x99\x46\x12\x32\n,NIFGEN_ATTRIBUTE_FLATNESS_CORRECTION_ENABLED\x10\xf3\x9a\x46\x12(\n\"NIFGEN_ATTRIBUTE_FPGA_BITFILE_PATH\x10\xcc\x9b\x46\x12\x31\n+NIFGEN_ATTRIBUTE_FREQ_LIST_DURATION_QUANTUM\x10\x86\x9a\x46\x12\'\n!NIFGEN_ATTRIBUTE_FREQ_LIST_HANDLE\x10\x80\x9a\x46\x12%\n\x1fNIFGEN_ATTRIBUTE_FUNC_AMPLITUDE\x10\xb6\xa6L\x12\'\n!NIFGEN_ATTRIBUTE_FUNC_BUFFER_SIZE\x10\x9e\x9a\x46\x12%\n\x1fNIFGEN_ATTRIBUTE_FUNC_DC_OFFSET\x10\xb7\xa6L\x12+\n%NIFGEN_ATTRIBUTE_FUNC_DUTY_CYCLE_HIGH\x10\xba\xa6L\x12%\n\x1fNIFGEN_ATTRIBUTE_FUNC_FREQUENCY\x10\xb8\xa6L\x12+\n%NIFGEN_ATTRIBUTE_FUNC_MAX_BUFFER_SIZE\x10\x9f\x9a\x46\x12\'\n!NIFGEN_ATTRIBUTE_FUNC_START_PHASE\x10\xb9\xa6L\x12$\n\x1eNIFGEN_ATTRIBUTE_FUNC_WAVEFORM\x10\xb5\xa6L\x12%\n\x1fNIFGEN_ATTRIBUTE_GAIN_DAC_VALUE\x10\x8f\x9a\x46\x12)\n#NIFGEN_ATTRIBUTE_GROUP_CAPABILITIES\x10\xa1\x8e@\x12(\n\"NIFGEN_ATTRIBUTE_ID_QUERY_RESPONSE\x10\xb1\x98\x46\x12$\n\x1eNIFGEN_ATTRIBUTE_IDLE_BEHAVIOR\x10\xa9\x9b\x46\x12!\n\x1bNIFGEN_ATTRIBUTE_IDLE_VALUE\x10\xaa\x9b\x46\x12\x33\n-NIFGEN_ATTRIBUTE_INSTRUMENT_FIRMWARE_REVISION\x10\x8e\x8f@\x12.\n(NIFGEN_ATTRIBUTE_INSTRUMENT_MANUFACTURER\x10\x8f\x8f@\x12\'\n!NIFGEN_ATTRIBUTE_INSTRUMENT_MODEL\x10\x90\x8f@\x12(\n\"NIFGEN_ATTRIBUTE_INTERCHANGE_CHECK\x10\xa5\x8b@\x12-\n\'NIFGEN_ATTRIBUTE_IO_RESOURCE_DESCRIPTOR\x10\xc0\x8d@\x12%\n\x1fNIFGEN_ATTRIBUTE_LOAD_IMPEDANCE\x10\x8c\x9a\x46\x12#\n\x1dNIFGEN_ATTRIBUTE_LOGICAL_NAME\x10\xc1\x8d@\x12)\n#NIFGEN_ATTRIBUTE_MARKER_EVENT_DELAY\x10\x92\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_MARKER_EVENT_DELAY_UNITS\x10\x93\x9b\x46\x12\x32\n,NIFGEN_ATTRIBUTE_MARKER_EVENT_LATCHED_STATUS\x10\x8e\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_MARKER_EVENT_LIVE_STATUS\x10\x89\x9b\x46\x12\x33\n-NIFGEN_ATTRIBUTE_MARKER_EVENT_OUTPUT_BEHAVIOR\x10\x86\x9b\x46\x12\x33\n-NIFGEN_ATTRIBUTE_MARKER_EVENT_OUTPUT_TERMINAL\x10\xe8\x9a\x46\x12\x32\n,NIFGEN_ATTRIBUTE_MARKER_EVENT_PULSE_POLARITY\x10\xe9\x9a\x46\x12/\n)NIFGEN_ATTRIBUTE_MARKER_EVENT_PULSE_WIDTH\x10\x84\x9b\x46\x12\x35\n/NIFGEN_ATTRIBUTE_MARKER_EVENT_PULSE_WIDTH_UNITS\x10\x85\x9b\x46\x12\x38\n2NIFGEN_ATTRIBUTE_MARKER_EVENT_TOGGLE_INITIAL_STATE\x10\x87\x9b\x46\x12*\n$NIFGEN_ATTRIBUTE_MARKER_EVENTS_COUNT\x10\xbf\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_MAX_FREQ_LIST_DURATION\x10\x85\x9a\x46\x12+\n%NIFGEN_ATTRIBUTE_MAX_FREQ_LIST_LENGTH\x10\x83\x9a\x46\x12%\n\x1fNIFGEN_ATTRIBUTE_MAX_LOOP_COUNT\x10\xa7\xa7L\x12)\n#NIFGEN_ATTRIBUTE_MAX_NUM_FREQ_LISTS\x10\x81\x9a\x46\x12(\n\"NIFGEN_ATTRIBUTE_MAX_NUM_SEQUENCES\x10\xa4\xa7L\x12(\n\"NIFGEN_ATTRIBUTE_MAX_NUM_WAVEFORMS\x10\x9d\xa7L\x12*\n$NIFGEN_ATTRIBUTE_MAX_SEQUENCE_LENGTH\x10\xa6\xa7L\x12(\n\"NIFGEN_ATTRIBUTE_MAX_WAVEFORM_SIZE\x10\xa0\xa7L\x12\"\n\x1cNIFGEN_ATTRIBUTE_MEMORY_SIZE\x10\xa2\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_MIN_FREQ_LIST_DURATION\x10\x84\x9a\x46\x12+\n%NIFGEN_ATTRIBUTE_MIN_FREQ_LIST_LENGTH\x10\x82\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_MIN_SEQUENCE_LENGTH\x10\xa5\xa7L\x12(\n\"NIFGEN_ATTRIBUTE_MIN_WAVEFORM_SIZE\x10\x9f\xa7L\x12&\n NIFGEN_ATTRIBUTE_MODULE_REVISION\x10\xb6\x9b\x46\x12\'\n!NIFGEN_ATTRIBUTE_OFFSET_DAC_VALUE\x10\x90\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_OSCILLATOR_FREQ_DAC_VALUE\x10\x91\x9a\x46\x12\x31\n+NIFGEN_ATTRIBUTE_OSCILLATOR_PHASE_DAC_VALUE\x10\x98\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_CARRIER_ENABLED\x10\xa9\x9a\x46\x12,\n&NIFGEN_ATTRIBUTE_OSP_CARRIER_FREQUENCY\x10\xaa\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_CARRIER_PHASE_I\x10\xab\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_CARRIER_PHASE_Q\x10\xac\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_OSP_CIC_FILTER_ENABLED\x10\xb1\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_CIC_FILTER_GAIN\x10\xb7\x9a\x46\x12\x33\n-NIFGEN_ATTRIBUTE_OSP_CIC_FILTER_INTERPOLATION\x10\xb2\x9a\x46\x12<\n6NIFGEN_ATTRIBUTE_OSP_COMPENSATE_FOR_FILTER_GROUP_DELAY\x10\xb5\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_OSP_DATA_PROCESSING_MODE\x10\xa7\x9a\x46\x12\"\n\x1cNIFGEN_ATTRIBUTE_OSP_ENABLED\x10\xa6\x9a\x46\x12-\n\'NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_ENABLED\x10\xaf\x9a\x46\x12\x33\n-NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_FLAT_PASSBAND\x10\xb5\x9a\x46\x12\x31\n+NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_GAUSSIAN_BT\x10\xb6\x9a\x46\x12\x33\n-NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_INTERPOLATION\x10\xb0\x9a\x46\x12\x39\n3NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_RAISED_COSINE_ALPHA\x10\xb4\x9a\x46\x12>\n8NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_ROOT_RAISED_COSINE_ALPHA\x10\xb3\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_FIR_FILTER_TYPE\x10\xad\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_FREQUENCY_SHIFT\x10\xa3\x9b\x46\x12\"\n\x1cNIFGEN_ATTRIBUTE_OSP_IQ_RATE\x10\xa8\x9a\x46\x12\x1f\n\x19NIFGEN_ATTRIBUTE_OSP_MODE\x10\xa2\x9b\x46\x12\x33\n-NIFGEN_ATTRIBUTE_OSP_OVERFLOW_ERROR_REPORTING\x10\xbc\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_OSP_OVERFLOW_STATUS\x10\xbd\x9a\x46\x12,\n&NIFGEN_ATTRIBUTE_OSP_PRE_FILTER_GAIN_I\x10\xb8\x9a\x46\x12,\n&NIFGEN_ATTRIBUTE_OSP_PRE_FILTER_GAIN_Q\x10\xb9\x9a\x46\x12.\n(NIFGEN_ATTRIBUTE_OSP_PRE_FILTER_OFFSET_I\x10\xba\x9a\x46\x12.\n(NIFGEN_ATTRIBUTE_OSP_PRE_FILTER_OFFSET_Q\x10\xbb\x9a\x46\x12%\n\x1fNIFGEN_ATTRIBUTE_OUTPUT_ENABLED\x10\xd3\xa5L\x12\'\n!NIFGEN_ATTRIBUTE_OUTPUT_IMPEDANCE\x10\xd4\xa5L\x12\"\n\x1cNIFGEN_ATTRIBUTE_OUTPUT_MODE\x10\xd1\xa5L\x12;\n5NIFGEN_ATTRIBUTE_P2P_DATA_TRANSFER_PERMISSION_ADDRESS\x10\xbe\x9b\x46\x12@\n:NIFGEN_ATTRIBUTE_P2P_DATA_TRANSFER_PERMISSION_ADDRESS_TYPE\x10\xbf\x9b\x46\x12\x43\n=NIFGEN_ATTRIBUTE_P2P_DATA_TRANSFER_PERMISSION_INITIAL_CREDITS\x10\xc8\x9b\x46\x12<\n6NIFGEN_ATTRIBUTE_P2P_DATA_TRANSFER_PERMISSION_INTERVAL\x10\xc0\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_P2P_DESTINATION_CHANNELS\x10\xb8\x9b\x46\x12\x34\n.NIFGEN_ATTRIBUTE_P2P_DONE_NOTIFICATION_ADDRESS\x10\xc5\x9b\x46\x12\x39\n3NIFGEN_ATTRIBUTE_P2P_DONE_NOTIFICATION_ADDRESS_TYPE\x10\xc6\x9b\x46\x12\x32\n,NIFGEN_ATTRIBUTE_P2P_DONE_NOTIFICATION_VALUE\x10\xc7\x9b\x46\x12\"\n\x1cNIFGEN_ATTRIBUTE_P2P_ENABLED\x10\xb7\x9b\x46\x12)\n#NIFGEN_ATTRIBUTE_P2P_ENDPOINT_COUNT\x10\xbc\x9b\x46\x12@\n:NIFGEN_ATTRIBUTE_P2P_ENDPOINT_FULLNESS_START_TRIGGER_LEVEL\x10\xca\x9b\x46\x12(\n\"NIFGEN_ATTRIBUTE_P2P_ENDPOINT_SIZE\x10\xb9\x9b\x46\x12\x32\n,NIFGEN_ATTRIBUTE_P2P_ENDPOINT_WINDOW_ADDRESS\x10\xc1\x9b\x46\x12\x37\n1NIFGEN_ATTRIBUTE_P2P_ENDPOINT_WINDOW_ADDRESS_TYPE\x10\xc2\x9b\x46\x12/\n)NIFGEN_ATTRIBUTE_P2P_ENDPOINT_WINDOW_SIZE\x10\xc3\x9b\x46\x12\x37\n1NIFGEN_ATTRIBUTE_P2P_MANUAL_CONFIGURATION_ENABLED\x10\xbd\x9b\x46\x12;\n5NIFGEN_ATTRIBUTE_P2P_MOST_SPACE_AVAILABLE_IN_ENDPOINT\x10\xbb\x9b\x46\x12\x36\n0NIFGEN_ATTRIBUTE_P2P_SPACE_AVAILABLE_IN_ENDPOINT\x10\xba\x9b\x46\x12\x34\n.NIFGEN_ATTRIBUTE_PCI_DMA_OPTIMIZATIONS_ENABLED\x10\x9a\x9b\x46\x12\x31\n+NIFGEN_ATTRIBUTE_POST_AMPLIFIER_ATTENUATION\x10\x95\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_PRE_AMPLIFIER_ATTENUATION\x10\x94\x9a\x46\x12.\n(NIFGEN_ATTRIBUTE_QUERY_INSTRUMENT_STATUS\x10\x93\x8b@\x12\"\n\x1cNIFGEN_ATTRIBUTE_RANGE_CHECK\x10\x92\x8b@\x12?\n9NIFGEN_ATTRIBUTE_READY_FOR_START_EVENT_LEVEL_ACTIVE_LEVEL\x10\xe7\x9a\x46\x12\x38\n2NIFGEN_ATTRIBUTE_READY_FOR_START_EVENT_LIVE_STATUS\x10\x8c\x9b\x46\x12<\n6NIFGEN_ATTRIBUTE_READY_FOR_START_EVENT_OUTPUT_TERMINAL\x10\xe6\x9a\x46\x12\'\n!NIFGEN_ATTRIBUTE_RECORD_COERCIONS\x10\x96\x8b@\x12*\n$NIFGEN_ATTRIBUTE_REF_CLOCK_FREQUENCY\x10\x9b\x99\x46\x12-\n\'NIFGEN_ATTRIBUTE_REFERENCE_CLOCK_SOURCE\x10\xa1\x99\x46\x12\x32\n,NIFGEN_ATTRIBUTE_SAMPLE_CLOCK_ABSOLUTE_DELAY\x10\x97\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_SAMPLE_CLOCK_SOURCE\x10\xa0\x99\x46\x12\x31\n+NIFGEN_ATTRIBUTE_SAMPLE_CLOCK_TIMEBASE_RATE\x10\xa0\x9b\x46\x12\x33\n-NIFGEN_ATTRIBUTE_SAMPLE_CLOCK_TIMEBASE_SOURCE\x10\x9f\x9b\x46\x12)\n#NIFGEN_ATTRIBUTE_SCRIPT_TO_GENERATE\x10\xbe\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_SCRIPT_TRIGGER_TYPE\x10\xd2\x9a\x46\x12,\n&NIFGEN_ATTRIBUTE_SCRIPT_TRIGGERS_COUNT\x10\xc0\x9a\x46\x12$\n\x1eNIFGEN_ATTRIBUTE_SERIAL_NUMBER\x10\xa3\x9a\x46\x12\x1f\n\x19NIFGEN_ATTRIBUTE_SIMULATE\x10\x95\x8b@\x12?\n9NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_CLASS_SPEC_MAJOR_VERSION\x10\x93\x8f@\x12?\n9NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_CLASS_SPEC_MINOR_VERSION\x10\x94\x8f@\x12\x32\n,NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_DESCRIPTION\x10\x92\x8f@\x12-\n\'NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_PREFIX\x10\xbe\x8d@\x12/\n)NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_REVISION\x10\xb7\x8f@\x12-\n\'NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_VENDOR\x10\x91\x8f@\x12)\n#NIFGEN_ATTRIBUTE_START_TRIGGER_TYPE\x10\xc8\x9a\x46\x12*\n$NIFGEN_ATTRIBUTE_STARTED_EVENT_DELAY\x10\x94\x9b\x46\x12\x30\n*NIFGEN_ATTRIBUTE_STARTED_EVENT_DELAY_UNITS\x10\x95\x9b\x46\x12\x33\n-NIFGEN_ATTRIBUTE_STARTED_EVENT_LATCHED_STATUS\x10\x90\x9b\x46\x12\x37\n1NIFGEN_ATTRIBUTE_STARTED_EVENT_LEVEL_ACTIVE_LEVEL\x10\xec\x9a\x46\x12\x34\n.NIFGEN_ATTRIBUTE_STARTED_EVENT_OUTPUT_BEHAVIOR\x10\xfb\x9a\x46\x12\x34\n.NIFGEN_ATTRIBUTE_STARTED_EVENT_OUTPUT_TERMINAL\x10\xea\x9a\x46\x12\x33\n-NIFGEN_ATTRIBUTE_STARTED_EVENT_PULSE_POLARITY\x10\xee\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_STARTED_EVENT_PULSE_WIDTH\x10\xff\x9a\x46\x12\x36\n0NIFGEN_ATTRIBUTE_STARTED_EVENT_PULSE_WIDTH_UNITS\x10\xfd\x9a\x46\x12<\n6NIFGEN_ATTRIBUTE_STREAMING_SPACE_AVAILABLE_IN_WAVEFORM\x10\xf5\x9a\x46\x12\x30\n*NIFGEN_ATTRIBUTE_STREAMING_WAVEFORM_HANDLE\x10\xf4\x9a\x46\x12.\n(NIFGEN_ATTRIBUTE_STREAMING_WAVEFORM_NAME\x10\xf6\x9a\x46\x12.\n(NIFGEN_ATTRIBUTE_STREAMING_WRITE_TIMEOUT\x10\xc9\x9b\x46\x12\x32\n,NIFGEN_ATTRIBUTE_SUPPORTED_INSTRUMENT_MODELS\x10\xd7\x8d@\x12+\n%NIFGEN_ATTRIBUTE_SYNC_DUTY_CYCLE_HIGH\x10\x99\x99\x46\x12/\n)NIFGEN_ATTRIBUTE_SYNC_OUT_OUTPUT_TERMINAL\x10\xfa\x9a\x46\x12&\n NIFGEN_ATTRIBUTE_SYNCHRONIZATION\x10\x9f\x99\x46\x12-\n\'NIFGEN_ATTRIBUTE_TERMINAL_CONFIGURATION\x10\x9d\x9b\x46\x12#\n\x1dNIFGEN_ATTRIBUTE_TRIGGER_MODE\x10\x9c\x99\x46\x12%\n\x1fNIFGEN_ATTRIBUTE_TRIGGER_SOURCE\x10\xfe\xa7L\x12*\n$NIFGEN_ATTRIBUTE_VIDEO_WAVEFORM_TYPE\x10\x88\x9a\x46\x12$\n\x1eNIFGEN_ATTRIBUTE_WAIT_BEHAVIOR\x10\xab\x9b\x46\x12!\n\x1bNIFGEN_ATTRIBUTE_WAIT_VALUE\x10\xac\x9b\x46\x12\'\n!NIFGEN_ATTRIBUTE_WAVEFORM_QUANTUM\x10\x9e\xa7L\x12\x34\n.NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_MAJOR_VERSION\x10\x87\x8f@\x12\x34\n.NIFGEN_ATTRIBUTE_SPECIFIC_DRIVER_MINOR_VERSION\x10\x88\x8f@\x12*\n$NIFGEN_ATTRIBUTE_UPDATE_CLOCK_SOURCE\x10\x9a\x99\x46*Z\n\tByteOrder\x12\'\n#BYTE_ORDER_NIFGEN_VAL_LITTLE_ENDIAN\x10\x00\x12$\n BYTE_ORDER_NIFGEN_VAL_BIG_ENDIAN\x10\x01*\x82\x01\n\tClockMode\x12)\n%CLOCK_MODE_NIFGEN_VAL_HIGH_RESOLUTION\x10\x00\x12%\n!CLOCK_MODE_NIFGEN_VAL_DIVIDE_DOWN\x10\x01\x12#\n\x1f\x43LOCK_MODE_NIFGEN_VAL_AUTOMATIC\x10\x02*\xe8\x01\n\rHardwareState\x12\"\n\x1eHARDWARE_STATE_NIFGEN_VAL_IDLE\x10\x00\x12\x37\n3HARDWARE_STATE_NIFGEN_VAL_WAITING_FOR_START_TRIGGER\x10\x64\x12&\n!HARDWARE_STATE_NIFGEN_VAL_RUNNING\x10\xc8\x01\x12#\n\x1eHARDWARE_STATE_NIFGEN_VAL_DONE\x10\xd8\x04\x12-\n(HARDWARE_STATE_NIFGEN_VAL_HARDWARE_ERROR\x10\xe8\x07*\xd9\x01\n\nOutputMode\x12&\n\"OUTPUT_MODE_NIFGEN_VAL_OUTPUT_FUNC\x10\x00\x12%\n!OUTPUT_MODE_NIFGEN_VAL_OUTPUT_ARB\x10\x01\x12%\n!OUTPUT_MODE_NIFGEN_VAL_OUTPUT_SEQ\x10\x02\x12+\n\'OUTPUT_MODE_NIFGEN_VAL_OUTPUT_FREQ_LIST\x10\x65\x12(\n$OUTPUT_MODE_NIFGEN_VAL_OUTPUT_SCRIPT\x10\x66*v\n\nRelativeTo\x12\x32\n.RELATIVE_TO_NIFGEN_VAL_WAVEFORM_POSITION_START\x10\x00\x12\x34\n0RELATIVE_TO_NIFGEN_VAL_WAVEFORM_POSITION_CURRENT\x10\x01*\xa0\x04\n\x06Signal\x12\x16\n\x12SIGNAL_UNSPECIFIED\x10\x00\x12.\n)SIGNAL_NIFGEN_VAL_ONBOARD_REFERENCE_CLOCK\x10\xfb\x07\x12\x1f\n\x1aSIGNAL_NIFGEN_VAL_SYNC_OUT\x10\xea\x07\x12$\n\x1fSIGNAL_NIFGEN_VAL_START_TRIGGER\x10\xec\x07\x12#\n\x1eSIGNAL_NIFGEN_VAL_MARKER_EVENT\x10\xe9\x07\x12,\n\'SIGNAL_NIFGEN_VAL_SAMPLE_CLOCK_TIMEBASE\x10\xee\x07\x12&\n!SIGNAL_NIFGEN_VAL_SYNCHRONIZATION\x10\xef\x07\x12\"\n\x1eSIGNAL_NIFGEN_VAL_SAMPLE_CLOCK\x10\x65\x12%\n!SIGNAL_NIFGEN_VAL_REFERENCE_CLOCK\x10\x66\x12$\n SIGNAL_NIFGEN_VAL_SCRIPT_TRIGGER\x10g\x12+\n\'SIGNAL_NIFGEN_VAL_READY_FOR_START_EVENT\x10i\x12#\n\x1fSIGNAL_NIFGEN_VAL_STARTED_EVENT\x10j\x12 \n\x1cSIGNAL_NIFGEN_VAL_DONE_EVENT\x10k\x12\'\n#SIGNAL_NIFGEN_VAL_DATA_MARKER_EVENT\x10l*p\n\x07Trigger\x12\x17\n\x13TRIGGER_UNSPECIFIED\x10\x00\x12%\n TRIGGER_NIFGEN_VAL_START_TRIGGER\x10\xec\x07\x12%\n!TRIGGER_NIFGEN_VAL_SCRIPT_TRIGGER\x10g*\xbf\x01\n\x0bTriggerMode\x12\x1c\n\x18TRIGGER_MODE_UNSPECIFIED\x10\x00\x12\"\n\x1eTRIGGER_MODE_NIFGEN_VAL_SINGLE\x10\x01\x12&\n\"TRIGGER_MODE_NIFGEN_VAL_CONTINUOUS\x10\x02\x12#\n\x1fTRIGGER_MODE_NIFGEN_VAL_STEPPED\x10\x03\x12!\n\x1dTRIGGER_MODE_NIFGEN_VAL_BURST\x10\x04*|\n\x0bTriggerWhen\x12\x1c\n\x18TRIGGER_WHEN_UNSPECIFIED\x10\x00\x12\'\n#TRIGGER_WHEN_NIFGEN_VAL_ACTIVE_HIGH\x10\x65\x12&\n\"TRIGGER_WHEN_NIFGEN_VAL_ACTIVE_LOW\x10\x66*\xc1\x02\n\x08Waveform\x12\x18\n\x14WAVEFORM_UNSPECIFIED\x10\x00\x12 \n\x1cWAVEFORM_NIFGEN_VAL_WFM_SINE\x10\x01\x12\"\n\x1eWAVEFORM_NIFGEN_VAL_WFM_SQUARE\x10\x02\x12$\n WAVEFORM_NIFGEN_VAL_WFM_TRIANGLE\x10\x03\x12#\n\x1fWAVEFORM_NIFGEN_VAL_WFM_RAMP_UP\x10\x04\x12%\n!WAVEFORM_NIFGEN_VAL_WFM_RAMP_DOWN\x10\x05\x12\x1e\n\x1aWAVEFORM_NIFGEN_VAL_WFM_DC\x10\x06\x12!\n\x1dWAVEFORM_NIFGEN_VAL_WFM_NOISE\x10\x65\x12 \n\x1cWAVEFORM_NIFGEN_VAL_WFM_USER\x10\x66*y\n\x14\x46requencyListOptions\x12&\n\"FREQUENCY_LIST_OPTIONS_UNSPECIFIED\x10\x00\x12\x39\n,FREQUENCY_LIST_OPTIONS_NIFGEN_VAL_ALL_FLISTS\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01*\x89\x07\n\x0fRouteSignalFrom\x12!\n\x1dROUTE_SIGNAL_FROM_UNSPECIFIED\x10\x00\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_MARKER\x10\xe9\x07\x12*\n%ROUTE_SIGNAL_FROM_NIFGEN_VAL_SYNC_OUT\x10\xea\x07\x12\x33\n.ROUTE_SIGNAL_FROM_NIFGEN_VAL_OUT_START_TRIGGER\x10\xec\x07\x12-\n(ROUTE_SIGNAL_FROM_NIFGEN_VAL_BOARD_CLOCK\x10\xee\x07\x12\x31\n,ROUTE_SIGNAL_FROM_NIFGEN_VAL_SYNCHRONIZATION\x10\xef\x07\x12.\n*ROUTE_SIGNAL_FROM_NIFGEN_VAL_SOFTWARE_TRIG\x10\x02\x12)\n$ROUTE_SIGNAL_FROM_NIFGEN_VAL_REF_OUT\x10\xf0\x07\x12+\n&ROUTE_SIGNAL_FROM_NIFGEN_VAL_CLOCK_OUT\x10\xf1\x07\x12*\n%ROUTE_SIGNAL_FROM_NIFGEN_VAL_PXI_STAR\x10\x83\x01\x12\'\n\"ROUTE_SIGNAL_FROM_NIFGEN_VAL_PFI_0\x10\xf3\x07\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_0\x10\x8d\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_1\x10\x8e\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_2\x10\x8f\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_3\x10\x90\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_4\x10\x91\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_5\x10\x92\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_6\x10\x93\x01\x12(\n#ROUTE_SIGNAL_FROM_NIFGEN_VAL_RTSI_7\x10\xf2\x07\x12\x39\n4ROUTE_SIGNAL_FROM_NIFGEN_VAL_ONBOARD_REFERENCE_CLOCK\x10\xfb\x07*\x91\x04\n\rRouteSignalTo\x12\x1f\n\x1bROUTE_SIGNAL_TO_UNSPECIFIED\x10\x00\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_0\x10\x8d\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_1\x10\x8e\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_2\x10\x8f\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_3\x10\x90\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_4\x10\x91\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_5\x10\x92\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_6\x10\x93\x01\x12&\n!ROUTE_SIGNAL_TO_NIFGEN_VAL_RTSI_7\x10\xf2\x07\x12\'\n\"ROUTE_SIGNAL_TO_NIFGEN_VAL_REF_OUT\x10\xf0\x07\x12%\n ROUTE_SIGNAL_TO_NIFGEN_VAL_PFI_0\x10\xf3\x07\x12%\n ROUTE_SIGNAL_TO_NIFGEN_VAL_PFI_1\x10\xf4\x07\x12(\n#ROUTE_SIGNAL_TO_NIFGEN_VAL_PXI_STAR\x10\x83\x01*h\n\x0eSequenceHandle\x12\x1f\n\x1bSEQUENCE_HANDLE_UNSPECIFIED\x10\x00\x12\x35\n(SEQUENCE_HANDLE_NIFGEN_VAL_ALL_SEQUENCES\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01*h\n\x0eWaveformHandle\x12\x1f\n\x1bWAVEFORM_HANDLE_UNSPECIFIED\x10\x00\x12\x35\n(WAVEFORM_HANDLE_NIFGEN_VAL_ALL_WAVEFORMS\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01*\xc1Q\n\x1aNiFgenInt32AttributeValues\x12\x1c\n\x18NIFGEN_INT32_UNSPECIFIED\x10\x00\x12/\n+NIFGEN_INT32_ADDRESS_TYPE_VAL_ADDR_PHYSICAL\x10\x00\x12.\n*NIFGEN_INT32_ADDRESS_TYPE_VAL_ADDR_VIRTUAL\x10\x01\x12\x31\n-NIFGEN_INT32_ANALOG_PATH_VAL_MAIN_ANALOG_PATH\x10\x00\x12\x33\n/NIFGEN_INT32_ANALOG_PATH_VAL_DIRECT_ANALOG_PATH\x10\x01\x12;\n7NIFGEN_INT32_ANALOG_PATH_VAL_FIXED_LOW_GAIN_ANALOG_PATH\x10\x02\x12<\n8NIFGEN_INT32_ANALOG_PATH_VAL_FIXED_HIGH_GAIN_ANALOG_PATH\x10\x03\x12\x46\n@NIFGEN_INT32_ARBITRARY_SEQUENCE_HANDLE_VAL_FIRST_SEQUENCE_HANDLE\x10\xa0\x8d\x06\x12\x45\n?NIFGEN_INT32_ARBITRARY_SEQUENCE_HANDLE_VAL_LAST_SEQUENCE_HANDLE\x10\xaf\xdb\x06\x12\x43\n6NIFGEN_INT32_ARBITRARY_SEQUENCE_HANDLE_VAL_NO_SEQUENCE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x45\n@NIFGEN_INT32_ARBITRARY_WAVEFORM_HANDLE_VAL_FIRST_WAVEFORM_HANDLE\x10\x90N\x12\x44\n?NIFGEN_INT32_ARBITRARY_WAVEFORM_HANDLE_VAL_LAST_WAVEFORM_HANDLE\x10\xf7U\x12\x43\n6NIFGEN_INT32_ARBITRARY_WAVEFORM_HANDLE_VAL_NO_WAVEFORM\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12=\n0NIFGEN_INT32_BURST_COUNT_VAL_GENERATE_CONTINUOUS\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12)\n%NIFGEN_INT32_BUS_TYPE_VAL_BUS_INVALID\x10\x00\x12$\n NIFGEN_INT32_BUS_TYPE_VAL_BUS_AT\x10\x01\x12%\n!NIFGEN_INT32_BUS_TYPE_VAL_BUS_PCI\x10\x02\x12%\n!NIFGEN_INT32_BUS_TYPE_VAL_BUS_PXI\x10\x03\x12%\n!NIFGEN_INT32_BUS_TYPE_VAL_BUS_VXI\x10\x04\x12(\n$NIFGEN_INT32_BUS_TYPE_VAL_BUS_PCMCIA\x10\x05\x12&\n\"NIFGEN_INT32_BUS_TYPE_VAL_BUS_PXIE\x10\x06\x12/\n+NIFGEN_INT32_CLOCK_MODE_VAL_HIGH_RESOLUTION\x10\x00\x12+\n\'NIFGEN_INT32_CLOCK_MODE_VAL_DIVIDE_DOWN\x10\x01\x12)\n%NIFGEN_INT32_CLOCK_MODE_VAL_AUTOMATIC\x10\x02\x12\x41\n=NIFGEN_INT32_DATA_MARKER_EVENT_LEVEL_POLARITY_VAL_ACTIVE_HIGH\x10\x65\x12@\n<NIFGEN_INT32_DATA_MARKER_EVENT_LEVEL_POLARITY_VAL_ACTIVE_LOW\x10\x66\x12\x32\n.NIFGEN_INT32_DATA_PROCESSING_MODE_VAL_OSP_REAL\x10\x00\x12\x35\n1NIFGEN_INT32_DATA_PROCESSING_MODE_VAL_OSP_COMPLEX\x10\x01\x12\x38\n4NIFGEN_INT32_DONE_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_HIGH\x10\x65\x12\x37\n3NIFGEN_INT32_DONE_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_LOW\x10\x66\x12@\n<NIFGEN_INT32_DONE_EVENT_DELAY_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12\x33\n/NIFGEN_INT32_DONE_EVENT_DELAY_UNITS_VAL_SECONDS\x10\x66\x12\x35\n1NIFGEN_INT32_DONE_EVENT_OUTPUT_BEHAVIOR_VAL_PULSE\x10\x65\x12\x35\n1NIFGEN_INT32_DONE_EVENT_OUTPUT_BEHAVIOR_VAL_LEVEL\x10\x66\x12:\n6NIFGEN_INT32_DONE_EVENT_PULSE_POLARITY_VAL_ACTIVE_HIGH\x10\x65\x12\x39\n5NIFGEN_INT32_DONE_EVENT_PULSE_POLARITY_VAL_ACTIVE_LOW\x10\x66\x12\x46\nBNIFGEN_INT32_DONE_EVENT_PULSE_WIDTH_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12\x39\n5NIFGEN_INT32_DONE_EVENT_PULSE_WIDTH_UNITS_VAL_SECONDS\x10\x66\x12)\n%NIFGEN_INT32_FILTER_TYPE_VAL_OSP_FLAT\x10\x00\x12\x32\n.NIFGEN_INT32_FILTER_TYPE_VAL_OSP_RAISED_COSINE\x10\x01\x12\x37\n3NIFGEN_INT32_FILTER_TYPE_VAL_OSP_ROOT_RAISED_COSINE\x10\x02\x12-\n)NIFGEN_INT32_FILTER_TYPE_VAL_OSP_GAUSSIAN\x10\x03\x12+\n\'NIFGEN_INT32_FILTER_TYPE_VAL_OSP_CUSTOM\x10\x04\x12\x43\n=NIFGEN_INT32_FREQUENCY_LIST_HANDLE_VAL_FIRST_FREQ_LIST_HANDLE\x10\xc0\x9a\x0c\x12\x42\n<NIFGEN_INT32_FREQUENCY_LIST_HANDLE_VAL_LAST_FREQ_LIST_HANDLE\x10\xcf\xe8\x0c\x12@\n3NIFGEN_INT32_FREQUENCY_LIST_HANDLE_VAL_NO_FREQ_LIST\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x33\n.NIFGEN_INT32_IDLE_BEHAVIOR_VAL_HOLD_LAST_VALUE\x10\x90\x03\x12\x31\n,NIFGEN_INT32_IDLE_BEHAVIOR_VAL_JUMP_TO_VALUE\x10\x91\x03\x12\x42\n>NIFGEN_INT32_MARKER_EVENT_DELAY_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12\x35\n1NIFGEN_INT32_MARKER_EVENT_DELAY_UNITS_VAL_SECONDS\x10\x66\x12\x37\n3NIFGEN_INT32_MARKER_EVENT_OUTPUT_BEHAVIOR_VAL_PULSE\x10\x65\x12\x37\n3NIFGEN_INT32_MARKER_EVENT_OUTPUT_BEHAVIOR_VAL_LEVEL\x10\x66\x12\x38\n4NIFGEN_INT32_MARKER_EVENT_OUTPUT_BEHAVIOR_VAL_TOGGLE\x10g\x12<\n8NIFGEN_INT32_MARKER_EVENT_PULSE_POLARITY_VAL_ACTIVE_HIGH\x10\x65\x12;\n7NIFGEN_INT32_MARKER_EVENT_PULSE_POLARITY_VAL_ACTIVE_LOW\x10\x66\x12H\nDNIFGEN_INT32_MARKER_EVENT_PULSE_WIDTH_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12;\n7NIFGEN_INT32_MARKER_EVENT_PULSE_WIDTH_UNITS_VAL_SECONDS\x10\x66\x12;\n7NIFGEN_INT32_MARKER_EVENT_TOGGLE_INITIAL_STATE_VAL_HIGH\x10\x65\x12:\n6NIFGEN_INT32_MARKER_EVENT_TOGGLE_INITIAL_STATE_VAL_LOW\x10\x66\x12$\n NIFGEN_INT32_OSP_MODE_VAL_OSP_IF\x10\x00\x12*\n&NIFGEN_INT32_OSP_MODE_VAL_OSP_BASEBAND\x10\x01\x12G\nCNIFGEN_INT32_OSP_OVERFLOW_ERROR_REPORTING_VAL_ERROR_REPORTING_ERROR\x10\x00\x12J\nFNIFGEN_INT32_OSP_OVERFLOW_ERROR_REPORTING_VAL_ERROR_REPORTING_DISABLED\x10\x02\x12:\n6NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_NONE\x10\x00\x12G\nCNIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PRE_FILTER_GAIN_I\x10\x01\x12G\nCNIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PRE_FILTER_GAIN_Q\x10\x02\x12I\nENIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PRE_FILTER_OFFSET_I\x10\x04\x12I\nENIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PRE_FILTER_OFFSET_Q\x10\x08\x12\x42\n>NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_FIR_FILTER_I\x10\x10\x12\x43\n?NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PFIR_FILTER_I\x10\x10\x12\x42\n>NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_FIR_FILTER_Q\x10 \x12\x43\n?NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_PFIR_FILTER_Q\x10 \x12\x42\n>NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_CIC_FILTER_I\x10@\x12\x43\n>NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_CIC_FILTER_Q\x10\x80\x01\x12\x43\n>NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_COMPLEX_DATA\x10\x80\x02\x12\x44\n?NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_CFIR_FILTER_I\x10\x80\x04\x12\x44\n?NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_CFIR_FILTER_Q\x10\x80\x08\x12@\n;NIFGEN_INT32_OSP_OVERFLOW_STATUS_VAL_OSP_OVERFLOW_EQUALIZER\x10\x80\x10\x12,\n(NIFGEN_INT32_OUTPUT_MODE_VAL_OUTPUT_FUNC\x10\x00\x12+\n\'NIFGEN_INT32_OUTPUT_MODE_VAL_OUTPUT_ARB\x10\x01\x12+\n\'NIFGEN_INT32_OUTPUT_MODE_VAL_OUTPUT_SEQ\x10\x02\x12\x31\n-NIFGEN_INT32_OUTPUT_MODE_VAL_OUTPUT_FREQ_LIST\x10\x65\x12.\n*NIFGEN_INT32_OUTPUT_MODE_VAL_OUTPUT_SCRIPT\x10\x66\x12\x43\n?NIFGEN_INT32_READY_FOR_START_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_HIGH\x10\x65\x12\x42\n>NIFGEN_INT32_READY_FOR_START_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_LOW\x10\x66\x12\x41\n=NIFGEN_INT32_SCRIPT_TRIGGER_DIGITAL_EDGE_EDGE_VAL_RISING_EDGE\x10\x65\x12\x42\n>NIFGEN_INT32_SCRIPT_TRIGGER_DIGITAL_EDGE_EDGE_VAL_FALLING_EDGE\x10\x66\x12J\nFNIFGEN_INT32_SCRIPT_TRIGGER_DIGITAL_LEVEL_ACTIVE_LEVEL_VAL_ACTIVE_HIGH\x10\x65\x12I\nENIFGEN_INT32_SCRIPT_TRIGGER_DIGITAL_LEVEL_ACTIVE_LEVEL_VAL_ACTIVE_LOW\x10\x66\x12\x32\n.NIFGEN_INT32_SCRIPT_TRIGGER_TYPE_VAL_TRIG_NONE\x10\x65\x12\x35\n1NIFGEN_INT32_SCRIPT_TRIGGER_TYPE_VAL_DIGITAL_EDGE\x10\x66\x12\x36\n2NIFGEN_INT32_SCRIPT_TRIGGER_TYPE_VAL_DIGITAL_LEVEL\x10g\x12\x36\n2NIFGEN_INT32_SCRIPT_TRIGGER_TYPE_VAL_SOFTWARE_EDGE\x10h\x12@\n<NIFGEN_INT32_START_TRIGGER_DIGITAL_EDGE_EDGE_VAL_RISING_EDGE\x10\x65\x12\x41\n=NIFGEN_INT32_START_TRIGGER_DIGITAL_EDGE_EDGE_VAL_FALLING_EDGE\x10\x66\x12\x31\n-NIFGEN_INT32_START_TRIGGER_TYPE_VAL_TRIG_NONE\x10\x65\x12\x34\n0NIFGEN_INT32_START_TRIGGER_TYPE_VAL_DIGITAL_EDGE\x10\x66\x12\x35\n1NIFGEN_INT32_START_TRIGGER_TYPE_VAL_SOFTWARE_EDGE\x10h\x12=\n9NIFGEN_INT32_START_TRIGGER_TYPE_VAL_P2P_ENDPOINT_FULLNESS\x10j\x12;\n7NIFGEN_INT32_STARTED_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_HIGH\x10\x65\x12:\n6NIFGEN_INT32_STARTED_EVENT_ACTIVE_LEVEL_VAL_ACTIVE_LOW\x10\x66\x12\x43\n?NIFGEN_INT32_STARTED_EVENT_DELAY_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12\x36\n2NIFGEN_INT32_STARTED_EVENT_DELAY_UNITS_VAL_SECONDS\x10\x66\x12\x38\n4NIFGEN_INT32_STARTED_EVENT_OUTPUT_BEHAVIOR_VAL_PULSE\x10\x65\x12\x38\n4NIFGEN_INT32_STARTED_EVENT_OUTPUT_BEHAVIOR_VAL_LEVEL\x10\x66\x12=\n9NIFGEN_INT32_STARTED_EVENT_PULSE_POLARITY_VAL_ACTIVE_HIGH\x10\x65\x12<\n8NIFGEN_INT32_STARTED_EVENT_PULSE_POLARITY_VAL_ACTIVE_LOW\x10\x66\x12I\nENIFGEN_INT32_STARTED_EVENT_PULSE_WIDTH_UNITS_VAL_SAMPLE_CLOCK_PERIODS\x10\x65\x12<\n8NIFGEN_INT32_STARTED_EVENT_PULSE_WIDTH_UNITS_VAL_SECONDS\x10\x66\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL0\x10o\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL1\x10p\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL2\x10q\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL3\x10r\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL4\x10s\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL5\x10t\x12\x30\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_TTL6\x10u\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_0\x10\x8d\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_1\x10\x8e\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_2\x10\x8f\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_3\x10\x90\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_4\x10\x91\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_5\x10\x92\x01\x12\x33\n.NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_RTSI_6\x10\x93\x01\x12\x31\n,NIFGEN_INT32_SYNCHRONIZATION_SOURCE_VAL_NONE\x10\xe8\x07\x12\x39\n4NIFGEN_INT32_TERMINAL_CONFIGURATION_VAL_SINGLE_ENDED\x10\xac\x02\x12\x39\n4NIFGEN_INT32_TERMINAL_CONFIGURATION_VAL_DIFFERENTIAL\x10\xad\x02\x12(\n$NIFGEN_INT32_TRIGGER_MODE_VAL_SINGLE\x10\x01\x12,\n(NIFGEN_INT32_TRIGGER_MODE_VAL_CONTINUOUS\x10\x02\x12)\n%NIFGEN_INT32_TRIGGER_MODE_VAL_STEPPED\x10\x03\x12\'\n#NIFGEN_INT32_TRIGGER_MODE_VAL_BURST\x10\x04\x12-\n)NIFGEN_INT32_TRIGGER_SOURCE_VAL_IMMEDIATE\x10\x00\x12,\n(NIFGEN_INT32_TRIGGER_SOURCE_VAL_EXTERNAL\x10\x01\x12\x31\n-NIFGEN_INT32_TRIGGER_SOURCE_VAL_SOFTWARE_TRIG\x10\x02\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL0\x10o\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL1\x10p\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL2\x10q\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL3\x10r\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL4\x10s\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL5\x10t\x12(\n$NIFGEN_INT32_TRIGGER_SOURCE_VAL_TTL6\x10u\x12-\n(NIFGEN_INT32_TRIGGER_SOURCE_VAL_PXI_STAR\x10\x83\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_0\x10\x8d\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_1\x10\x8e\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_2\x10\x8f\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_3\x10\x90\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_4\x10\x91\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_5\x10\x92\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_6\x10\x93\x01\x12+\n&NIFGEN_INT32_TRIGGER_SOURCE_VAL_RTSI_7\x10\xf2\x07\x12*\n%NIFGEN_INT32_TRIGGER_SOURCE_VAL_PFI_0\x10\xf3\x07\x12*\n%NIFGEN_INT32_TRIGGER_SOURCE_VAL_PFI_1\x10\xf4\x07\x12*\n%NIFGEN_INT32_TRIGGER_SOURCE_VAL_PFI_2\x10\xf5\x07\x12*\n%NIFGEN_INT32_TRIGGER_SOURCE_VAL_PFI_3\x10\xf6\x07\x12\x33\n.NIFGEN_INT32_TRIGGER_SOURCE_VAL_OTHER_TERMINAL\x10\xfa\x07\x12\x31\n-NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_INTERNAL\x10\x00\x12\x31\n-NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_EXTERNAL\x10\x01\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL1\x10p\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL2\x10q\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL3\x10r\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL4\x10s\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL5\x10t\x12-\n)NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_TTL6\x10u\x12\x32\n-NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_PXI_STAR\x10\x83\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_0\x10\x8d\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_1\x10\x8e\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_2\x10\x8f\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_3\x10\x90\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_4\x10\x91\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_5\x10\x92\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_6\x10\x93\x01\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_RTSI_7\x10\xf2\x07\x12\x38\n3NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_OTHER_TERMINAL\x10\xfa\x07\x12\x30\n+NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_CLK_IN\x10\xb2\t\x12\x34\n/NIFGEN_INT32_UPDATE_CLOCK_SOURCE_VAL_DDC_CLK_IN\x10\xb3\t\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_B\x10\x00\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_D\x10\x01\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_G\x10\x02\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_H\x10\x03\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_I\x10\x04\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_M\x10\x05\x12.\n*NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_PAL_N\x10\x06\x12/\n+NIFGEN_INT32_VIDEO_WAVEFORM_TYPE_VAL_NTSC_M\x10\x07\x12\x33\n.NIFGEN_INT32_WAIT_BEHAVIOR_VAL_HOLD_LAST_VALUE\x10\x90\x03\x12\x31\n,NIFGEN_INT32_WAIT_BEHAVIOR_VAL_JUMP_TO_VALUE\x10\x91\x03\x12&\n\"NIFGEN_INT32_WAVEFORM_VAL_WFM_SINE\x10\x01\x12(\n$NIFGEN_INT32_WAVEFORM_VAL_WFM_SQUARE\x10\x02\x12*\n&NIFGEN_INT32_WAVEFORM_VAL_WFM_TRIANGLE\x10\x03\x12)\n%NIFGEN_INT32_WAVEFORM_VAL_WFM_RAMP_UP\x10\x04\x12+\n\'NIFGEN_INT32_WAVEFORM_VAL_WFM_RAMP_DOWN\x10\x05\x12$\n NIFGEN_INT32_WAVEFORM_VAL_WFM_DC\x10\x06\x12\'\n#NIFGEN_INT32_WAVEFORM_VAL_WFM_NOISE\x10\x65\x12&\n\"NIFGEN_INT32_WAVEFORM_VAL_WFM_USER\x10\x66\x1a\x02\x10\x01*\xa7\x02\n\x1bNiFgenReal64AttributeValues\x12\x1d\n\x19NIFGEN_REAL64_UNSPECIFIED\x10\x00\x12\x44\n7NIFGEN_REAL64_LOAD_IMPEDANCE_VAL_MATCHED_LOAD_IMPEDANCE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12.\n*NIFGEN_REAL64_OUTPUT_IMPEDANCE_VAL_50_OHMS\x10\x32\x12.\n*NIFGEN_REAL64_OUTPUT_IMPEDANCE_VAL_75_OHMS\x10K\x12?\n2NIFGEN_REAL64_SAMPLE_RATE_VAL_EXTERNAL_SAMPLE_RATE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x1a\x02\x10\x01*\xcf\n\n!NiFgenStringAttributeValuesMapped\x12$\n NIFGEN_STRING_MAPPED_UNSPECIFIED\x10\x00\x12I\nENIFGEN_STRING_REFERENCE_CLOCK_SOURCE_VAL_CLOCK_IN_COLLISION_AVOIDANCE\x10\x01\x12\x45\nANIFGEN_STRING_REFERENCE_CLOCK_SOURCE_VAL_NONE_COLLISION_AVOIDANCE\x10\x02\x12X\nTNIFGEN_STRING_REFERENCE_CLOCK_SOURCE_VAL_ONBOARD_REFERENCE_CLOCK_COLLISION_AVOIDANCE\x10\x03\x12J\nFNIFGEN_STRING_REFERENCE_CLOCK_SOURCE_VAL_PXI_CLOCK_COLLISION_AVOIDANCE\x10\x04\x12G\nCNIFGEN_STRING_REFERENCE_CLOCK_SOURCE_VAL_RTSI_7_COLLISION_AVOIDANCE\x10\x05\x12\x32\n.NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_CLOCK_IN\x10\x06\x12\x36\n2NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_DDC_CLOCK_IN\x10\x07\x12\x37\n3NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_ONBOARD_CLOCK\x10\x08\x12\x37\n3NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_STAR_LINE\x10\t\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_0_RTSI_0\x10\n\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_1_RTSI_1\x10\x0b\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_2_RTSI_2\x10\x0c\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_3_RTSI_3\x10\r\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_4_RTSI_4\x10\x0e\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_5_RTSI_5\x10\x0f\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_6_RTSI_6\x10\x10\x12\x43\n?NIFGEN_STRING_SAMPLE_CLOCK_SOURCE_VAL_PXI_TRIGGER_LINE_7_RTSI_7\x10\x11\x12;\n7NIFGEN_STRING_SAMPLE_CLOCK_TIMEBASE_SOURCE_VAL_CLOCK_IN\x10\x12\x12@\n<NIFGEN_STRING_SAMPLE_CLOCK_TIMEBASE_SOURCE_VAL_ONBOARD_CLOCK\x10\x13\x32\xdbn\n\x06NiFgen\x12\\\n\x0f\x41\x62ortGeneration\x12#.nifgen_grpc.AbortGenerationRequest\x1a$.nifgen_grpc.AbortGenerationResponse\x12\x89\x01\n\x1e\x41\x64justSampleClockRelativeDelay\x12\x32.nifgen_grpc.AdjustSampleClockRelativeDelayRequest\x1a\x33.nifgen_grpc.AdjustSampleClockRelativeDelayResponse\x12n\n\x15\x41llocateNamedWaveform\x12).nifgen_grpc.AllocateNamedWaveformRequest\x1a*.nifgen_grpc.AllocateNamedWaveformResponse\x12_\n\x10\x41llocateWaveform\x12$.nifgen_grpc.AllocateWaveformRequest\x1a%.nifgen_grpc.AllocateWaveformResponse\x12t\n\x17\x43heckAttributeViBoolean\x12+.nifgen_grpc.CheckAttributeViBooleanRequest\x1a,.nifgen_grpc.CheckAttributeViBooleanResponse\x12n\n\x15\x43heckAttributeViInt32\x12).nifgen_grpc.CheckAttributeViInt32Request\x1a*.nifgen_grpc.CheckAttributeViInt32Response\x12n\n\x15\x43heckAttributeViInt64\x12).nifgen_grpc.CheckAttributeViInt64Request\x1a*.nifgen_grpc.CheckAttributeViInt64Response\x12q\n\x16\x43heckAttributeViReal64\x12*.nifgen_grpc.CheckAttributeViReal64Request\x1a+.nifgen_grpc.CheckAttributeViReal64Response\x12t\n\x17\x43heckAttributeViSession\x12+.nifgen_grpc.CheckAttributeViSessionRequest\x1a,.nifgen_grpc.CheckAttributeViSessionResponse\x12q\n\x16\x43heckAttributeViString\x12*.nifgen_grpc.CheckAttributeViStringRequest\x1a+.nifgen_grpc.CheckAttributeViStringResponse\x12Y\n\x0e\x43learArbMemory\x12\".nifgen_grpc.ClearArbMemoryRequest\x1a#.nifgen_grpc.ClearArbMemoryResponse\x12_\n\x10\x43learArbSequence\x12$.nifgen_grpc.ClearArbSequenceRequest\x1a%.nifgen_grpc.ClearArbSequenceResponse\x12_\n\x10\x43learArbWaveform\x12$.nifgen_grpc.ClearArbWaveformRequest\x1a%.nifgen_grpc.ClearArbWaveformResponse\x12M\n\nClearError\x12\x1e.nifgen_grpc.ClearErrorRequest\x1a\x1f.nifgen_grpc.ClearErrorResponse\x12V\n\rClearFreqList\x12!.nifgen_grpc.ClearFreqListRequest\x1a\".nifgen_grpc.ClearFreqListResponse\x12w\n\x18\x43learInterchangeWarnings\x12,.nifgen_grpc.ClearInterchangeWarningsRequest\x1a-.nifgen_grpc.ClearInterchangeWarningsResponse\x12z\n\x19\x43learUserStandardWaveform\x12-.nifgen_grpc.ClearUserStandardWaveformRequest\x1a..nifgen_grpc.ClearUserStandardWaveformResponse\x12>\n\x05\x43lose\x12\x19.nifgen_grpc.CloseRequest\x1a\x1a.nifgen_grpc.CloseResponse\x12\x41\n\x06\x43ommit\x12\x1a.nifgen_grpc.CommitRequest\x1a\x1b.nifgen_grpc.CommitResponse\x12\x65\n\x12\x43onfigureAmplitude\x12&.nifgen_grpc.ConfigureAmplitudeRequest\x1a\'.nifgen_grpc.ConfigureAmplitudeResponse\x12k\n\x14\x43onfigureArbSequence\x12(.nifgen_grpc.ConfigureArbSequenceRequest\x1a).nifgen_grpc.ConfigureArbSequenceResponse\x12k\n\x14\x43onfigureArbWaveform\x12(.nifgen_grpc.ConfigureArbWaveformRequest\x1a).nifgen_grpc.ConfigureArbWaveformResponse\x12\x62\n\x11\x43onfigureChannels\x12%.nifgen_grpc.ConfigureChannelsRequest\x1a&.nifgen_grpc.ConfigureChannelsResponse\x12\x65\n\x12\x43onfigureClockMode\x12&.nifgen_grpc.ConfigureClockModeRequest\x1a\'.nifgen_grpc.ConfigureClockModeResponse\x12\x9b\x01\n$ConfigureCustomFIRFilterCoefficients\x12\x38.nifgen_grpc.ConfigureCustomFIRFilterCoefficientsRequest\x1a\x39.nifgen_grpc.ConfigureCustomFIRFilterCoefficientsResponse\x12\x92\x01\n!ConfigureDigitalEdgeScriptTrigger\x12\x35.nifgen_grpc.ConfigureDigitalEdgeScriptTriggerRequest\x1a\x36.nifgen_grpc.ConfigureDigitalEdgeScriptTriggerResponse\x12\x8f\x01\n ConfigureDigitalEdgeStartTrigger\x12\x34.nifgen_grpc.ConfigureDigitalEdgeStartTriggerRequest\x1a\x35.nifgen_grpc.ConfigureDigitalEdgeStartTriggerResponse\x12\x95\x01\n\"ConfigureDigitalLevelScriptTrigger\x12\x36.nifgen_grpc.ConfigureDigitalLevelScriptTriggerRequest\x1a\x37.nifgen_grpc.ConfigureDigitalLevelScriptTriggerResponse\x12\x62\n\x11\x43onfigureFreqList\x12%.nifgen_grpc.ConfigureFreqListRequest\x1a&.nifgen_grpc.ConfigureFreqListResponse\x12\x65\n\x12\x43onfigureFrequency\x12&.nifgen_grpc.ConfigureFrequencyRequest\x1a\'.nifgen_grpc.ConfigureFrequencyResponse\x12q\n\x16\x43onfigureOperationMode\x12*.nifgen_grpc.ConfigureOperationModeRequest\x1a+.nifgen_grpc.ConfigureOperationModeResponse\x12q\n\x16\x43onfigureOutputEnabled\x12*.nifgen_grpc.ConfigureOutputEnabledRequest\x1a+.nifgen_grpc.ConfigureOutputEnabledResponse\x12w\n\x18\x43onfigureOutputImpedance\x12,.nifgen_grpc.ConfigureOutputImpedanceRequest\x1a-.nifgen_grpc.ConfigureOutputImpedanceResponse\x12h\n\x13\x43onfigureOutputMode\x12\'.nifgen_grpc.ConfigureOutputModeRequest\x1a(.nifgen_grpc.ConfigureOutputModeResponse\x12\xa7\x01\n(ConfigureP2PEndpointFullnessStartTrigger\x12<.nifgen_grpc.ConfigureP2PEndpointFullnessStartTriggerRequest\x1a=.nifgen_grpc.ConfigureP2PEndpointFullnessStartTriggerResponse\x12t\n\x17\x43onfigureReferenceClock\x12+.nifgen_grpc.ConfigureReferenceClockRequest\x1a,.nifgen_grpc.ConfigureReferenceClockResponse\x12}\n\x1a\x43onfigureSampleClockSource\x12..nifgen_grpc.ConfigureSampleClockSourceRequest\x1a/.nifgen_grpc.ConfigureSampleClockSourceResponse\x12h\n\x13\x43onfigureSampleRate\x12\'.nifgen_grpc.ConfigureSampleRateRequest\x1a(.nifgen_grpc.ConfigureSampleRateResponse\x12\x95\x01\n\"ConfigureSoftwareEdgeScriptTrigger\x12\x36.nifgen_grpc.ConfigureSoftwareEdgeScriptTriggerRequest\x1a\x37.nifgen_grpc.ConfigureSoftwareEdgeScriptTriggerResponse\x12\x92\x01\n!ConfigureSoftwareEdgeStartTrigger\x12\x35.nifgen_grpc.ConfigureSoftwareEdgeStartTriggerRequest\x1a\x36.nifgen_grpc.ConfigureSoftwareEdgeStartTriggerResponse\x12z\n\x19\x43onfigureStandardWaveform\x12-.nifgen_grpc.ConfigureStandardWaveformRequest\x1a..nifgen_grpc.ConfigureStandardWaveformResponse\x12w\n\x18\x43onfigureSynchronization\x12,.nifgen_grpc.ConfigureSynchronizationRequest\x1a-.nifgen_grpc.ConfigureSynchronizationResponse\x12k\n\x14\x43onfigureTriggerMode\x12(.nifgen_grpc.ConfigureTriggerModeRequest\x1a).nifgen_grpc.ConfigureTriggerModeResponse\x12z\n\x19\x43reateAdvancedArbSequence\x12-.nifgen_grpc.CreateAdvancedArbSequenceRequest\x1a..nifgen_grpc.CreateAdvancedArbSequenceResponse\x12\x62\n\x11\x43reateArbSequence\x12%.nifgen_grpc.CreateArbSequenceRequest\x1a&.nifgen_grpc.CreateArbSequenceResponse\x12Y\n\x0e\x43reateFreqList\x12\".nifgen_grpc.CreateFreqListRequest\x1a#.nifgen_grpc.CreateFreqListResponse\x12w\n\x18\x43reateWaveformComplexF64\x12,.nifgen_grpc.CreateWaveformComplexF64Request\x1a-.nifgen_grpc.CreateWaveformComplexF64Response\x12\x62\n\x11\x43reateWaveformF64\x12%.nifgen_grpc.CreateWaveformF64Request\x1a&.nifgen_grpc.CreateWaveformF64Response\x12z\n\x19\x43reateWaveformFromFileF64\x12-.nifgen_grpc.CreateWaveformFromFileF64Request\x1a..nifgen_grpc.CreateWaveformFromFileF64Response\x12z\n\x19\x43reateWaveformFromFileI16\x12-.nifgen_grpc.CreateWaveformFromFileI16Request\x1a..nifgen_grpc.CreateWaveformFromFileI16Response\x12\x62\n\x11\x43reateWaveformI16\x12%.nifgen_grpc.CreateWaveformI16Request\x1a&.nifgen_grpc.CreateWaveformI16Response\x12}\n\x1a\x44\x65\x66ineUserStandardWaveform\x12..nifgen_grpc.DefineUserStandardWaveformRequest\x1a/.nifgen_grpc.DefineUserStandardWaveformResponse\x12h\n\x13\x44\x65leteNamedWaveform\x12\'.nifgen_grpc.DeleteNamedWaveformRequest\x1a(.nifgen_grpc.DeleteNamedWaveformResponse\x12S\n\x0c\x44\x65leteScript\x12 .nifgen_grpc.DeleteScriptRequest\x1a!.nifgen_grpc.DeleteScriptResponse\x12\x44\n\x07\x44isable\x12\x1b.nifgen_grpc.DisableRequest\x1a\x1c.nifgen_grpc.DisableResponse\x12h\n\x13\x44isableAnalogFilter\x12\'.nifgen_grpc.DisableAnalogFilterRequest\x1a(.nifgen_grpc.DisableAnalogFilterResponse\x12k\n\x14\x44isableDigitalFilter\x12(.nifgen_grpc.DisableDigitalFilterRequest\x1a).nifgen_grpc.DisableDigitalFilterResponse\x12w\n\x18\x44isableDigitalPatterning\x12,.nifgen_grpc.DisableDigitalPatterningRequest\x1a-.nifgen_grpc.DisableDigitalPatterningResponse\x12k\n\x14\x44isableScriptTrigger\x12(.nifgen_grpc.DisableScriptTriggerRequest\x1a).nifgen_grpc.DisableScriptTriggerResponse\x12h\n\x13\x44isableStartTrigger\x12\'.nifgen_grpc.DisableStartTriggerRequest\x1a(.nifgen_grpc.DisableStartTriggerResponse\x12\x65\n\x12\x45nableAnalogFilter\x12&.nifgen_grpc.EnableAnalogFilterRequest\x1a\'.nifgen_grpc.EnableAnalogFilterResponse\x12h\n\x13\x45nableDigitalFilter\x12\'.nifgen_grpc.EnableDigitalFilterRequest\x1a(.nifgen_grpc.EnableDigitalFilterResponse\x12t\n\x17\x45nableDigitalPatterning\x12+.nifgen_grpc.EnableDigitalPatterningRequest\x1a,.nifgen_grpc.EnableDigitalPatterningResponse\x12S\n\x0c\x45rrorHandler\x12 .nifgen_grpc.ErrorHandlerRequest\x1a!.nifgen_grpc.ErrorHandlerResponse\x12S\n\x0c\x45rrorMessage\x12 .nifgen_grpc.ErrorMessageRequest\x1a!.nifgen_grpc.ErrorMessageResponse\x12M\n\nErrorQuery\x12\x1e.nifgen_grpc.ErrorQueryRequest\x1a\x1f.nifgen_grpc.ErrorQueryResponse\x12\x95\x01\n\"ExportAttributeConfigurationBuffer\x12\x36.nifgen_grpc.ExportAttributeConfigurationBufferRequest\x1a\x37.nifgen_grpc.ExportAttributeConfigurationBufferResponse\x12\x8f\x01\n ExportAttributeConfigurationFile\x12\x34.nifgen_grpc.ExportAttributeConfigurationFileRequest\x1a\x35.nifgen_grpc.ExportAttributeConfigurationFileResponse\x12S\n\x0c\x45xportSignal\x12 .nifgen_grpc.ExportSignalRequest\x1a!.nifgen_grpc.ExportSignalResponse\x12n\n\x15GetAttributeViBoolean\x12).nifgen_grpc.GetAttributeViBooleanRequest\x1a*.nifgen_grpc.GetAttributeViBooleanResponse\x12h\n\x13GetAttributeViInt32\x12\'.nifgen_grpc.GetAttributeViInt32Request\x1a(.nifgen_grpc.GetAttributeViInt32Response\x12h\n\x13GetAttributeViInt64\x12\'.nifgen_grpc.GetAttributeViInt64Request\x1a(.nifgen_grpc.GetAttributeViInt64Response\x12k\n\x14GetAttributeViReal64\x12(.nifgen_grpc.GetAttributeViReal64Request\x1a).nifgen_grpc.GetAttributeViReal64Response\x12n\n\x15GetAttributeViSession\x12).nifgen_grpc.GetAttributeViSessionRequest\x1a*.nifgen_grpc.GetAttributeViSessionResponse\x12k\n\x14GetAttributeViString\x12(.nifgen_grpc.GetAttributeViStringRequest\x1a).nifgen_grpc.GetAttributeViStringResponse\x12Y\n\x0eGetChannelName\x12\".nifgen_grpc.GetChannelNameRequest\x1a#.nifgen_grpc.GetChannelNameResponse\x12G\n\x08GetError\x12\x1c.nifgen_grpc.GetErrorRequest\x1a\x1d.nifgen_grpc.GetErrorResponse\x12w\n\x18GetExtCalLastDateAndTime\x12,.nifgen_grpc.GetExtCalLastDateAndTimeRequest\x1a-.nifgen_grpc.GetExtCalLastDateAndTimeResponse\x12\x62\n\x11GetExtCalLastTemp\x12%.nifgen_grpc.GetExtCalLastTempRequest\x1a&.nifgen_grpc.GetExtCalLastTempResponse\x12\x83\x01\n\x1cGetExtCalRecommendedInterval\x12\x30.nifgen_grpc.GetExtCalRecommendedIntervalRequest\x1a\x31.nifgen_grpc.GetExtCalRecommendedIntervalResponse\x12w\n\x18GetFIRFilterCoefficients\x12,.nifgen_grpc.GetFIRFilterCoefficientsRequest\x1a-.nifgen_grpc.GetFIRFilterCoefficientsResponse\x12_\n\x10GetHardwareState\x12$.nifgen_grpc.GetHardwareStateRequest\x1a%.nifgen_grpc.GetHardwareStateResponse\x12z\n\x19GetSelfCalLastDateAndTime\x12-.nifgen_grpc.GetSelfCalLastDateAndTimeRequest\x1a..nifgen_grpc.GetSelfCalLastDateAndTimeResponse\x12\x65\n\x12GetSelfCalLastTemp\x12&.nifgen_grpc.GetSelfCalLastTempRequest\x1a\'.nifgen_grpc.GetSelfCalLastTempResponse\x12h\n\x13GetSelfCalSupported\x12\'.nifgen_grpc.GetSelfCalSupportedRequest\x1a(.nifgen_grpc.GetSelfCalSupportedResponse\x12t\n\x17GetStreamEndpointHandle\x12+.nifgen_grpc.GetStreamEndpointHandleRequest\x1a,.nifgen_grpc.GetStreamEndpointHandleResponse\x12\x95\x01\n\"ImportAttributeConfigurationBuffer\x12\x36.nifgen_grpc.ImportAttributeConfigurationBufferRequest\x1a\x37.nifgen_grpc.ImportAttributeConfigurationBufferResponse\x12\x8f\x01\n ImportAttributeConfigurationFile\x12\x34.nifgen_grpc.ImportAttributeConfigurationFileRequest\x1a\x35.nifgen_grpc.ImportAttributeConfigurationFileResponse\x12;\n\x04Init\x12\x18.nifgen_grpc.InitRequest\x1a\x19.nifgen_grpc.InitResponse\x12\\\n\x0fInitWithOptions\x12#.nifgen_grpc.InitWithOptionsRequest\x1a$.nifgen_grpc.InitWithOptionsResponse\x12q\n\x16InitializeWithChannels\x12*.nifgen_grpc.InitializeWithChannelsRequest\x1a+.nifgen_grpc.InitializeWithChannelsResponse\x12\x65\n\x12InitiateGeneration\x12&.nifgen_grpc.InitiateGenerationRequest\x1a\'.nifgen_grpc.InitiateGenerationResponse\x12t\n\x17InvalidateAllAttributes\x12+.nifgen_grpc.InvalidateAllAttributesRequest\x1a,.nifgen_grpc.InvalidateAllAttributesResponse\x12\x41\n\x06IsDone\x12\x1a.nifgen_grpc.IsDoneRequest\x1a\x1b.nifgen_grpc.IsDoneResponse\x12t\n\x17QueryArbSeqCapabilities\x12+.nifgen_grpc.QueryArbSeqCapabilitiesRequest\x1a,.nifgen_grpc.QueryArbSeqCapabilitiesResponse\x12t\n\x17QueryArbWfmCapabilities\x12+.nifgen_grpc.QueryArbWfmCapabilitiesRequest\x1a,.nifgen_grpc.QueryArbWfmCapabilitiesResponse\x12z\n\x19QueryFreqListCapabilities\x12-.nifgen_grpc.QueryFreqListCapabilitiesRequest\x1a..nifgen_grpc.QueryFreqListCapabilitiesResponse\x12q\n\x16ReadCurrentTemperature\x12*.nifgen_grpc.ReadCurrentTemperatureRequest\x1a+.nifgen_grpc.ReadCurrentTemperatureResponse\x12>\n\x05Reset\x12\x19.nifgen_grpc.ResetRequest\x1a\x1a.nifgen_grpc.ResetResponse\x12Y\n\x0eResetAttribute\x12\".nifgen_grpc.ResetAttributeRequest\x1a#.nifgen_grpc.ResetAttributeResponse\x12P\n\x0bResetDevice\x12\x1f.nifgen_grpc.ResetDeviceRequest\x1a .nifgen_grpc.ResetDeviceResponse\x12n\n\x15ResetInterchangeCheck\x12).nifgen_grpc.ResetInterchangeCheckRequest\x1a*.nifgen_grpc.ResetInterchangeCheckResponse\x12\x62\n\x11ResetWithDefaults\x12%.nifgen_grpc.ResetWithDefaultsRequest\x1a&.nifgen_grpc.ResetWithDefaultsResponse\x12V\n\rRevisionQuery\x12!.nifgen_grpc.RevisionQueryRequest\x1a\".nifgen_grpc.RevisionQueryResponse\x12Y\n\x0eRouteSignalOut\x12\".nifgen_grpc.RouteSignalOutRequest\x1a#.nifgen_grpc.RouteSignalOutResponse\x12\x44\n\x07SelfCal\x12\x1b.nifgen_grpc.SelfCalRequest\x1a\x1c.nifgen_grpc.SelfCalResponse\x12G\n\x08SelfTest\x12\x1c.nifgen_grpc.SelfTestRequest\x1a\x1d.nifgen_grpc.SelfTestResponse\x12t\n\x17SendSoftwareEdgeTrigger\x12+.nifgen_grpc.SendSoftwareEdgeTriggerRequest\x1a,.nifgen_grpc.SendSoftwareEdgeTriggerResponse\x12n\n\x15SetAttributeViBoolean\x12).nifgen_grpc.SetAttributeViBooleanRequest\x1a*.nifgen_grpc.SetAttributeViBooleanResponse\x12h\n\x13SetAttributeViInt32\x12\'.nifgen_grpc.SetAttributeViInt32Request\x1a(.nifgen_grpc.SetAttributeViInt32Response\x12h\n\x13SetAttributeViInt64\x12\'.nifgen_grpc.SetAttributeViInt64Request\x1a(.nifgen_grpc.SetAttributeViInt64Response\x12k\n\x14SetAttributeViReal64\x12(.nifgen_grpc.SetAttributeViReal64Request\x1a).nifgen_grpc.SetAttributeViReal64Response\x12n\n\x15SetAttributeViSession\x12).nifgen_grpc.SetAttributeViSessionRequest\x1a*.nifgen_grpc.SetAttributeViSessionResponse\x12k\n\x14SetAttributeViString\x12(.nifgen_grpc.SetAttributeViStringRequest\x1a).nifgen_grpc.SetAttributeViStringResponse\x12\x92\x01\n!SetNamedWaveformNextWritePosition\x12\x35.nifgen_grpc.SetNamedWaveformNextWritePositionRequest\x1a\x36.nifgen_grpc.SetNamedWaveformNextWritePositionResponse\x12\x83\x01\n\x1cSetWaveformNextWritePosition\x12\x30.nifgen_grpc.SetWaveformNextWritePositionRequest\x1a\x31.nifgen_grpc.SetWaveformNextWritePositionResponse\x12V\n\rWaitUntilDone\x12!.nifgen_grpc.WaitUntilDoneRequest\x1a\".nifgen_grpc.WaitUntilDoneResponse\x12n\n\x15WriteBinary16Waveform\x12).nifgen_grpc.WriteBinary16WaveformRequest\x1a*.nifgen_grpc.WriteBinary16WaveformResponse\x12\x83\x01\n\x1cWriteComplexBinary16Waveform\x12\x30.nifgen_grpc.WriteComplexBinary16WaveformRequest\x1a\x31.nifgen_grpc.WriteComplexBinary16WaveformResponse\x12\x83\x01\n\x1cWriteNamedWaveformComplexF64\x12\x30.nifgen_grpc.WriteNamedWaveformComplexF64Request\x1a\x31.nifgen_grpc.WriteNamedWaveformComplexF64Response\x12\x83\x01\n\x1cWriteNamedWaveformComplexI16\x12\x30.nifgen_grpc.WriteNamedWaveformComplexI16Request\x1a\x31.nifgen_grpc.WriteNamedWaveformComplexI16Response\x12n\n\x15WriteNamedWaveformF64\x12).nifgen_grpc.WriteNamedWaveformF64Request\x1a*.nifgen_grpc.WriteNamedWaveformF64Response\x12n\n\x15WriteNamedWaveformI16\x12).nifgen_grpc.WriteNamedWaveformI16Request\x1a*.nifgen_grpc.WriteNamedWaveformI16Response\x12h\n\x13WriteP2PEndpointI16\x12\'.nifgen_grpc.WriteP2PEndpointI16Request\x1a(.nifgen_grpc.WriteP2PEndpointI16Response\x12P\n\x0bWriteScript\x12\x1f.nifgen_grpc.WriteScriptRequest\x1a .nifgen_grpc.WriteScriptResponse\x12V\n\rWriteWaveform\x12!.nifgen_grpc.WriteWaveformRequest\x1a\".nifgen_grpc.WriteWaveformResponse\x12t\n\x17WriteWaveformComplexF64\x12+.nifgen_grpc.WriteWaveformComplexF64Request\x1a,.nifgen_grpc.WriteWaveformComplexF64Response\x12z\n\x19\x43reateWaveformFromFileHWS\x12-.nifgen_grpc.CreateWaveformFromFileHWSRequest\x1a..nifgen_grpc.CreateWaveformFromFileHWSResponse\x12n\n\x15ManualEnableP2PStream\x12).nifgen_grpc.ManualEnableP2PStreamRequest\x1a*.nifgen_grpc.ManualEnableP2PStreamResponseB<\n\x10\x63om.ni.grpc.fgenB\x06NiFgenP\x01\xaa\x02\x1dNationalInstruments.Grpc.Fgenb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nifgen_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nifgen_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\020com.ni.grpc.fgenB\006NiFgenP\001\252\002\035NationalInstruments.Grpc.Fgen'
   _NIFGENINT32ATTRIBUTEVALUES._options = None
   _NIFGENINT32ATTRIBUTEVALUES._serialized_options = b'\020\001'
   _NIFGENREAL64ATTRIBUTEVALUES._options = None
   _NIFGENREAL64ATTRIBUTEVALUES._serialized_options = b'\020\001'
   _INITRESPONSE.fields_by_name['error_message']._options = None
   _INITRESPONSE.fields_by_name['error_message']._serialized_options = b'\030\001'
   _INITWITHOPTIONSRESPONSE.fields_by_name['error_message']._options = None
   _INITWITHOPTIONSRESPONSE.fields_by_name['error_message']._serialized_options = b'\030\001'
   _INITIALIZEWITHCHANNELSRESPONSE.fields_by_name['error_message']._options = None
   _INITIALIZEWITHCHANNELSRESPONSE.fields_by_name['error_message']._serialized_options = b'\030\001'
-  _NIFGENATTRIBUTE._serialized_start=24956
-  _NIFGENATTRIBUTE._serialized_end=35621
-  _BYTEORDER._serialized_start=35623
-  _BYTEORDER._serialized_end=35713
-  _CLOCKMODE._serialized_start=35716
-  _CLOCKMODE._serialized_end=35846
-  _FREQUENCYLISTOPTIONS._serialized_start=35848
-  _FREQUENCYLISTOPTIONS._serialized_end=35969
-  _HARDWARESTATE._serialized_start=35972
-  _HARDWARESTATE._serialized_end=36204
-  _NIFGENINT32ATTRIBUTEVALUES._serialized_start=36207
-  _NIFGENINT32ATTRIBUTEVALUES._serialized_end=46640
-  _NIFGENREAL64ATTRIBUTEVALUES._serialized_start=46643
-  _NIFGENREAL64ATTRIBUTEVALUES._serialized_end=46938
-  _NIFGENSTRINGATTRIBUTEVALUESMAPPED._serialized_start=46941
-  _NIFGENSTRINGATTRIBUTEVALUESMAPPED._serialized_end=48300
-  _OUTPUTMODE._serialized_start=48303
-  _OUTPUTMODE._serialized_end=48520
-  _RELATIVETO._serialized_start=48522
-  _RELATIVETO._serialized_end=48640
-  _ROUTESIGNALFROM._serialized_start=48643
-  _ROUTESIGNALFROM._serialized_end=49548
-  _ROUTESIGNALTO._serialized_start=49551
-  _ROUTESIGNALTO._serialized_end=50080
-  _SEQUENCEHANDLE._serialized_start=50082
-  _SEQUENCEHANDLE._serialized_end=50186
-  _SIGNAL._serialized_start=50189
-  _SIGNAL._serialized_end=50733
-  _TRIGGER._serialized_start=50735
-  _TRIGGER._serialized_end=50847
-  _TRIGGERMODE._serialized_start=50850
-  _TRIGGERMODE._serialized_end=51041
-  _TRIGGERWHEN._serialized_start=51043
-  _TRIGGERWHEN._serialized_end=51167
-  _WAVEFORM._serialized_start=51170
-  _WAVEFORM._serialized_end=51491
-  _WAVEFORMHANDLE._serialized_start=51493
-  _WAVEFORMHANDLE._serialized_end=51597
-  _ABORTGENERATIONREQUEST._serialized_start=60
-  _ABORTGENERATIONREQUEST._serialized_end=120
-  _ABORTGENERATIONRESPONSE._serialized_start=122
-  _ABORTGENERATIONRESPONSE._serialized_end=163
-  _ADJUSTSAMPLECLOCKRELATIVEDELAYREQUEST._serialized_start=165
-  _ADJUSTSAMPLECLOCKRELATIVEDELAYREQUEST._serialized_end=265
-  _ADJUSTSAMPLECLOCKRELATIVEDELAYRESPONSE._serialized_start=267
-  _ADJUSTSAMPLECLOCKRELATIVEDELAYRESPONSE._serialized_end=323
-  _ALLOCATENAMEDWAVEFORMREQUEST._serialized_start=326
-  _ALLOCATENAMEDWAVEFORMREQUEST._serialized_end=460
-  _ALLOCATENAMEDWAVEFORMRESPONSE._serialized_start=462
-  _ALLOCATENAMEDWAVEFORMRESPONSE._serialized_end=509
-  _ALLOCATEWAVEFORMREQUEST._serialized_start=511
-  _ALLOCATEWAVEFORMREQUEST._serialized_end=617
-  _ALLOCATEWAVEFORMRESPONSE._serialized_start=619
-  _ALLOCATEWAVEFORMRESPONSE._serialized_end=686
-  _CHECKATTRIBUTEVIBOOLEANREQUEST._serialized_start=689
-  _CHECKATTRIBUTEVIBOOLEANREQUEST._serialized_end=856
-  _CHECKATTRIBUTEVIBOOLEANRESPONSE._serialized_start=858
-  _CHECKATTRIBUTEVIBOOLEANRESPONSE._serialized_end=907
-  _CHECKATTRIBUTEVIINT32REQUEST._serialized_start=910
-  _CHECKATTRIBUTEVIINT32REQUEST._serialized_end=1173
-  _CHECKATTRIBUTEVIINT32RESPONSE._serialized_start=1175
-  _CHECKATTRIBUTEVIINT32RESPONSE._serialized_end=1222
-  _CHECKATTRIBUTEVIINT64REQUEST._serialized_start=1225
-  _CHECKATTRIBUTEVIINT64REQUEST._serialized_end=1394
-  _CHECKATTRIBUTEVIINT64RESPONSE._serialized_start=1396
-  _CHECKATTRIBUTEVIINT64RESPONSE._serialized_end=1443
-  _CHECKATTRIBUTEVIREAL64REQUEST._serialized_start=1446
-  _CHECKATTRIBUTEVIREAL64REQUEST._serialized_end=1711
-  _CHECKATTRIBUTEVIREAL64RESPONSE._serialized_start=1713
-  _CHECKATTRIBUTEVIREAL64RESPONSE._serialized_end=1761
-  _CHECKATTRIBUTEVISESSIONREQUEST._serialized_start=1764
-  _CHECKATTRIBUTEVISESSIONREQUEST._serialized_end=1955
-  _CHECKATTRIBUTEVISESSIONRESPONSE._serialized_start=1957
-  _CHECKATTRIBUTEVISESSIONRESPONSE._serialized_end=2006
-  _CHECKATTRIBUTEVISTRINGREQUEST._serialized_start=2009
-  _CHECKATTRIBUTEVISTRINGREQUEST._serialized_end=2287
-  _CHECKATTRIBUTEVISTRINGRESPONSE._serialized_start=2289
-  _CHECKATTRIBUTEVISTRINGRESPONSE._serialized_end=2337
-  _CLEARARBMEMORYREQUEST._serialized_start=2339
-  _CLEARARBMEMORYREQUEST._serialized_end=2398
-  _CLEARARBMEMORYRESPONSE._serialized_start=2400
-  _CLEARARBMEMORYRESPONSE._serialized_end=2440
-  _CLEARARBSEQUENCEREQUEST._serialized_start=2443
-  _CLEARARBSEQUENCEREQUEST._serialized_end=2615
-  _CLEARARBSEQUENCERESPONSE._serialized_start=2617
-  _CLEARARBSEQUENCERESPONSE._serialized_end=2659
-  _CLEARARBWAVEFORMREQUEST._serialized_start=2662
-  _CLEARARBWAVEFORMREQUEST._serialized_end=2834
-  _CLEARARBWAVEFORMRESPONSE._serialized_start=2836
-  _CLEARARBWAVEFORMRESPONSE._serialized_end=2878
-  _CLEARERRORREQUEST._serialized_start=2880
-  _CLEARERRORREQUEST._serialized_end=2935
-  _CLEARERRORRESPONSE._serialized_start=2937
-  _CLEARERRORRESPONSE._serialized_end=2973
-  _CLEARFREQLISTREQUEST._serialized_start=2976
-  _CLEARFREQLISTREQUEST._serialized_end=3169
-  _CLEARFREQLISTRESPONSE._serialized_start=3171
-  _CLEARFREQLISTRESPONSE._serialized_end=3210
-  _CLEARINTERCHANGEWARNINGSREQUEST._serialized_start=3212
-  _CLEARINTERCHANGEWARNINGSREQUEST._serialized_end=3281
-  _CLEARINTERCHANGEWARNINGSRESPONSE._serialized_start=3283
-  _CLEARINTERCHANGEWARNINGSRESPONSE._serialized_end=3333
-  _CLEARUSERSTANDARDWAVEFORMREQUEST._serialized_start=3335
-  _CLEARUSERSTANDARDWAVEFORMREQUEST._serialized_end=3427
-  _CLEARUSERSTANDARDWAVEFORMRESPONSE._serialized_start=3429
-  _CLEARUSERSTANDARDWAVEFORMRESPONSE._serialized_end=3480
-  _CLOSEREQUEST._serialized_start=3482
-  _CLOSEREQUEST._serialized_end=3532
-  _CLOSERESPONSE._serialized_start=3534
-  _CLOSERESPONSE._serialized_end=3565
-  _COMMITREQUEST._serialized_start=3567
-  _COMMITREQUEST._serialized_end=3618
-  _COMMITRESPONSE._serialized_start=3620
-  _COMMITRESPONSE._serialized_end=3652
-  _CONFIGUREAMPLITUDEREQUEST._serialized_start=3654
-  _CONFIGUREAMPLITUDEREQUEST._serialized_end=3758
-  _CONFIGUREAMPLITUDERESPONSE._serialized_start=3760
-  _CONFIGUREAMPLITUDERESPONSE._serialized_end=3804
-  _CONFIGUREARBSEQUENCEREQUEST._serialized_start=3807
-  _CONFIGUREARBSEQUENCEREQUEST._serialized_end=3949
-  _CONFIGUREARBSEQUENCERESPONSE._serialized_start=3951
-  _CONFIGUREARBSEQUENCERESPONSE._serialized_end=3997
-  _CONFIGUREARBWAVEFORMREQUEST._serialized_start=4000
-  _CONFIGUREARBWAVEFORMREQUEST._serialized_end=4142
-  _CONFIGUREARBWAVEFORMRESPONSE._serialized_start=4144
-  _CONFIGUREARBWAVEFORMRESPONSE._serialized_end=4190
-  _CONFIGURECHANNELSREQUEST._serialized_start=4192
-  _CONFIGURECHANNELSREQUEST._serialized_end=4272
-  _CONFIGURECHANNELSRESPONSE._serialized_start=4274
-  _CONFIGURECHANNELSRESPONSE._serialized_end=4317
-  _CONFIGURECLOCKMODEREQUEST._serialized_start=4320
-  _CONFIGURECLOCKMODEREQUEST._serialized_end=4474
-  _CONFIGURECLOCKMODERESPONSE._serialized_start=4476
-  _CONFIGURECLOCKMODERESPONSE._serialized_end=4520
-  _CONFIGURECUSTOMFIRFILTERCOEFFICIENTSREQUEST._serialized_start=4523
-  _CONFIGURECUSTOMFIRFILTERCOEFFICIENTSREQUEST._serialized_end=4654
-  _CONFIGURECUSTOMFIRFILTERCOEFFICIENTSRESPONSE._serialized_start=4656
-  _CONFIGURECUSTOMFIRFILTERCOEFFICIENTSRESPONSE._serialized_end=4718
-  _CONFIGUREDIGITALEDGESCRIPTTRIGGERREQUEST._serialized_start=4721
-  _CONFIGUREDIGITALEDGESCRIPTTRIGGERREQUEST._serialized_end=4849
-  _CONFIGUREDIGITALEDGESCRIPTTRIGGERRESPONSE._serialized_start=4851
-  _CONFIGUREDIGITALEDGESCRIPTTRIGGERRESPONSE._serialized_end=4910
-  _CONFIGUREDIGITALEDGESTARTTRIGGERREQUEST._serialized_start=4912
-  _CONFIGUREDIGITALEDGESTARTTRIGGERREQUEST._serialized_end=5019
-  _CONFIGUREDIGITALEDGESTARTTRIGGERRESPONSE._serialized_start=5021
-  _CONFIGUREDIGITALEDGESTARTTRIGGERRESPONSE._serialized_end=5079
-  _CONFIGUREDIGITALLEVELSCRIPTTRIGGERREQUEST._serialized_start=5082
-  _CONFIGUREDIGITALLEVELSCRIPTTRIGGERREQUEST._serialized_end=5296
-  _CONFIGUREDIGITALLEVELSCRIPTTRIGGERRESPONSE._serialized_start=5298
-  _CONFIGUREDIGITALLEVELSCRIPTTRIGGERRESPONSE._serialized_end=5358
-  _CONFIGUREFREQLISTREQUEST._serialized_start=5361
-  _CONFIGUREFREQLISTREQUEST._serialized_end=5535
-  _CONFIGUREFREQLISTRESPONSE._serialized_start=5537
-  _CONFIGUREFREQLISTRESPONSE._serialized_end=5580
-  _CONFIGUREFREQUENCYREQUEST._serialized_start=5582
-  _CONFIGUREFREQUENCYREQUEST._serialized_end=5686
-  _CONFIGUREFREQUENCYRESPONSE._serialized_start=5688
-  _CONFIGUREFREQUENCYRESPONSE._serialized_end=5732
-  _CONFIGUREOPERATIONMODEREQUEST._serialized_start=5734
-  _CONFIGUREOPERATIONMODEREQUEST._serialized_end=5847
-  _CONFIGUREOPERATIONMODERESPONSE._serialized_start=5849
-  _CONFIGUREOPERATIONMODERESPONSE._serialized_end=5897
-  _CONFIGUREOUTPUTENABLEDREQUEST._serialized_start=5899
-  _CONFIGUREOUTPUTENABLEDREQUEST._serialized_end=6005
-  _CONFIGUREOUTPUTENABLEDRESPONSE._serialized_start=6007
-  _CONFIGUREOUTPUTENABLEDRESPONSE._serialized_end=6055
-  _CONFIGUREOUTPUTIMPEDANCEREQUEST._serialized_start=6057
-  _CONFIGUREOUTPUTIMPEDANCEREQUEST._serialized_end=6167
-  _CONFIGUREOUTPUTIMPEDANCERESPONSE._serialized_start=6169
-  _CONFIGUREOUTPUTIMPEDANCERESPONSE._serialized_end=6219
-  _CONFIGUREOUTPUTMODEREQUEST._serialized_start=6222
-  _CONFIGUREOUTPUTMODEREQUEST._serialized_end=6381
-  _CONFIGUREOUTPUTMODERESPONSE._serialized_start=6383
-  _CONFIGUREOUTPUTMODERESPONSE._serialized_end=6428
-  _CONFIGUREP2PENDPOINTFULLNESSSTARTTRIGGERREQUEST._serialized_start=6430
-  _CONFIGUREP2PENDPOINTFULLNESSSTARTTRIGGERREQUEST._serialized_end=6552
-  _CONFIGUREP2PENDPOINTFULLNESSSTARTTRIGGERRESPONSE._serialized_start=6554
-  _CONFIGUREP2PENDPOINTFULLNESSSTARTTRIGGERRESPONSE._serialized_end=6620
-  _CONFIGUREREFERENCECLOCKREQUEST._serialized_start=6623
-  _CONFIGUREREFERENCECLOCKREQUEST._serialized_end=6758
-  _CONFIGUREREFERENCECLOCKRESPONSE._serialized_start=6760
-  _CONFIGUREREFERENCECLOCKRESPONSE._serialized_end=6809
-  _CONFIGURESAMPLECLOCKSOURCEREQUEST._serialized_start=6811
-  _CONFIGURESAMPLECLOCKSOURCEREQUEST._serialized_end=6911
-  _CONFIGURESAMPLECLOCKSOURCERESPONSE._serialized_start=6913
-  _CONFIGURESAMPLECLOCKSOURCERESPONSE._serialized_end=6965
-  _CONFIGURESAMPLERATEREQUEST._serialized_start=6967
-  _CONFIGURESAMPLERATEREQUEST._serialized_end=7052
-  _CONFIGURESAMPLERATERESPONSE._serialized_start=7054
-  _CONFIGURESAMPLERATERESPONSE._serialized_end=7099
-  _CONFIGURESOFTWAREEDGESCRIPTTRIGGERREQUEST._serialized_start=7101
-  _CONFIGURESOFTWAREEDGESCRIPTTRIGGERREQUEST._serialized_end=7200
-  _CONFIGURESOFTWAREEDGESCRIPTTRIGGERRESPONSE._serialized_start=7202
-  _CONFIGURESOFTWAREEDGESCRIPTTRIGGERRESPONSE._serialized_end=7262
-  _CONFIGURESOFTWAREEDGESTARTTRIGGERREQUEST._serialized_start=7264
-  _CONFIGURESOFTWAREEDGESTARTTRIGGERREQUEST._serialized_end=7342
-  _CONFIGURESOFTWAREEDGESTARTTRIGGERRESPONSE._serialized_start=7344
-  _CONFIGURESOFTWAREEDGESTARTTRIGGERRESPONSE._serialized_end=7403
-  _CONFIGURESTANDARDWAVEFORMREQUEST._serialized_start=7406
-  _CONFIGURESTANDARDWAVEFORMREQUEST._serialized_end=7660
-  _CONFIGURESTANDARDWAVEFORMRESPONSE._serialized_start=7662
-  _CONFIGURESTANDARDWAVEFORMRESPONSE._serialized_end=7713
-  _CONFIGURESYNCHRONIZATIONREQUEST._serialized_start=7715
-  _CONFIGURESYNCHRONIZATIONREQUEST._serialized_end=7838
-  _CONFIGURESYNCHRONIZATIONRESPONSE._serialized_start=7840
-  _CONFIGURESYNCHRONIZATIONRESPONSE._serialized_end=7890
-  _CONFIGURETRIGGERMODEREQUEST._serialized_start=7893
-  _CONFIGURETRIGGERMODEREQUEST._serialized_end=8079
-  _CONFIGURETRIGGERMODERESPONSE._serialized_start=8081
-  _CONFIGURETRIGGERMODERESPONSE._serialized_end=8127
-  _CREATEADVANCEDARBSEQUENCEREQUEST._serialized_start=8130
-  _CREATEADVANCEDARBSEQUENCEREQUEST._serialized_end=8319
-  _CREATEADVANCEDARBSEQUENCERESPONSE._serialized_start=8321
-  _CREATEADVANCEDARBSEQUENCERESPONSE._serialized_end=8428
-  _CREATEARBSEQUENCEREQUEST._serialized_start=8430
-  _CREATEARBSEQUENCEREQUEST._serialized_end=8551
-  _CREATEARBSEQUENCERESPONSE._serialized_start=8553
-  _CREATEARBSEQUENCERESPONSE._serialized_end=8621
-  _CREATEFREQLISTREQUEST._serialized_start=8624
-  _CREATEFREQLISTREQUEST._serialized_end=8816
-  _CREATEFREQLISTRESPONSE._serialized_start=8818
-  _CREATEFREQLISTRESPONSE._serialized_end=8889
-  _CREATEWAVEFORMCOMPLEXF64REQUEST._serialized_start=8892
-  _CREATEWAVEFORMCOMPLEXF64REQUEST._serialized_end=9044
-  _CREATEWAVEFORMCOMPLEXF64RESPONSE._serialized_start=9046
-  _CREATEWAVEFORMCOMPLEXF64RESPONSE._serialized_end=9121
-  _CREATEWAVEFORMF64REQUEST._serialized_start=9123
-  _CREATEWAVEFORMF64REQUEST._serialized_end=9236
-  _CREATEWAVEFORMF64RESPONSE._serialized_start=9238
-  _CREATEWAVEFORMF64RESPONSE._serialized_end=9306
-  _CREATEWAVEFORMFROMFILEF64REQUEST._serialized_start=9309
-  _CREATEWAVEFORMFROMFILEF64REQUEST._serialized_end=9511
-  _CREATEWAVEFORMFROMFILEF64RESPONSE._serialized_start=9513
-  _CREATEWAVEFORMFROMFILEF64RESPONSE._serialized_end=9589
-  _CREATEWAVEFORMFROMFILEHWSREQUEST._serialized_start=9592
-  _CREATEWAVEFORMFROMFILEHWSREQUEST._serialized_end=9778
-  _CREATEWAVEFORMFROMFILEHWSRESPONSE._serialized_start=9780
-  _CREATEWAVEFORMFROMFILEHWSRESPONSE._serialized_end=9856
-  _CREATEWAVEFORMFROMFILEI16REQUEST._serialized_start=9859
-  _CREATEWAVEFORMFROMFILEI16REQUEST._serialized_end=10061
-  _CREATEWAVEFORMFROMFILEI16RESPONSE._serialized_start=10063
-  _CREATEWAVEFORMFROMFILEI16RESPONSE._serialized_end=10139
-  _CREATEWAVEFORMI16REQUEST._serialized_start=10141
-  _CREATEWAVEFORMI16REQUEST._serialized_end=10254
-  _CREATEWAVEFORMI16RESPONSE._serialized_start=10256
-  _CREATEWAVEFORMI16RESPONSE._serialized_end=10324
-  _DEFINEUSERSTANDARDWAVEFORMREQUEST._serialized_start=10326
-  _DEFINEUSERSTANDARDWAVEFORMREQUEST._serialized_end=10448
-  _DEFINEUSERSTANDARDWAVEFORMRESPONSE._serialized_start=10450
-  _DEFINEUSERSTANDARDWAVEFORMRESPONSE._serialized_end=10502
-  _DELETENAMEDWAVEFORMREQUEST._serialized_start=10504
-  _DELETENAMEDWAVEFORMREQUEST._serialized_end=10613
-  _DELETENAMEDWAVEFORMRESPONSE._serialized_start=10615
-  _DELETENAMEDWAVEFORMRESPONSE._serialized_end=10660
-  _DELETESCRIPTREQUEST._serialized_start=10662
-  _DELETESCRIPTREQUEST._serialized_end=10762
-  _DELETESCRIPTRESPONSE._serialized_start=10764
-  _DELETESCRIPTRESPONSE._serialized_end=10802
-  _DISABLEREQUEST._serialized_start=10804
-  _DISABLEREQUEST._serialized_end=10856
-  _DISABLERESPONSE._serialized_start=10858
-  _DISABLERESPONSE._serialized_end=10891
-  _DISABLEANALOGFILTERREQUEST._serialized_start=10893
-  _DISABLEANALOGFILTERREQUEST._serialized_end=10979
-  _DISABLEANALOGFILTERRESPONSE._serialized_start=10981
-  _DISABLEANALOGFILTERRESPONSE._serialized_end=11026
-  _DISABLEDIGITALFILTERREQUEST._serialized_start=11028
-  _DISABLEDIGITALFILTERREQUEST._serialized_end=11115
-  _DISABLEDIGITALFILTERRESPONSE._serialized_start=11117
-  _DISABLEDIGITALFILTERRESPONSE._serialized_end=11163
-  _DISABLEDIGITALPATTERNINGREQUEST._serialized_start=11165
-  _DISABLEDIGITALPATTERNINGREQUEST._serialized_end=11256
-  _DISABLEDIGITALPATTERNINGRESPONSE._serialized_start=11258
-  _DISABLEDIGITALPATTERNINGRESPONSE._serialized_end=11308
-  _DISABLESCRIPTTRIGGERREQUEST._serialized_start=11310
-  _DISABLESCRIPTTRIGGERREQUEST._serialized_end=11395
-  _DISABLESCRIPTTRIGGERRESPONSE._serialized_start=11397
-  _DISABLESCRIPTTRIGGERRESPONSE._serialized_end=11443
-  _DISABLESTARTTRIGGERREQUEST._serialized_start=11445
-  _DISABLESTARTTRIGGERREQUEST._serialized_end=11509
-  _DISABLESTARTTRIGGERRESPONSE._serialized_start=11511
-  _DISABLESTARTTRIGGERRESPONSE._serialized_end=11556
-  _ENABLEANALOGFILTERREQUEST._serialized_start=11558
-  _ENABLEANALOGFILTERREQUEST._serialized_end=11680
-  _ENABLEANALOGFILTERRESPONSE._serialized_start=11682
-  _ENABLEANALOGFILTERRESPONSE._serialized_end=11726
-  _ENABLEDIGITALFILTERREQUEST._serialized_start=11728
-  _ENABLEDIGITALFILTERREQUEST._serialized_end=11814
-  _ENABLEDIGITALFILTERRESPONSE._serialized_start=11816
-  _ENABLEDIGITALFILTERRESPONSE._serialized_end=11861
-  _ENABLEDIGITALPATTERNINGREQUEST._serialized_start=11863
-  _ENABLEDIGITALPATTERNINGREQUEST._serialized_end=11953
-  _ENABLEDIGITALPATTERNINGRESPONSE._serialized_start=11955
-  _ENABLEDIGITALPATTERNINGRESPONSE._serialized_end=12004
-  _ERRORHANDLERREQUEST._serialized_start=12006
-  _ERRORHANDLERREQUEST._serialized_end=12083
-  _ERRORHANDLERRESPONSE._serialized_start=12085
-  _ERRORHANDLERRESPONSE._serialized_end=12146
-  _ERRORMESSAGEREQUEST._serialized_start=12148
-  _ERRORMESSAGEREQUEST._serialized_end=12225
-  _ERRORMESSAGERESPONSE._serialized_start=12227
-  _ERRORMESSAGERESPONSE._serialized_end=12288
-  _ERRORQUERYREQUEST._serialized_start=12290
-  _ERRORQUERYREQUEST._serialized_end=12345
-  _ERRORQUERYRESPONSE._serialized_start=12347
-  _ERRORQUERYRESPONSE._serialized_end=12426
-  _EXPORTATTRIBUTECONFIGURATIONBUFFERREQUEST._serialized_start=12428
-  _EXPORTATTRIBUTECONFIGURATIONBUFFERREQUEST._serialized_end=12507
-  _EXPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE._serialized_start=12509
-  _EXPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE._serialized_end=12592
-  _EXPORTATTRIBUTECONFIGURATIONFILEREQUEST._serialized_start=12594
-  _EXPORTATTRIBUTECONFIGURATIONFILEREQUEST._serialized_end=12690
-  _EXPORTATTRIBUTECONFIGURATIONFILERESPONSE._serialized_start=12692
-  _EXPORTATTRIBUTECONFIGURATIONFILERESPONSE._serialized_end=12750
-  _EXPORTSIGNALREQUEST._serialized_start=12753
-  _EXPORTSIGNALREQUEST._serialized_end=12938
-  _EXPORTSIGNALRESPONSE._serialized_start=12940
-  _EXPORTSIGNALRESPONSE._serialized_end=12978
-  _GETATTRIBUTEVIBOOLEANREQUEST._serialized_start=12981
-  _GETATTRIBUTEVIBOOLEANREQUEST._serialized_end=13121
-  _GETATTRIBUTEVIBOOLEANRESPONSE._serialized_start=13123
-  _GETATTRIBUTEVIBOOLEANRESPONSE._serialized_end=13195
-  _GETATTRIBUTEVIINT32REQUEST._serialized_start=13198
-  _GETATTRIBUTEVIINT32REQUEST._serialized_end=13336
-  _GETATTRIBUTEVIINT32RESPONSE._serialized_start=13338
-  _GETATTRIBUTEVIINT32RESPONSE._serialized_end=13408
-  _GETATTRIBUTEVIINT64REQUEST._serialized_start=13411
-  _GETATTRIBUTEVIINT64REQUEST._serialized_end=13549
-  _GETATTRIBUTEVIINT64RESPONSE._serialized_start=13551
-  _GETATTRIBUTEVIINT64RESPONSE._serialized_end=13621
-  _GETATTRIBUTEVIREAL64REQUEST._serialized_start=13624
-  _GETATTRIBUTEVIREAL64REQUEST._serialized_end=13763
-  _GETATTRIBUTEVIREAL64RESPONSE._serialized_start=13765
-  _GETATTRIBUTEVIREAL64RESPONSE._serialized_end=13836
-  _GETATTRIBUTEVISESSIONREQUEST._serialized_start=13839
-  _GETATTRIBUTEVISESSIONREQUEST._serialized_end=13979
-  _GETATTRIBUTEVISESSIONRESPONSE._serialized_start=13981
-  _GETATTRIBUTEVISESSIONRESPONSE._serialized_end=14077
-  _GETATTRIBUTEVISTRINGREQUEST._serialized_start=14080
-  _GETATTRIBUTEVISTRINGREQUEST._serialized_end=14219
-  _GETATTRIBUTEVISTRINGRESPONSE._serialized_start=14221
-  _GETATTRIBUTEVISTRINGRESPONSE._serialized_end=14292
-  _GETCHANNELNAMEREQUEST._serialized_start=14294
-  _GETCHANNELNAMEREQUEST._serialized_end=14368
-  _GETCHANNELNAMERESPONSE._serialized_start=14370
-  _GETCHANNELNAMERESPONSE._serialized_end=14434
-  _GETERRORREQUEST._serialized_start=14436
-  _GETERRORREQUEST._serialized_end=14489
-  _GETERRORRESPONSE._serialized_start=14491
-  _GETERRORRESPONSE._serialized_end=14572
-  _GETEXTCALLASTDATEANDTIMEREQUEST._serialized_start=14574
-  _GETEXTCALLASTDATEANDTIMEREQUEST._serialized_end=14643
-  _GETEXTCALLASTDATEANDTIMERESPONSE._serialized_start=14645
-  _GETEXTCALLASTDATEANDTIMERESPONSE._serialized_end=14767
-  _GETEXTCALLASTTEMPREQUEST._serialized_start=14769
-  _GETEXTCALLASTTEMPREQUEST._serialized_end=14831
-  _GETEXTCALLASTTEMPRESPONSE._serialized_start=14833
-  _GETEXTCALLASTTEMPRESPONSE._serialized_end=14897
-  _GETEXTCALRECOMMENDEDINTERVALREQUEST._serialized_start=14899
-  _GETEXTCALRECOMMENDEDINTERVALREQUEST._serialized_end=14972
-  _GETEXTCALRECOMMENDEDINTERVALRESPONSE._serialized_start=14974
-  _GETEXTCALRECOMMENDEDINTERVALRESPONSE._serialized_end=15044
-  _GETFIRFILTERCOEFFICIENTSREQUEST._serialized_start=15046
-  _GETFIRFILTERCOEFFICIENTSREQUEST._serialized_end=15137
-  _GETFIRFILTERCOEFFICIENTSRESPONSE._serialized_start=15139
-  _GETFIRFILTERCOEFFICIENTSRESPONSE._serialized_end=15254
-  _GETHARDWARESTATEREQUEST._serialized_start=15256
-  _GETHARDWARESTATEREQUEST._serialized_end=15317
-  _GETHARDWARESTATERESPONSE._serialized_start=15319
-  _GETHARDWARESTATERESPONSE._serialized_end=15423
-  _GETNEXTCOERCIONRECORDREQUEST._serialized_start=15425
-  _GETNEXTCOERCIONRECORDREQUEST._serialized_end=15491
-  _GETNEXTCOERCIONRECORDRESPONSE._serialized_start=15493
-  _GETNEXTCOERCIONRECORDRESPONSE._serialized_end=15565
-  _GETNEXTINTERCHANGEWARNINGREQUEST._serialized_start=15567
-  _GETNEXTINTERCHANGEWARNINGREQUEST._serialized_end=15637
-  _GETNEXTINTERCHANGEWARNINGRESPONSE._serialized_start=15639
-  _GETNEXTINTERCHANGEWARNINGRESPONSE._serialized_end=15719
-  _GETSELFCALLASTDATEANDTIMEREQUEST._serialized_start=15721
-  _GETSELFCALLASTDATEANDTIMEREQUEST._serialized_end=15791
-  _GETSELFCALLASTDATEANDTIMERESPONSE._serialized_start=15793
-  _GETSELFCALLASTDATEANDTIMERESPONSE._serialized_end=15916
-  _GETSELFCALLASTTEMPREQUEST._serialized_start=15918
-  _GETSELFCALLASTTEMPREQUEST._serialized_end=15981
-  _GETSELFCALLASTTEMPRESPONSE._serialized_start=15983
-  _GETSELFCALLASTTEMPRESPONSE._serialized_end=16048
-  _GETSELFCALSUPPORTEDREQUEST._serialized_start=16050
-  _GETSELFCALSUPPORTEDREQUEST._serialized_end=16114
-  _GETSELFCALSUPPORTEDRESPONSE._serialized_start=16116
-  _GETSELFCALSUPPORTEDRESPONSE._serialized_end=16189
-  _GETSTREAMENDPOINTHANDLEREQUEST._serialized_start=16191
-  _GETSTREAMENDPOINTHANDLEREQUEST._serialized_end=16284
-  _GETSTREAMENDPOINTHANDLERESPONSE._serialized_start=16286
-  _GETSTREAMENDPOINTHANDLERESPONSE._serialized_end=16358
-  _IMPORTATTRIBUTECONFIGURATIONBUFFERREQUEST._serialized_start=16360
-  _IMPORTATTRIBUTECONFIGURATIONBUFFERREQUEST._serialized_end=16462
-  _IMPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE._serialized_start=16464
-  _IMPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE._serialized_end=16524
-  _IMPORTATTRIBUTECONFIGURATIONFILEREQUEST._serialized_start=16526
-  _IMPORTATTRIBUTECONFIGURATIONFILEREQUEST._serialized_end=16622
-  _IMPORTATTRIBUTECONFIGURATIONFILERESPONSE._serialized_start=16624
-  _IMPORTATTRIBUTECONFIGURATIONFILERESPONSE._serialized_end=16682
-  _INITREQUEST._serialized_start=16685
-  _INITREQUEST._serialized_end=16862
-  _INITRESPONSE._serialized_start=16864
-  _INITRESPONSE._serialized_end=16990
-  _INITWITHOPTIONSREQUEST._serialized_start=16993
-  _INITWITHOPTIONSREQUEST._serialized_end=17204
-  _INITWITHOPTIONSRESPONSE._serialized_start=17207
-  _INITWITHOPTIONSRESPONSE._serialized_end=17344
-  _INITIALIZEWITHCHANNELSREQUEST._serialized_start=17347
-  _INITIALIZEWITHCHANNELSREQUEST._serialized_end=17569
-  _INITIALIZEWITHCHANNELSRESPONSE._serialized_start=17572
-  _INITIALIZEWITHCHANNELSRESPONSE._serialized_end=17716
-  _INITIATEGENERATIONREQUEST._serialized_start=17718
-  _INITIATEGENERATIONREQUEST._serialized_end=17781
-  _INITIATEGENERATIONRESPONSE._serialized_start=17783
-  _INITIATEGENERATIONRESPONSE._serialized_end=17827
-  _INVALIDATEALLATTRIBUTESREQUEST._serialized_start=17829
-  _INVALIDATEALLATTRIBUTESREQUEST._serialized_end=17897
-  _INVALIDATEALLATTRIBUTESRESPONSE._serialized_start=17899
-  _INVALIDATEALLATTRIBUTESRESPONSE._serialized_end=17948
-  _ISDONEREQUEST._serialized_start=17950
-  _ISDONEREQUEST._serialized_end=18001
-  _ISDONERESPONSE._serialized_start=18003
-  _ISDONERESPONSE._serialized_end=18049
-  _MANUALENABLEP2PSTREAMREQUEST._serialized_start=18051
-  _MANUALENABLEP2PSTREAMREQUEST._serialized_end=18140
-  _MANUALENABLEP2PSTREAMRESPONSE._serialized_start=18142
-  _MANUALENABLEP2PSTREAMRESPONSE._serialized_end=18189
-  _QUERYARBSEQCAPABILITIESREQUEST._serialized_start=18191
-  _QUERYARBSEQCAPABILITIESREQUEST._serialized_end=18259
-  _QUERYARBSEQCAPABILITIESRESPONSE._serialized_start=18262
-  _QUERYARBSEQCAPABILITIESRESPONSE._serialized_end=18442
-  _QUERYARBWFMCAPABILITIESREQUEST._serialized_start=18444
-  _QUERYARBWFMCAPABILITIESREQUEST._serialized_end=18512
-  _QUERYARBWFMCAPABILITIESRESPONSE._serialized_start=18515
-  _QUERYARBWFMCAPABILITIESRESPONSE._serialized_end=18689
-  _QUERYFREQLISTCAPABILITIESREQUEST._serialized_start=18691
-  _QUERYFREQLISTCAPABILITIESREQUEST._serialized_end=18761
-  _QUERYFREQLISTCAPABILITIESRESPONSE._serialized_start=18764
-  _QUERYFREQLISTCAPABILITIESRESPONSE._serialized_end=19054
-  _READCURRENTTEMPERATUREREQUEST._serialized_start=19056
-  _READCURRENTTEMPERATUREREQUEST._serialized_end=19123
-  _READCURRENTTEMPERATURERESPONSE._serialized_start=19125
-  _READCURRENTTEMPERATURERESPONSE._serialized_end=19194
-  _RESETREQUEST._serialized_start=19196
-  _RESETREQUEST._serialized_end=19246
-  _RESETRESPONSE._serialized_start=19248
-  _RESETRESPONSE._serialized_end=19279
-  _RESETATTRIBUTEREQUEST._serialized_start=19282
-  _RESETATTRIBUTEREQUEST._serialized_end=19415
-  _RESETATTRIBUTERESPONSE._serialized_start=19417
-  _RESETATTRIBUTERESPONSE._serialized_end=19457
-  _RESETDEVICEREQUEST._serialized_start=19459
-  _RESETDEVICEREQUEST._serialized_end=19515
-  _RESETDEVICERESPONSE._serialized_start=19517
-  _RESETDEVICERESPONSE._serialized_end=19554
-  _RESETINTERCHANGECHECKREQUEST._serialized_start=19556
-  _RESETINTERCHANGECHECKREQUEST._serialized_end=19622
-  _RESETINTERCHANGECHECKRESPONSE._serialized_start=19624
-  _RESETINTERCHANGECHECKRESPONSE._serialized_end=19671
-  _RESETWITHDEFAULTSREQUEST._serialized_start=19673
-  _RESETWITHDEFAULTSREQUEST._serialized_end=19735
-  _RESETWITHDEFAULTSRESPONSE._serialized_start=19737
-  _RESETWITHDEFAULTSRESPONSE._serialized_end=19780
-  _REVISIONQUERYREQUEST._serialized_start=19782
-  _REVISIONQUERYREQUEST._serialized_end=19840
-  _REVISIONQUERYRESPONSE._serialized_start=19842
-  _REVISIONQUERYRESPONSE._serialized_end=19944
-  _ROUTESIGNALOUTREQUEST._serialized_start=19947
-  _ROUTESIGNALOUTREQUEST._serialized_end=20256
-  _ROUTESIGNALOUTRESPONSE._serialized_start=20258
-  _ROUTESIGNALOUTRESPONSE._serialized_end=20298
-  _SELFCALREQUEST._serialized_start=20300
-  _SELFCALREQUEST._serialized_end=20352
-  _SELFCALRESPONSE._serialized_start=20354
-  _SELFCALRESPONSE._serialized_end=20387
-  _SELFTESTREQUEST._serialized_start=20389
-  _SELFTESTREQUEST._serialized_end=20442
-  _SELFTESTRESPONSE._serialized_start=20444
-  _SELFTESTRESPONSE._serialized_end=20531
-  _SENDSOFTWAREEDGETRIGGERREQUEST._serialized_start=20534
-  _SENDSOFTWAREEDGETRIGGERREQUEST._serialized_end=20702
-  _SENDSOFTWAREEDGETRIGGERRESPONSE._serialized_start=20704
-  _SENDSOFTWAREEDGETRIGGERRESPONSE._serialized_end=20753
-  _SETATTRIBUTEVIBOOLEANREQUEST._serialized_start=20756
-  _SETATTRIBUTEVIBOOLEANREQUEST._serialized_end=20921
-  _SETATTRIBUTEVIBOOLEANRESPONSE._serialized_start=20923
-  _SETATTRIBUTEVIBOOLEANRESPONSE._serialized_end=20970
-  _SETATTRIBUTEVIINT32REQUEST._serialized_start=20973
-  _SETATTRIBUTEVIINT32REQUEST._serialized_end=21234
-  _SETATTRIBUTEVIINT32RESPONSE._serialized_start=21236
-  _SETATTRIBUTEVIINT32RESPONSE._serialized_end=21281
-  _SETATTRIBUTEVIINT64REQUEST._serialized_start=21284
-  _SETATTRIBUTEVIINT64REQUEST._serialized_end=21451
-  _SETATTRIBUTEVIINT64RESPONSE._serialized_start=21453
-  _SETATTRIBUTEVIINT64RESPONSE._serialized_end=21498
-  _SETATTRIBUTEVIREAL64REQUEST._serialized_start=21501
-  _SETATTRIBUTEVIREAL64REQUEST._serialized_end=21764
-  _SETATTRIBUTEVIREAL64RESPONSE._serialized_start=21766
-  _SETATTRIBUTEVIREAL64RESPONSE._serialized_end=21812
-  _SETATTRIBUTEVISESSIONREQUEST._serialized_start=21815
-  _SETATTRIBUTEVISESSIONREQUEST._serialized_end=22004
-  _SETATTRIBUTEVISESSIONRESPONSE._serialized_start=22006
-  _SETATTRIBUTEVISESSIONRESPONSE._serialized_end=22053
-  _SETATTRIBUTEVISTRINGREQUEST._serialized_start=22056
-  _SETATTRIBUTEVISTRINGREQUEST._serialized_end=22332
-  _SETATTRIBUTEVISTRINGRESPONSE._serialized_start=22334
-  _SETATTRIBUTEVISTRINGRESPONSE._serialized_end=22380
-  _SETNAMEDWAVEFORMNEXTWRITEPOSITIONREQUEST._serialized_start=22383
-  _SETNAMEDWAVEFORMNEXTWRITEPOSITIONREQUEST._serialized_end=22617
-  _SETNAMEDWAVEFORMNEXTWRITEPOSITIONRESPONSE._serialized_start=22619
-  _SETNAMEDWAVEFORMNEXTWRITEPOSITIONRESPONSE._serialized_end=22678
-  _SETWAVEFORMNEXTWRITEPOSITIONREQUEST._serialized_start=22681
-  _SETWAVEFORMNEXTWRITEPOSITIONREQUEST._serialized_end=22912
-  _SETWAVEFORMNEXTWRITEPOSITIONRESPONSE._serialized_start=22914
-  _SETWAVEFORMNEXTWRITEPOSITIONRESPONSE._serialized_end=22968
-  _WAITUNTILDONEREQUEST._serialized_start=22970
-  _WAITUNTILDONEREQUEST._serialized_end=23046
-  _WAITUNTILDONERESPONSE._serialized_start=23048
-  _WAITUNTILDONERESPONSE._serialized_end=23087
-  _WRITEBINARY16WAVEFORMREQUEST._serialized_start=23089
-  _WRITEBINARY16WAVEFORMREQUEST._serialized_end=23216
-  _WRITEBINARY16WAVEFORMRESPONSE._serialized_start=23218
-  _WRITEBINARY16WAVEFORMRESPONSE._serialized_end=23265
-  _WRITECOMPLEXBINARY16WAVEFORMREQUEST._serialized_start=23268
-  _WRITECOMPLEXBINARY16WAVEFORMREQUEST._serialized_end=23431
-  _WRITECOMPLEXBINARY16WAVEFORMRESPONSE._serialized_start=23433
-  _WRITECOMPLEXBINARY16WAVEFORMRESPONSE._serialized_end=23487
-  _WRITENAMEDWAVEFORMCOMPLEXF64REQUEST._serialized_start=23490
-  _WRITENAMEDWAVEFORMCOMPLEXF64REQUEST._serialized_end=23654
-  _WRITENAMEDWAVEFORMCOMPLEXF64RESPONSE._serialized_start=23656
-  _WRITENAMEDWAVEFORMCOMPLEXF64RESPONSE._serialized_end=23710
-  _WRITENAMEDWAVEFORMCOMPLEXI16REQUEST._serialized_start=23713
-  _WRITENAMEDWAVEFORMCOMPLEXI16REQUEST._serialized_end=23874
-  _WRITENAMEDWAVEFORMCOMPLEXI16RESPONSE._serialized_start=23876
-  _WRITENAMEDWAVEFORMCOMPLEXI16RESPONSE._serialized_end=23930
-  _WRITENAMEDWAVEFORMF64REQUEST._serialized_start=23932
-  _WRITENAMEDWAVEFORMF64REQUEST._serialized_end=24057
-  _WRITENAMEDWAVEFORMF64RESPONSE._serialized_start=24059
-  _WRITENAMEDWAVEFORMF64RESPONSE._serialized_end=24106
-  _WRITENAMEDWAVEFORMI16REQUEST._serialized_start=24108
-  _WRITENAMEDWAVEFORMI16REQUEST._serialized_end=24233
-  _WRITENAMEDWAVEFORMI16RESPONSE._serialized_start=24235
-  _WRITENAMEDWAVEFORMI16RESPONSE._serialized_end=24282
-  _WRITEP2PENDPOINTI16REQUEST._serialized_start=24284
-  _WRITEP2PENDPOINTI16REQUEST._serialized_end=24394
-  _WRITEP2PENDPOINTI16RESPONSE._serialized_start=24396
-  _WRITEP2PENDPOINTI16RESPONSE._serialized_end=24441
-  _WRITESCRIPTREQUEST._serialized_start=24443
-  _WRITESCRIPTREQUEST._serialized_end=24537
-  _WRITESCRIPTRESPONSE._serialized_start=24539
-  _WRITESCRIPTRESPONSE._serialized_end=24576
-  _WRITEWAVEFORMREQUEST._serialized_start=24578
-  _WRITEWAVEFORMREQUEST._serialized_end=24697
-  _WRITEWAVEFORMRESPONSE._serialized_start=24699
-  _WRITEWAVEFORMRESPONSE._serialized_end=24738
-  _WRITEWAVEFORMCOMPLEXF64REQUEST._serialized_start=24741
-  _WRITEWAVEFORMCOMPLEXF64REQUEST._serialized_end=24902
-  _WRITEWAVEFORMCOMPLEXF64RESPONSE._serialized_start=24904
-  _WRITEWAVEFORMCOMPLEXF64RESPONSE._serialized_end=24953
-  _NIFGEN._serialized_start=51600
-  _NIFGEN._serialized_end=66007
+  _globals['_NIFGENATTRIBUTE']._serialized_start=24660
+  _globals['_NIFGENATTRIBUTE']._serialized_end=35325
+  _globals['_BYTEORDER']._serialized_start=35327
+  _globals['_BYTEORDER']._serialized_end=35417
+  _globals['_CLOCKMODE']._serialized_start=35420
+  _globals['_CLOCKMODE']._serialized_end=35550
+  _globals['_HARDWARESTATE']._serialized_start=35553
+  _globals['_HARDWARESTATE']._serialized_end=35785
+  _globals['_OUTPUTMODE']._serialized_start=35788
+  _globals['_OUTPUTMODE']._serialized_end=36005
+  _globals['_RELATIVETO']._serialized_start=36007
+  _globals['_RELATIVETO']._serialized_end=36125
+  _globals['_SIGNAL']._serialized_start=36128
+  _globals['_SIGNAL']._serialized_end=36672
+  _globals['_TRIGGER']._serialized_start=36674
+  _globals['_TRIGGER']._serialized_end=36786
+  _globals['_TRIGGERMODE']._serialized_start=36789
+  _globals['_TRIGGERMODE']._serialized_end=36980
+  _globals['_TRIGGERWHEN']._serialized_start=36982
+  _globals['_TRIGGERWHEN']._serialized_end=37106
+  _globals['_WAVEFORM']._serialized_start=37109
+  _globals['_WAVEFORM']._serialized_end=37430
+  _globals['_FREQUENCYLISTOPTIONS']._serialized_start=37432
+  _globals['_FREQUENCYLISTOPTIONS']._serialized_end=37553
+  _globals['_ROUTESIGNALFROM']._serialized_start=37556
+  _globals['_ROUTESIGNALFROM']._serialized_end=38461
+  _globals['_ROUTESIGNALTO']._serialized_start=38464
+  _globals['_ROUTESIGNALTO']._serialized_end=38993
+  _globals['_SEQUENCEHANDLE']._serialized_start=38995
+  _globals['_SEQUENCEHANDLE']._serialized_end=39099
+  _globals['_WAVEFORMHANDLE']._serialized_start=39101
+  _globals['_WAVEFORMHANDLE']._serialized_end=39205
+  _globals['_NIFGENINT32ATTRIBUTEVALUES']._serialized_start=39208
+  _globals['_NIFGENINT32ATTRIBUTEVALUES']._serialized_end=49641
+  _globals['_NIFGENREAL64ATTRIBUTEVALUES']._serialized_start=49644
+  _globals['_NIFGENREAL64ATTRIBUTEVALUES']._serialized_end=49939
+  _globals['_NIFGENSTRINGATTRIBUTEVALUESMAPPED']._serialized_start=49942
+  _globals['_NIFGENSTRINGATTRIBUTEVALUESMAPPED']._serialized_end=51301
+  _globals['_ABORTGENERATIONREQUEST']._serialized_start=60
+  _globals['_ABORTGENERATIONREQUEST']._serialized_end=120
+  _globals['_ABORTGENERATIONRESPONSE']._serialized_start=122
+  _globals['_ABORTGENERATIONRESPONSE']._serialized_end=163
+  _globals['_ADJUSTSAMPLECLOCKRELATIVEDELAYREQUEST']._serialized_start=165
+  _globals['_ADJUSTSAMPLECLOCKRELATIVEDELAYREQUEST']._serialized_end=265
+  _globals['_ADJUSTSAMPLECLOCKRELATIVEDELAYRESPONSE']._serialized_start=267
+  _globals['_ADJUSTSAMPLECLOCKRELATIVEDELAYRESPONSE']._serialized_end=323
+  _globals['_ALLOCATENAMEDWAVEFORMREQUEST']._serialized_start=326
+  _globals['_ALLOCATENAMEDWAVEFORMREQUEST']._serialized_end=460
+  _globals['_ALLOCATENAMEDWAVEFORMRESPONSE']._serialized_start=462
+  _globals['_ALLOCATENAMEDWAVEFORMRESPONSE']._serialized_end=509
+  _globals['_ALLOCATEWAVEFORMREQUEST']._serialized_start=511
+  _globals['_ALLOCATEWAVEFORMREQUEST']._serialized_end=617
+  _globals['_ALLOCATEWAVEFORMRESPONSE']._serialized_start=619
+  _globals['_ALLOCATEWAVEFORMRESPONSE']._serialized_end=686
+  _globals['_CHECKATTRIBUTEVIBOOLEANREQUEST']._serialized_start=689
+  _globals['_CHECKATTRIBUTEVIBOOLEANREQUEST']._serialized_end=856
+  _globals['_CHECKATTRIBUTEVIBOOLEANRESPONSE']._serialized_start=858
+  _globals['_CHECKATTRIBUTEVIBOOLEANRESPONSE']._serialized_end=907
+  _globals['_CHECKATTRIBUTEVIINT32REQUEST']._serialized_start=910
+  _globals['_CHECKATTRIBUTEVIINT32REQUEST']._serialized_end=1173
+  _globals['_CHECKATTRIBUTEVIINT32RESPONSE']._serialized_start=1175
+  _globals['_CHECKATTRIBUTEVIINT32RESPONSE']._serialized_end=1222
+  _globals['_CHECKATTRIBUTEVIINT64REQUEST']._serialized_start=1225
+  _globals['_CHECKATTRIBUTEVIINT64REQUEST']._serialized_end=1394
+  _globals['_CHECKATTRIBUTEVIINT64RESPONSE']._serialized_start=1396
+  _globals['_CHECKATTRIBUTEVIINT64RESPONSE']._serialized_end=1443
+  _globals['_CHECKATTRIBUTEVIREAL64REQUEST']._serialized_start=1446
+  _globals['_CHECKATTRIBUTEVIREAL64REQUEST']._serialized_end=1711
+  _globals['_CHECKATTRIBUTEVIREAL64RESPONSE']._serialized_start=1713
+  _globals['_CHECKATTRIBUTEVIREAL64RESPONSE']._serialized_end=1761
+  _globals['_CHECKATTRIBUTEVISESSIONREQUEST']._serialized_start=1764
+  _globals['_CHECKATTRIBUTEVISESSIONREQUEST']._serialized_end=1955
+  _globals['_CHECKATTRIBUTEVISESSIONRESPONSE']._serialized_start=1957
+  _globals['_CHECKATTRIBUTEVISESSIONRESPONSE']._serialized_end=2006
+  _globals['_CHECKATTRIBUTEVISTRINGREQUEST']._serialized_start=2009
+  _globals['_CHECKATTRIBUTEVISTRINGREQUEST']._serialized_end=2287
+  _globals['_CHECKATTRIBUTEVISTRINGRESPONSE']._serialized_start=2289
+  _globals['_CHECKATTRIBUTEVISTRINGRESPONSE']._serialized_end=2337
+  _globals['_CLEARARBMEMORYREQUEST']._serialized_start=2339
+  _globals['_CLEARARBMEMORYREQUEST']._serialized_end=2398
+  _globals['_CLEARARBMEMORYRESPONSE']._serialized_start=2400
+  _globals['_CLEARARBMEMORYRESPONSE']._serialized_end=2440
+  _globals['_CLEARARBSEQUENCEREQUEST']._serialized_start=2443
+  _globals['_CLEARARBSEQUENCEREQUEST']._serialized_end=2615
+  _globals['_CLEARARBSEQUENCERESPONSE']._serialized_start=2617
+  _globals['_CLEARARBSEQUENCERESPONSE']._serialized_end=2659
+  _globals['_CLEARARBWAVEFORMREQUEST']._serialized_start=2662
+  _globals['_CLEARARBWAVEFORMREQUEST']._serialized_end=2834
+  _globals['_CLEARARBWAVEFORMRESPONSE']._serialized_start=2836
+  _globals['_CLEARARBWAVEFORMRESPONSE']._serialized_end=2878
+  _globals['_CLEARERRORREQUEST']._serialized_start=2880
+  _globals['_CLEARERRORREQUEST']._serialized_end=2935
+  _globals['_CLEARERRORRESPONSE']._serialized_start=2937
+  _globals['_CLEARERRORRESPONSE']._serialized_end=2973
+  _globals['_CLEARFREQLISTREQUEST']._serialized_start=2976
+  _globals['_CLEARFREQLISTREQUEST']._serialized_end=3169
+  _globals['_CLEARFREQLISTRESPONSE']._serialized_start=3171
+  _globals['_CLEARFREQLISTRESPONSE']._serialized_end=3210
+  _globals['_CLEARINTERCHANGEWARNINGSREQUEST']._serialized_start=3212
+  _globals['_CLEARINTERCHANGEWARNINGSREQUEST']._serialized_end=3281
+  _globals['_CLEARINTERCHANGEWARNINGSRESPONSE']._serialized_start=3283
+  _globals['_CLEARINTERCHANGEWARNINGSRESPONSE']._serialized_end=3333
+  _globals['_CLEARUSERSTANDARDWAVEFORMREQUEST']._serialized_start=3335
+  _globals['_CLEARUSERSTANDARDWAVEFORMREQUEST']._serialized_end=3427
+  _globals['_CLEARUSERSTANDARDWAVEFORMRESPONSE']._serialized_start=3429
+  _globals['_CLEARUSERSTANDARDWAVEFORMRESPONSE']._serialized_end=3480
+  _globals['_CLOSEREQUEST']._serialized_start=3482
+  _globals['_CLOSEREQUEST']._serialized_end=3532
+  _globals['_CLOSERESPONSE']._serialized_start=3534
+  _globals['_CLOSERESPONSE']._serialized_end=3565
+  _globals['_COMMITREQUEST']._serialized_start=3567
+  _globals['_COMMITREQUEST']._serialized_end=3618
+  _globals['_COMMITRESPONSE']._serialized_start=3620
+  _globals['_COMMITRESPONSE']._serialized_end=3652
+  _globals['_CONFIGUREAMPLITUDEREQUEST']._serialized_start=3654
+  _globals['_CONFIGUREAMPLITUDEREQUEST']._serialized_end=3758
+  _globals['_CONFIGUREAMPLITUDERESPONSE']._serialized_start=3760
+  _globals['_CONFIGUREAMPLITUDERESPONSE']._serialized_end=3804
+  _globals['_CONFIGUREARBSEQUENCEREQUEST']._serialized_start=3807
+  _globals['_CONFIGUREARBSEQUENCEREQUEST']._serialized_end=3949
+  _globals['_CONFIGUREARBSEQUENCERESPONSE']._serialized_start=3951
+  _globals['_CONFIGUREARBSEQUENCERESPONSE']._serialized_end=3997
+  _globals['_CONFIGUREARBWAVEFORMREQUEST']._serialized_start=4000
+  _globals['_CONFIGUREARBWAVEFORMREQUEST']._serialized_end=4142
+  _globals['_CONFIGUREARBWAVEFORMRESPONSE']._serialized_start=4144
+  _globals['_CONFIGUREARBWAVEFORMRESPONSE']._serialized_end=4190
+  _globals['_CONFIGURECHANNELSREQUEST']._serialized_start=4192
+  _globals['_CONFIGURECHANNELSREQUEST']._serialized_end=4272
+  _globals['_CONFIGURECHANNELSRESPONSE']._serialized_start=4274
+  _globals['_CONFIGURECHANNELSRESPONSE']._serialized_end=4317
+  _globals['_CONFIGURECLOCKMODEREQUEST']._serialized_start=4320
+  _globals['_CONFIGURECLOCKMODEREQUEST']._serialized_end=4474
+  _globals['_CONFIGURECLOCKMODERESPONSE']._serialized_start=4476
+  _globals['_CONFIGURECLOCKMODERESPONSE']._serialized_end=4520
+  _globals['_CONFIGURECUSTOMFIRFILTERCOEFFICIENTSREQUEST']._serialized_start=4523
+  _globals['_CONFIGURECUSTOMFIRFILTERCOEFFICIENTSREQUEST']._serialized_end=4654
+  _globals['_CONFIGURECUSTOMFIRFILTERCOEFFICIENTSRESPONSE']._serialized_start=4656
+  _globals['_CONFIGURECUSTOMFIRFILTERCOEFFICIENTSRESPONSE']._serialized_end=4718
+  _globals['_CONFIGUREDIGITALEDGESCRIPTTRIGGERREQUEST']._serialized_start=4721
+  _globals['_CONFIGUREDIGITALEDGESCRIPTTRIGGERREQUEST']._serialized_end=4849
+  _globals['_CONFIGUREDIGITALEDGESCRIPTTRIGGERRESPONSE']._serialized_start=4851
+  _globals['_CONFIGUREDIGITALEDGESCRIPTTRIGGERRESPONSE']._serialized_end=4910
+  _globals['_CONFIGUREDIGITALEDGESTARTTRIGGERREQUEST']._serialized_start=4912
+  _globals['_CONFIGUREDIGITALEDGESTARTTRIGGERREQUEST']._serialized_end=5019
+  _globals['_CONFIGUREDIGITALEDGESTARTTRIGGERRESPONSE']._serialized_start=5021
+  _globals['_CONFIGUREDIGITALEDGESTARTTRIGGERRESPONSE']._serialized_end=5079
+  _globals['_CONFIGUREDIGITALLEVELSCRIPTTRIGGERREQUEST']._serialized_start=5082
+  _globals['_CONFIGUREDIGITALLEVELSCRIPTTRIGGERREQUEST']._serialized_end=5296
+  _globals['_CONFIGUREDIGITALLEVELSCRIPTTRIGGERRESPONSE']._serialized_start=5298
+  _globals['_CONFIGUREDIGITALLEVELSCRIPTTRIGGERRESPONSE']._serialized_end=5358
+  _globals['_CONFIGUREFREQLISTREQUEST']._serialized_start=5361
+  _globals['_CONFIGUREFREQLISTREQUEST']._serialized_end=5535
+  _globals['_CONFIGUREFREQLISTRESPONSE']._serialized_start=5537
+  _globals['_CONFIGUREFREQLISTRESPONSE']._serialized_end=5580
+  _globals['_CONFIGUREFREQUENCYREQUEST']._serialized_start=5582
+  _globals['_CONFIGUREFREQUENCYREQUEST']._serialized_end=5686
+  _globals['_CONFIGUREFREQUENCYRESPONSE']._serialized_start=5688
+  _globals['_CONFIGUREFREQUENCYRESPONSE']._serialized_end=5732
+  _globals['_CONFIGUREOPERATIONMODEREQUEST']._serialized_start=5734
+  _globals['_CONFIGUREOPERATIONMODEREQUEST']._serialized_end=5847
+  _globals['_CONFIGUREOPERATIONMODERESPONSE']._serialized_start=5849
+  _globals['_CONFIGUREOPERATIONMODERESPONSE']._serialized_end=5897
+  _globals['_CONFIGUREOUTPUTENABLEDREQUEST']._serialized_start=5899
+  _globals['_CONFIGUREOUTPUTENABLEDREQUEST']._serialized_end=6005
+  _globals['_CONFIGUREOUTPUTENABLEDRESPONSE']._serialized_start=6007
+  _globals['_CONFIGUREOUTPUTENABLEDRESPONSE']._serialized_end=6055
+  _globals['_CONFIGUREOUTPUTIMPEDANCEREQUEST']._serialized_start=6057
+  _globals['_CONFIGUREOUTPUTIMPEDANCEREQUEST']._serialized_end=6167
+  _globals['_CONFIGUREOUTPUTIMPEDANCERESPONSE']._serialized_start=6169
+  _globals['_CONFIGUREOUTPUTIMPEDANCERESPONSE']._serialized_end=6219
+  _globals['_CONFIGUREOUTPUTMODEREQUEST']._serialized_start=6222
+  _globals['_CONFIGUREOUTPUTMODEREQUEST']._serialized_end=6381
+  _globals['_CONFIGUREOUTPUTMODERESPONSE']._serialized_start=6383
+  _globals['_CONFIGUREOUTPUTMODERESPONSE']._serialized_end=6428
+  _globals['_CONFIGUREP2PENDPOINTFULLNESSSTARTTRIGGERREQUEST']._serialized_start=6430
+  _globals['_CONFIGUREP2PENDPOINTFULLNESSSTARTTRIGGERREQUEST']._serialized_end=6552
+  _globals['_CONFIGUREP2PENDPOINTFULLNESSSTARTTRIGGERRESPONSE']._serialized_start=6554
+  _globals['_CONFIGUREP2PENDPOINTFULLNESSSTARTTRIGGERRESPONSE']._serialized_end=6620
+  _globals['_CONFIGUREREFERENCECLOCKREQUEST']._serialized_start=6623
+  _globals['_CONFIGUREREFERENCECLOCKREQUEST']._serialized_end=6758
+  _globals['_CONFIGUREREFERENCECLOCKRESPONSE']._serialized_start=6760
+  _globals['_CONFIGUREREFERENCECLOCKRESPONSE']._serialized_end=6809
+  _globals['_CONFIGURESAMPLECLOCKSOURCEREQUEST']._serialized_start=6811
+  _globals['_CONFIGURESAMPLECLOCKSOURCEREQUEST']._serialized_end=6911
+  _globals['_CONFIGURESAMPLECLOCKSOURCERESPONSE']._serialized_start=6913
+  _globals['_CONFIGURESAMPLECLOCKSOURCERESPONSE']._serialized_end=6965
+  _globals['_CONFIGURESAMPLERATEREQUEST']._serialized_start=6967
+  _globals['_CONFIGURESAMPLERATEREQUEST']._serialized_end=7052
+  _globals['_CONFIGURESAMPLERATERESPONSE']._serialized_start=7054
+  _globals['_CONFIGURESAMPLERATERESPONSE']._serialized_end=7099
+  _globals['_CONFIGURESOFTWAREEDGESCRIPTTRIGGERREQUEST']._serialized_start=7101
+  _globals['_CONFIGURESOFTWAREEDGESCRIPTTRIGGERREQUEST']._serialized_end=7200
+  _globals['_CONFIGURESOFTWAREEDGESCRIPTTRIGGERRESPONSE']._serialized_start=7202
+  _globals['_CONFIGURESOFTWAREEDGESCRIPTTRIGGERRESPONSE']._serialized_end=7262
+  _globals['_CONFIGURESOFTWAREEDGESTARTTRIGGERREQUEST']._serialized_start=7264
+  _globals['_CONFIGURESOFTWAREEDGESTARTTRIGGERREQUEST']._serialized_end=7342
+  _globals['_CONFIGURESOFTWAREEDGESTARTTRIGGERRESPONSE']._serialized_start=7344
+  _globals['_CONFIGURESOFTWAREEDGESTARTTRIGGERRESPONSE']._serialized_end=7403
+  _globals['_CONFIGURESTANDARDWAVEFORMREQUEST']._serialized_start=7406
+  _globals['_CONFIGURESTANDARDWAVEFORMREQUEST']._serialized_end=7660
+  _globals['_CONFIGURESTANDARDWAVEFORMRESPONSE']._serialized_start=7662
+  _globals['_CONFIGURESTANDARDWAVEFORMRESPONSE']._serialized_end=7713
+  _globals['_CONFIGURESYNCHRONIZATIONREQUEST']._serialized_start=7715
+  _globals['_CONFIGURESYNCHRONIZATIONREQUEST']._serialized_end=7838
+  _globals['_CONFIGURESYNCHRONIZATIONRESPONSE']._serialized_start=7840
+  _globals['_CONFIGURESYNCHRONIZATIONRESPONSE']._serialized_end=7890
+  _globals['_CONFIGURETRIGGERMODEREQUEST']._serialized_start=7893
+  _globals['_CONFIGURETRIGGERMODEREQUEST']._serialized_end=8079
+  _globals['_CONFIGURETRIGGERMODERESPONSE']._serialized_start=8081
+  _globals['_CONFIGURETRIGGERMODERESPONSE']._serialized_end=8127
+  _globals['_CREATEADVANCEDARBSEQUENCEREQUEST']._serialized_start=8130
+  _globals['_CREATEADVANCEDARBSEQUENCEREQUEST']._serialized_end=8319
+  _globals['_CREATEADVANCEDARBSEQUENCERESPONSE']._serialized_start=8321
+  _globals['_CREATEADVANCEDARBSEQUENCERESPONSE']._serialized_end=8428
+  _globals['_CREATEARBSEQUENCEREQUEST']._serialized_start=8430
+  _globals['_CREATEARBSEQUENCEREQUEST']._serialized_end=8551
+  _globals['_CREATEARBSEQUENCERESPONSE']._serialized_start=8553
+  _globals['_CREATEARBSEQUENCERESPONSE']._serialized_end=8621
+  _globals['_CREATEFREQLISTREQUEST']._serialized_start=8624
+  _globals['_CREATEFREQLISTREQUEST']._serialized_end=8816
+  _globals['_CREATEFREQLISTRESPONSE']._serialized_start=8818
+  _globals['_CREATEFREQLISTRESPONSE']._serialized_end=8889
+  _globals['_CREATEWAVEFORMCOMPLEXF64REQUEST']._serialized_start=8892
+  _globals['_CREATEWAVEFORMCOMPLEXF64REQUEST']._serialized_end=9044
+  _globals['_CREATEWAVEFORMCOMPLEXF64RESPONSE']._serialized_start=9046
+  _globals['_CREATEWAVEFORMCOMPLEXF64RESPONSE']._serialized_end=9121
+  _globals['_CREATEWAVEFORMF64REQUEST']._serialized_start=9123
+  _globals['_CREATEWAVEFORMF64REQUEST']._serialized_end=9236
+  _globals['_CREATEWAVEFORMF64RESPONSE']._serialized_start=9238
+  _globals['_CREATEWAVEFORMF64RESPONSE']._serialized_end=9306
+  _globals['_CREATEWAVEFORMFROMFILEF64REQUEST']._serialized_start=9309
+  _globals['_CREATEWAVEFORMFROMFILEF64REQUEST']._serialized_end=9511
+  _globals['_CREATEWAVEFORMFROMFILEF64RESPONSE']._serialized_start=9513
+  _globals['_CREATEWAVEFORMFROMFILEF64RESPONSE']._serialized_end=9589
+  _globals['_CREATEWAVEFORMFROMFILEI16REQUEST']._serialized_start=9592
+  _globals['_CREATEWAVEFORMFROMFILEI16REQUEST']._serialized_end=9794
+  _globals['_CREATEWAVEFORMFROMFILEI16RESPONSE']._serialized_start=9796
+  _globals['_CREATEWAVEFORMFROMFILEI16RESPONSE']._serialized_end=9872
+  _globals['_CREATEWAVEFORMI16REQUEST']._serialized_start=9874
+  _globals['_CREATEWAVEFORMI16REQUEST']._serialized_end=9987
+  _globals['_CREATEWAVEFORMI16RESPONSE']._serialized_start=9989
+  _globals['_CREATEWAVEFORMI16RESPONSE']._serialized_end=10057
+  _globals['_DEFINEUSERSTANDARDWAVEFORMREQUEST']._serialized_start=10059
+  _globals['_DEFINEUSERSTANDARDWAVEFORMREQUEST']._serialized_end=10181
+  _globals['_DEFINEUSERSTANDARDWAVEFORMRESPONSE']._serialized_start=10183
+  _globals['_DEFINEUSERSTANDARDWAVEFORMRESPONSE']._serialized_end=10235
+  _globals['_DELETENAMEDWAVEFORMREQUEST']._serialized_start=10237
+  _globals['_DELETENAMEDWAVEFORMREQUEST']._serialized_end=10346
+  _globals['_DELETENAMEDWAVEFORMRESPONSE']._serialized_start=10348
+  _globals['_DELETENAMEDWAVEFORMRESPONSE']._serialized_end=10393
+  _globals['_DELETESCRIPTREQUEST']._serialized_start=10395
+  _globals['_DELETESCRIPTREQUEST']._serialized_end=10495
+  _globals['_DELETESCRIPTRESPONSE']._serialized_start=10497
+  _globals['_DELETESCRIPTRESPONSE']._serialized_end=10535
+  _globals['_DISABLEREQUEST']._serialized_start=10537
+  _globals['_DISABLEREQUEST']._serialized_end=10589
+  _globals['_DISABLERESPONSE']._serialized_start=10591
+  _globals['_DISABLERESPONSE']._serialized_end=10624
+  _globals['_DISABLEANALOGFILTERREQUEST']._serialized_start=10626
+  _globals['_DISABLEANALOGFILTERREQUEST']._serialized_end=10712
+  _globals['_DISABLEANALOGFILTERRESPONSE']._serialized_start=10714
+  _globals['_DISABLEANALOGFILTERRESPONSE']._serialized_end=10759
+  _globals['_DISABLEDIGITALFILTERREQUEST']._serialized_start=10761
+  _globals['_DISABLEDIGITALFILTERREQUEST']._serialized_end=10848
+  _globals['_DISABLEDIGITALFILTERRESPONSE']._serialized_start=10850
+  _globals['_DISABLEDIGITALFILTERRESPONSE']._serialized_end=10896
+  _globals['_DISABLEDIGITALPATTERNINGREQUEST']._serialized_start=10898
+  _globals['_DISABLEDIGITALPATTERNINGREQUEST']._serialized_end=10989
+  _globals['_DISABLEDIGITALPATTERNINGRESPONSE']._serialized_start=10991
+  _globals['_DISABLEDIGITALPATTERNINGRESPONSE']._serialized_end=11041
+  _globals['_DISABLESCRIPTTRIGGERREQUEST']._serialized_start=11043
+  _globals['_DISABLESCRIPTTRIGGERREQUEST']._serialized_end=11128
+  _globals['_DISABLESCRIPTTRIGGERRESPONSE']._serialized_start=11130
+  _globals['_DISABLESCRIPTTRIGGERRESPONSE']._serialized_end=11176
+  _globals['_DISABLESTARTTRIGGERREQUEST']._serialized_start=11178
+  _globals['_DISABLESTARTTRIGGERREQUEST']._serialized_end=11242
+  _globals['_DISABLESTARTTRIGGERRESPONSE']._serialized_start=11244
+  _globals['_DISABLESTARTTRIGGERRESPONSE']._serialized_end=11289
+  _globals['_ENABLEANALOGFILTERREQUEST']._serialized_start=11291
+  _globals['_ENABLEANALOGFILTERREQUEST']._serialized_end=11413
+  _globals['_ENABLEANALOGFILTERRESPONSE']._serialized_start=11415
+  _globals['_ENABLEANALOGFILTERRESPONSE']._serialized_end=11459
+  _globals['_ENABLEDIGITALFILTERREQUEST']._serialized_start=11461
+  _globals['_ENABLEDIGITALFILTERREQUEST']._serialized_end=11547
+  _globals['_ENABLEDIGITALFILTERRESPONSE']._serialized_start=11549
+  _globals['_ENABLEDIGITALFILTERRESPONSE']._serialized_end=11594
+  _globals['_ENABLEDIGITALPATTERNINGREQUEST']._serialized_start=11596
+  _globals['_ENABLEDIGITALPATTERNINGREQUEST']._serialized_end=11686
+  _globals['_ENABLEDIGITALPATTERNINGRESPONSE']._serialized_start=11688
+  _globals['_ENABLEDIGITALPATTERNINGRESPONSE']._serialized_end=11737
+  _globals['_ERRORHANDLERREQUEST']._serialized_start=11739
+  _globals['_ERRORHANDLERREQUEST']._serialized_end=11816
+  _globals['_ERRORHANDLERRESPONSE']._serialized_start=11818
+  _globals['_ERRORHANDLERRESPONSE']._serialized_end=11879
+  _globals['_ERRORMESSAGEREQUEST']._serialized_start=11881
+  _globals['_ERRORMESSAGEREQUEST']._serialized_end=11958
+  _globals['_ERRORMESSAGERESPONSE']._serialized_start=11960
+  _globals['_ERRORMESSAGERESPONSE']._serialized_end=12021
+  _globals['_ERRORQUERYREQUEST']._serialized_start=12023
+  _globals['_ERRORQUERYREQUEST']._serialized_end=12078
+  _globals['_ERRORQUERYRESPONSE']._serialized_start=12080
+  _globals['_ERRORQUERYRESPONSE']._serialized_end=12159
+  _globals['_EXPORTATTRIBUTECONFIGURATIONBUFFERREQUEST']._serialized_start=12161
+  _globals['_EXPORTATTRIBUTECONFIGURATIONBUFFERREQUEST']._serialized_end=12240
+  _globals['_EXPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE']._serialized_start=12242
+  _globals['_EXPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE']._serialized_end=12325
+  _globals['_EXPORTATTRIBUTECONFIGURATIONFILEREQUEST']._serialized_start=12327
+  _globals['_EXPORTATTRIBUTECONFIGURATIONFILEREQUEST']._serialized_end=12423
+  _globals['_EXPORTATTRIBUTECONFIGURATIONFILERESPONSE']._serialized_start=12425
+  _globals['_EXPORTATTRIBUTECONFIGURATIONFILERESPONSE']._serialized_end=12483
+  _globals['_EXPORTSIGNALREQUEST']._serialized_start=12486
+  _globals['_EXPORTSIGNALREQUEST']._serialized_end=12671
+  _globals['_EXPORTSIGNALRESPONSE']._serialized_start=12673
+  _globals['_EXPORTSIGNALRESPONSE']._serialized_end=12711
+  _globals['_GETATTRIBUTEVIBOOLEANREQUEST']._serialized_start=12714
+  _globals['_GETATTRIBUTEVIBOOLEANREQUEST']._serialized_end=12854
+  _globals['_GETATTRIBUTEVIBOOLEANRESPONSE']._serialized_start=12856
+  _globals['_GETATTRIBUTEVIBOOLEANRESPONSE']._serialized_end=12928
+  _globals['_GETATTRIBUTEVIINT32REQUEST']._serialized_start=12931
+  _globals['_GETATTRIBUTEVIINT32REQUEST']._serialized_end=13069
+  _globals['_GETATTRIBUTEVIINT32RESPONSE']._serialized_start=13071
+  _globals['_GETATTRIBUTEVIINT32RESPONSE']._serialized_end=13141
+  _globals['_GETATTRIBUTEVIINT64REQUEST']._serialized_start=13144
+  _globals['_GETATTRIBUTEVIINT64REQUEST']._serialized_end=13282
+  _globals['_GETATTRIBUTEVIINT64RESPONSE']._serialized_start=13284
+  _globals['_GETATTRIBUTEVIINT64RESPONSE']._serialized_end=13354
+  _globals['_GETATTRIBUTEVIREAL64REQUEST']._serialized_start=13357
+  _globals['_GETATTRIBUTEVIREAL64REQUEST']._serialized_end=13496
+  _globals['_GETATTRIBUTEVIREAL64RESPONSE']._serialized_start=13498
+  _globals['_GETATTRIBUTEVIREAL64RESPONSE']._serialized_end=13569
+  _globals['_GETATTRIBUTEVISESSIONREQUEST']._serialized_start=13572
+  _globals['_GETATTRIBUTEVISESSIONREQUEST']._serialized_end=13712
+  _globals['_GETATTRIBUTEVISESSIONRESPONSE']._serialized_start=13714
+  _globals['_GETATTRIBUTEVISESSIONRESPONSE']._serialized_end=13810
+  _globals['_GETATTRIBUTEVISTRINGREQUEST']._serialized_start=13813
+  _globals['_GETATTRIBUTEVISTRINGREQUEST']._serialized_end=13952
+  _globals['_GETATTRIBUTEVISTRINGRESPONSE']._serialized_start=13954
+  _globals['_GETATTRIBUTEVISTRINGRESPONSE']._serialized_end=14025
+  _globals['_GETCHANNELNAMEREQUEST']._serialized_start=14027
+  _globals['_GETCHANNELNAMEREQUEST']._serialized_end=14101
+  _globals['_GETCHANNELNAMERESPONSE']._serialized_start=14103
+  _globals['_GETCHANNELNAMERESPONSE']._serialized_end=14167
+  _globals['_GETERRORREQUEST']._serialized_start=14169
+  _globals['_GETERRORREQUEST']._serialized_end=14222
+  _globals['_GETERRORRESPONSE']._serialized_start=14224
+  _globals['_GETERRORRESPONSE']._serialized_end=14305
+  _globals['_GETEXTCALLASTDATEANDTIMEREQUEST']._serialized_start=14307
+  _globals['_GETEXTCALLASTDATEANDTIMEREQUEST']._serialized_end=14376
+  _globals['_GETEXTCALLASTDATEANDTIMERESPONSE']._serialized_start=14378
+  _globals['_GETEXTCALLASTDATEANDTIMERESPONSE']._serialized_end=14500
+  _globals['_GETEXTCALLASTTEMPREQUEST']._serialized_start=14502
+  _globals['_GETEXTCALLASTTEMPREQUEST']._serialized_end=14564
+  _globals['_GETEXTCALLASTTEMPRESPONSE']._serialized_start=14566
+  _globals['_GETEXTCALLASTTEMPRESPONSE']._serialized_end=14630
+  _globals['_GETEXTCALRECOMMENDEDINTERVALREQUEST']._serialized_start=14632
+  _globals['_GETEXTCALRECOMMENDEDINTERVALREQUEST']._serialized_end=14705
+  _globals['_GETEXTCALRECOMMENDEDINTERVALRESPONSE']._serialized_start=14707
+  _globals['_GETEXTCALRECOMMENDEDINTERVALRESPONSE']._serialized_end=14777
+  _globals['_GETFIRFILTERCOEFFICIENTSREQUEST']._serialized_start=14779
+  _globals['_GETFIRFILTERCOEFFICIENTSREQUEST']._serialized_end=14870
+  _globals['_GETFIRFILTERCOEFFICIENTSRESPONSE']._serialized_start=14872
+  _globals['_GETFIRFILTERCOEFFICIENTSRESPONSE']._serialized_end=14987
+  _globals['_GETHARDWARESTATEREQUEST']._serialized_start=14989
+  _globals['_GETHARDWARESTATEREQUEST']._serialized_end=15050
+  _globals['_GETHARDWARESTATERESPONSE']._serialized_start=15052
+  _globals['_GETHARDWARESTATERESPONSE']._serialized_end=15156
+  _globals['_GETSELFCALLASTDATEANDTIMEREQUEST']._serialized_start=15158
+  _globals['_GETSELFCALLASTDATEANDTIMEREQUEST']._serialized_end=15228
+  _globals['_GETSELFCALLASTDATEANDTIMERESPONSE']._serialized_start=15230
+  _globals['_GETSELFCALLASTDATEANDTIMERESPONSE']._serialized_end=15353
+  _globals['_GETSELFCALLASTTEMPREQUEST']._serialized_start=15355
+  _globals['_GETSELFCALLASTTEMPREQUEST']._serialized_end=15418
+  _globals['_GETSELFCALLASTTEMPRESPONSE']._serialized_start=15420
+  _globals['_GETSELFCALLASTTEMPRESPONSE']._serialized_end=15485
+  _globals['_GETSELFCALSUPPORTEDREQUEST']._serialized_start=15487
+  _globals['_GETSELFCALSUPPORTEDREQUEST']._serialized_end=15551
+  _globals['_GETSELFCALSUPPORTEDRESPONSE']._serialized_start=15553
+  _globals['_GETSELFCALSUPPORTEDRESPONSE']._serialized_end=15626
+  _globals['_GETSTREAMENDPOINTHANDLEREQUEST']._serialized_start=15628
+  _globals['_GETSTREAMENDPOINTHANDLEREQUEST']._serialized_end=15721
+  _globals['_GETSTREAMENDPOINTHANDLERESPONSE']._serialized_start=15723
+  _globals['_GETSTREAMENDPOINTHANDLERESPONSE']._serialized_end=15795
+  _globals['_IMPORTATTRIBUTECONFIGURATIONBUFFERREQUEST']._serialized_start=15797
+  _globals['_IMPORTATTRIBUTECONFIGURATIONBUFFERREQUEST']._serialized_end=15899
+  _globals['_IMPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE']._serialized_start=15901
+  _globals['_IMPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE']._serialized_end=15961
+  _globals['_IMPORTATTRIBUTECONFIGURATIONFILEREQUEST']._serialized_start=15963
+  _globals['_IMPORTATTRIBUTECONFIGURATIONFILEREQUEST']._serialized_end=16059
+  _globals['_IMPORTATTRIBUTECONFIGURATIONFILERESPONSE']._serialized_start=16061
+  _globals['_IMPORTATTRIBUTECONFIGURATIONFILERESPONSE']._serialized_end=16119
+  _globals['_INITREQUEST']._serialized_start=16122
+  _globals['_INITREQUEST']._serialized_end=16299
+  _globals['_INITRESPONSE']._serialized_start=16301
+  _globals['_INITRESPONSE']._serialized_end=16427
+  _globals['_INITWITHOPTIONSREQUEST']._serialized_start=16430
+  _globals['_INITWITHOPTIONSREQUEST']._serialized_end=16641
+  _globals['_INITWITHOPTIONSRESPONSE']._serialized_start=16644
+  _globals['_INITWITHOPTIONSRESPONSE']._serialized_end=16781
+  _globals['_INITIALIZEWITHCHANNELSREQUEST']._serialized_start=16784
+  _globals['_INITIALIZEWITHCHANNELSREQUEST']._serialized_end=17006
+  _globals['_INITIALIZEWITHCHANNELSRESPONSE']._serialized_start=17009
+  _globals['_INITIALIZEWITHCHANNELSRESPONSE']._serialized_end=17153
+  _globals['_INITIATEGENERATIONREQUEST']._serialized_start=17155
+  _globals['_INITIATEGENERATIONREQUEST']._serialized_end=17218
+  _globals['_INITIATEGENERATIONRESPONSE']._serialized_start=17220
+  _globals['_INITIATEGENERATIONRESPONSE']._serialized_end=17264
+  _globals['_INVALIDATEALLATTRIBUTESREQUEST']._serialized_start=17266
+  _globals['_INVALIDATEALLATTRIBUTESREQUEST']._serialized_end=17334
+  _globals['_INVALIDATEALLATTRIBUTESRESPONSE']._serialized_start=17336
+  _globals['_INVALIDATEALLATTRIBUTESRESPONSE']._serialized_end=17385
+  _globals['_ISDONEREQUEST']._serialized_start=17387
+  _globals['_ISDONEREQUEST']._serialized_end=17438
+  _globals['_ISDONERESPONSE']._serialized_start=17440
+  _globals['_ISDONERESPONSE']._serialized_end=17486
+  _globals['_QUERYARBSEQCAPABILITIESREQUEST']._serialized_start=17488
+  _globals['_QUERYARBSEQCAPABILITIESREQUEST']._serialized_end=17556
+  _globals['_QUERYARBSEQCAPABILITIESRESPONSE']._serialized_start=17559
+  _globals['_QUERYARBSEQCAPABILITIESRESPONSE']._serialized_end=17739
+  _globals['_QUERYARBWFMCAPABILITIESREQUEST']._serialized_start=17741
+  _globals['_QUERYARBWFMCAPABILITIESREQUEST']._serialized_end=17809
+  _globals['_QUERYARBWFMCAPABILITIESRESPONSE']._serialized_start=17812
+  _globals['_QUERYARBWFMCAPABILITIESRESPONSE']._serialized_end=17986
+  _globals['_QUERYFREQLISTCAPABILITIESREQUEST']._serialized_start=17988
+  _globals['_QUERYFREQLISTCAPABILITIESREQUEST']._serialized_end=18058
+  _globals['_QUERYFREQLISTCAPABILITIESRESPONSE']._serialized_start=18061
+  _globals['_QUERYFREQLISTCAPABILITIESRESPONSE']._serialized_end=18351
+  _globals['_READCURRENTTEMPERATUREREQUEST']._serialized_start=18353
+  _globals['_READCURRENTTEMPERATUREREQUEST']._serialized_end=18420
+  _globals['_READCURRENTTEMPERATURERESPONSE']._serialized_start=18422
+  _globals['_READCURRENTTEMPERATURERESPONSE']._serialized_end=18491
+  _globals['_RESETREQUEST']._serialized_start=18493
+  _globals['_RESETREQUEST']._serialized_end=18543
+  _globals['_RESETRESPONSE']._serialized_start=18545
+  _globals['_RESETRESPONSE']._serialized_end=18576
+  _globals['_RESETATTRIBUTEREQUEST']._serialized_start=18579
+  _globals['_RESETATTRIBUTEREQUEST']._serialized_end=18712
+  _globals['_RESETATTRIBUTERESPONSE']._serialized_start=18714
+  _globals['_RESETATTRIBUTERESPONSE']._serialized_end=18754
+  _globals['_RESETDEVICEREQUEST']._serialized_start=18756
+  _globals['_RESETDEVICEREQUEST']._serialized_end=18812
+  _globals['_RESETDEVICERESPONSE']._serialized_start=18814
+  _globals['_RESETDEVICERESPONSE']._serialized_end=18851
+  _globals['_RESETINTERCHANGECHECKREQUEST']._serialized_start=18853
+  _globals['_RESETINTERCHANGECHECKREQUEST']._serialized_end=18919
+  _globals['_RESETINTERCHANGECHECKRESPONSE']._serialized_start=18921
+  _globals['_RESETINTERCHANGECHECKRESPONSE']._serialized_end=18968
+  _globals['_RESETWITHDEFAULTSREQUEST']._serialized_start=18970
+  _globals['_RESETWITHDEFAULTSREQUEST']._serialized_end=19032
+  _globals['_RESETWITHDEFAULTSRESPONSE']._serialized_start=19034
+  _globals['_RESETWITHDEFAULTSRESPONSE']._serialized_end=19077
+  _globals['_REVISIONQUERYREQUEST']._serialized_start=19079
+  _globals['_REVISIONQUERYREQUEST']._serialized_end=19137
+  _globals['_REVISIONQUERYRESPONSE']._serialized_start=19139
+  _globals['_REVISIONQUERYRESPONSE']._serialized_end=19241
+  _globals['_ROUTESIGNALOUTREQUEST']._serialized_start=19244
+  _globals['_ROUTESIGNALOUTREQUEST']._serialized_end=19553
+  _globals['_ROUTESIGNALOUTRESPONSE']._serialized_start=19555
+  _globals['_ROUTESIGNALOUTRESPONSE']._serialized_end=19595
+  _globals['_SELFCALREQUEST']._serialized_start=19597
+  _globals['_SELFCALREQUEST']._serialized_end=19649
+  _globals['_SELFCALRESPONSE']._serialized_start=19651
+  _globals['_SELFCALRESPONSE']._serialized_end=19684
+  _globals['_SELFTESTREQUEST']._serialized_start=19686
+  _globals['_SELFTESTREQUEST']._serialized_end=19739
+  _globals['_SELFTESTRESPONSE']._serialized_start=19741
+  _globals['_SELFTESTRESPONSE']._serialized_end=19828
+  _globals['_SENDSOFTWAREEDGETRIGGERREQUEST']._serialized_start=19831
+  _globals['_SENDSOFTWAREEDGETRIGGERREQUEST']._serialized_end=19999
+  _globals['_SENDSOFTWAREEDGETRIGGERRESPONSE']._serialized_start=20001
+  _globals['_SENDSOFTWAREEDGETRIGGERRESPONSE']._serialized_end=20050
+  _globals['_SETATTRIBUTEVIBOOLEANREQUEST']._serialized_start=20053
+  _globals['_SETATTRIBUTEVIBOOLEANREQUEST']._serialized_end=20218
+  _globals['_SETATTRIBUTEVIBOOLEANRESPONSE']._serialized_start=20220
+  _globals['_SETATTRIBUTEVIBOOLEANRESPONSE']._serialized_end=20267
+  _globals['_SETATTRIBUTEVIINT32REQUEST']._serialized_start=20270
+  _globals['_SETATTRIBUTEVIINT32REQUEST']._serialized_end=20531
+  _globals['_SETATTRIBUTEVIINT32RESPONSE']._serialized_start=20533
+  _globals['_SETATTRIBUTEVIINT32RESPONSE']._serialized_end=20578
+  _globals['_SETATTRIBUTEVIINT64REQUEST']._serialized_start=20581
+  _globals['_SETATTRIBUTEVIINT64REQUEST']._serialized_end=20748
+  _globals['_SETATTRIBUTEVIINT64RESPONSE']._serialized_start=20750
+  _globals['_SETATTRIBUTEVIINT64RESPONSE']._serialized_end=20795
+  _globals['_SETATTRIBUTEVIREAL64REQUEST']._serialized_start=20798
+  _globals['_SETATTRIBUTEVIREAL64REQUEST']._serialized_end=21061
+  _globals['_SETATTRIBUTEVIREAL64RESPONSE']._serialized_start=21063
+  _globals['_SETATTRIBUTEVIREAL64RESPONSE']._serialized_end=21109
+  _globals['_SETATTRIBUTEVISESSIONREQUEST']._serialized_start=21112
+  _globals['_SETATTRIBUTEVISESSIONREQUEST']._serialized_end=21301
+  _globals['_SETATTRIBUTEVISESSIONRESPONSE']._serialized_start=21303
+  _globals['_SETATTRIBUTEVISESSIONRESPONSE']._serialized_end=21350
+  _globals['_SETATTRIBUTEVISTRINGREQUEST']._serialized_start=21353
+  _globals['_SETATTRIBUTEVISTRINGREQUEST']._serialized_end=21629
+  _globals['_SETATTRIBUTEVISTRINGRESPONSE']._serialized_start=21631
+  _globals['_SETATTRIBUTEVISTRINGRESPONSE']._serialized_end=21677
+  _globals['_SETNAMEDWAVEFORMNEXTWRITEPOSITIONREQUEST']._serialized_start=21680
+  _globals['_SETNAMEDWAVEFORMNEXTWRITEPOSITIONREQUEST']._serialized_end=21914
+  _globals['_SETNAMEDWAVEFORMNEXTWRITEPOSITIONRESPONSE']._serialized_start=21916
+  _globals['_SETNAMEDWAVEFORMNEXTWRITEPOSITIONRESPONSE']._serialized_end=21975
+  _globals['_SETWAVEFORMNEXTWRITEPOSITIONREQUEST']._serialized_start=21978
+  _globals['_SETWAVEFORMNEXTWRITEPOSITIONREQUEST']._serialized_end=22209
+  _globals['_SETWAVEFORMNEXTWRITEPOSITIONRESPONSE']._serialized_start=22211
+  _globals['_SETWAVEFORMNEXTWRITEPOSITIONRESPONSE']._serialized_end=22265
+  _globals['_WAITUNTILDONEREQUEST']._serialized_start=22267
+  _globals['_WAITUNTILDONEREQUEST']._serialized_end=22343
+  _globals['_WAITUNTILDONERESPONSE']._serialized_start=22345
+  _globals['_WAITUNTILDONERESPONSE']._serialized_end=22384
+  _globals['_WRITEBINARY16WAVEFORMREQUEST']._serialized_start=22386
+  _globals['_WRITEBINARY16WAVEFORMREQUEST']._serialized_end=22513
+  _globals['_WRITEBINARY16WAVEFORMRESPONSE']._serialized_start=22515
+  _globals['_WRITEBINARY16WAVEFORMRESPONSE']._serialized_end=22562
+  _globals['_WRITECOMPLEXBINARY16WAVEFORMREQUEST']._serialized_start=22565
+  _globals['_WRITECOMPLEXBINARY16WAVEFORMREQUEST']._serialized_end=22728
+  _globals['_WRITECOMPLEXBINARY16WAVEFORMRESPONSE']._serialized_start=22730
+  _globals['_WRITECOMPLEXBINARY16WAVEFORMRESPONSE']._serialized_end=22784
+  _globals['_WRITENAMEDWAVEFORMCOMPLEXF64REQUEST']._serialized_start=22787
+  _globals['_WRITENAMEDWAVEFORMCOMPLEXF64REQUEST']._serialized_end=22951
+  _globals['_WRITENAMEDWAVEFORMCOMPLEXF64RESPONSE']._serialized_start=22953
+  _globals['_WRITENAMEDWAVEFORMCOMPLEXF64RESPONSE']._serialized_end=23007
+  _globals['_WRITENAMEDWAVEFORMCOMPLEXI16REQUEST']._serialized_start=23010
+  _globals['_WRITENAMEDWAVEFORMCOMPLEXI16REQUEST']._serialized_end=23171
+  _globals['_WRITENAMEDWAVEFORMCOMPLEXI16RESPONSE']._serialized_start=23173
+  _globals['_WRITENAMEDWAVEFORMCOMPLEXI16RESPONSE']._serialized_end=23227
+  _globals['_WRITENAMEDWAVEFORMF64REQUEST']._serialized_start=23229
+  _globals['_WRITENAMEDWAVEFORMF64REQUEST']._serialized_end=23354
+  _globals['_WRITENAMEDWAVEFORMF64RESPONSE']._serialized_start=23356
+  _globals['_WRITENAMEDWAVEFORMF64RESPONSE']._serialized_end=23403
+  _globals['_WRITENAMEDWAVEFORMI16REQUEST']._serialized_start=23405
+  _globals['_WRITENAMEDWAVEFORMI16REQUEST']._serialized_end=23530
+  _globals['_WRITENAMEDWAVEFORMI16RESPONSE']._serialized_start=23532
+  _globals['_WRITENAMEDWAVEFORMI16RESPONSE']._serialized_end=23579
+  _globals['_WRITEP2PENDPOINTI16REQUEST']._serialized_start=23581
+  _globals['_WRITEP2PENDPOINTI16REQUEST']._serialized_end=23691
+  _globals['_WRITEP2PENDPOINTI16RESPONSE']._serialized_start=23693
+  _globals['_WRITEP2PENDPOINTI16RESPONSE']._serialized_end=23738
+  _globals['_WRITESCRIPTREQUEST']._serialized_start=23740
+  _globals['_WRITESCRIPTREQUEST']._serialized_end=23834
+  _globals['_WRITESCRIPTRESPONSE']._serialized_start=23836
+  _globals['_WRITESCRIPTRESPONSE']._serialized_end=23873
+  _globals['_WRITEWAVEFORMREQUEST']._serialized_start=23875
+  _globals['_WRITEWAVEFORMREQUEST']._serialized_end=23994
+  _globals['_WRITEWAVEFORMRESPONSE']._serialized_start=23996
+  _globals['_WRITEWAVEFORMRESPONSE']._serialized_end=24035
+  _globals['_WRITEWAVEFORMCOMPLEXF64REQUEST']._serialized_start=24038
+  _globals['_WRITEWAVEFORMCOMPLEXF64REQUEST']._serialized_end=24199
+  _globals['_WRITEWAVEFORMCOMPLEXF64RESPONSE']._serialized_start=24201
+  _globals['_WRITEWAVEFORMCOMPLEXF64RESPONSE']._serialized_end=24250
+  _globals['_CREATEWAVEFORMFROMFILEHWSREQUEST']._serialized_start=24253
+  _globals['_CREATEWAVEFORMFROMFILEHWSREQUEST']._serialized_end=24439
+  _globals['_CREATEWAVEFORMFROMFILEHWSRESPONSE']._serialized_start=24441
+  _globals['_CREATEWAVEFORMFROMFILEHWSRESPONSE']._serialized_end=24517
+  _globals['_MANUALENABLEP2PSTREAMREQUEST']._serialized_start=24519
+  _globals['_MANUALENABLEP2PSTREAMREQUEST']._serialized_end=24608
+  _globals['_MANUALENABLEP2PSTREAMRESPONSE']._serialized_start=24610
+  _globals['_MANUALENABLEP2PSTREAMRESPONSE']._serialized_end=24657
+  _globals['_NIFGEN']._serialized_start=51304
+  _globals['_NIFGEN']._serialized_end=65475
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nifgen-1.4.7/nifgen/nifgen_pb2_grpc.py` & `nifgen-1.4.8/nifgen/nifgen_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,19 +255,14 @@
                 response_deserializer=nifgen__pb2.CreateWaveformF64Response.FromString,
                 )
         self.CreateWaveformFromFileF64 = channel.unary_unary(
                 '/nifgen_grpc.NiFgen/CreateWaveformFromFileF64',
                 request_serializer=nifgen__pb2.CreateWaveformFromFileF64Request.SerializeToString,
                 response_deserializer=nifgen__pb2.CreateWaveformFromFileF64Response.FromString,
                 )
-        self.CreateWaveformFromFileHWS = channel.unary_unary(
-                '/nifgen_grpc.NiFgen/CreateWaveformFromFileHWS',
-                request_serializer=nifgen__pb2.CreateWaveformFromFileHWSRequest.SerializeToString,
-                response_deserializer=nifgen__pb2.CreateWaveformFromFileHWSResponse.FromString,
-                )
         self.CreateWaveformFromFileI16 = channel.unary_unary(
                 '/nifgen_grpc.NiFgen/CreateWaveformFromFileI16',
                 request_serializer=nifgen__pb2.CreateWaveformFromFileI16Request.SerializeToString,
                 response_deserializer=nifgen__pb2.CreateWaveformFromFileI16Response.FromString,
                 )
         self.CreateWaveformI16 = channel.unary_unary(
                 '/nifgen_grpc.NiFgen/CreateWaveformI16',
@@ -425,24 +420,14 @@
                 response_deserializer=nifgen__pb2.GetFIRFilterCoefficientsResponse.FromString,
                 )
         self.GetHardwareState = channel.unary_unary(
                 '/nifgen_grpc.NiFgen/GetHardwareState',
                 request_serializer=nifgen__pb2.GetHardwareStateRequest.SerializeToString,
                 response_deserializer=nifgen__pb2.GetHardwareStateResponse.FromString,
                 )
-        self.GetNextCoercionRecord = channel.unary_unary(
-                '/nifgen_grpc.NiFgen/GetNextCoercionRecord',
-                request_serializer=nifgen__pb2.GetNextCoercionRecordRequest.SerializeToString,
-                response_deserializer=nifgen__pb2.GetNextCoercionRecordResponse.FromString,
-                )
-        self.GetNextInterchangeWarning = channel.unary_unary(
-                '/nifgen_grpc.NiFgen/GetNextInterchangeWarning',
-                request_serializer=nifgen__pb2.GetNextInterchangeWarningRequest.SerializeToString,
-                response_deserializer=nifgen__pb2.GetNextInterchangeWarningResponse.FromString,
-                )
         self.GetSelfCalLastDateAndTime = channel.unary_unary(
                 '/nifgen_grpc.NiFgen/GetSelfCalLastDateAndTime',
                 request_serializer=nifgen__pb2.GetSelfCalLastDateAndTimeRequest.SerializeToString,
                 response_deserializer=nifgen__pb2.GetSelfCalLastDateAndTimeResponse.FromString,
                 )
         self.GetSelfCalLastTemp = channel.unary_unary(
                 '/nifgen_grpc.NiFgen/GetSelfCalLastTemp',
@@ -495,19 +480,14 @@
                 response_deserializer=nifgen__pb2.InvalidateAllAttributesResponse.FromString,
                 )
         self.IsDone = channel.unary_unary(
                 '/nifgen_grpc.NiFgen/IsDone',
                 request_serializer=nifgen__pb2.IsDoneRequest.SerializeToString,
                 response_deserializer=nifgen__pb2.IsDoneResponse.FromString,
                 )
-        self.ManualEnableP2PStream = channel.unary_unary(
-                '/nifgen_grpc.NiFgen/ManualEnableP2PStream',
-                request_serializer=nifgen__pb2.ManualEnableP2PStreamRequest.SerializeToString,
-                response_deserializer=nifgen__pb2.ManualEnableP2PStreamResponse.FromString,
-                )
         self.QueryArbSeqCapabilities = channel.unary_unary(
                 '/nifgen_grpc.NiFgen/QueryArbSeqCapabilities',
                 request_serializer=nifgen__pb2.QueryArbSeqCapabilitiesRequest.SerializeToString,
                 response_deserializer=nifgen__pb2.QueryArbSeqCapabilitiesResponse.FromString,
                 )
         self.QueryArbWfmCapabilities = channel.unary_unary(
                 '/nifgen_grpc.NiFgen/QueryArbWfmCapabilities',
@@ -665,14 +645,24 @@
                 response_deserializer=nifgen__pb2.WriteWaveformResponse.FromString,
                 )
         self.WriteWaveformComplexF64 = channel.unary_unary(
                 '/nifgen_grpc.NiFgen/WriteWaveformComplexF64',
                 request_serializer=nifgen__pb2.WriteWaveformComplexF64Request.SerializeToString,
                 response_deserializer=nifgen__pb2.WriteWaveformComplexF64Response.FromString,
                 )
+        self.CreateWaveformFromFileHWS = channel.unary_unary(
+                '/nifgen_grpc.NiFgen/CreateWaveformFromFileHWS',
+                request_serializer=nifgen__pb2.CreateWaveformFromFileHWSRequest.SerializeToString,
+                response_deserializer=nifgen__pb2.CreateWaveformFromFileHWSResponse.FromString,
+                )
+        self.ManualEnableP2PStream = channel.unary_unary(
+                '/nifgen_grpc.NiFgen/ManualEnableP2PStream',
+                request_serializer=nifgen__pb2.ManualEnableP2PStreamRequest.SerializeToString,
+                response_deserializer=nifgen__pb2.ManualEnableP2PStreamResponse.FromString,
+                )
 
 
 class NiFgenServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def AbortGeneration(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -964,20 +954,14 @@
 
     def CreateWaveformFromFileF64(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateWaveformFromFileHWS(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def CreateWaveformFromFileI16(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateWaveformI16(self, request, context):
@@ -1168,26 +1152,14 @@
 
     def GetHardwareState(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetNextCoercionRecord(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetNextInterchangeWarning(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def GetSelfCalLastDateAndTime(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSelfCalLastTemp(self, request, context):
@@ -1252,20 +1224,14 @@
 
     def IsDone(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ManualEnableP2PStream(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def QueryArbSeqCapabilities(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def QueryArbWfmCapabilities(self, request, context):
@@ -1456,14 +1422,26 @@
 
     def WriteWaveformComplexF64(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def CreateWaveformFromFileHWS(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ManualEnableP2PStream(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_NiFgenServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'AbortGeneration': grpc.unary_unary_rpc_method_handler(
                     servicer.AbortGeneration,
                     request_deserializer=nifgen__pb2.AbortGenerationRequest.FromString,
                     response_serializer=nifgen__pb2.AbortGenerationResponse.SerializeToString,
@@ -1704,19 +1682,14 @@
                     response_serializer=nifgen__pb2.CreateWaveformF64Response.SerializeToString,
             ),
             'CreateWaveformFromFileF64': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateWaveformFromFileF64,
                     request_deserializer=nifgen__pb2.CreateWaveformFromFileF64Request.FromString,
                     response_serializer=nifgen__pb2.CreateWaveformFromFileF64Response.SerializeToString,
             ),
-            'CreateWaveformFromFileHWS': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateWaveformFromFileHWS,
-                    request_deserializer=nifgen__pb2.CreateWaveformFromFileHWSRequest.FromString,
-                    response_serializer=nifgen__pb2.CreateWaveformFromFileHWSResponse.SerializeToString,
-            ),
             'CreateWaveformFromFileI16': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateWaveformFromFileI16,
                     request_deserializer=nifgen__pb2.CreateWaveformFromFileI16Request.FromString,
                     response_serializer=nifgen__pb2.CreateWaveformFromFileI16Response.SerializeToString,
             ),
             'CreateWaveformI16': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateWaveformI16,
@@ -1874,24 +1847,14 @@
                     response_serializer=nifgen__pb2.GetFIRFilterCoefficientsResponse.SerializeToString,
             ),
             'GetHardwareState': grpc.unary_unary_rpc_method_handler(
                     servicer.GetHardwareState,
                     request_deserializer=nifgen__pb2.GetHardwareStateRequest.FromString,
                     response_serializer=nifgen__pb2.GetHardwareStateResponse.SerializeToString,
             ),
-            'GetNextCoercionRecord': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetNextCoercionRecord,
-                    request_deserializer=nifgen__pb2.GetNextCoercionRecordRequest.FromString,
-                    response_serializer=nifgen__pb2.GetNextCoercionRecordResponse.SerializeToString,
-            ),
-            'GetNextInterchangeWarning': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetNextInterchangeWarning,
-                    request_deserializer=nifgen__pb2.GetNextInterchangeWarningRequest.FromString,
-                    response_serializer=nifgen__pb2.GetNextInterchangeWarningResponse.SerializeToString,
-            ),
             'GetSelfCalLastDateAndTime': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSelfCalLastDateAndTime,
                     request_deserializer=nifgen__pb2.GetSelfCalLastDateAndTimeRequest.FromString,
                     response_serializer=nifgen__pb2.GetSelfCalLastDateAndTimeResponse.SerializeToString,
             ),
             'GetSelfCalLastTemp': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSelfCalLastTemp,
@@ -1944,19 +1907,14 @@
                     response_serializer=nifgen__pb2.InvalidateAllAttributesResponse.SerializeToString,
             ),
             'IsDone': grpc.unary_unary_rpc_method_handler(
                     servicer.IsDone,
                     request_deserializer=nifgen__pb2.IsDoneRequest.FromString,
                     response_serializer=nifgen__pb2.IsDoneResponse.SerializeToString,
             ),
-            'ManualEnableP2PStream': grpc.unary_unary_rpc_method_handler(
-                    servicer.ManualEnableP2PStream,
-                    request_deserializer=nifgen__pb2.ManualEnableP2PStreamRequest.FromString,
-                    response_serializer=nifgen__pb2.ManualEnableP2PStreamResponse.SerializeToString,
-            ),
             'QueryArbSeqCapabilities': grpc.unary_unary_rpc_method_handler(
                     servicer.QueryArbSeqCapabilities,
                     request_deserializer=nifgen__pb2.QueryArbSeqCapabilitiesRequest.FromString,
                     response_serializer=nifgen__pb2.QueryArbSeqCapabilitiesResponse.SerializeToString,
             ),
             'QueryArbWfmCapabilities': grpc.unary_unary_rpc_method_handler(
                     servicer.QueryArbWfmCapabilities,
@@ -2114,14 +2072,24 @@
                     response_serializer=nifgen__pb2.WriteWaveformResponse.SerializeToString,
             ),
             'WriteWaveformComplexF64': grpc.unary_unary_rpc_method_handler(
                     servicer.WriteWaveformComplexF64,
                     request_deserializer=nifgen__pb2.WriteWaveformComplexF64Request.FromString,
                     response_serializer=nifgen__pb2.WriteWaveformComplexF64Response.SerializeToString,
             ),
+            'CreateWaveformFromFileHWS': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateWaveformFromFileHWS,
+                    request_deserializer=nifgen__pb2.CreateWaveformFromFileHWSRequest.FromString,
+                    response_serializer=nifgen__pb2.CreateWaveformFromFileHWSResponse.SerializeToString,
+            ),
+            'ManualEnableP2PStream': grpc.unary_unary_rpc_method_handler(
+                    servicer.ManualEnableP2PStream,
+                    request_deserializer=nifgen__pb2.ManualEnableP2PStreamRequest.FromString,
+                    response_serializer=nifgen__pb2.ManualEnableP2PStreamResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'nifgen_grpc.NiFgen', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -2958,31 +2926,14 @@
         return grpc.experimental.unary_unary(request, target, '/nifgen_grpc.NiFgen/CreateWaveformFromFileF64',
             nifgen__pb2.CreateWaveformFromFileF64Request.SerializeToString,
             nifgen__pb2.CreateWaveformFromFileF64Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CreateWaveformFromFileHWS(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nifgen_grpc.NiFgen/CreateWaveformFromFileHWS',
-            nifgen__pb2.CreateWaveformFromFileHWSRequest.SerializeToString,
-            nifgen__pb2.CreateWaveformFromFileHWSResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def CreateWaveformFromFileI16(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -3536,48 +3487,14 @@
         return grpc.experimental.unary_unary(request, target, '/nifgen_grpc.NiFgen/GetHardwareState',
             nifgen__pb2.GetHardwareStateRequest.SerializeToString,
             nifgen__pb2.GetHardwareStateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetNextCoercionRecord(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nifgen_grpc.NiFgen/GetNextCoercionRecord',
-            nifgen__pb2.GetNextCoercionRecordRequest.SerializeToString,
-            nifgen__pb2.GetNextCoercionRecordResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetNextInterchangeWarning(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nifgen_grpc.NiFgen/GetNextInterchangeWarning',
-            nifgen__pb2.GetNextInterchangeWarningRequest.SerializeToString,
-            nifgen__pb2.GetNextInterchangeWarningResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetSelfCalLastDateAndTime(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -3774,31 +3691,14 @@
         return grpc.experimental.unary_unary(request, target, '/nifgen_grpc.NiFgen/IsDone',
             nifgen__pb2.IsDoneRequest.SerializeToString,
             nifgen__pb2.IsDoneResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ManualEnableP2PStream(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nifgen_grpc.NiFgen/ManualEnableP2PStream',
-            nifgen__pb2.ManualEnableP2PStreamRequest.SerializeToString,
-            nifgen__pb2.ManualEnableP2PStreamResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def QueryArbSeqCapabilities(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -4350,7 +4250,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/nifgen_grpc.NiFgen/WriteWaveformComplexF64',
             nifgen__pb2.WriteWaveformComplexF64Request.SerializeToString,
             nifgen__pb2.WriteWaveformComplexF64Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CreateWaveformFromFileHWS(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/nifgen_grpc.NiFgen/CreateWaveformFromFileHWS',
+            nifgen__pb2.CreateWaveformFromFileHWSRequest.SerializeToString,
+            nifgen__pb2.CreateWaveformFromFileHWSResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ManualEnableP2PStream(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/nifgen_grpc.NiFgen/ManualEnableP2PStream',
+            nifgen__pb2.ManualEnableP2PStreamRequest.SerializeToString,
+            nifgen__pb2.ManualEnableP2PStreamResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `nifgen-1.4.7/nifgen/session.py` & `nifgen-1.4.8/nifgen/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,14 +434,24 @@
     Specifies the static value that replaces data masked by digital_data_mask.
     '''
     done_event_output_terminal = _attributes.AttributeViString(1150315)
     '''Type: str
 
     Specifies the destination terminal for the Done Event.
     '''
+    done_event_pulse_width = _attributes.AttributeViReal64(1150336)
+    '''Type: float
+
+    Specifies the pulse width for the Done Event.
+    '''
+    done_event_pulse_width_units = _attributes.AttributeEnum(_attributes.AttributeViInt32, enums.EventPulseWidthUnits, 1150334)
+    '''Type: enums.EventPulseWidthUnits
+
+    Specifies the pulse width units for the Done Event.
+    '''
     driver_setup = _attributes.AttributeViString(1050007)
     '''Type: str
 
     Specifies the driver setup portion of the option string that was passed into the InitWithOptions method.
 
     Note:
     One or more of the referenced methods are not in the Python API for this driver.
@@ -750,14 +760,44 @@
 
     Example: :py:attr:`my_session.markers[ ... ].marker_event_output_terminal`
 
     To set/get on all markers, you can call the property directly on the :py:class:`nifgen.Session`.
 
     Example: :py:attr:`my_session.marker_event_output_terminal`
     '''
+    marker_event_pulse_width = _attributes.AttributeViReal64(1150340)
+    '''Type: float
+
+    Specifies the pulse width for the Marker Event.
+
+    Tip:
+    This property can be set/get on specific markers within your :py:class:`nifgen.Session` instance.
+    Use Python index notation on the repeated capabilities container markers to specify a subset.
+
+    Example: :py:attr:`my_session.markers[ ... ].marker_event_pulse_width`
+
+    To set/get on all markers, you can call the property directly on the :py:class:`nifgen.Session`.
+
+    Example: :py:attr:`my_session.marker_event_pulse_width`
+    '''
+    marker_event_pulse_width_units = _attributes.AttributeEnum(_attributes.AttributeViInt32, enums.EventPulseWidthUnits, 1150341)
+    '''Type: enums.EventPulseWidthUnits
+
+    Specifies the pulse width units for the Marker Event.
+
+    Tip:
+    This property can be set/get on specific markers within your :py:class:`nifgen.Session` instance.
+    Use Python index notation on the repeated capabilities container markers to specify a subset.
+
+    Example: :py:attr:`my_session.markers[ ... ].marker_event_pulse_width_units`
+
+    To set/get on all markers, you can call the property directly on the :py:class:`nifgen.Session`.
+
+    Example: :py:attr:`my_session.marker_event_pulse_width_units`
+    '''
     max_freq_list_duration = _attributes.AttributeViReal64(1150213)
     '''Type: float
 
     Returns the maximum duration of any one step in the frequency  list.
     '''
     max_freq_list_length = _attributes.AttributeViInt32(1150211)
     '''Type: int
@@ -978,14 +1018,24 @@
     A string that contains the name of the vendor that supplies NI-FGEN.
     '''
     started_event_output_terminal = _attributes.AttributeViString(1150314)
     '''Type: str
 
     Specifies the destination terminal for the Started Event.
     '''
+    started_event_pulse_width = _attributes.AttributeViReal64(1150335)
+    '''Type: float
+
+    Specifies the pulse width for the Started Event.
+    '''
+    started_event_pulse_width_units = _attributes.AttributeEnum(_attributes.AttributeViInt32, enums.EventPulseWidthUnits, 1150333)
+    '''Type: enums.EventPulseWidthUnits
+
+    Specifies the pulse width units for the Started Event.
+    '''
     start_trigger_type = _attributes.AttributeEnum(_attributes.AttributeViInt32, enums.StartTriggerType, 1150280)
     '''Type: enums.StartTriggerType
 
     Specifies whether you want the Start trigger to be a Digital Edge, or Software trigger. You can also choose None as the value for this property.
     '''
     streaming_space_available_in_waveform = _attributes.AttributeViInt32(1150325)
     '''Type: int
@@ -1543,22 +1593,22 @@
         if str(type(waveform_data_array)).find("'numpy.ndarray'") != -1:
             import numpy
             if waveform_data_array.dtype == numpy.float64:
                 return self._create_waveform_f64_numpy(waveform_data_array)
             elif waveform_data_array.dtype == numpy.int16:
                 return self._create_waveform_i16_numpy(waveform_data_array)
             else:
-                raise TypeError("Unsupported dtype. Is {0}, expected {1} or {2}".format(waveform_data_array.dtype, numpy.float64, numpy.int16))
+                raise TypeError("Unsupported dtype. Is {}, expected {} or {}".format(waveform_data_array.dtype, numpy.float64, numpy.int16))
         elif isinstance(waveform_data_array, array.array):
             if waveform_data_array.typecode == 'd':
                 return self._create_waveform_f64(waveform_data_array)
             elif waveform_data_array.typecode == 'h':
                 return self._create_waveform_i16(waveform_data_array)
             else:
-                raise TypeError("Unsupported dtype. Is {0}, expected {1} or {2}".format(waveform_data_array.typecode, 'd (double)', 'h (16 bit int)'))
+                raise TypeError("Unsupported dtype. Is {}, expected {} or {}".format(waveform_data_array.typecode, 'd (double)', 'h (16 bit int)'))
 
         return self._create_waveform_f64(waveform_data_array)
 
     @ivi_synchronized
     def _create_waveform_f64(self, waveform_data_array):
         r'''_create_waveform_f64
 
@@ -2208,15 +2258,15 @@
                 trigger_id = "None"
                 trigger = enums.Trigger.START
 
         elif trigger is not None and trigger_id is not None:
             pass  # This is how the function should be called
 
         else:
-            raise ValueError('Both trigger ({0}) and trigger_id ({1}) should be passed in to the method'.format(str(trigger), str(trigger_id)))
+            raise ValueError('Both trigger ({}) and trigger_id ({}) should be passed in to the method'.format(str(trigger), str(trigger_id)))
 
         if type(trigger) is not enums.Trigger:
             raise TypeError('Parameter trigger must be of type ' + str(enums.Trigger))
         self._interpreter.send_software_edge_trigger(trigger, trigger_id)
 
     @ivi_synchronized
     def _set_attribute_vi_boolean(self, attribute_id, attribute_value):
@@ -2932,22 +2982,22 @@
         if str(type(data)).find("'numpy.ndarray'") != -1:
             import numpy
             if data.dtype == numpy.float64:
                 return self._write_named_waveform_f64_numpy(waveform_name_or_handle, data) if use_named else self._write_waveform_numpy(waveform_name_or_handle, data)
             elif data.dtype == numpy.int16:
                 return self._write_named_waveform_i16_numpy(waveform_name_or_handle, data) if use_named else self._write_binary16_waveform_numpy(waveform_name_or_handle, data)
             else:
-                raise TypeError("Unsupported dtype. Is {0}, expected {1} or {2}".format(data.dtype, numpy.float64, numpy.int16))
+                raise TypeError("Unsupported dtype. Is {}, expected {} or {}".format(data.dtype, numpy.float64, numpy.int16))
         elif isinstance(data, array.array):
             if data.typecode == 'd':
                 return self._write_named_waveform_f64(waveform_name_or_handle, data) if use_named else self._write_waveform(waveform_name_or_handle, data)
             elif data.typecode == 'h':
                 return self._write_named_waveform_i16(waveform_name_or_handle, data) if use_named else self._write_binary16_waveform(waveform_name_or_handle, data)
             else:
-                raise TypeError("Unsupported dtype. Is {0}, expected {1} or {2}".format(data.typecode, 'd (double)', 'h (16 bit int)'))
+                raise TypeError("Unsupported dtype. Is {}, expected {} or {}".format(data.typecode, 'd (double)', 'h (16 bit int)'))
 
         return self._write_named_waveform_f64(waveform_name_or_handle, data) if use_named else self._write_waveform(waveform_name_or_handle, data)
 
     def _error_message(self, error_code):
         r'''_error_message
 
         Converts a status code returned by an NI-FGEN method into a
```

### Comparing `nifgen-1.4.7/nifgen/session_pb2.py` & `nifgen-1.4.8/nifgen/session_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: session.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rsession.proto\x12\rnidevice_grpc\"2\n\x07Session\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x12\x0c\n\x02id\x18\x02 \x01(\rH\x00\x42\t\n\x07session\"j\n\x10\x44\x65viceProperties\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05model\x18\x02 \x01(\t\x12\x0e\n\x06vendor\x18\x03 \x01(\t\x12\x15\n\rserial_number\x18\x04 \x01(\t\x12\x12\n\nproduct_id\x18\x05 \x01(\r\"\x19\n\x17\x45numerateDevicesRequest\"L\n\x18\x45numerateDevicesResponse\x12\x30\n\x07\x64\x65vices\x18\x01 \x03(\x0b\x32\x1f.nidevice_grpc.DeviceProperties\";\n\x0eReserveRequest\x12\x16\n\x0ereservation_id\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t\"&\n\x0fReserveResponse\x12\x13\n\x0bis_reserved\x18\x01 \x01(\x08\"F\n\x19IsReservedByClientRequest\x12\x16\n\x0ereservation_id\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t\"1\n\x1aIsReservedByClientResponse\x12\x13\n\x0bis_reserved\x18\x01 \x01(\x08\"=\n\x10UnreserveRequest\x12\x16\n\x0ereservation_id\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t\"*\n\x11UnreserveResponse\x12\x15\n\ris_unreserved\x18\x01 \x01(\x08\"\x14\n\x12ResetServerRequest\".\n\x13ResetServerResponse\x12\x17\n\x0fis_server_reset\x18\x01 \x01(\x08*\xbc\x01\n\x1dSessionInitializationBehavior\x12/\n+SESSION_INITIALIZATION_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x32\n.SESSION_INITIALIZATION_BEHAVIOR_INITIALIZE_NEW\x10\x01\x12\x36\n2SESSION_INITIALIZATION_BEHAVIOR_ATTACH_TO_EXISTING\x10\x02\x32\xd2\x03\n\x10SessionUtilities\x12\x63\n\x10\x45numerateDevices\x12&.nidevice_grpc.EnumerateDevicesRequest\x1a\'.nidevice_grpc.EnumerateDevicesResponse\x12H\n\x07Reserve\x12\x1d.nidevice_grpc.ReserveRequest\x1a\x1e.nidevice_grpc.ReserveResponse\x12i\n\x12IsReservedByClient\x12(.nidevice_grpc.IsReservedByClientRequest\x1a).nidevice_grpc.IsReservedByClientResponse\x12N\n\tUnreserve\x12\x1f.nidevice_grpc.UnreserveRequest\x1a .nidevice_grpc.UnreserveResponse\x12T\n\x0bResetServer\x12!.nidevice_grpc.ResetServerRequest\x1a\".nidevice_grpc.ResetServerResponseBB\n\x12\x63om.ni.grpc.deviceB\x08NiDeviceP\x01\xaa\x02\x1fNationalInstruments.Grpc.Deviceb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'session_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'session_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.ni.grpc.deviceB\010NiDeviceP\001\252\002\037NationalInstruments.Grpc.Device'
-  _SESSIONINITIALIZATIONBEHAVIOR._serialized_start=699
-  _SESSIONINITIALIZATIONBEHAVIOR._serialized_end=887
-  _SESSION._serialized_start=32
-  _SESSION._serialized_end=82
-  _DEVICEPROPERTIES._serialized_start=84
-  _DEVICEPROPERTIES._serialized_end=190
-  _ENUMERATEDEVICESREQUEST._serialized_start=192
-  _ENUMERATEDEVICESREQUEST._serialized_end=217
-  _ENUMERATEDEVICESRESPONSE._serialized_start=219
-  _ENUMERATEDEVICESRESPONSE._serialized_end=295
-  _RESERVEREQUEST._serialized_start=297
-  _RESERVEREQUEST._serialized_end=356
-  _RESERVERESPONSE._serialized_start=358
-  _RESERVERESPONSE._serialized_end=396
-  _ISRESERVEDBYCLIENTREQUEST._serialized_start=398
-  _ISRESERVEDBYCLIENTREQUEST._serialized_end=468
-  _ISRESERVEDBYCLIENTRESPONSE._serialized_start=470
-  _ISRESERVEDBYCLIENTRESPONSE._serialized_end=519
-  _UNRESERVEREQUEST._serialized_start=521
-  _UNRESERVEREQUEST._serialized_end=582
-  _UNRESERVERESPONSE._serialized_start=584
-  _UNRESERVERESPONSE._serialized_end=626
-  _RESETSERVERREQUEST._serialized_start=628
-  _RESETSERVERREQUEST._serialized_end=648
-  _RESETSERVERRESPONSE._serialized_start=650
-  _RESETSERVERRESPONSE._serialized_end=696
-  _SESSIONUTILITIES._serialized_start=890
-  _SESSIONUTILITIES._serialized_end=1356
+  _globals['_SESSIONINITIALIZATIONBEHAVIOR']._serialized_start=699
+  _globals['_SESSIONINITIALIZATIONBEHAVIOR']._serialized_end=887
+  _globals['_SESSION']._serialized_start=32
+  _globals['_SESSION']._serialized_end=82
+  _globals['_DEVICEPROPERTIES']._serialized_start=84
+  _globals['_DEVICEPROPERTIES']._serialized_end=190
+  _globals['_ENUMERATEDEVICESREQUEST']._serialized_start=192
+  _globals['_ENUMERATEDEVICESREQUEST']._serialized_end=217
+  _globals['_ENUMERATEDEVICESRESPONSE']._serialized_start=219
+  _globals['_ENUMERATEDEVICESRESPONSE']._serialized_end=295
+  _globals['_RESERVEREQUEST']._serialized_start=297
+  _globals['_RESERVEREQUEST']._serialized_end=356
+  _globals['_RESERVERESPONSE']._serialized_start=358
+  _globals['_RESERVERESPONSE']._serialized_end=396
+  _globals['_ISRESERVEDBYCLIENTREQUEST']._serialized_start=398
+  _globals['_ISRESERVEDBYCLIENTREQUEST']._serialized_end=468
+  _globals['_ISRESERVEDBYCLIENTRESPONSE']._serialized_start=470
+  _globals['_ISRESERVEDBYCLIENTRESPONSE']._serialized_end=519
+  _globals['_UNRESERVEREQUEST']._serialized_start=521
+  _globals['_UNRESERVEREQUEST']._serialized_end=582
+  _globals['_UNRESERVERESPONSE']._serialized_start=584
+  _globals['_UNRESERVERESPONSE']._serialized_end=626
+  _globals['_RESETSERVERREQUEST']._serialized_start=628
+  _globals['_RESETSERVERREQUEST']._serialized_end=648
+  _globals['_RESETSERVERRESPONSE']._serialized_start=650
+  _globals['_RESETSERVERRESPONSE']._serialized_end=696
+  _globals['_SESSIONUTILITIES']._serialized_start=890
+  _globals['_SESSIONUTILITIES']._serialized_end=1356
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nifgen-1.4.7/nifgen/session_pb2_grpc.py` & `nifgen-1.4.8/nifgen/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.7/nifgen.egg-info/PKG-INFO` & `nifgen-1.4.8/nifgen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifgen
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI-FGEN Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -17,22 +17,23 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Description-Content-Type: text/x-rst
 Requires-Dist: hightime>=0.2.0
 Requires-Dist: nitclk
 Provides-Extra: grpc
-Requires-Dist: grpcio<2.0,>=1.49.1; extra == "grpc"
-Requires-Dist: protobuf<5.0,>=4.21; extra == "grpc"
+Requires-Dist: grpcio<2.0,>=1.59.0; extra == "grpc"
+Requires-Dist: protobuf<5.0,>=4.21.6; extra == "grpc"
 
 Overall Status
 --------------
 
 +----------------------+------------------------------------------------------------------------------------------------------------------------------------+
 | master branch status | |BuildStatus| |MITLicense| |CoverageStatus|                                                                                        |
 +----------------------+------------------------------------------------------------------------------------------------------------------------------------+
@@ -81,15 +82,15 @@
 
 NI-FGEN Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-FGEN (nifgen)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 2023 Q1.1             |
+| Driver Version Tested Against | 2023 Q4               |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nifgenLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nifgenPythonVersion| |
 +-------------------------------+-----------------------+
 | Documentation                 | |nifgenDocs|          |
 +-------------------------------+-----------------------+
@@ -130,15 +131,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nifgen** module, you must install the NI-FGEN runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-FGEN**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nifgen~=1.4.7
+  $ python -m pip install nifgen~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nifgen-1.4.7/nifgen.egg-info/SOURCES.txt` & `nifgen-1.4.8/nifgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.7/setup.py` & `nifgen-1.4.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/python
-# -*- coding: utf-8 -*-
 # This file was generated
 
 
 from setuptools.command.test import test as test_command
 from setuptools import setup
 
 
@@ -25,15 +24,15 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.7',
+    version='1.4.8',
     description='NI-FGEN Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
@@ -44,16 +43,16 @@
     packages=['nifgen'],
     install_requires=[
         'hightime>=0.2.0',
         'nitclk',
     ],
     extras_require={
         'grpc': [
-            'grpcio>=1.49.1,<2.0',
-            'protobuf>=4.21,<5.0'
+            'grpcio>=1.59.0,<2.0',
+            'protobuf>=4.21.6,<5.0'
         ],
     },
     setup_requires=['pytest-runner', ],
     tests_require=['pytest'],
     test_suite='tests',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
@@ -64,13 +63,14 @@
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: System :: Hardware :: Hardware Drivers"
     ],
     cmdclass={'test': PyTest},
     package_data={pypi_name: ['VERSION']},
 )
```

