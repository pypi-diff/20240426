# Comparing `tmp/niswitch-1.4.7.tar.gz` & `tmp/niswitch-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niswitch-1.4.7.tar", last modified: Fri Dec 15 19:31:33 2023, max compression
+gzip compressed data, was "niswitch-1.4.8.tar", last modified: Fri Apr 26 18:17:50 2024, max compression
```

## Comparing `niswitch-1.4.7.tar` & `niswitch-1.4.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:42.580242 niswitch-1.4.7/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8045 2023-12-15 19:31:42.573242 niswitch-1.4.7/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     6876 2023-12-15 19:29:00.000000 niswitch-1.4.7/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:42.353675 niswitch-1.4.7/niswitch/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-12-15 19:28:47.000000 niswitch-1.4.7/niswitch/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3047 2023-12-15 19:28:45.000000 niswitch-1.4.7/niswitch/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5444 2023-12-15 19:28:38.000000 niswitch-1.4.7/niswitch/_attributes.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13875 2023-12-15 19:28:46.000000 niswitch-1.4.7/niswitch/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12848 2023-12-15 19:28:47.000000 niswitch-1.4.7/niswitch/_grpc_stub_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    25549 2023-12-15 19:28:40.000000 niswitch-1.4.7/niswitch/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    26760 2023-12-15 19:28:41.000000 niswitch-1.4.7/niswitch/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1731 2023-12-15 19:28:41.000000 niswitch-1.4.7/niswitch/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-12-15 19:28:51.000000 niswitch-1.4.7/niswitch/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13707 2023-12-15 19:28:39.000000 niswitch-1.4.7/niswitch/enums.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4377 2023-12-15 19:28:43.000000 niswitch-1.4.7/niswitch/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3456 2023-12-15 19:28:48.000000 niswitch-1.4.7/niswitch/grpc_session_options.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-12-15 19:28:50.000000 niswitch-1.4.7/niswitch/nidevice_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-12-15 19:28:50.000000 niswitch-1.4.7/niswitch/nidevice_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    55730 2023-12-15 19:28:49.000000 niswitch-1.4.7/niswitch/niswitch_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    96817 2023-12-15 19:28:49.000000 niswitch-1.4.7/niswitch/niswitch_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   114951 2023-12-15 19:28:42.000000 niswitch-1.4.7/niswitch/session.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-12-15 19:28:51.000000 niswitch-1.4.7/niswitch/session_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-12-15 19:28:51.000000 niswitch-1.4.7/niswitch/session_pb2_grpc.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:42.564242 niswitch-1.4.7/niswitch.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8045 2023-12-15 19:31:41.000000 niswitch-1.4.7/niswitch.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      686 2023-12-15 19:31:42.000000 niswitch-1.4.7/niswitch.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:31:41.000000 niswitch-1.4.7/niswitch.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       64 2023-12-15 19:31:41.000000 niswitch-1.4.7/niswitch.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-12-15 19:31:41.000000 niswitch-1.4.7/niswitch.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:31:41.000000 niswitch-1.4.7/niswitch.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-12-15 19:31:42.581242 niswitch-1.4.7/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2086 2023-12-15 19:29:01.000000 niswitch-1.4.7/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:17:50.860315 niswitch-1.4.8/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8098 2024-04-26 18:17:50.853357 niswitch-1.4.8/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     6876 2024-04-26 18:10:54.000000 niswitch-1.4.8/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:17:50.655622 niswitch-1.4.8/niswitch/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2024-04-26 18:10:41.000000 niswitch-1.4.8/niswitch/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3566 2024-04-26 18:10:39.000000 niswitch-1.4.8/niswitch/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5444 2024-04-26 18:10:32.000000 niswitch-1.4.8/niswitch/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13875 2024-04-26 18:10:40.000000 niswitch-1.4.8/niswitch/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12848 2024-04-26 18:10:41.000000 niswitch-1.4.8/niswitch/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    25549 2024-04-26 18:10:34.000000 niswitch-1.4.8/niswitch/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    26760 2024-04-26 18:10:35.000000 niswitch-1.4.8/niswitch/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1731 2024-04-26 18:10:35.000000 niswitch-1.4.8/niswitch/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      635 2024-04-26 18:10:45.000000 niswitch-1.4.8/niswitch/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13707 2024-04-26 18:10:33.000000 niswitch-1.4.8/niswitch/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4371 2024-04-26 18:10:37.000000 niswitch-1.4.8/niswitch/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3456 2024-04-26 18:10:42.000000 niswitch-1.4.8/niswitch/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2009 2024-04-26 18:10:44.000000 niswitch-1.4.8/niswitch/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2024-04-26 18:10:44.000000 niswitch-1.4.8/niswitch/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    58868 2024-04-26 18:10:43.000000 niswitch-1.4.8/niswitch/niswitch_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    96817 2024-04-26 18:10:43.000000 niswitch-1.4.8/niswitch/niswitch_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   114951 2024-04-26 18:10:36.000000 niswitch-1.4.8/niswitch/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4550 2024-04-26 18:10:45.000000 niswitch-1.4.8/niswitch/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2024-04-26 18:10:45.000000 niswitch-1.4.8/niswitch/session_pb2_grpc.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:17:50.846360 niswitch-1.4.8/niswitch.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8098 2024-04-26 18:17:50.000000 niswitch-1.4.8/niswitch.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      686 2024-04-26 18:17:50.000000 niswitch-1.4.8/niswitch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:17:50.000000 niswitch-1.4.8/niswitch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       66 2024-04-26 18:17:50.000000 niswitch-1.4.8/niswitch.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2024-04-26 18:17:50.000000 niswitch-1.4.8/niswitch.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:17:50.000000 niswitch-1.4.8/niswitch.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2024-04-26 18:17:50.861316 niswitch-1.4.8/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2114 2024-04-26 18:10:54.000000 niswitch-1.4.8/setup.py
```

### Comparing `niswitch-1.4.7/PKG-INFO` & `niswitch-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niswitch
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI-SWITCH Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -17,21 +17,22 @@
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
@@ -80,15 +81,15 @@
 
 NI-SWITCH Python API Status
 ---------------------------
 
 +-------------------------------+-------------------------+
 | NI-SWITCH (niswitch)          |                         |
 +===============================+=========================+
-| Driver Version Tested Against | 2023 Q1                 |
+| Driver Version Tested Against | 2023 Q4                 |
 +-------------------------------+-------------------------+
 | PyPI Version                  | |niswitchLatestVersion| |
 +-------------------------------+-------------------------+
 | Supported Python Version      | |niswitchPythonVersion| |
 +-------------------------------+-------------------------+
 | Documentation                 | |niswitchDocs|          |
 +-------------------------------+-------------------------+
@@ -129,15 +130,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **niswitch** module, you must install the NI-SWITCH runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SWITCH**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niswitch~=1.4.7
+  $ python -m pip install niswitch~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `niswitch-1.4.7/README.rst` & `niswitch-1.4.8/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 NI-SWITCH Python API Status
 ---------------------------
 
 +-------------------------------+-------------------------+
 | NI-SWITCH (niswitch)          |                         |
 +===============================+=========================+
-| Driver Version Tested Against | 2023 Q1                 |
+| Driver Version Tested Against | 2023 Q4                 |
 +-------------------------------+-------------------------+
 | PyPI Version                  | |niswitchLatestVersion| |
 +-------------------------------+-------------------------+
 | Supported Python Version      | |niswitchPythonVersion| |
 +-------------------------------+-------------------------+
 | Documentation                 | |niswitchDocs|          |
 +-------------------------------+-------------------------+
@@ -98,15 +98,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **niswitch** module, you must install the NI-SWITCH runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SWITCH**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niswitch~=1.4.7
+  $ python -m pip install niswitch~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `niswitch-1.4.7/niswitch/__init__.py` & `niswitch-1.4.8/niswitch/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.7'
+__version__ = '1.4.8'
 
 from niswitch.enums import *  # noqa: F403,F401,H303
 from niswitch.errors import DriverWarning  # noqa: F401
 from niswitch.errors import Error  # noqa: F401
 from niswitch.grpc_session_options import *  # noqa: F403,F401,H303
 from niswitch.session import Session  # noqa: F401
 
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
     info['driver']['name'] = "NI-SWITCH"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'niswitch'
-    info['module']['version'] = "1.4.7"
+    info['module']['version'] = "1.4.8"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `niswitch-1.4.7/niswitch/_attributes.py` & `niswitch-1.4.8/niswitch/_attributes.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/niswitch/_converters.py` & `niswitch-1.4.8/niswitch/_converters.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/niswitch/_grpc_stub_interpreter.py` & `niswitch-1.4.8/niswitch/_grpc_stub_interpreter.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/niswitch/_library.py` & `niswitch-1.4.8/niswitch/_library.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/niswitch/_library_interpreter.py` & `niswitch-1.4.8/niswitch/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/niswitch/_library_singleton.py` & `niswitch-1.4.8/niswitch/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/niswitch/_visatype.py` & `niswitch-1.4.8/niswitch/_visatype.py`

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

### Comparing `niswitch-1.4.7/niswitch/enums.py` & `niswitch-1.4.8/niswitch/enums.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/niswitch/errors.py` & `niswitch-1.4.8/niswitch/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-SWITCH driver'''
 
     def __init__(self, code, description):
         assert _is_warning(code), "Should not create Warning if code is not positive."
-        super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
+        super(DriverWarning, self).__init__('Warning {} occurred.\n\n{}'.format(code, description))
 
 
 class RpcError(Error):
     '''An error specific to sessions to the NI gRPC Device Server'''
 
     def __init__(self, rpc_code, description):
         self.rpc_code = rpc_code
@@ -85,24 +85,24 @@
         super(DriverTooNewError, self).__init__('The NI-SWITCH runtime returned an unexpected value. This can occur if it is too new for the niswitch Python module. Upgrade the niswitch Python module.')
 
 
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
 
     Helper function for handling errors returned by niswitch.Library.
     It calls back into the LibraryInterpreter to get the corresponding error
```

### Comparing `niswitch-1.4.7/niswitch/grpc_session_options.py` & `niswitch-1.4.8/niswitch/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/niswitch/nidevice_pb2.py` & `niswitch-1.4.8/niswitch/nidevice_pb2.py`

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

### Comparing `niswitch-1.4.7/niswitch/niswitch_pb2.py` & `niswitch-1.4.8/niswitch/niswitch_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,293 +1,293 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: niswitch.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import session_pb2 as session__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eniswitch.proto\x12\rniswitch_grpc\x1a\rsession.proto\"6\n\x10\x41\x62ortScanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"#\n\x11\x41\x62ortScanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"[\n\x11\x43\x61nConnectRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x10\n\x08\x63hannel1\x18\x02 \x01(\t\x12\x10\n\x08\x63hannel2\x18\x03 \x01(\t\"y\n\x12\x43\x61nConnectResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x36\n\x0fpath_capability\x18\x02 \x01(\x0e\x32\x1d.niswitch_grpc.PathCapability\x12\x1b\n\x13path_capability_raw\x18\x03 \x01(\x11\"\xab\x01\n\x1e\x43heckAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\x12\x17\n\x0f\x61ttribute_value\x18\x04 \x01(\x08\"1\n\x1f\x43heckAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8f\x02\n\x1c\x43heckAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\x12\x1d\n\x13\x61ttribute_value_raw\x18\x04 \x01(\x11H\x00\x12\x46\n\x0f\x61ttribute_value\x18\x05 \x01(\x0e\x32+.niswitch_grpc.NiSwitchInt32AttributeValuesH\x00\x42\x16\n\x14\x61ttribute_value_enum\"/\n\x1d\x43heckAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xae\x01\n\x1d\x43heckAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\x12\x1b\n\x13\x61ttribute_value_raw\x18\x04 \x01(\x01\"0\n\x1e\x43heckAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xc3\x01\n\x1e\x43heckAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\x12/\n\x0f\x61ttribute_value\x18\x04 \x01(\x0b\x32\x16.nidevice_grpc.Session\"1\n\x1f\x43heckAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xae\x01\n\x1d\x43heckAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\x12\x1b\n\x13\x61ttribute_value_raw\x18\x04 \x01(\t\"0\n\x1e\x43heckAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"7\n\x11\x43learErrorRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"$\n\x12\x43learErrorResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"E\n\x1f\x43learInterchangeWarningsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"2\n ClearInterchangeWarningsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"2\n\x0c\x43loseRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rCloseResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"3\n\rCommitRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\" \n\x0e\x43ommitResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa9\x01\n\x18\x43onfigureScanListRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x10\n\x08scanlist\x18\x02 \x01(\t\x12,\n\tscan_mode\x18\x03 \x01(\x0e\x32\x17.niswitch_grpc.ScanModeH\x00\x12\x17\n\rscan_mode_raw\x18\x04 \x01(\x11H\x00\x42\x10\n\x0escan_mode_enum\"+\n\x19\x43onfigureScanListResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xc2\x02\n\x1b\x43onfigureScanTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nscan_delay\x18\x02 \x01(\x01\x12\x34\n\rtrigger_input\x18\x03 \x01(\x0e\x32\x1b.niswitch_grpc.TriggerInputH\x00\x12\x1b\n\x11trigger_input_raw\x18\x04 \x01(\x11H\x00\x12\x41\n\x14scan_advanced_output\x18\x05 \x01(\x0e\x32!.niswitch_grpc.ScanAdvancedOutputH\x01\x12\"\n\x18scan_advanced_output_raw\x18\x06 \x01(\x11H\x01\x42\x14\n\x12trigger_input_enumB\x1b\n\x19scan_advanced_output_enum\".\n\x1c\x43onfigureScanTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"X\n\x0e\x43onnectRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x10\n\x08\x63hannel1\x18\x02 \x01(\t\x12\x10\n\x08\x63hannel2\x18\x03 \x01(\t\"!\n\x0f\x43onnectResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"U\n\x16\x43onnectMultipleRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x17\n\x0f\x63onnection_list\x18\x02 \x01(\t\")\n\x17\x43onnectMultipleResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"4\n\x0e\x44isableRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"!\n\x0f\x44isableResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"[\n\x11\x44isconnectRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x10\n\x08\x63hannel1\x18\x02 \x01(\t\x12\x10\n\x08\x63hannel2\x18\x03 \x01(\t\"$\n\x12\x44isconnectResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\":\n\x14\x44isconnectAllRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\'\n\x15\x44isconnectAllResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"[\n\x19\x44isconnectMultipleRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x1a\n\x12\x64isconnection_list\x18\x02 \x01(\t\",\n\x1a\x44isconnectMultipleResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"M\n\x13\x45rrorMessageRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nerror_code\x18\x02 \x01(\x11\"=\n\x14\x45rrorMessageResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"7\n\x11\x45rrorQueryRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"O\n\x12\x45rrorQueryResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x12\n\nerror_code\x18\x02 \x01(\x11\x12\x15\n\rerror_message\x18\x03 \x01(\t\"\x90\x01\n\x1cGetAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\"H\n\x1dGetAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\x08\"\x8e\x01\n\x1aGetAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\"F\n\x1bGetAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\x11\"\x8f\x01\n\x1bGetAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\"G\n\x1cGetAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\x01\"\x90\x01\n\x1cGetAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\"`\n\x1dGetAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12/\n\x0f\x61ttribute_value\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x8f\x01\n\x1bGetAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\"G\n\x1cGetAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x61ttribute_value\x18\x02 \x01(\t\"J\n\x15GetChannelNameRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\r\n\x05index\x18\x02 \x01(\x11\"E\n\x16GetChannelNameResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1b\n\x13\x63hannel_name_buffer\x18\x02 \x01(\t\"5\n\x0fGetErrorRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"E\n\x10GetErrorResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04\x63ode\x18\x02 \x01(\x11\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\"B\n\x1cGetNextCoercionRecordRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"H\n\x1dGetNextCoercionRecordResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x63oercion_record\x18\x02 \x01(\t\"F\n GetNextInterchangeWarningRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"P\n!GetNextInterchangeWarningResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1b\n\x13interchange_warning\x18\x02 \x01(\t\"X\n\x0eGetPathRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x10\n\x08\x63hannel1\x18\x02 \x01(\t\x12\x10\n\x08\x63hannel2\x18\x03 \x01(\t\"/\n\x0fGetPathResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04path\x18\x02 \x01(\t\"N\n\x14GetRelayCountRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nrelay_name\x18\x02 \x01(\t\"<\n\x15GetRelayCountResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0brelay_count\x18\x02 \x01(\x11\"H\n\x13GetRelayNameRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\r\n\x05index\x18\x02 \x01(\x11\"A\n\x14GetRelayNameResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x19\n\x11relay_name_buffer\x18\x02 \x01(\t\"Q\n\x17GetRelayPositionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nrelay_name\x18\x02 \x01(\t\"|\n\x18GetRelayPositionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x34\n\x0erelay_position\x18\x02 \x01(\x0e\x32\x1c.niswitch_grpc.RelayPosition\x12\x1a\n\x12relay_position_raw\x18\x03 \x01(\x11\"\xb1\x01\n\x0bInitRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x10\n\x08id_query\x18\x03 \x01(\x08\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12M\n\x17initialization_behavior\x18\x05 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"~\n\x0cInitResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"\xd3\x01\n\x16InitWithOptionsRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x10\n\x08id_query\x18\x03 \x01(\x08\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12\x15\n\roption_string\x18\x05 \x01(\t\x12M\n\x17initialization_behavior\x18\x06 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"\x89\x01\n\x17InitWithOptionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"\xcf\x01\n\x17InitWithTopologyRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x10\n\x08topology\x18\x03 \x01(\t\x12\x10\n\x08simulate\x18\x04 \x01(\x08\x12\x14\n\x0creset_device\x18\x05 \x01(\x08\x12M\n\x17initialization_behavior\x18\x06 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"\x8a\x01\n\x18InitWithTopologyResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"9\n\x13InitiateScanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"&\n\x14InitiateScanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"D\n\x1eInvalidateAllAttributesRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"1\n\x1fInvalidateAllAttributesResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"8\n\x12IsDebouncedRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\";\n\x13IsDebouncedResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x14\n\x0cis_debounced\x18\x02 \x01(\x08\"7\n\x11IsScanningRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"9\n\x12IsScanningResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0bis_scanning\x18\x02 \x01(\x08\"\xb2\x01\n\x13RelayControlRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nrelay_name\x18\x02 \x01(\t\x12\x32\n\x0crelay_action\x18\x03 \x01(\x0e\x32\x1a.niswitch_grpc.RelayActionH\x00\x12\x1a\n\x10relay_action_raw\x18\x04 \x01(\x11H\x00\x42\x13\n\x11relay_action_enum\"&\n\x14RelayControlResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"2\n\x0cResetRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rResetResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"B\n\x1cResetInterchangeCheckRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"/\n\x1dResetInterchangeCheckResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\">\n\x18ResetWithDefaultsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"+\n\x19ResetWithDefaultsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\":\n\x14RevisionQueryRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"f\n\x15RevisionQueryResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x1ainstrument_driver_revision\x18\x02 \x01(\t\x12\x19\n\x11\x66irmware_revision\x18\x03 \x01(\t\"\x95\x03\n\x1eRouteScanAdvancedOutputRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12K\n\x1escan_advanced_output_connector\x18\x02 \x01(\x0e\x32!.niswitch_grpc.ScanAdvancedOutputH\x00\x12,\n\"scan_advanced_output_connector_raw\x18\x03 \x01(\x11H\x00\x12J\n\x1dscan_advanced_output_bus_line\x18\x04 \x01(\x0e\x32!.niswitch_grpc.ScanAdvancedOutputH\x01\x12+\n!scan_advanced_output_bus_line_raw\x18\x05 \x01(\x11H\x01\x12\x0e\n\x06invert\x18\x06 \x01(\x08\x42%\n#scan_advanced_output_connector_enumB$\n\"scan_advanced_output_bus_line_enum\"1\n\x1fRouteScanAdvancedOutputResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xd9\x02\n\x18RouteTriggerInputRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12>\n\x17trigger_input_connector\x18\x02 \x01(\x0e\x32\x1b.niswitch_grpc.TriggerInputH\x00\x12%\n\x1btrigger_input_connector_raw\x18\x03 \x01(\x11H\x00\x12=\n\x16trigger_input_bus_line\x18\x04 \x01(\x0e\x32\x1b.niswitch_grpc.TriggerInputH\x01\x12$\n\x1atrigger_input_bus_line_raw\x18\x05 \x01(\x11H\x01\x12\x0e\n\x06invert\x18\x06 \x01(\x08\x42\x1e\n\x1ctrigger_input_connector_enumB\x1d\n\x1btrigger_input_bus_line_enum\"+\n\x19RouteTriggerInputResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xac\x01\n\x0bScanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x10\n\x08scanlist\x18\x02 \x01(\t\x12:\n\ninitiation\x18\x03 \x01(\x0e\x32$.niswitch_grpc.HandshakingInitiationH\x00\x12\x18\n\x0einitiation_raw\x18\x04 \x01(\x11H\x00\x42\x11\n\x0finitiation_enum\"\x1e\n\x0cScanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"5\n\x0fSelfTestRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"W\n\x10SelfTestResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x18\n\x10self_test_result\x18\x02 \x01(\x11\x12\x19\n\x11self_test_message\x18\x03 \x01(\t\"@\n\x1aSendSoftwareTriggerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"-\n\x1bSendSoftwareTriggerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa9\x01\n\x1cSetAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\x12\x17\n\x0f\x61ttribute_value\x18\x04 \x01(\x08\"/\n\x1dSetAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8d\x02\n\x1aSetAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\x12\x1d\n\x13\x61ttribute_value_raw\x18\x04 \x01(\x11H\x00\x12\x46\n\x0f\x61ttribute_value\x18\x05 \x01(\x0e\x32+.niswitch_grpc.NiSwitchInt32AttributeValuesH\x00\x42\x16\n\x14\x61ttribute_value_enum\"-\n\x1bSetAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xac\x01\n\x1bSetAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\x12\x1b\n\x13\x61ttribute_value_raw\x18\x04 \x01(\x01\".\n\x1cSetAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xc1\x01\n\x1cSetAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\x12/\n\x0f\x61ttribute_value\x18\x04 \x01(\x0b\x32\x16.nidevice_grpc.Session\"/\n\x1dSetAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xac\x01\n\x1bSetAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x36\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32 .niswitch_grpc.NiSwitchAttribute\x12\x1b\n\x13\x61ttribute_value_raw\x18\x04 \x01(\t\".\n\x1cSetAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"W\n\x18SetContinuousScanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x17\n\x0f\x63ontinuous_scan\x18\x02 \x01(\x08\"+\n\x19SetContinuousScanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"G\n\x0eSetPathRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x11\n\tpath_list\x18\x02 \x01(\t\"!\n\x0fSetPathResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"U\n\x16WaitForDebounceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x17\n\x0fmaximum_time_ms\x18\x02 \x01(\x11\")\n\x17WaitForDebounceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"Y\n\x1aWaitForScanCompleteRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x17\n\x0fmaximum_time_ms\x18\x02 \x01(\x11\"-\n\x1bWaitForScanCompleteResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05*\xb0\x17\n\x11NiSwitchAttribute\x12\"\n\x1eNISWITCH_ATTRIBUTE_UNSPECIFIED\x10\x00\x12$\n\x1eNISWITCH_ATTRIBUTE_RANGE_CHECK\x10\x92\x8b@\x12\x30\n*NISWITCH_ATTRIBUTE_QUERY_INSTRUMENT_STATUS\x10\x93\x8b@\x12\x1e\n\x18NISWITCH_ATTRIBUTE_CACHE\x10\x94\x8b@\x12!\n\x1bNISWITCH_ATTRIBUTE_SIMULATE\x10\x95\x8b@\x12)\n#NISWITCH_ATTRIBUTE_RECORD_COERCIONS\x10\x96\x8b@\x12%\n\x1fNISWITCH_ATTRIBUTE_DRIVER_SETUP\x10\x97\x8b@\x12*\n$NISWITCH_ATTRIBUTE_INTERCHANGE_CHECK\x10\xa5\x8b@\x12&\n NISWITCH_ATTRIBUTE_CHANNEL_COUNT\x10\xdb\x8c@\x12/\n)NISWITCH_ATTRIBUTE_SPECIFIC_DRIVER_PREFIX\x10\xbe\x8d@\x12/\n)NISWITCH_ATTRIBUTE_IO_RESOURCE_DESCRIPTOR\x10\xc0\x8d@\x12%\n\x1fNISWITCH_ATTRIBUTE_LOGICAL_NAME\x10\xc1\x8d@\x12\x34\n.NISWITCH_ATTRIBUTE_SUPPORTED_INSTRUMENT_MODELS\x10\xd7\x8d@\x12+\n%NISWITCH_ATTRIBUTE_GROUP_CAPABILITIES\x10\xa1\x8e@\x12\x35\n/NISWITCH_ATTRIBUTE_INSTRUMENT_FIRMWARE_REVISION\x10\x8e\x8f@\x12\x30\n*NISWITCH_ATTRIBUTE_INSTRUMENT_MANUFACTURER\x10\x8f\x8f@\x12)\n#NISWITCH_ATTRIBUTE_INSTRUMENT_MODEL\x10\x90\x8f@\x12/\n)NISWITCH_ATTRIBUTE_SPECIFIC_DRIVER_VENDOR\x10\x91\x8f@\x12\x34\n.NISWITCH_ATTRIBUTE_SPECIFIC_DRIVER_DESCRIPTION\x10\x92\x8f@\x12\x41\n;NISWITCH_ATTRIBUTE_SPECIFIC_DRIVER_CLASS_SPEC_MAJOR_VERSION\x10\x93\x8f@\x12\x41\n;NISWITCH_ATTRIBUTE_SPECIFIC_DRIVER_CLASS_SPEC_MINOR_VERSION\x10\x94\x8f@\x12\x31\n+NISWITCH_ATTRIBUTE_SPECIFIC_DRIVER_REVISION\x10\xb7\x8f@\x12*\n$NISWITCH_ATTRIBUTE_SERIAL_NUMBER_I32\x10\xb1\x98\x46\x12,\n&NISWITCH_ATTRIBUTE_IS_WAITING_FOR_TRIG\x10\xb4\x98\x46\x12%\n\x1fNISWITCH_ATTRIBUTE_TRIGGER_MODE\x10\xb5\x98\x46\x12\x31\n+NISWITCH_ATTRIBUTE_MASTER_SLAVE_TRIGGER_BUS\x10\xb6\x98\x46\x12\x37\n1NISWITCH_ATTRIBUTE_MASTER_SLAVE_SCAN_ADVANCED_BUS\x10\xb7\x98\x46\x12\x32\n,NISWITCH_ATTRIBUTE_CABLED_MODULE_TRIGGER_BUS\x10\xb8\x98\x46\x12\x38\n2NISWITCH_ATTRIBUTE_CABLED_MODULE_SCAN_ADVANCED_BUS\x10\xb9\x98\x46\x12/\n)NISWITCH_ATTRIBUTE_TRIGGER_INPUT_POLARITY\x10\xba\x98\x46\x12/\n)NISWITCH_ATTRIBUTE_SCAN_ADVANCED_POLARITY\x10\xbb\x98\x46\x12)\n#NISWITCH_ATTRIBUTE_PARSED_SCAN_LIST\x10\xbc\x98\x46\x12/\n)NISWITCH_ATTRIBUTE_HANDSHAKING_INITIATION\x10\xbd\x98\x46\x12)\n#NISWITCH_ATTRIBUTE_NUMBER_OF_RELAYS\x10\xbe\x98\x46\x12&\n NISWITCH_ATTRIBUTE_SERIAL_NUMBER\x10\xbf\x98\x46\x12.\n(NISWITCH_ATTRIBUTE_DIGITAL_FILTER_ENABLE\x10\xc0\x98\x46\x12\x42\n<NISWITCH_ATTRIBUTE_POWER_DOWN_LATCHING_RELAYS_AFTER_DEBOUNCE\x10\xc1\x98\x46\x12\x32\n,NISWITCH_ATTRIBUTE_ANALOG_BUS_SHARING_ENABLE\x10\xc2\x98\x46\x12$\n\x1eNISWITCH_ATTRIBUTE_TEMPERATURE\x10\xc3\x98\x46\x12*\n$NISWITCH_ATTRIBUTE_IS_SOURCE_CHANNEL\x10\xd1\xa5L\x12%\n\x1fNISWITCH_ATTRIBUTE_IS_DEBOUNCED\x10\xd2\xa5L\x12\x31\n+NISWITCH_ATTRIBUTE_IS_CONFIGURATION_CHANNEL\x10\xd3\xa5L\x12&\n NISWITCH_ATTRIBUTE_SETTLING_TIME\x10\xd4\xa5L\x12\"\n\x1cNISWITCH_ATTRIBUTE_BANDWIDTH\x10\xd5\xa5L\x12\'\n!NISWITCH_ATTRIBUTE_MAX_DC_VOLTAGE\x10\xd6\xa5L\x12\'\n!NISWITCH_ATTRIBUTE_MAX_AC_VOLTAGE\x10\xd7\xa5L\x12\x31\n+NISWITCH_ATTRIBUTE_MAX_SWITCHING_DC_CURRENT\x10\xd8\xa5L\x12\x31\n+NISWITCH_ATTRIBUTE_MAX_SWITCHING_AC_CURRENT\x10\xd9\xa5L\x12-\n\'NISWITCH_ATTRIBUTE_MAX_CARRY_DC_CURRENT\x10\xda\xa5L\x12-\n\'NISWITCH_ATTRIBUTE_MAX_CARRY_AC_CURRENT\x10\xdb\xa5L\x12/\n)NISWITCH_ATTRIBUTE_MAX_SWITCHING_DC_POWER\x10\xdc\xa5L\x12/\n)NISWITCH_ATTRIBUTE_MAX_SWITCHING_AC_POWER\x10\xdd\xa5L\x12+\n%NISWITCH_ATTRIBUTE_MAX_CARRY_DC_POWER\x10\xde\xa5L\x12+\n%NISWITCH_ATTRIBUTE_MAX_CARRY_AC_POWER\x10\xdf\xa5L\x12\x31\n+NISWITCH_ATTRIBUTE_CHARACTERISTIC_IMPEDANCE\x10\xe0\xa5L\x12\"\n\x1cNISWITCH_ATTRIBUTE_WIRE_MODE\x10\xe1\xa5L\x12$\n\x1eNISWITCH_ATTRIBUTE_NUM_OF_ROWS\x10\xe2\xa5L\x12\'\n!NISWITCH_ATTRIBUTE_NUM_OF_COLUMNS\x10\xe3\xa5L\x12\"\n\x1cNISWITCH_ATTRIBUTE_SCAN_LIST\x10\xe4\xa5L\x12\"\n\x1cNISWITCH_ATTRIBUTE_SCAN_MODE\x10\xe5\xa5L\x12&\n NISWITCH_ATTRIBUTE_TRIGGER_INPUT\x10\xe6\xa5L\x12-\n\'NISWITCH_ATTRIBUTE_SCAN_ADVANCED_OUTPUT\x10\xe7\xa5L\x12$\n\x1eNISWITCH_ATTRIBUTE_IS_SCANNING\x10\xe8\xa5L\x12#\n\x1dNISWITCH_ATTRIBUTE_SCAN_DELAY\x10\xe9\xa5L\x12(\n\"NISWITCH_ATTRIBUTE_CONTINUOUS_SCAN\x10\xea\xa5L*\x97\x01\n\x15HandshakingInitiation\x12\x44\n@HANDSHAKING_INITIATION_NISWITCH_VAL_MEASUREMENT_DEVICE_INITIATED\x10\x00\x12\x38\n4HANDSHAKING_INITIATION_NISWITCH_VAL_SWITCH_INITIATED\x10\x01*\xad(\n\x1cNiSwitchInt32AttributeValues\x12\x1e\n\x1aNISWITCH_INT32_UNSPECIFIED\x10\x00\x12J\nFNISWITCH_INT32_HANDSHAKING_INITIATION_VAL_MEASUREMENT_DEVICE_INITIATED\x10\x00\x12>\n:NISWITCH_INT32_HANDSHAKING_INITIATION_VAL_SWITCH_INITIATED\x10\x01\x12\x30\n,NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_NONE\x10\x00\x12\x34\n0NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_EXTERNAL\x10\x02\x12\x30\n,NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_TTL0\x10o\x12\x30\n,NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_TTL1\x10p\x12\x30\n,NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_TTL2\x10q\x12\x30\n,NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_TTL3\x10r\x12\x30\n,NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_TTL4\x10s\x12\x30\n,NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_TTL5\x10t\x12\x30\n,NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_TTL6\x10u\x12\x30\n,NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_TTL7\x10v\x12\x34\n0NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_PXI_STAR\x10}\x12:\n5NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR\x10\xe8\x07\x12;\n6NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR\x10\xe9\x07\x12\x42\n=NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE1\x10\xfd\x07\x12\x42\n=NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE2\x10\xfe\x07\x12\x42\n=NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE3\x10\xff\x07\x12\x42\n=NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE4\x10\x80\x08\x12\x42\n=NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE5\x10\x81\x08\x12\x42\n=NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE6\x10\x82\x08\x12\x42\n=NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE7\x10\x83\x08\x12\x42\n=NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE8\x10\x84\x08\x12\x42\n=NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE9\x10\x85\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE10\x10\x86\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE11\x10\x87\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_REARCONNECTOR_MODULE12\x10\x88\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE1\x10\x91\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE2\x10\x92\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE3\x10\x93\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE4\x10\x94\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE5\x10\x95\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE6\x10\x96\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE7\x10\x97\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE8\x10\x98\x08\x12\x43\n>NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE9\x10\x99\x08\x12\x44\n?NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE10\x10\x9a\x08\x12\x44\n?NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE11\x10\x9b\x08\x12\x44\n?NISWITCH_INT32_SCAN_ADVANCED_OUTPUT_VAL_FRONTCONNECTOR_MODULE12\x10\x9c\x08\x12\x39\n5NISWITCH_INT32_SCAN_ADVANCED_POLARITY_VAL_RISING_EDGE\x10\x00\x12:\n6NISWITCH_INT32_SCAN_ADVANCED_POLARITY_VAL_FALLING_EDGE\x10\x01\x12%\n!NISWITCH_INT32_SCAN_MODE_VAL_NONE\x10\x00\x12\x32\n.NISWITCH_INT32_SCAN_MODE_VAL_BREAK_BEFORE_MAKE\x10\x01\x12\x31\n-NISWITCH_INT32_SCAN_MODE_VAL_BREAK_AFTER_MAKE\x10\x02\x12.\n*NISWITCH_INT32_TRIGGER_INPUT_VAL_IMMEDIATE\x10\x01\x12-\n)NISWITCH_INT32_TRIGGER_INPUT_VAL_EXTERNAL\x10\x02\x12\x32\n.NISWITCH_INT32_TRIGGER_INPUT_VAL_SOFTWARE_TRIG\x10\x03\x12)\n%NISWITCH_INT32_TRIGGER_INPUT_VAL_TTL0\x10o\x12)\n%NISWITCH_INT32_TRIGGER_INPUT_VAL_TTL1\x10p\x12)\n%NISWITCH_INT32_TRIGGER_INPUT_VAL_TTL2\x10q\x12)\n%NISWITCH_INT32_TRIGGER_INPUT_VAL_TTL3\x10r\x12)\n%NISWITCH_INT32_TRIGGER_INPUT_VAL_TTL4\x10s\x12)\n%NISWITCH_INT32_TRIGGER_INPUT_VAL_TTL5\x10t\x12)\n%NISWITCH_INT32_TRIGGER_INPUT_VAL_TTL6\x10u\x12)\n%NISWITCH_INT32_TRIGGER_INPUT_VAL_TTL7\x10v\x12-\n)NISWITCH_INT32_TRIGGER_INPUT_VAL_PXI_STAR\x10}\x12\x33\n.NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR\x10\xe8\x07\x12\x34\n/NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR\x10\xe9\x07\x12;\n6NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE1\x10\xfd\x07\x12;\n6NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE2\x10\xfe\x07\x12;\n6NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE3\x10\xff\x07\x12;\n6NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE4\x10\x80\x08\x12;\n6NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE5\x10\x81\x08\x12;\n6NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE6\x10\x82\x08\x12;\n6NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE7\x10\x83\x08\x12;\n6NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE8\x10\x84\x08\x12;\n6NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE9\x10\x85\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE10\x10\x86\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE11\x10\x87\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_REARCONNECTOR_MODULE12\x10\x88\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE1\x10\x91\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE2\x10\x92\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE3\x10\x93\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE4\x10\x94\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE5\x10\x95\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE6\x10\x96\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE7\x10\x97\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE8\x10\x98\x08\x12<\n7NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE9\x10\x99\x08\x12=\n8NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE10\x10\x9a\x08\x12=\n8NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE11\x10\x9b\x08\x12=\n8NISWITCH_INT32_TRIGGER_INPUT_VAL_FRONTCONNECTOR_MODULE12\x10\x9c\x08\x12\x39\n5NISWITCH_INT32_TRIGGER_INPUT_POLARITY_VAL_RISING_EDGE\x10\x00\x12:\n6NISWITCH_INT32_TRIGGER_INPUT_POLARITY_VAL_FALLING_EDGE\x10\x01\x12\'\n#NISWITCH_INT32_WIRE_MODE_VAL_1_WIRE\x10\x01\x12\'\n#NISWITCH_INT32_WIRE_MODE_VAL_2_WIRE\x10\x02\x12\'\n#NISWITCH_INT32_WIRE_MODE_VAL_4_WIRE\x10\x04\x1a\x02\x10\x01*\xdf\x02\n\x0ePathCapability\x12\x1f\n\x1bPATH_CAPABILITY_UNSPECIFIED\x10\x00\x12/\n+PATH_CAPABILITY_NISWITCH_VAL_PATH_AVAILABLE\x10\x01\x12,\n(PATH_CAPABILITY_NISWITCH_VAL_PATH_EXISTS\x10\x02\x12\x31\n-PATH_CAPABILITY_NISWITCH_VAL_PATH_UNSUPPORTED\x10\x03\x12\x30\n,PATH_CAPABILITY_NISWITCH_VAL_RESOURCE_IN_USE\x10\x04\x12\x30\n,PATH_CAPABILITY_NISWITCH_VAL_SOURCE_CONFLICT\x10\x05\x12\x36\n2PATH_CAPABILITY_NISWITCH_VAL_CHANNEL_NOT_AVAILABLE\x10\x06*\x80\x01\n\x0bRelayAction\x12\x1c\n\x18RELAY_ACTION_UNSPECIFIED\x10\x00\x12(\n$RELAY_ACTION_NISWITCH_VAL_OPEN_RELAY\x10\x14\x12)\n%RELAY_ACTION_NISWITCH_VAL_CLOSE_RELAY\x10\x15*}\n\rRelayPosition\x12\x1e\n\x1aRELAY_POSITION_UNSPECIFIED\x10\x00\x12$\n RELAY_POSITION_NISWITCH_VAL_OPEN\x10\n\x12&\n\"RELAY_POSITION_NISWITCH_VAL_CLOSED\x10\x0b*\xcf\x10\n\x12ScanAdvancedOutput\x12*\n&SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_NONE\x10\x00\x12.\n*SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_EXTERNAL\x10\x02\x12*\n&SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_TTL0\x10o\x12*\n&SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_TTL1\x10p\x12*\n&SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_TTL2\x10q\x12*\n&SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_TTL3\x10r\x12*\n&SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_TTL4\x10s\x12*\n&SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_TTL5\x10t\x12*\n&SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_TTL6\x10u\x12*\n&SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_TTL7\x10v\x12.\n*SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_PXI_STAR\x10}\x12\x34\n/SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR\x10\xe8\x07\x12\x35\n0SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR\x10\xe9\x07\x12<\n7SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE1\x10\xfd\x07\x12<\n7SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE2\x10\xfe\x07\x12<\n7SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE3\x10\xff\x07\x12<\n7SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE4\x10\x80\x08\x12<\n7SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE5\x10\x81\x08\x12<\n7SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE6\x10\x82\x08\x12<\n7SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE7\x10\x83\x08\x12<\n7SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE8\x10\x84\x08\x12<\n7SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE9\x10\x85\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE10\x10\x86\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE11\x10\x87\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_REARCONNECTOR_MODULE12\x10\x88\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE1\x10\x91\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE2\x10\x92\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE3\x10\x93\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE4\x10\x94\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE5\x10\x95\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE6\x10\x96\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE7\x10\x97\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE8\x10\x98\x08\x12=\n8SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE9\x10\x99\x08\x12>\n9SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE10\x10\x9a\x08\x12>\n9SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE11\x10\x9b\x08\x12>\n9SCAN_ADVANCED_OUTPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE12\x10\x9c\x08*\x86\x01\n\x08ScanMode\x12\x1f\n\x1bSCAN_MODE_NISWITCH_VAL_NONE\x10\x00\x12,\n(SCAN_MODE_NISWITCH_VAL_BREAK_BEFORE_MAKE\x10\x01\x12+\n\'SCAN_MODE_NISWITCH_VAL_BREAK_AFTER_MAKE\x10\x02*\x98\x0f\n\x0cTriggerInput\x12\x1d\n\x19TRIGGER_INPUT_UNSPECIFIED\x10\x00\x12(\n$TRIGGER_INPUT_NISWITCH_VAL_IMMEDIATE\x10\x01\x12\'\n#TRIGGER_INPUT_NISWITCH_VAL_EXTERNAL\x10\x02\x12,\n(TRIGGER_INPUT_NISWITCH_VAL_SOFTWARE_TRIG\x10\x03\x12#\n\x1fTRIGGER_INPUT_NISWITCH_VAL_TTL0\x10o\x12#\n\x1fTRIGGER_INPUT_NISWITCH_VAL_TTL1\x10p\x12#\n\x1fTRIGGER_INPUT_NISWITCH_VAL_TTL2\x10q\x12#\n\x1fTRIGGER_INPUT_NISWITCH_VAL_TTL3\x10r\x12#\n\x1fTRIGGER_INPUT_NISWITCH_VAL_TTL4\x10s\x12#\n\x1fTRIGGER_INPUT_NISWITCH_VAL_TTL5\x10t\x12#\n\x1fTRIGGER_INPUT_NISWITCH_VAL_TTL6\x10u\x12#\n\x1fTRIGGER_INPUT_NISWITCH_VAL_TTL7\x10v\x12\'\n#TRIGGER_INPUT_NISWITCH_VAL_PXI_STAR\x10}\x12-\n(TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR\x10\xe8\x07\x12.\n)TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR\x10\xe9\x07\x12\x35\n0TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE1\x10\xfd\x07\x12\x35\n0TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE2\x10\xfe\x07\x12\x35\n0TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE3\x10\xff\x07\x12\x35\n0TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE4\x10\x80\x08\x12\x35\n0TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE5\x10\x81\x08\x12\x35\n0TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE6\x10\x82\x08\x12\x35\n0TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE7\x10\x83\x08\x12\x35\n0TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE8\x10\x84\x08\x12\x35\n0TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE9\x10\x85\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE10\x10\x86\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE11\x10\x87\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_REARCONNECTOR_MODULE12\x10\x88\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE1\x10\x91\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE2\x10\x92\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE3\x10\x93\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE4\x10\x94\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE5\x10\x95\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE6\x10\x96\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE7\x10\x97\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE8\x10\x98\x08\x12\x36\n1TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE9\x10\x99\x08\x12\x37\n2TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE10\x10\x9a\x08\x12\x37\n2TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE11\x10\x9b\x08\x12\x37\n2TRIGGER_INPUT_NISWITCH_VAL_FRONTCONNECTOR_MODULE12\x10\x9c\x08\x32\xa0.\n\x08NiSwitch\x12N\n\tAbortScan\x12\x1f.niswitch_grpc.AbortScanRequest\x1a .niswitch_grpc.AbortScanResponse\x12Q\n\nCanConnect\x12 .niswitch_grpc.CanConnectRequest\x1a!.niswitch_grpc.CanConnectResponse\x12x\n\x17\x43heckAttributeViBoolean\x12-.niswitch_grpc.CheckAttributeViBooleanRequest\x1a..niswitch_grpc.CheckAttributeViBooleanResponse\x12r\n\x15\x43heckAttributeViInt32\x12+.niswitch_grpc.CheckAttributeViInt32Request\x1a,.niswitch_grpc.CheckAttributeViInt32Response\x12u\n\x16\x43heckAttributeViReal64\x12,.niswitch_grpc.CheckAttributeViReal64Request\x1a-.niswitch_grpc.CheckAttributeViReal64Response\x12x\n\x17\x43heckAttributeViSession\x12-.niswitch_grpc.CheckAttributeViSessionRequest\x1a..niswitch_grpc.CheckAttributeViSessionResponse\x12u\n\x16\x43heckAttributeViString\x12,.niswitch_grpc.CheckAttributeViStringRequest\x1a-.niswitch_grpc.CheckAttributeViStringResponse\x12Q\n\nClearError\x12 .niswitch_grpc.ClearErrorRequest\x1a!.niswitch_grpc.ClearErrorResponse\x12{\n\x18\x43learInterchangeWarnings\x12..niswitch_grpc.ClearInterchangeWarningsRequest\x1a/.niswitch_grpc.ClearInterchangeWarningsResponse\x12\x42\n\x05\x43lose\x12\x1b.niswitch_grpc.CloseRequest\x1a\x1c.niswitch_grpc.CloseResponse\x12\x45\n\x06\x43ommit\x12\x1c.niswitch_grpc.CommitRequest\x1a\x1d.niswitch_grpc.CommitResponse\x12\x66\n\x11\x43onfigureScanList\x12\'.niswitch_grpc.ConfigureScanListRequest\x1a(.niswitch_grpc.ConfigureScanListResponse\x12o\n\x14\x43onfigureScanTrigger\x12*.niswitch_grpc.ConfigureScanTriggerRequest\x1a+.niswitch_grpc.ConfigureScanTriggerResponse\x12H\n\x07\x43onnect\x12\x1d.niswitch_grpc.ConnectRequest\x1a\x1e.niswitch_grpc.ConnectResponse\x12`\n\x0f\x43onnectMultiple\x12%.niswitch_grpc.ConnectMultipleRequest\x1a&.niswitch_grpc.ConnectMultipleResponse\x12H\n\x07\x44isable\x12\x1d.niswitch_grpc.DisableRequest\x1a\x1e.niswitch_grpc.DisableResponse\x12Q\n\nDisconnect\x12 .niswitch_grpc.DisconnectRequest\x1a!.niswitch_grpc.DisconnectResponse\x12Z\n\rDisconnectAll\x12#.niswitch_grpc.DisconnectAllRequest\x1a$.niswitch_grpc.DisconnectAllResponse\x12i\n\x12\x44isconnectMultiple\x12(.niswitch_grpc.DisconnectMultipleRequest\x1a).niswitch_grpc.DisconnectMultipleResponse\x12W\n\x0c\x45rrorMessage\x12\".niswitch_grpc.ErrorMessageRequest\x1a#.niswitch_grpc.ErrorMessageResponse\x12Q\n\nErrorQuery\x12 .niswitch_grpc.ErrorQueryRequest\x1a!.niswitch_grpc.ErrorQueryResponse\x12r\n\x15GetAttributeViBoolean\x12+.niswitch_grpc.GetAttributeViBooleanRequest\x1a,.niswitch_grpc.GetAttributeViBooleanResponse\x12l\n\x13GetAttributeViInt32\x12).niswitch_grpc.GetAttributeViInt32Request\x1a*.niswitch_grpc.GetAttributeViInt32Response\x12o\n\x14GetAttributeViReal64\x12*.niswitch_grpc.GetAttributeViReal64Request\x1a+.niswitch_grpc.GetAttributeViReal64Response\x12r\n\x15GetAttributeViSession\x12+.niswitch_grpc.GetAttributeViSessionRequest\x1a,.niswitch_grpc.GetAttributeViSessionResponse\x12o\n\x14GetAttributeViString\x12*.niswitch_grpc.GetAttributeViStringRequest\x1a+.niswitch_grpc.GetAttributeViStringResponse\x12]\n\x0eGetChannelName\x12$.niswitch_grpc.GetChannelNameRequest\x1a%.niswitch_grpc.GetChannelNameResponse\x12K\n\x08GetError\x12\x1e.niswitch_grpc.GetErrorRequest\x1a\x1f.niswitch_grpc.GetErrorResponse\x12r\n\x15GetNextCoercionRecord\x12+.niswitch_grpc.GetNextCoercionRecordRequest\x1a,.niswitch_grpc.GetNextCoercionRecordResponse\x12~\n\x19GetNextInterchangeWarning\x12/.niswitch_grpc.GetNextInterchangeWarningRequest\x1a\x30.niswitch_grpc.GetNextInterchangeWarningResponse\x12H\n\x07GetPath\x12\x1d.niswitch_grpc.GetPathRequest\x1a\x1e.niswitch_grpc.GetPathResponse\x12Z\n\rGetRelayCount\x12#.niswitch_grpc.GetRelayCountRequest\x1a$.niswitch_grpc.GetRelayCountResponse\x12W\n\x0cGetRelayName\x12\".niswitch_grpc.GetRelayNameRequest\x1a#.niswitch_grpc.GetRelayNameResponse\x12\x63\n\x10GetRelayPosition\x12&.niswitch_grpc.GetRelayPositionRequest\x1a\'.niswitch_grpc.GetRelayPositionResponse\x12?\n\x04Init\x12\x1a.niswitch_grpc.InitRequest\x1a\x1b.niswitch_grpc.InitResponse\x12`\n\x0fInitWithOptions\x12%.niswitch_grpc.InitWithOptionsRequest\x1a&.niswitch_grpc.InitWithOptionsResponse\x12\x63\n\x10InitWithTopology\x12&.niswitch_grpc.InitWithTopologyRequest\x1a\'.niswitch_grpc.InitWithTopologyResponse\x12W\n\x0cInitiateScan\x12\".niswitch_grpc.InitiateScanRequest\x1a#.niswitch_grpc.InitiateScanResponse\x12x\n\x17InvalidateAllAttributes\x12-.niswitch_grpc.InvalidateAllAttributesRequest\x1a..niswitch_grpc.InvalidateAllAttributesResponse\x12T\n\x0bIsDebounced\x12!.niswitch_grpc.IsDebouncedRequest\x1a\".niswitch_grpc.IsDebouncedResponse\x12Q\n\nIsScanning\x12 .niswitch_grpc.IsScanningRequest\x1a!.niswitch_grpc.IsScanningResponse\x12W\n\x0cRelayControl\x12\".niswitch_grpc.RelayControlRequest\x1a#.niswitch_grpc.RelayControlResponse\x12\x42\n\x05Reset\x12\x1b.niswitch_grpc.ResetRequest\x1a\x1c.niswitch_grpc.ResetResponse\x12r\n\x15ResetInterchangeCheck\x12+.niswitch_grpc.ResetInterchangeCheckRequest\x1a,.niswitch_grpc.ResetInterchangeCheckResponse\x12\x66\n\x11ResetWithDefaults\x12\'.niswitch_grpc.ResetWithDefaultsRequest\x1a(.niswitch_grpc.ResetWithDefaultsResponse\x12Z\n\rRevisionQuery\x12#.niswitch_grpc.RevisionQueryRequest\x1a$.niswitch_grpc.RevisionQueryResponse\x12x\n\x17RouteScanAdvancedOutput\x12-.niswitch_grpc.RouteScanAdvancedOutputRequest\x1a..niswitch_grpc.RouteScanAdvancedOutputResponse\x12\x66\n\x11RouteTriggerInput\x12\'.niswitch_grpc.RouteTriggerInputRequest\x1a(.niswitch_grpc.RouteTriggerInputResponse\x12?\n\x04Scan\x12\x1a.niswitch_grpc.ScanRequest\x1a\x1b.niswitch_grpc.ScanResponse\x12K\n\x08SelfTest\x12\x1e.niswitch_grpc.SelfTestRequest\x1a\x1f.niswitch_grpc.SelfTestResponse\x12l\n\x13SendSoftwareTrigger\x12).niswitch_grpc.SendSoftwareTriggerRequest\x1a*.niswitch_grpc.SendSoftwareTriggerResponse\x12r\n\x15SetAttributeViBoolean\x12+.niswitch_grpc.SetAttributeViBooleanRequest\x1a,.niswitch_grpc.SetAttributeViBooleanResponse\x12l\n\x13SetAttributeViInt32\x12).niswitch_grpc.SetAttributeViInt32Request\x1a*.niswitch_grpc.SetAttributeViInt32Response\x12o\n\x14SetAttributeViReal64\x12*.niswitch_grpc.SetAttributeViReal64Request\x1a+.niswitch_grpc.SetAttributeViReal64Response\x12r\n\x15SetAttributeViSession\x12+.niswitch_grpc.SetAttributeViSessionRequest\x1a,.niswitch_grpc.SetAttributeViSessionResponse\x12o\n\x14SetAttributeViString\x12*.niswitch_grpc.SetAttributeViStringRequest\x1a+.niswitch_grpc.SetAttributeViStringResponse\x12\x66\n\x11SetContinuousScan\x12\'.niswitch_grpc.SetContinuousScanRequest\x1a(.niswitch_grpc.SetContinuousScanResponse\x12H\n\x07SetPath\x12\x1d.niswitch_grpc.SetPathRequest\x1a\x1e.niswitch_grpc.SetPathResponse\x12`\n\x0fWaitForDebounce\x12%.niswitch_grpc.WaitForDebounceRequest\x1a&.niswitch_grpc.WaitForDebounceResponse\x12l\n\x13WaitForScanComplete\x12).niswitch_grpc.WaitForScanCompleteRequest\x1a*.niswitch_grpc.WaitForScanCompleteResponseBD\n\x14\x63om.ni.grpc.niswitchB\x08NiSwitchP\x01\xaa\x02\x1fNationalInstruments.Grpc.Switchb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'niswitch_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'niswitch_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\024com.ni.grpc.niswitchB\010NiSwitchP\001\252\002\037NationalInstruments.Grpc.Switch'
   _NISWITCHINT32ATTRIBUTEVALUES._options = None
   _NISWITCHINT32ATTRIBUTEVALUES._serialized_options = b'\020\001'
   _INITRESPONSE.fields_by_name['error_message']._options = None
   _INITRESPONSE.fields_by_name['error_message']._serialized_options = b'\030\001'
   _INITWITHOPTIONSRESPONSE.fields_by_name['error_message']._options = None
   _INITWITHOPTIONSRESPONSE.fields_by_name['error_message']._serialized_options = b'\030\001'
   _INITWITHTOPOLOGYRESPONSE.fields_by_name['error_message']._options = None
   _INITWITHTOPOLOGYRESPONSE.fields_by_name['error_message']._serialized_options = b'\030\001'
-  _NISWITCHATTRIBUTE._serialized_start=11126
-  _NISWITCHATTRIBUTE._serialized_end=14118
-  _HANDSHAKINGINITIATION._serialized_start=14121
-  _HANDSHAKINGINITIATION._serialized_end=14272
-  _NISWITCHINT32ATTRIBUTEVALUES._serialized_start=14275
-  _NISWITCHINT32ATTRIBUTEVALUES._serialized_end=19440
-  _PATHCAPABILITY._serialized_start=19443
-  _PATHCAPABILITY._serialized_end=19794
-  _RELAYACTION._serialized_start=19797
-  _RELAYACTION._serialized_end=19925
-  _RELAYPOSITION._serialized_start=19927
-  _RELAYPOSITION._serialized_end=20052
-  _SCANADVANCEDOUTPUT._serialized_start=20055
-  _SCANADVANCEDOUTPUT._serialized_end=22182
-  _SCANMODE._serialized_start=22185
-  _SCANMODE._serialized_end=22319
-  _TRIGGERINPUT._serialized_start=22322
-  _TRIGGERINPUT._serialized_end=24266
-  _ABORTSCANREQUEST._serialized_start=48
-  _ABORTSCANREQUEST._serialized_end=102
-  _ABORTSCANRESPONSE._serialized_start=104
-  _ABORTSCANRESPONSE._serialized_end=139
-  _CANCONNECTREQUEST._serialized_start=141
-  _CANCONNECTREQUEST._serialized_end=232
-  _CANCONNECTRESPONSE._serialized_start=234
-  _CANCONNECTRESPONSE._serialized_end=355
-  _CHECKATTRIBUTEVIBOOLEANREQUEST._serialized_start=358
-  _CHECKATTRIBUTEVIBOOLEANREQUEST._serialized_end=529
-  _CHECKATTRIBUTEVIBOOLEANRESPONSE._serialized_start=531
-  _CHECKATTRIBUTEVIBOOLEANRESPONSE._serialized_end=580
-  _CHECKATTRIBUTEVIINT32REQUEST._serialized_start=583
-  _CHECKATTRIBUTEVIINT32REQUEST._serialized_end=854
-  _CHECKATTRIBUTEVIINT32RESPONSE._serialized_start=856
-  _CHECKATTRIBUTEVIINT32RESPONSE._serialized_end=903
-  _CHECKATTRIBUTEVIREAL64REQUEST._serialized_start=906
-  _CHECKATTRIBUTEVIREAL64REQUEST._serialized_end=1080
-  _CHECKATTRIBUTEVIREAL64RESPONSE._serialized_start=1082
-  _CHECKATTRIBUTEVIREAL64RESPONSE._serialized_end=1130
-  _CHECKATTRIBUTEVISESSIONREQUEST._serialized_start=1133
-  _CHECKATTRIBUTEVISESSIONREQUEST._serialized_end=1328
-  _CHECKATTRIBUTEVISESSIONRESPONSE._serialized_start=1330
-  _CHECKATTRIBUTEVISESSIONRESPONSE._serialized_end=1379
-  _CHECKATTRIBUTEVISTRINGREQUEST._serialized_start=1382
-  _CHECKATTRIBUTEVISTRINGREQUEST._serialized_end=1556
-  _CHECKATTRIBUTEVISTRINGRESPONSE._serialized_start=1558
-  _CHECKATTRIBUTEVISTRINGRESPONSE._serialized_end=1606
-  _CLEARERRORREQUEST._serialized_start=1608
-  _CLEARERRORREQUEST._serialized_end=1663
-  _CLEARERRORRESPONSE._serialized_start=1665
-  _CLEARERRORRESPONSE._serialized_end=1701
-  _CLEARINTERCHANGEWARNINGSREQUEST._serialized_start=1703
-  _CLEARINTERCHANGEWARNINGSREQUEST._serialized_end=1772
-  _CLEARINTERCHANGEWARNINGSRESPONSE._serialized_start=1774
-  _CLEARINTERCHANGEWARNINGSRESPONSE._serialized_end=1824
-  _CLOSEREQUEST._serialized_start=1826
-  _CLOSEREQUEST._serialized_end=1876
-  _CLOSERESPONSE._serialized_start=1878
-  _CLOSERESPONSE._serialized_end=1909
-  _COMMITREQUEST._serialized_start=1911
-  _COMMITREQUEST._serialized_end=1962
-  _COMMITRESPONSE._serialized_start=1964
-  _COMMITRESPONSE._serialized_end=1996
-  _CONFIGURESCANLISTREQUEST._serialized_start=1999
-  _CONFIGURESCANLISTREQUEST._serialized_end=2168
-  _CONFIGURESCANLISTRESPONSE._serialized_start=2170
-  _CONFIGURESCANLISTRESPONSE._serialized_end=2213
-  _CONFIGURESCANTRIGGERREQUEST._serialized_start=2216
-  _CONFIGURESCANTRIGGERREQUEST._serialized_end=2538
-  _CONFIGURESCANTRIGGERRESPONSE._serialized_start=2540
-  _CONFIGURESCANTRIGGERRESPONSE._serialized_end=2586
-  _CONNECTREQUEST._serialized_start=2588
-  _CONNECTREQUEST._serialized_end=2676
-  _CONNECTRESPONSE._serialized_start=2678
-  _CONNECTRESPONSE._serialized_end=2711
-  _CONNECTMULTIPLEREQUEST._serialized_start=2713
-  _CONNECTMULTIPLEREQUEST._serialized_end=2798
-  _CONNECTMULTIPLERESPONSE._serialized_start=2800
-  _CONNECTMULTIPLERESPONSE._serialized_end=2841
-  _DISABLEREQUEST._serialized_start=2843
-  _DISABLEREQUEST._serialized_end=2895
-  _DISABLERESPONSE._serialized_start=2897
-  _DISABLERESPONSE._serialized_end=2930
-  _DISCONNECTREQUEST._serialized_start=2932
-  _DISCONNECTREQUEST._serialized_end=3023
-  _DISCONNECTRESPONSE._serialized_start=3025
-  _DISCONNECTRESPONSE._serialized_end=3061
-  _DISCONNECTALLREQUEST._serialized_start=3063
-  _DISCONNECTALLREQUEST._serialized_end=3121
-  _DISCONNECTALLRESPONSE._serialized_start=3123
-  _DISCONNECTALLRESPONSE._serialized_end=3162
-  _DISCONNECTMULTIPLEREQUEST._serialized_start=3164
-  _DISCONNECTMULTIPLEREQUEST._serialized_end=3255
-  _DISCONNECTMULTIPLERESPONSE._serialized_start=3257
-  _DISCONNECTMULTIPLERESPONSE._serialized_end=3301
-  _ERRORMESSAGEREQUEST._serialized_start=3303
-  _ERRORMESSAGEREQUEST._serialized_end=3380
-  _ERRORMESSAGERESPONSE._serialized_start=3382
-  _ERRORMESSAGERESPONSE._serialized_end=3443
-  _ERRORQUERYREQUEST._serialized_start=3445
-  _ERRORQUERYREQUEST._serialized_end=3500
-  _ERRORQUERYRESPONSE._serialized_start=3502
-  _ERRORQUERYRESPONSE._serialized_end=3581
-  _GETATTRIBUTEVIBOOLEANREQUEST._serialized_start=3584
-  _GETATTRIBUTEVIBOOLEANREQUEST._serialized_end=3728
-  _GETATTRIBUTEVIBOOLEANRESPONSE._serialized_start=3730
-  _GETATTRIBUTEVIBOOLEANRESPONSE._serialized_end=3802
-  _GETATTRIBUTEVIINT32REQUEST._serialized_start=3805
-  _GETATTRIBUTEVIINT32REQUEST._serialized_end=3947
-  _GETATTRIBUTEVIINT32RESPONSE._serialized_start=3949
-  _GETATTRIBUTEVIINT32RESPONSE._serialized_end=4019
-  _GETATTRIBUTEVIREAL64REQUEST._serialized_start=4022
-  _GETATTRIBUTEVIREAL64REQUEST._serialized_end=4165
-  _GETATTRIBUTEVIREAL64RESPONSE._serialized_start=4167
-  _GETATTRIBUTEVIREAL64RESPONSE._serialized_end=4238
-  _GETATTRIBUTEVISESSIONREQUEST._serialized_start=4241
-  _GETATTRIBUTEVISESSIONREQUEST._serialized_end=4385
-  _GETATTRIBUTEVISESSIONRESPONSE._serialized_start=4387
-  _GETATTRIBUTEVISESSIONRESPONSE._serialized_end=4483
-  _GETATTRIBUTEVISTRINGREQUEST._serialized_start=4486
-  _GETATTRIBUTEVISTRINGREQUEST._serialized_end=4629
-  _GETATTRIBUTEVISTRINGRESPONSE._serialized_start=4631
-  _GETATTRIBUTEVISTRINGRESPONSE._serialized_end=4702
-  _GETCHANNELNAMEREQUEST._serialized_start=4704
-  _GETCHANNELNAMEREQUEST._serialized_end=4778
-  _GETCHANNELNAMERESPONSE._serialized_start=4780
-  _GETCHANNELNAMERESPONSE._serialized_end=4849
-  _GETERRORREQUEST._serialized_start=4851
-  _GETERRORREQUEST._serialized_end=4904
-  _GETERRORRESPONSE._serialized_start=4906
-  _GETERRORRESPONSE._serialized_end=4975
-  _GETNEXTCOERCIONRECORDREQUEST._serialized_start=4977
-  _GETNEXTCOERCIONRECORDREQUEST._serialized_end=5043
-  _GETNEXTCOERCIONRECORDRESPONSE._serialized_start=5045
-  _GETNEXTCOERCIONRECORDRESPONSE._serialized_end=5117
-  _GETNEXTINTERCHANGEWARNINGREQUEST._serialized_start=5119
-  _GETNEXTINTERCHANGEWARNINGREQUEST._serialized_end=5189
-  _GETNEXTINTERCHANGEWARNINGRESPONSE._serialized_start=5191
-  _GETNEXTINTERCHANGEWARNINGRESPONSE._serialized_end=5271
-  _GETPATHREQUEST._serialized_start=5273
-  _GETPATHREQUEST._serialized_end=5361
-  _GETPATHRESPONSE._serialized_start=5363
-  _GETPATHRESPONSE._serialized_end=5410
-  _GETRELAYCOUNTREQUEST._serialized_start=5412
-  _GETRELAYCOUNTREQUEST._serialized_end=5490
-  _GETRELAYCOUNTRESPONSE._serialized_start=5492
-  _GETRELAYCOUNTRESPONSE._serialized_end=5552
-  _GETRELAYNAMEREQUEST._serialized_start=5554
-  _GETRELAYNAMEREQUEST._serialized_end=5626
-  _GETRELAYNAMERESPONSE._serialized_start=5628
-  _GETRELAYNAMERESPONSE._serialized_end=5693
-  _GETRELAYPOSITIONREQUEST._serialized_start=5695
-  _GETRELAYPOSITIONREQUEST._serialized_end=5776
-  _GETRELAYPOSITIONRESPONSE._serialized_start=5778
-  _GETRELAYPOSITIONRESPONSE._serialized_end=5902
-  _INITREQUEST._serialized_start=5905
-  _INITREQUEST._serialized_end=6082
-  _INITRESPONSE._serialized_start=6084
-  _INITRESPONSE._serialized_end=6210
-  _INITWITHOPTIONSREQUEST._serialized_start=6213
-  _INITWITHOPTIONSREQUEST._serialized_end=6424
-  _INITWITHOPTIONSRESPONSE._serialized_start=6427
-  _INITWITHOPTIONSRESPONSE._serialized_end=6564
-  _INITWITHTOPOLOGYREQUEST._serialized_start=6567
-  _INITWITHTOPOLOGYREQUEST._serialized_end=6774
-  _INITWITHTOPOLOGYRESPONSE._serialized_start=6777
-  _INITWITHTOPOLOGYRESPONSE._serialized_end=6915
-  _INITIATESCANREQUEST._serialized_start=6917
-  _INITIATESCANREQUEST._serialized_end=6974
-  _INITIATESCANRESPONSE._serialized_start=6976
-  _INITIATESCANRESPONSE._serialized_end=7014
-  _INVALIDATEALLATTRIBUTESREQUEST._serialized_start=7016
-  _INVALIDATEALLATTRIBUTESREQUEST._serialized_end=7084
-  _INVALIDATEALLATTRIBUTESRESPONSE._serialized_start=7086
-  _INVALIDATEALLATTRIBUTESRESPONSE._serialized_end=7135
-  _ISDEBOUNCEDREQUEST._serialized_start=7137
-  _ISDEBOUNCEDREQUEST._serialized_end=7193
-  _ISDEBOUNCEDRESPONSE._serialized_start=7195
-  _ISDEBOUNCEDRESPONSE._serialized_end=7254
-  _ISSCANNINGREQUEST._serialized_start=7256
-  _ISSCANNINGREQUEST._serialized_end=7311
-  _ISSCANNINGRESPONSE._serialized_start=7313
-  _ISSCANNINGRESPONSE._serialized_end=7370
-  _RELAYCONTROLREQUEST._serialized_start=7373
-  _RELAYCONTROLREQUEST._serialized_end=7551
-  _RELAYCONTROLRESPONSE._serialized_start=7553
-  _RELAYCONTROLRESPONSE._serialized_end=7591
-  _RESETREQUEST._serialized_start=7593
-  _RESETREQUEST._serialized_end=7643
-  _RESETRESPONSE._serialized_start=7645
-  _RESETRESPONSE._serialized_end=7676
-  _RESETINTERCHANGECHECKREQUEST._serialized_start=7678
-  _RESETINTERCHANGECHECKREQUEST._serialized_end=7744
-  _RESETINTERCHANGECHECKRESPONSE._serialized_start=7746
-  _RESETINTERCHANGECHECKRESPONSE._serialized_end=7793
-  _RESETWITHDEFAULTSREQUEST._serialized_start=7795
-  _RESETWITHDEFAULTSREQUEST._serialized_end=7857
-  _RESETWITHDEFAULTSRESPONSE._serialized_start=7859
-  _RESETWITHDEFAULTSRESPONSE._serialized_end=7902
-  _REVISIONQUERYREQUEST._serialized_start=7904
-  _REVISIONQUERYREQUEST._serialized_end=7962
-  _REVISIONQUERYRESPONSE._serialized_start=7964
-  _REVISIONQUERYRESPONSE._serialized_end=8066
-  _ROUTESCANADVANCEDOUTPUTREQUEST._serialized_start=8069
-  _ROUTESCANADVANCEDOUTPUTREQUEST._serialized_end=8474
-  _ROUTESCANADVANCEDOUTPUTRESPONSE._serialized_start=8476
-  _ROUTESCANADVANCEDOUTPUTRESPONSE._serialized_end=8525
-  _ROUTETRIGGERINPUTREQUEST._serialized_start=8528
-  _ROUTETRIGGERINPUTREQUEST._serialized_end=8873
-  _ROUTETRIGGERINPUTRESPONSE._serialized_start=8875
-  _ROUTETRIGGERINPUTRESPONSE._serialized_end=8918
-  _SCANREQUEST._serialized_start=8921
-  _SCANREQUEST._serialized_end=9093
-  _SCANRESPONSE._serialized_start=9095
-  _SCANRESPONSE._serialized_end=9125
-  _SELFTESTREQUEST._serialized_start=9127
-  _SELFTESTREQUEST._serialized_end=9180
-  _SELFTESTRESPONSE._serialized_start=9182
-  _SELFTESTRESPONSE._serialized_end=9269
-  _SENDSOFTWARETRIGGERREQUEST._serialized_start=9271
-  _SENDSOFTWARETRIGGERREQUEST._serialized_end=9335
-  _SENDSOFTWARETRIGGERRESPONSE._serialized_start=9337
-  _SENDSOFTWARETRIGGERRESPONSE._serialized_end=9382
-  _SETATTRIBUTEVIBOOLEANREQUEST._serialized_start=9385
-  _SETATTRIBUTEVIBOOLEANREQUEST._serialized_end=9554
-  _SETATTRIBUTEVIBOOLEANRESPONSE._serialized_start=9556
-  _SETATTRIBUTEVIBOOLEANRESPONSE._serialized_end=9603
-  _SETATTRIBUTEVIINT32REQUEST._serialized_start=9606
-  _SETATTRIBUTEVIINT32REQUEST._serialized_end=9875
-  _SETATTRIBUTEVIINT32RESPONSE._serialized_start=9877
-  _SETATTRIBUTEVIINT32RESPONSE._serialized_end=9922
-  _SETATTRIBUTEVIREAL64REQUEST._serialized_start=9925
-  _SETATTRIBUTEVIREAL64REQUEST._serialized_end=10097
-  _SETATTRIBUTEVIREAL64RESPONSE._serialized_start=10099
-  _SETATTRIBUTEVIREAL64RESPONSE._serialized_end=10145
-  _SETATTRIBUTEVISESSIONREQUEST._serialized_start=10148
-  _SETATTRIBUTEVISESSIONREQUEST._serialized_end=10341
-  _SETATTRIBUTEVISESSIONRESPONSE._serialized_start=10343
-  _SETATTRIBUTEVISESSIONRESPONSE._serialized_end=10390
-  _SETATTRIBUTEVISTRINGREQUEST._serialized_start=10393
-  _SETATTRIBUTEVISTRINGREQUEST._serialized_end=10565
-  _SETATTRIBUTEVISTRINGRESPONSE._serialized_start=10567
-  _SETATTRIBUTEVISTRINGRESPONSE._serialized_end=10613
-  _SETCONTINUOUSSCANREQUEST._serialized_start=10615
-  _SETCONTINUOUSSCANREQUEST._serialized_end=10702
-  _SETCONTINUOUSSCANRESPONSE._serialized_start=10704
-  _SETCONTINUOUSSCANRESPONSE._serialized_end=10747
-  _SETPATHREQUEST._serialized_start=10749
-  _SETPATHREQUEST._serialized_end=10820
-  _SETPATHRESPONSE._serialized_start=10822
-  _SETPATHRESPONSE._serialized_end=10855
-  _WAITFORDEBOUNCEREQUEST._serialized_start=10857
-  _WAITFORDEBOUNCEREQUEST._serialized_end=10942
-  _WAITFORDEBOUNCERESPONSE._serialized_start=10944
-  _WAITFORDEBOUNCERESPONSE._serialized_end=10985
-  _WAITFORSCANCOMPLETEREQUEST._serialized_start=10987
-  _WAITFORSCANCOMPLETEREQUEST._serialized_end=11076
-  _WAITFORSCANCOMPLETERESPONSE._serialized_start=11078
-  _WAITFORSCANCOMPLETERESPONSE._serialized_end=11123
-  _NISWITCH._serialized_start=24269
-  _NISWITCH._serialized_end=30189
+  _globals['_NISWITCHATTRIBUTE']._serialized_start=11126
+  _globals['_NISWITCHATTRIBUTE']._serialized_end=14118
+  _globals['_HANDSHAKINGINITIATION']._serialized_start=14121
+  _globals['_HANDSHAKINGINITIATION']._serialized_end=14272
+  _globals['_NISWITCHINT32ATTRIBUTEVALUES']._serialized_start=14275
+  _globals['_NISWITCHINT32ATTRIBUTEVALUES']._serialized_end=19440
+  _globals['_PATHCAPABILITY']._serialized_start=19443
+  _globals['_PATHCAPABILITY']._serialized_end=19794
+  _globals['_RELAYACTION']._serialized_start=19797
+  _globals['_RELAYACTION']._serialized_end=19925
+  _globals['_RELAYPOSITION']._serialized_start=19927
+  _globals['_RELAYPOSITION']._serialized_end=20052
+  _globals['_SCANADVANCEDOUTPUT']._serialized_start=20055
+  _globals['_SCANADVANCEDOUTPUT']._serialized_end=22182
+  _globals['_SCANMODE']._serialized_start=22185
+  _globals['_SCANMODE']._serialized_end=22319
+  _globals['_TRIGGERINPUT']._serialized_start=22322
+  _globals['_TRIGGERINPUT']._serialized_end=24266
+  _globals['_ABORTSCANREQUEST']._serialized_start=48
+  _globals['_ABORTSCANREQUEST']._serialized_end=102
+  _globals['_ABORTSCANRESPONSE']._serialized_start=104
+  _globals['_ABORTSCANRESPONSE']._serialized_end=139
+  _globals['_CANCONNECTREQUEST']._serialized_start=141
+  _globals['_CANCONNECTREQUEST']._serialized_end=232
+  _globals['_CANCONNECTRESPONSE']._serialized_start=234
+  _globals['_CANCONNECTRESPONSE']._serialized_end=355
+  _globals['_CHECKATTRIBUTEVIBOOLEANREQUEST']._serialized_start=358
+  _globals['_CHECKATTRIBUTEVIBOOLEANREQUEST']._serialized_end=529
+  _globals['_CHECKATTRIBUTEVIBOOLEANRESPONSE']._serialized_start=531
+  _globals['_CHECKATTRIBUTEVIBOOLEANRESPONSE']._serialized_end=580
+  _globals['_CHECKATTRIBUTEVIINT32REQUEST']._serialized_start=583
+  _globals['_CHECKATTRIBUTEVIINT32REQUEST']._serialized_end=854
+  _globals['_CHECKATTRIBUTEVIINT32RESPONSE']._serialized_start=856
+  _globals['_CHECKATTRIBUTEVIINT32RESPONSE']._serialized_end=903
+  _globals['_CHECKATTRIBUTEVIREAL64REQUEST']._serialized_start=906
+  _globals['_CHECKATTRIBUTEVIREAL64REQUEST']._serialized_end=1080
+  _globals['_CHECKATTRIBUTEVIREAL64RESPONSE']._serialized_start=1082
+  _globals['_CHECKATTRIBUTEVIREAL64RESPONSE']._serialized_end=1130
+  _globals['_CHECKATTRIBUTEVISESSIONREQUEST']._serialized_start=1133
+  _globals['_CHECKATTRIBUTEVISESSIONREQUEST']._serialized_end=1328
+  _globals['_CHECKATTRIBUTEVISESSIONRESPONSE']._serialized_start=1330
+  _globals['_CHECKATTRIBUTEVISESSIONRESPONSE']._serialized_end=1379
+  _globals['_CHECKATTRIBUTEVISTRINGREQUEST']._serialized_start=1382
+  _globals['_CHECKATTRIBUTEVISTRINGREQUEST']._serialized_end=1556
+  _globals['_CHECKATTRIBUTEVISTRINGRESPONSE']._serialized_start=1558
+  _globals['_CHECKATTRIBUTEVISTRINGRESPONSE']._serialized_end=1606
+  _globals['_CLEARERRORREQUEST']._serialized_start=1608
+  _globals['_CLEARERRORREQUEST']._serialized_end=1663
+  _globals['_CLEARERRORRESPONSE']._serialized_start=1665
+  _globals['_CLEARERRORRESPONSE']._serialized_end=1701
+  _globals['_CLEARINTERCHANGEWARNINGSREQUEST']._serialized_start=1703
+  _globals['_CLEARINTERCHANGEWARNINGSREQUEST']._serialized_end=1772
+  _globals['_CLEARINTERCHANGEWARNINGSRESPONSE']._serialized_start=1774
+  _globals['_CLEARINTERCHANGEWARNINGSRESPONSE']._serialized_end=1824
+  _globals['_CLOSEREQUEST']._serialized_start=1826
+  _globals['_CLOSEREQUEST']._serialized_end=1876
+  _globals['_CLOSERESPONSE']._serialized_start=1878
+  _globals['_CLOSERESPONSE']._serialized_end=1909
+  _globals['_COMMITREQUEST']._serialized_start=1911
+  _globals['_COMMITREQUEST']._serialized_end=1962
+  _globals['_COMMITRESPONSE']._serialized_start=1964
+  _globals['_COMMITRESPONSE']._serialized_end=1996
+  _globals['_CONFIGURESCANLISTREQUEST']._serialized_start=1999
+  _globals['_CONFIGURESCANLISTREQUEST']._serialized_end=2168
+  _globals['_CONFIGURESCANLISTRESPONSE']._serialized_start=2170
+  _globals['_CONFIGURESCANLISTRESPONSE']._serialized_end=2213
+  _globals['_CONFIGURESCANTRIGGERREQUEST']._serialized_start=2216
+  _globals['_CONFIGURESCANTRIGGERREQUEST']._serialized_end=2538
+  _globals['_CONFIGURESCANTRIGGERRESPONSE']._serialized_start=2540
+  _globals['_CONFIGURESCANTRIGGERRESPONSE']._serialized_end=2586
+  _globals['_CONNECTREQUEST']._serialized_start=2588
+  _globals['_CONNECTREQUEST']._serialized_end=2676
+  _globals['_CONNECTRESPONSE']._serialized_start=2678
+  _globals['_CONNECTRESPONSE']._serialized_end=2711
+  _globals['_CONNECTMULTIPLEREQUEST']._serialized_start=2713
+  _globals['_CONNECTMULTIPLEREQUEST']._serialized_end=2798
+  _globals['_CONNECTMULTIPLERESPONSE']._serialized_start=2800
+  _globals['_CONNECTMULTIPLERESPONSE']._serialized_end=2841
+  _globals['_DISABLEREQUEST']._serialized_start=2843
+  _globals['_DISABLEREQUEST']._serialized_end=2895
+  _globals['_DISABLERESPONSE']._serialized_start=2897
+  _globals['_DISABLERESPONSE']._serialized_end=2930
+  _globals['_DISCONNECTREQUEST']._serialized_start=2932
+  _globals['_DISCONNECTREQUEST']._serialized_end=3023
+  _globals['_DISCONNECTRESPONSE']._serialized_start=3025
+  _globals['_DISCONNECTRESPONSE']._serialized_end=3061
+  _globals['_DISCONNECTALLREQUEST']._serialized_start=3063
+  _globals['_DISCONNECTALLREQUEST']._serialized_end=3121
+  _globals['_DISCONNECTALLRESPONSE']._serialized_start=3123
+  _globals['_DISCONNECTALLRESPONSE']._serialized_end=3162
+  _globals['_DISCONNECTMULTIPLEREQUEST']._serialized_start=3164
+  _globals['_DISCONNECTMULTIPLEREQUEST']._serialized_end=3255
+  _globals['_DISCONNECTMULTIPLERESPONSE']._serialized_start=3257
+  _globals['_DISCONNECTMULTIPLERESPONSE']._serialized_end=3301
+  _globals['_ERRORMESSAGEREQUEST']._serialized_start=3303
+  _globals['_ERRORMESSAGEREQUEST']._serialized_end=3380
+  _globals['_ERRORMESSAGERESPONSE']._serialized_start=3382
+  _globals['_ERRORMESSAGERESPONSE']._serialized_end=3443
+  _globals['_ERRORQUERYREQUEST']._serialized_start=3445
+  _globals['_ERRORQUERYREQUEST']._serialized_end=3500
+  _globals['_ERRORQUERYRESPONSE']._serialized_start=3502
+  _globals['_ERRORQUERYRESPONSE']._serialized_end=3581
+  _globals['_GETATTRIBUTEVIBOOLEANREQUEST']._serialized_start=3584
+  _globals['_GETATTRIBUTEVIBOOLEANREQUEST']._serialized_end=3728
+  _globals['_GETATTRIBUTEVIBOOLEANRESPONSE']._serialized_start=3730
+  _globals['_GETATTRIBUTEVIBOOLEANRESPONSE']._serialized_end=3802
+  _globals['_GETATTRIBUTEVIINT32REQUEST']._serialized_start=3805
+  _globals['_GETATTRIBUTEVIINT32REQUEST']._serialized_end=3947
+  _globals['_GETATTRIBUTEVIINT32RESPONSE']._serialized_start=3949
+  _globals['_GETATTRIBUTEVIINT32RESPONSE']._serialized_end=4019
+  _globals['_GETATTRIBUTEVIREAL64REQUEST']._serialized_start=4022
+  _globals['_GETATTRIBUTEVIREAL64REQUEST']._serialized_end=4165
+  _globals['_GETATTRIBUTEVIREAL64RESPONSE']._serialized_start=4167
+  _globals['_GETATTRIBUTEVIREAL64RESPONSE']._serialized_end=4238
+  _globals['_GETATTRIBUTEVISESSIONREQUEST']._serialized_start=4241
+  _globals['_GETATTRIBUTEVISESSIONREQUEST']._serialized_end=4385
+  _globals['_GETATTRIBUTEVISESSIONRESPONSE']._serialized_start=4387
+  _globals['_GETATTRIBUTEVISESSIONRESPONSE']._serialized_end=4483
+  _globals['_GETATTRIBUTEVISTRINGREQUEST']._serialized_start=4486
+  _globals['_GETATTRIBUTEVISTRINGREQUEST']._serialized_end=4629
+  _globals['_GETATTRIBUTEVISTRINGRESPONSE']._serialized_start=4631
+  _globals['_GETATTRIBUTEVISTRINGRESPONSE']._serialized_end=4702
+  _globals['_GETCHANNELNAMEREQUEST']._serialized_start=4704
+  _globals['_GETCHANNELNAMEREQUEST']._serialized_end=4778
+  _globals['_GETCHANNELNAMERESPONSE']._serialized_start=4780
+  _globals['_GETCHANNELNAMERESPONSE']._serialized_end=4849
+  _globals['_GETERRORREQUEST']._serialized_start=4851
+  _globals['_GETERRORREQUEST']._serialized_end=4904
+  _globals['_GETERRORRESPONSE']._serialized_start=4906
+  _globals['_GETERRORRESPONSE']._serialized_end=4975
+  _globals['_GETNEXTCOERCIONRECORDREQUEST']._serialized_start=4977
+  _globals['_GETNEXTCOERCIONRECORDREQUEST']._serialized_end=5043
+  _globals['_GETNEXTCOERCIONRECORDRESPONSE']._serialized_start=5045
+  _globals['_GETNEXTCOERCIONRECORDRESPONSE']._serialized_end=5117
+  _globals['_GETNEXTINTERCHANGEWARNINGREQUEST']._serialized_start=5119
+  _globals['_GETNEXTINTERCHANGEWARNINGREQUEST']._serialized_end=5189
+  _globals['_GETNEXTINTERCHANGEWARNINGRESPONSE']._serialized_start=5191
+  _globals['_GETNEXTINTERCHANGEWARNINGRESPONSE']._serialized_end=5271
+  _globals['_GETPATHREQUEST']._serialized_start=5273
+  _globals['_GETPATHREQUEST']._serialized_end=5361
+  _globals['_GETPATHRESPONSE']._serialized_start=5363
+  _globals['_GETPATHRESPONSE']._serialized_end=5410
+  _globals['_GETRELAYCOUNTREQUEST']._serialized_start=5412
+  _globals['_GETRELAYCOUNTREQUEST']._serialized_end=5490
+  _globals['_GETRELAYCOUNTRESPONSE']._serialized_start=5492
+  _globals['_GETRELAYCOUNTRESPONSE']._serialized_end=5552
+  _globals['_GETRELAYNAMEREQUEST']._serialized_start=5554
+  _globals['_GETRELAYNAMEREQUEST']._serialized_end=5626
+  _globals['_GETRELAYNAMERESPONSE']._serialized_start=5628
+  _globals['_GETRELAYNAMERESPONSE']._serialized_end=5693
+  _globals['_GETRELAYPOSITIONREQUEST']._serialized_start=5695
+  _globals['_GETRELAYPOSITIONREQUEST']._serialized_end=5776
+  _globals['_GETRELAYPOSITIONRESPONSE']._serialized_start=5778
+  _globals['_GETRELAYPOSITIONRESPONSE']._serialized_end=5902
+  _globals['_INITREQUEST']._serialized_start=5905
+  _globals['_INITREQUEST']._serialized_end=6082
+  _globals['_INITRESPONSE']._serialized_start=6084
+  _globals['_INITRESPONSE']._serialized_end=6210
+  _globals['_INITWITHOPTIONSREQUEST']._serialized_start=6213
+  _globals['_INITWITHOPTIONSREQUEST']._serialized_end=6424
+  _globals['_INITWITHOPTIONSRESPONSE']._serialized_start=6427
+  _globals['_INITWITHOPTIONSRESPONSE']._serialized_end=6564
+  _globals['_INITWITHTOPOLOGYREQUEST']._serialized_start=6567
+  _globals['_INITWITHTOPOLOGYREQUEST']._serialized_end=6774
+  _globals['_INITWITHTOPOLOGYRESPONSE']._serialized_start=6777
+  _globals['_INITWITHTOPOLOGYRESPONSE']._serialized_end=6915
+  _globals['_INITIATESCANREQUEST']._serialized_start=6917
+  _globals['_INITIATESCANREQUEST']._serialized_end=6974
+  _globals['_INITIATESCANRESPONSE']._serialized_start=6976
+  _globals['_INITIATESCANRESPONSE']._serialized_end=7014
+  _globals['_INVALIDATEALLATTRIBUTESREQUEST']._serialized_start=7016
+  _globals['_INVALIDATEALLATTRIBUTESREQUEST']._serialized_end=7084
+  _globals['_INVALIDATEALLATTRIBUTESRESPONSE']._serialized_start=7086
+  _globals['_INVALIDATEALLATTRIBUTESRESPONSE']._serialized_end=7135
+  _globals['_ISDEBOUNCEDREQUEST']._serialized_start=7137
+  _globals['_ISDEBOUNCEDREQUEST']._serialized_end=7193
+  _globals['_ISDEBOUNCEDRESPONSE']._serialized_start=7195
+  _globals['_ISDEBOUNCEDRESPONSE']._serialized_end=7254
+  _globals['_ISSCANNINGREQUEST']._serialized_start=7256
+  _globals['_ISSCANNINGREQUEST']._serialized_end=7311
+  _globals['_ISSCANNINGRESPONSE']._serialized_start=7313
+  _globals['_ISSCANNINGRESPONSE']._serialized_end=7370
+  _globals['_RELAYCONTROLREQUEST']._serialized_start=7373
+  _globals['_RELAYCONTROLREQUEST']._serialized_end=7551
+  _globals['_RELAYCONTROLRESPONSE']._serialized_start=7553
+  _globals['_RELAYCONTROLRESPONSE']._serialized_end=7591
+  _globals['_RESETREQUEST']._serialized_start=7593
+  _globals['_RESETREQUEST']._serialized_end=7643
+  _globals['_RESETRESPONSE']._serialized_start=7645
+  _globals['_RESETRESPONSE']._serialized_end=7676
+  _globals['_RESETINTERCHANGECHECKREQUEST']._serialized_start=7678
+  _globals['_RESETINTERCHANGECHECKREQUEST']._serialized_end=7744
+  _globals['_RESETINTERCHANGECHECKRESPONSE']._serialized_start=7746
+  _globals['_RESETINTERCHANGECHECKRESPONSE']._serialized_end=7793
+  _globals['_RESETWITHDEFAULTSREQUEST']._serialized_start=7795
+  _globals['_RESETWITHDEFAULTSREQUEST']._serialized_end=7857
+  _globals['_RESETWITHDEFAULTSRESPONSE']._serialized_start=7859
+  _globals['_RESETWITHDEFAULTSRESPONSE']._serialized_end=7902
+  _globals['_REVISIONQUERYREQUEST']._serialized_start=7904
+  _globals['_REVISIONQUERYREQUEST']._serialized_end=7962
+  _globals['_REVISIONQUERYRESPONSE']._serialized_start=7964
+  _globals['_REVISIONQUERYRESPONSE']._serialized_end=8066
+  _globals['_ROUTESCANADVANCEDOUTPUTREQUEST']._serialized_start=8069
+  _globals['_ROUTESCANADVANCEDOUTPUTREQUEST']._serialized_end=8474
+  _globals['_ROUTESCANADVANCEDOUTPUTRESPONSE']._serialized_start=8476
+  _globals['_ROUTESCANADVANCEDOUTPUTRESPONSE']._serialized_end=8525
+  _globals['_ROUTETRIGGERINPUTREQUEST']._serialized_start=8528
+  _globals['_ROUTETRIGGERINPUTREQUEST']._serialized_end=8873
+  _globals['_ROUTETRIGGERINPUTRESPONSE']._serialized_start=8875
+  _globals['_ROUTETRIGGERINPUTRESPONSE']._serialized_end=8918
+  _globals['_SCANREQUEST']._serialized_start=8921
+  _globals['_SCANREQUEST']._serialized_end=9093
+  _globals['_SCANRESPONSE']._serialized_start=9095
+  _globals['_SCANRESPONSE']._serialized_end=9125
+  _globals['_SELFTESTREQUEST']._serialized_start=9127
+  _globals['_SELFTESTREQUEST']._serialized_end=9180
+  _globals['_SELFTESTRESPONSE']._serialized_start=9182
+  _globals['_SELFTESTRESPONSE']._serialized_end=9269
+  _globals['_SENDSOFTWARETRIGGERREQUEST']._serialized_start=9271
+  _globals['_SENDSOFTWARETRIGGERREQUEST']._serialized_end=9335
+  _globals['_SENDSOFTWARETRIGGERRESPONSE']._serialized_start=9337
+  _globals['_SENDSOFTWARETRIGGERRESPONSE']._serialized_end=9382
+  _globals['_SETATTRIBUTEVIBOOLEANREQUEST']._serialized_start=9385
+  _globals['_SETATTRIBUTEVIBOOLEANREQUEST']._serialized_end=9554
+  _globals['_SETATTRIBUTEVIBOOLEANRESPONSE']._serialized_start=9556
+  _globals['_SETATTRIBUTEVIBOOLEANRESPONSE']._serialized_end=9603
+  _globals['_SETATTRIBUTEVIINT32REQUEST']._serialized_start=9606
+  _globals['_SETATTRIBUTEVIINT32REQUEST']._serialized_end=9875
+  _globals['_SETATTRIBUTEVIINT32RESPONSE']._serialized_start=9877
+  _globals['_SETATTRIBUTEVIINT32RESPONSE']._serialized_end=9922
+  _globals['_SETATTRIBUTEVIREAL64REQUEST']._serialized_start=9925
+  _globals['_SETATTRIBUTEVIREAL64REQUEST']._serialized_end=10097
+  _globals['_SETATTRIBUTEVIREAL64RESPONSE']._serialized_start=10099
+  _globals['_SETATTRIBUTEVIREAL64RESPONSE']._serialized_end=10145
+  _globals['_SETATTRIBUTEVISESSIONREQUEST']._serialized_start=10148
+  _globals['_SETATTRIBUTEVISESSIONREQUEST']._serialized_end=10341
+  _globals['_SETATTRIBUTEVISESSIONRESPONSE']._serialized_start=10343
+  _globals['_SETATTRIBUTEVISESSIONRESPONSE']._serialized_end=10390
+  _globals['_SETATTRIBUTEVISTRINGREQUEST']._serialized_start=10393
+  _globals['_SETATTRIBUTEVISTRINGREQUEST']._serialized_end=10565
+  _globals['_SETATTRIBUTEVISTRINGRESPONSE']._serialized_start=10567
+  _globals['_SETATTRIBUTEVISTRINGRESPONSE']._serialized_end=10613
+  _globals['_SETCONTINUOUSSCANREQUEST']._serialized_start=10615
+  _globals['_SETCONTINUOUSSCANREQUEST']._serialized_end=10702
+  _globals['_SETCONTINUOUSSCANRESPONSE']._serialized_start=10704
+  _globals['_SETCONTINUOUSSCANRESPONSE']._serialized_end=10747
+  _globals['_SETPATHREQUEST']._serialized_start=10749
+  _globals['_SETPATHREQUEST']._serialized_end=10820
+  _globals['_SETPATHRESPONSE']._serialized_start=10822
+  _globals['_SETPATHRESPONSE']._serialized_end=10855
+  _globals['_WAITFORDEBOUNCEREQUEST']._serialized_start=10857
+  _globals['_WAITFORDEBOUNCEREQUEST']._serialized_end=10942
+  _globals['_WAITFORDEBOUNCERESPONSE']._serialized_start=10944
+  _globals['_WAITFORDEBOUNCERESPONSE']._serialized_end=10985
+  _globals['_WAITFORSCANCOMPLETEREQUEST']._serialized_start=10987
+  _globals['_WAITFORSCANCOMPLETEREQUEST']._serialized_end=11076
+  _globals['_WAITFORSCANCOMPLETERESPONSE']._serialized_start=11078
+  _globals['_WAITFORSCANCOMPLETERESPONSE']._serialized_end=11123
+  _globals['_NISWITCH']._serialized_start=24269
+  _globals['_NISWITCH']._serialized_end=30189
 # @@protoc_insertion_point(module_scope)
```

### Comparing `niswitch-1.4.7/niswitch/niswitch_pb2_grpc.py` & `niswitch-1.4.8/niswitch/niswitch_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/niswitch/session.py` & `niswitch-1.4.8/niswitch/session.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/niswitch/session_pb2.py` & `niswitch-1.4.8/niswitch/session_pb2.py`

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

### Comparing `niswitch-1.4.7/niswitch/session_pb2_grpc.py` & `niswitch-1.4.8/niswitch/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/niswitch.egg-info/PKG-INFO` & `niswitch-1.4.8/niswitch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niswitch
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI-SWITCH Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -17,21 +17,22 @@
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
@@ -80,15 +81,15 @@
 
 NI-SWITCH Python API Status
 ---------------------------
 
 +-------------------------------+-------------------------+
 | NI-SWITCH (niswitch)          |                         |
 +===============================+=========================+
-| Driver Version Tested Against | 2023 Q1                 |
+| Driver Version Tested Against | 2023 Q4                 |
 +-------------------------------+-------------------------+
 | PyPI Version                  | |niswitchLatestVersion| |
 +-------------------------------+-------------------------+
 | Supported Python Version      | |niswitchPythonVersion| |
 +-------------------------------+-------------------------+
 | Documentation                 | |niswitchDocs|          |
 +-------------------------------+-------------------------+
@@ -129,15 +130,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **niswitch** module, you must install the NI-SWITCH runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SWITCH**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niswitch~=1.4.7
+  $ python -m pip install niswitch~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `niswitch-1.4.7/niswitch.egg-info/SOURCES.txt` & `niswitch-1.4.8/niswitch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.7/setup.py` & `niswitch-1.4.8/setup.py`

 * *Files 13% similar despite different names*

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
     description='NI-SWITCH Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
@@ -43,16 +42,16 @@
     include_package_data=True,
     packages=['niswitch'],
     install_requires=[
         'hightime>=0.2.0',
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
@@ -63,13 +62,14 @@
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

