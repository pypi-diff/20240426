# Comparing `tmp/niscope-1.4.7.tar.gz` & `tmp/niscope-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niscope-1.4.7.tar", last modified: Fri Dec 15 19:31:17 2023, max compression
+gzip compressed data, was "niscope-1.4.8.tar", last modified: Fri Apr 26 18:16:57 2024, max compression
```

## Comparing `niscope-1.4.7.tar` & `niscope-1.4.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:26.354684 niscope-1.4.7/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     9056 2023-12-15 19:31:26.347687 niscope-1.4.7/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7868 2023-12-15 19:28:34.000000 niscope-1.4.7/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:26.130453 niscope-1.4.7/niscope/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-12-15 19:28:18.000000 niscope-1.4.7/niscope/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3243 2023-12-15 19:28:16.000000 niscope-1.4.7/niscope/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5440 2023-12-15 19:28:08.000000 niscope-1.4.7/niscope/_attributes.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13873 2023-12-15 19:28:17.000000 niscope-1.4.7/niscope/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    20927 2023-12-15 19:28:19.000000 niscope-1.4.7/niscope/_grpc_stub_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    43533 2023-12-15 19:28:09.000000 niscope-1.4.7/niscope/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    48611 2023-12-15 19:28:10.000000 niscope-1.4.7/niscope/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1725 2023-12-15 19:28:11.000000 niscope-1.4.7/niscope/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-12-15 19:28:23.000000 niscope-1.4.7/niscope/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    18294 2023-12-15 19:28:09.000000 niscope-1.4.7/niscope/enums.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4366 2023-12-15 19:28:13.000000 niscope-1.4.7/niscope/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3454 2023-12-15 19:28:20.000000 niscope-1.4.7/niscope/grpc_session_options.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1748 2023-12-15 19:28:23.000000 niscope-1.4.7/niscope/measurement_stats.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-12-15 19:28:22.000000 niscope-1.4.7/niscope/nidevice_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-12-15 19:28:22.000000 niscope-1.4.7/niscope/nidevice_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   111818 2023-12-15 19:28:21.000000 niscope-1.4.7/niscope/niscope_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   148144 2023-12-15 19:28:21.000000 niscope-1.4.7/niscope/niscope_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   254446 2023-12-15 19:28:12.000000 niscope-1.4.7/niscope/session.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-12-15 19:28:22.000000 niscope-1.4.7/niscope/session_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-12-15 19:28:22.000000 niscope-1.4.7/niscope/session_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     6425 2023-12-15 19:28:23.000000 niscope-1.4.7/niscope/waveform_info.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:26.339052 niscope-1.4.7/niscope.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     9056 2023-12-15 19:31:25.000000 niscope-1.4.7/niscope.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      713 2023-12-15 19:31:25.000000 niscope-1.4.7/niscope.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:31:25.000000 niscope-1.4.7/niscope.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       71 2023-12-15 19:31:25.000000 niscope-1.4.7/niscope.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        8 2023-12-15 19:31:25.000000 niscope-1.4.7/niscope.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:31:25.000000 niscope-1.4.7/niscope.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-12-15 19:31:26.355686 niscope-1.4.7/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2100 2023-12-15 19:28:35.000000 niscope-1.4.7/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:16:57.343716 niscope-1.4.8/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     9106 2024-04-26 18:16:57.337716 niscope-1.4.8/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7865 2024-04-26 18:10:28.000000 niscope-1.4.8/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:16:57.139667 niscope-1.4.8/niscope/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2024-04-26 18:10:12.000000 niscope-1.4.8/niscope/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3762 2024-04-26 18:10:10.000000 niscope-1.4.8/niscope/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5440 2024-04-26 18:10:01.000000 niscope-1.4.8/niscope/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13873 2024-04-26 18:10:11.000000 niscope-1.4.8/niscope/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    20927 2024-04-26 18:10:13.000000 niscope-1.4.8/niscope/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    43533 2024-04-26 18:10:03.000000 niscope-1.4.8/niscope/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    48611 2024-04-26 18:10:04.000000 niscope-1.4.8/niscope/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1725 2024-04-26 18:10:05.000000 niscope-1.4.8/niscope/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      635 2024-04-26 18:10:17.000000 niscope-1.4.8/niscope/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    18294 2024-04-26 18:10:02.000000 niscope-1.4.8/niscope/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4360 2024-04-26 18:10:07.000000 niscope-1.4.8/niscope/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3454 2024-04-26 18:10:14.000000 niscope-1.4.8/niscope/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1690 2024-04-26 18:10:17.000000 niscope-1.4.8/niscope/measurement_stats.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2009 2024-04-26 18:10:16.000000 niscope-1.4.8/niscope/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2024-04-26 18:10:16.000000 niscope-1.4.8/niscope/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   116861 2024-04-26 18:10:15.000000 niscope-1.4.8/niscope/niscope_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   148144 2024-04-26 18:10:15.000000 niscope-1.4.8/niscope/niscope_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   254441 2024-04-26 18:10:06.000000 niscope-1.4.8/niscope/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4550 2024-04-26 18:10:17.000000 niscope-1.4.8/niscope/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2024-04-26 18:10:17.000000 niscope-1.4.8/niscope/session_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     6375 2024-04-26 18:10:17.000000 niscope-1.4.8/niscope/waveform_info.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:16:57.329716 niscope-1.4.8/niscope.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     9106 2024-04-26 18:16:56.000000 niscope-1.4.8/niscope.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      713 2024-04-26 18:16:56.000000 niscope-1.4.8/niscope.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:16:56.000000 niscope-1.4.8/niscope.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       73 2024-04-26 18:16:56.000000 niscope-1.4.8/niscope.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        8 2024-04-26 18:16:56.000000 niscope-1.4.8/niscope.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:16:56.000000 niscope-1.4.8/niscope.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2024-04-26 18:16:57.344718 niscope-1.4.8/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2128 2024-04-26 18:10:29.000000 niscope-1.4.8/setup.py
```

### Comparing `niscope-1.4.7/PKG-INFO` & `niscope-1.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niscope
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI-SCOPE Python API
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
 
 NI-SCOPE Python API Status
 --------------------------
 
 +-------------------------------+------------------------+
 | NI-SCOPE (niscope)            |                        |
 +===============================+========================+
-| Driver Version Tested Against | 2023 Q1.1              |
+| Driver Version Tested Against | 2023 Q4                |
 +-------------------------------+------------------------+
 | PyPI Version                  | |niscopeLatestVersion| |
 +-------------------------------+------------------------+
 | Supported Python Version      | |niscopePythonVersion| |
 +-------------------------------+------------------------+
 | Documentation                 | |niscopeDocs|          |
 +-------------------------------+------------------------+
@@ -130,15 +131,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **niscope** module, you must install the NI-SCOPE runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SCOPE**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niscope~=1.4.7
+  $ python -m pip install niscope~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -153,15 +154,15 @@
     with niscope.Session("Dev1") as session:
         session.channels[0].configure_vertical(range=1.0, coupling=niscope.VerticalCoupling.AC)
         session.channels[1].configure_vertical(range=10.0, coupling=niscope.VerticalCoupling.DC)
         session.configure_horizontal_timing(min_sample_rate=50000000, min_num_pts=1000, ref_position=50.0, num_records=5, enforce_realtime=True)
         with session.initiate():
             waveforms = session.channels[0,1].fetch(num_records=5)
         for wfm in waveforms:
-            print('Channel {0}, record {1} samples acquired: {2:,}\n'.format(wfm.channel, wfm.record, len(wfm.samples)))
+            print('Channel {}, record {} samples acquired: {:,}\n'.format(wfm.channel, wfm.record, len(wfm.samples)))
 
         # Find all channel 1 records (Note channel name is always a string even if integers used in channel[])
         chan1 = [wfm for wfm in waveforms if wfm.channel == '0']
 
         # Find all record number 3
         rec3 = [wfm for wfm in waveforms if wfm.record == 3]
```

### Comparing `niscope-1.4.7/README.rst` & `niscope-1.4.8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 NI-SCOPE Python API Status
 --------------------------
 
 +-------------------------------+------------------------+
 | NI-SCOPE (niscope)            |                        |
 +===============================+========================+
-| Driver Version Tested Against | 2023 Q1.1              |
+| Driver Version Tested Against | 2023 Q4                |
 +-------------------------------+------------------------+
 | PyPI Version                  | |niscopeLatestVersion| |
 +-------------------------------+------------------------+
 | Supported Python Version      | |niscopePythonVersion| |
 +-------------------------------+------------------------+
 | Documentation                 | |niscopeDocs|          |
 +-------------------------------+------------------------+
@@ -98,15 +98,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **niscope** module, you must install the NI-SCOPE runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SCOPE**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niscope~=1.4.7
+  $ python -m pip install niscope~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -121,15 +121,15 @@
     with niscope.Session("Dev1") as session:
         session.channels[0].configure_vertical(range=1.0, coupling=niscope.VerticalCoupling.AC)
         session.channels[1].configure_vertical(range=10.0, coupling=niscope.VerticalCoupling.DC)
         session.configure_horizontal_timing(min_sample_rate=50000000, min_num_pts=1000, ref_position=50.0, num_records=5, enforce_realtime=True)
         with session.initiate():
             waveforms = session.channels[0,1].fetch(num_records=5)
         for wfm in waveforms:
-            print('Channel {0}, record {1} samples acquired: {2:,}\n'.format(wfm.channel, wfm.record, len(wfm.samples)))
+            print('Channel {}, record {} samples acquired: {:,}\n'.format(wfm.channel, wfm.record, len(wfm.samples)))
 
         # Find all channel 1 records (Note channel name is always a string even if integers used in channel[])
         chan1 = [wfm for wfm in waveforms if wfm.channel == '0']
 
         # Find all record number 3
         rec3 = [wfm for wfm in waveforms if wfm.record == 3]
```

### Comparing `niscope-1.4.7/niscope/__init__.py` & `niscope-1.4.8/niscope/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.7'
+__version__ = '1.4.8'
 
 from niscope.enums import *  # noqa: F403,F401,H303
 from niscope.errors import DriverWarning  # noqa: F401
 from niscope.errors import Error  # noqa: F401
 from niscope.grpc_session_options import *  # noqa: F403,F401,H303
 from niscope.session import Session  # noqa: F401
 
@@ -20,16 +20,16 @@
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
 
@@ -58,24 +58,37 @@
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
     info['driver']['name'] = "NI-SCOPE"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'niscope'
-    info['module']['version'] = "1.4.7"
+    info['module']['version'] = "1.4.8"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `niscope-1.4.7/niscope/_attributes.py` & `niscope-1.4.8/niscope/_attributes.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.7/niscope/_converters.py` & `niscope-1.4.8/niscope/_converters.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.7/niscope/_grpc_stub_interpreter.py` & `niscope-1.4.8/niscope/_grpc_stub_interpreter.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.7/niscope/_library.py` & `niscope-1.4.8/niscope/_library.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.7/niscope/_library_interpreter.py` & `niscope-1.4.8/niscope/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.7/niscope/_library_singleton.py` & `niscope-1.4.8/niscope/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.7/niscope/_visatype.py` & `niscope-1.4.8/niscope/_visatype.py`

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

### Comparing `niscope-1.4.7/niscope/enums.py` & `niscope-1.4.8/niscope/enums.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.7/niscope/errors.py` & `niscope-1.4.8/niscope/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-SCOPE driver'''
 
     def __init__(self, code, description):
         assert _is_warning(code), "Should not create Warning if code is not positive."
-        super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
+        super(DriverWarning, self).__init__('Warning {} occurred.\n\n{}'.format(code, description))
 
 
 class RpcError(Error):
     '''An error specific to sessions to the NI gRPC Device Server'''
 
     def __init__(self, rpc_code, description):
         self.rpc_code = rpc_code
@@ -85,24 +85,24 @@
         super(DriverTooNewError, self).__init__('The NI-SCOPE runtime returned an unexpected value. This can occur if it is too new for the niscope Python module. Upgrade the niscope Python module.')
 
 
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
 
     Helper function for handling errors returned by niscope.Library.
     It calls back into the LibraryInterpreter to get the corresponding error
```

### Comparing `niscope-1.4.7/niscope/grpc_session_options.py` & `niscope-1.4.8/niscope/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.7/niscope/measurement_stats.py` & `niscope-1.4.8/niscope/measurement_stats.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-class MeasurementStats(object):
+class MeasurementStats:
     def __init__(self, result=0.0, mean=0.0, stdev=0.0, min_val=0.0, max_val=0.0, num_in_stats=0):
         self.result = result
         self.mean = mean
         self.stdev = stdev
         self.min_val = min_val
         self.max_val = max_val
         self.num_in_stats = num_in_stats
 
         self.channel = None
         self.record = None
 
     def __repr__(self):
         parameter_list = [
-            'result={}'.format(self.result),
-            'mean={}'.format(self.mean),
-            'stdev={}'.format(self.stdev),
-            'min_val={}'.format(self.min_val),
-            'max_val={}'.format(self.max_val),
-            'num_in_stats={}'.format(self.num_in_stats)
+            f'result={self.result}',
+            f'mean={self.mean}',
+            f'stdev={self.stdev}',
+            f'min_val={self.min_val}',
+            f'max_val={self.max_val}',
+            f'num_in_stats={self.num_in_stats}'
         ]
 
-        return '{0}({1})'.format(self.__class__.__name__, ', '.join(parameter_list))
+        return '{}({})'.format(self.__class__.__name__, ', '.join(parameter_list))
 
     def __str__(self):
         row_format_g = '{:<20}: {:,.6g}\n'
         row_format_d = '{:<20}: {:,}\n'
         row_format_s = '{:<20}: {:}\n'
 
         string_representation = ''
```

### Comparing `niscope-1.4.7/niscope/nidevice_pb2.py` & `niscope-1.4.8/niscope/nidevice_pb2.py`

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

### Comparing `niscope-1.4.7/niscope/niscope_pb2.py` & `niscope-1.4.8/niscope/niscope_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,452 +1,452 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: niscope.proto
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
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rniscope.proto\x12\x0cniscope_grpc\x1a\x0enidevice.proto\x1a\rsession.proto\"U\n\x0f\x43oefficientInfo\x12\x0e\n\x06offset\x18\x01 \x01(\x01\x12\x0c\n\x04gain\x18\x02 \x01(\x01\x12\x11\n\treserved1\x18\x03 \x01(\x01\x12\x11\n\treserved2\x18\x04 \x01(\x01\"\xb7\x01\n\x0cWaveformInfo\x12\x1a\n\x12\x61\x62solute_initial_x\x18\x01 \x01(\x01\x12\x1a\n\x12relative_initial_x\x18\x02 \x01(\x01\x12\x13\n\x0bx_increment\x18\x03 \x01(\x01\x12\x16\n\x0e\x61\x63tual_samples\x18\x04 \x01(\x11\x12\x0e\n\x06offset\x18\x05 \x01(\x01\x12\x0c\n\x04gain\x18\x06 \x01(\x01\x12\x11\n\treserved1\x18\x07 \x01(\x01\x12\x11\n\treserved2\x18\x08 \x01(\x01\"2\n\x0c\x41\x62ortRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rAbortResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\">\n\x18\x41\x63quisitionStatusRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x88\x01\n\x19\x41\x63quisitionStatusResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12;\n\x12\x61\x63quisition_status\x18\x02 \x01(\x0e\x32\x1f.niscope_grpc.AcquisitionStatus\x12\x1e\n\x16\x61\x63quisition_status_raw\x18\x03 \x01(\x11\"\xbc\x01\n\x18\x41\x63tualMeasWfmSizeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12=\n\x13\x61rray_meas_function\x18\x02 \x01(\x0e\x32\x1e.niscope_grpc.ArrayMeasurementH\x00\x12!\n\x17\x61rray_meas_function_raw\x18\x03 \x01(\x11H\x00\x42\x1a\n\x18\x61rray_meas_function_enum\"G\n\x19\x41\x63tualMeasWfmSizeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1a\n\x12meas_waveform_size\x18\x02 \x01(\x11\"P\n\x14\x41\x63tualNumWfmsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\"9\n\x15\x41\x63tualNumWfmsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08num_wfms\x18\x02 \x01(\x11\"?\n\x19\x41\x63tualRecordLengthRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"C\n\x1a\x41\x63tualRecordLengthResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rrecord_length\x18\x02 \x01(\x11\"\xc4\x01\n\x1c\x41\x64\x64WaveformProcessingRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x37\n\rmeas_function\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.ArrayMeasurementH\x00\x12\x1b\n\x11meas_function_raw\x18\x04 \x01(\x11H\x00\x42\x14\n\x12meas_function_enum\"/\n\x1d\x41\x64\x64WaveformProcessingResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"Z\n%AdjustSampleClockRelativeDelayRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\r\n\x05\x64\x65lay\x18\x02 \x01(\x01\"8\n&AdjustSampleClockRelativeDelayResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"6\n\x10\x41utoSetupRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"#\n\x11\x41utoSetupResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"B\n\x1c\x43\x61\x62leSenseSignalStartRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"/\n\x1d\x43\x61\x62leSenseSignalStartResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"A\n\x1b\x43\x61\x62leSenseSignalStopRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\".\n\x1c\x43\x61\x62leSenseSignalStopResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x99\x01\n\x13\x43\x61lFetchDateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x33\n\twhich_one\x18\x02 \x01(\x0e\x32\x1e.niscope_grpc.CalibrationTypesH\x00\x12\x17\n\rwhich_one_raw\x18\x03 \x01(\x11H\x00\x42\x10\n\x0ewhich_one_enum\"P\n\x14\x43\x61lFetchDateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04year\x18\x02 \x01(\x11\x12\r\n\x05month\x18\x03 \x01(\x11\x12\x0b\n\x03\x64\x61y\x18\x04 \x01(\x11\"\xa0\x01\n\x1a\x43\x61lFetchTemperatureRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x33\n\twhich_one\x18\x02 \x01(\x0e\x32\x1e.niscope_grpc.CalibrationTypesH\x00\x12\x17\n\rwhich_one_raw\x18\x03 \x01(\x11H\x00\x42\x10\n\x0ewhich_one_enum\"B\n\x1b\x43\x61lFetchTemperatureResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"\xa0\x01\n\x17\x43\x61lSelfCalibrateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12&\n\x06option\x18\x03 \x01(\x0e\x32\x14.niscope_grpc.OptionH\x00\x12\x14\n\noption_raw\x18\x04 \x01(\x11H\x00\x42\r\n\x0boption_enum\"*\n\x18\x43\x61lSelfCalibrateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x9f\x01\n\x1e\x43heckAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\r\n\x05value\x18\x04 \x01(\x08\"1\n\x1f\x43heckAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xed\x01\n\x1c\x43heckAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x13\n\tvalue_raw\x18\x04 \x01(\x11H\x00\x12:\n\x05value\x18\x05 \x01(\x0e\x32).niscope_grpc.NiScopeInt32AttributeValuesH\x00\x42\x0c\n\nvalue_enum\"/\n\x1d\x43heckAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa1\x01\n\x1c\x43heckAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x11\n\tvalue_raw\x18\x04 \x01(\x03\"/\n\x1d\x43heckAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb9\x02\n\x1d\x43heckAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x13\n\tvalue_raw\x18\x04 \x01(\x01H\x00\x12;\n\x05value\x18\x05 \x01(\x0e\x32*.niscope_grpc.NiScopeReal64AttributeValuesH\x00\x12H\n\x0cvalue_mapped\x18\x06 \x01(\x0e\x32\x30.niscope_grpc.NiScopeReal64AttributeValuesMappedH\x00\x42\x0c\n\nvalue_enum\"0\n\x1e\x43heckAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb7\x01\n\x1e\x43heckAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12%\n\x05value\x18\x04 \x01(\x0b\x32\x16.nidevice_grpc.Session\"1\n\x1f\x43heckAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xfc\x01\n\x1d\x43heckAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12H\n\x0cvalue_mapped\x18\x04 \x01(\x0e\x32\x30.niscope_grpc.NiScopeStringAttributeValuesMappedH\x00\x12\x13\n\tvalue_raw\x18\x05 \x01(\tH\x00\x42\x0c\n\nvalue_enum\"0\n\x1e\x43heckAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x83\x02\n$ClearWaveformMeasurementStatsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12L\n\x1e\x63learable_measurement_function\x18\x03 \x01(\x0e\x32\".niscope_grpc.ClearableMeasurementH\x00\x12,\n\"clearable_measurement_function_raw\x18\x04 \x01(\x11H\x00\x42%\n#clearable_measurement_function_enum\"7\n%ClearWaveformMeasurementStatsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"Z\n\x1e\x43learWaveformProcessingRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\"1\n\x1f\x43learWaveformProcessingResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"2\n\x0c\x43loseRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rCloseResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"3\n\rCommitRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\" \n\x0e\x43ommitResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"[\n\x1b\x43onfigureAcquisitionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x18\n\x10\x61\x63quisition_type\x18\x02 \x01(\x11\".\n\x1c\x43onfigureAcquisitionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x95\x01\n#ConfigureChanCharacteristicsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x17\n\x0finput_impedance\x18\x03 \x01(\x01\x12\x1b\n\x13max_input_frequency\x18\x04 \x01(\x01\"6\n$ConfigureChanCharacteristicsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xfd\x03\n\x15\x43onfigureClockRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12 \n\x16input_clock_source_raw\x18\x02 \x01(\tH\x00\x12I\n\x19input_clock_source_mapped\x18\x06 \x01(\x0e\x32$.niscope_grpc.ClockingTerminalValuesH\x00\x12!\n\x17output_clock_source_raw\x18\x03 \x01(\tH\x01\x12J\n\x1aoutput_clock_source_mapped\x18\x07 \x01(\x0e\x32$.niscope_grpc.ClockingTerminalValuesH\x01\x12%\n\x1b\x63lock_sync_pulse_source_raw\x18\x04 \x01(\tH\x02\x12N\n\x1e\x63lock_sync_pulse_source_mapped\x18\x08 \x01(\x0e\x32$.niscope_grpc.ClockingTerminalValuesH\x02\x12\x16\n\x0emaster_enabled\x18\x05 \x01(\x08\x42\x19\n\x17input_clock_source_enumB\x1a\n\x18output_clock_source_enumB\x1e\n\x1c\x63lock_sync_pulse_source_enum\"(\n\x16\x43onfigureClockResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x80\x01\n.ConfigureEqualizationFilterCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x14\n\x0c\x63oefficients\x18\x03 \x03(\x01\"A\n/ConfigureEqualizationFilterCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb9\x01\n ConfigureHorizontalTimingRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x17\n\x0fmin_sample_rate\x18\x02 \x01(\x01\x12\x13\n\x0bmin_num_pts\x18\x03 \x01(\x11\x12\x14\n\x0cref_position\x18\x04 \x01(\x01\x12\x13\n\x0bnum_records\x18\x05 \x01(\x11\x12\x18\n\x10\x65nforce_realtime\x18\x06 \x01(\x08\"3\n!ConfigureHorizontalTimingResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xcc\x01\n\x1e\x43onfigureTriggerDigitalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12+\n\x05slope\x18\x03 \x01(\x0e\x32\x1a.niscope_grpc.TriggerSlopeH\x00\x12\x13\n\tslope_raw\x18\x04 \x01(\x11H\x00\x12\x0f\n\x07holdoff\x18\x05 \x01(\x01\x12\r\n\x05\x64\x65lay\x18\x06 \x01(\x01\x42\x0c\n\nslope_enum\"1\n\x1f\x43onfigureTriggerDigitalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xcc\x02\n\x1b\x43onfigureTriggerEdgeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\x01\x12+\n\x05slope\x18\x04 \x01(\x0e\x32\x1a.niscope_grpc.TriggerSlopeH\x00\x12\x13\n\tslope_raw\x18\x05 \x01(\x11H\x00\x12\x39\n\x10trigger_coupling\x18\x06 \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x01\x12\x1e\n\x14trigger_coupling_raw\x18\x07 \x01(\x11H\x01\x12\x0f\n\x07holdoff\x18\x08 \x01(\x01\x12\r\n\x05\x64\x65lay\x18\t \x01(\x01\x42\x0c\n\nslope_enumB\x17\n\x15trigger_coupling_enum\".\n\x1c\x43onfigureTriggerEdgeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xdc\x03\n\x1d\x43onfigureTriggerGlitchRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\x01\x12\r\n\x05width\x18\x04 \x01(\x01\x12\x30\n\x08polarity\x18\x05 \x01(\x0e\x32\x1c.niscope_grpc.GlitchPolarityH\x00\x12\x16\n\x0cpolarity_raw\x18\x06 \x01(\x11H\x00\x12\x39\n\x10glitch_condition\x18\x07 \x01(\x0e\x32\x1d.niscope_grpc.GlitchConditionH\x01\x12\x1e\n\x14glitch_condition_raw\x18\x08 \x01(\x11H\x01\x12\x39\n\x10trigger_coupling\x18\t \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x02\x12\x1e\n\x14trigger_coupling_raw\x18\n \x01(\x11H\x02\x12\x0f\n\x07holdoff\x18\x0b \x01(\x01\x12\r\n\x05\x64\x65lay\x18\x0c \x01(\x01\x42\x0f\n\rpolarity_enumB\x17\n\x15glitch_condition_enumB\x17\n\x15trigger_coupling_enum\"0\n\x1e\x43onfigureTriggerGlitchResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xe6\x02\n!ConfigureTriggerHysteresisRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\x01\x12\x12\n\nhysteresis\x18\x04 \x01(\x01\x12+\n\x05slope\x18\x05 \x01(\x0e\x32\x1a.niscope_grpc.TriggerSlopeH\x00\x12\x13\n\tslope_raw\x18\x06 \x01(\x11H\x00\x12\x39\n\x10trigger_coupling\x18\x07 \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x01\x12\x1e\n\x14trigger_coupling_raw\x18\x08 \x01(\x11H\x01\x12\x0f\n\x07holdoff\x18\t \x01(\x01\x12\r\n\x05\x64\x65lay\x18\n \x01(\x01\x42\x0c\n\nslope_enumB\x17\n\x15trigger_coupling_enum\"4\n\"ConfigureTriggerHysteresisResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"F\n ConfigureTriggerImmediateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"3\n!ConfigureTriggerImmediateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xf5\x02\n\x1b\x43onfigureTriggerRuntRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\x15\n\rlow_threshold\x18\x03 \x01(\x01\x12\x16\n\x0ehigh_threshold\x18\x04 \x01(\x01\x12.\n\x08polarity\x18\x05 \x01(\x0e\x32\x1a.niscope_grpc.RuntPolarityH\x00\x12\x16\n\x0cpolarity_raw\x18\x06 \x01(\x11H\x00\x12\x39\n\x10trigger_coupling\x18\x07 \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x01\x12\x1e\n\x14trigger_coupling_raw\x18\x08 \x01(\x11H\x01\x12\x0f\n\x07holdoff\x18\t \x01(\x01\x12\r\n\x05\x64\x65lay\x18\n \x01(\x01\x42\x0f\n\rpolarity_enumB\x17\n\x15trigger_coupling_enum\".\n\x1c\x43onfigureTriggerRuntResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"e\n\x1f\x43onfigureTriggerSoftwareRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x0f\n\x07holdoff\x18\x02 \x01(\x01\x12\r\n\x05\x64\x65lay\x18\x03 \x01(\x01\"2\n ConfigureTriggerSoftwareResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xba\x04\n\x1c\x43onfigureTriggerVideoRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\x19\n\x11\x65nable_dc_restore\x18\x03 \x01(\x08\x12\x38\n\rsignal_format\x18\x04 \x01(\x0e\x32\x1f.niscope_grpc.VideoSignalFormatH\x00\x12\x1b\n\x11signal_format_raw\x18\x05 \x01(\x11H\x00\x12\x30\n\x05\x65vent\x18\x06 \x01(\x0e\x32\x1f.niscope_grpc.VideoTriggerEventH\x01\x12\x13\n\tevent_raw\x18\x07 \x01(\x11H\x01\x12\x13\n\x0bline_number\x18\x08 \x01(\x11\x12/\n\x08polarity\x18\t \x01(\x0e\x32\x1b.niscope_grpc.VideoPolarityH\x02\x12\x16\n\x0cpolarity_raw\x18\n \x01(\x11H\x02\x12\x39\n\x10trigger_coupling\x18\x0b \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x03\x12\x1e\n\x14trigger_coupling_raw\x18\x0c \x01(\x11H\x03\x12\x0f\n\x07holdoff\x18\r \x01(\x01\x12\r\n\x05\x64\x65lay\x18\x0e \x01(\x01\x42\x14\n\x12signal_format_enumB\x0c\n\nevent_enumB\x0f\n\rpolarity_enumB\x17\n\x15trigger_coupling_enum\"/\n\x1d\x43onfigureTriggerVideoResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xe4\x03\n\x1c\x43onfigureTriggerWidthRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\x01\x12\x15\n\rlow_threshold\x18\x04 \x01(\x01\x12\x16\n\x0ehigh_threshold\x18\x05 \x01(\x01\x12/\n\x08polarity\x18\x06 \x01(\x0e\x32\x1b.niscope_grpc.WidthPolarityH\x00\x12\x16\n\x0cpolarity_raw\x18\x07 \x01(\x11H\x00\x12\x31\n\tcondition\x18\x08 \x01(\x0e\x32\x1c.niscope_grpc.WidthConditionH\x01\x12\x17\n\rcondition_raw\x18\t \x01(\x11H\x01\x12\x39\n\x10trigger_coupling\x18\n \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x02\x12\x1e\n\x14trigger_coupling_raw\x18\x0b \x01(\x11H\x02\x12\x0f\n\x07holdoff\x18\x0c \x01(\x01\x12\r\n\x05\x64\x65lay\x18\r \x01(\x01\x42\x0f\n\rpolarity_enumB\x10\n\x0e\x63ondition_enumB\x17\n\x15trigger_coupling_enum\"/\n\x1d\x43onfigureTriggerWidthResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xfd\x02\n\x1d\x43onfigureTriggerWindowRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\x11\n\tlow_level\x18\x03 \x01(\x01\x12\x12\n\nhigh_level\x18\x04 \x01(\x01\x12\x36\n\x0bwindow_mode\x18\x05 \x01(\x0e\x32\x1f.niscope_grpc.TriggerWindowModeH\x00\x12\x19\n\x0fwindow_mode_raw\x18\x06 \x01(\x11H\x00\x12\x39\n\x10trigger_coupling\x18\x07 \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x01\x12\x1e\n\x14trigger_coupling_raw\x18\x08 \x01(\x11H\x01\x12\x0f\n\x07holdoff\x18\t \x01(\x01\x12\r\n\x05\x64\x65lay\x18\n \x01(\x01\x42\x12\n\x10window_mode_enumB\x17\n\x15trigger_coupling_enum\"0\n\x1e\x43onfigureTriggerWindowResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xfc\x01\n\x18\x43onfigureVerticalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\r\n\x05range\x18\x03 \x01(\x01\x12\x0e\n\x06offset\x18\x04 \x01(\x01\x12\x32\n\x08\x63oupling\x18\x05 \x01(\x0e\x32\x1e.niscope_grpc.VerticalCouplingH\x00\x12\x16\n\x0c\x63oupling_raw\x18\x06 \x01(\x11H\x00\x12\x19\n\x11probe_attenuation\x18\x07 \x01(\x01\x12\x0f\n\x07\x65nabled\x18\x08 \x01(\x08\x42\x0f\n\rcoupling_enum\"+\n\x19\x43onfigureVerticalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"4\n\x0e\x44isableRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"!\n\x0f\x44isableResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"c\n\x13\x45rrorHandlerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nerror_code\x18\x02 \x01(\x11\x12\x14\n\x0c\x65rror_source\x18\x03 \x01(\t\"A\n\x14\x45rrorHandlerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x19\n\x11\x65rror_description\x18\x02 \x01(\t\"O\n)ExportAttributeConfigurationBufferRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"S\n*ExportAttributeConfigurationBufferResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rconfiguration\x18\x02 \x01(\x0c\"`\n\'ExportAttributeConfigurationFileRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x11\n\tfile_path\x18\x02 \x01(\t\":\n(ExportAttributeConfigurationFileResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xab\x02\n\x13\x45xportSignalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x31\n\x06signal\x18\x02 \x01(\x0e\x32\x1f.niscope_grpc.ExportableSignalsH\x00\x12\x14\n\nsignal_raw\x18\x03 \x01(\x11H\x00\x12\x19\n\x11signal_identifier\x18\x04 \x01(\t\x12\x46\n\x16output_terminal_mapped\x18\x05 \x01(\x0e\x32$.niscope_grpc.ClockingTerminalValuesH\x01\x12\x1d\n\x13output_terminal_raw\x18\x06 \x01(\tH\x01\x42\r\n\x0bsignal_enumB\x16\n\x14output_terminal_enum\"&\n\x14\x45xportSignalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"n\n\x0c\x46\x65tchRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"_\n\rFetchResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08waveform\x18\x02 \x03(\x01\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"\x95\x02\n\x1c\x46\x65tchArrayMeasurementRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12=\n\x13\x61rray_meas_function\x18\x04 \x01(\x0e\x32\x1e.niscope_grpc.ArrayMeasurementH\x00\x12!\n\x17\x61rray_meas_function_raw\x18\x05 \x01(\x11H\x00\x12\x1a\n\rmeas_wfm_size\x18\x06 \x01(\x11H\x01\x88\x01\x01\x42\x1a\n\x18\x61rray_meas_function_enumB\x10\n\x0e_meas_wfm_size\"o\n\x1d\x46\x65tchArrayMeasurementResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08meas_wfm\x18\x02 \x03(\x01\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"v\n\x14\x46\x65tchBinary16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"g\n\x15\x46\x65tchBinary16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08waveform\x18\x02 \x03(\x11\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"v\n\x14\x46\x65tchBinary32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"g\n\x15\x46\x65tchBinary32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08waveform\x18\x02 \x03(\x11\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"u\n\x13\x46\x65tchBinary8Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"f\n\x14\x46\x65tchBinary8Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08waveform\x18\x02 \x01(\x0c\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"u\n\x13\x46\x65tchComplexRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"\x81\x01\n\x14\x46\x65tchComplexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12+\n\x03wfm\x18\x02 \x03(\x0b\x32\x1e.nidevice_grpc.NIComplexNumber\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"}\n\x1b\x46\x65tchComplexBinary16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"\x86\x01\n\x1c\x46\x65tchComplexBinary16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12(\n\x03wfm\x18\x02 \x03(\x0b\x32\x1b.nidevice_grpc.NIComplexI16\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"\xe6\x01\n\x17\x46\x65tchMeasurementRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12?\n\x14scalar_meas_function\x18\x04 \x01(\x0e\x32\x1f.niscope_grpc.ScalarMeasurementH\x00\x12\"\n\x18scalar_meas_function_raw\x18\x05 \x01(\x11H\x00\x42\x1b\n\x19scalar_meas_function_enum\":\n\x18\x46\x65tchMeasurementResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x03(\x01\"\xeb\x01\n\x1c\x46\x65tchMeasurementStatsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12?\n\x14scalar_meas_function\x18\x04 \x01(\x0e\x32\x1f.niscope_grpc.ScalarMeasurementH\x00\x12\"\n\x18scalar_meas_function_raw\x18\x05 \x01(\x11H\x00\x42\x1b\n\x19scalar_meas_function_enum\"\x8c\x01\n\x1d\x46\x65tchMeasurementStatsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x03(\x01\x12\x0c\n\x04mean\x18\x03 \x03(\x01\x12\r\n\x05stdev\x18\x04 \x03(\x01\x12\x0b\n\x03min\x18\x05 \x03(\x01\x12\x0b\n\x03max\x18\x06 \x03(\x01\x12\x14\n\x0cnum_in_stats\x18\x07 \x03(\x11\"\x8e\x01\n\x1cGetAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\">\n\x1dGetAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x08\"\x8c\x01\n\x1aGetAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\"<\n\x1bGetAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x11\"\x8c\x01\n\x1aGetAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\"<\n\x1bGetAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x03\"\x8d\x01\n\x1bGetAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\"=\n\x1cGetAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x01\"\x8e\x01\n\x1cGetAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\"V\n\x1dGetAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x8d\x01\n\x1bGetAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\"=\n\x1cGetAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t\"J\n\x15GetChannelNameRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\r\n\x05index\x18\x02 \x01(\x11\"@\n\x16GetChannelNameResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x16\n\x0e\x63hannel_string\x18\x02 \x01(\t\"T\n\x1fGetChannelNameFromStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\r\n\x05index\x18\x02 \x01(\t\"@\n GetChannelNameFromStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x7f\n(GetEqualizationFilterCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\t\x12\x1e\n\x16number_of_coefficients\x18\x03 \x01(\x11\"Q\n)GetEqualizationFilterCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x14\n\x0c\x63oefficients\x18\x02 \x03(\x01\"5\n\x0fGetErrorRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"K\n\x10GetErrorResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x12\n\nerror_code\x18\x02 \x01(\x11\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\"P\n\x16GetErrorMessageRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nerror_code\x18\x02 \x01(\x11\"@\n\x17GetErrorMessageResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"g\n\x1bGetFrequencyResponseRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\t\x12\x13\n\x0b\x62uffer_size\x18\x03 \x01(\x11\"\x86\x01\n\x1cGetFrequencyResponseResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0b\x66requencies\x18\x02 \x03(\x01\x12\x12\n\namplitudes\x18\x03 \x03(\x01\x12\x0e\n\x06phases\x18\x04 \x03(\x01\x12\x1d\n\x15number_of_frequencies\x18\x05 \x01(\x11\"_\n#GetNormalizationCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\"\x93\x01\n$GetNormalizationCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x37\n\x10\x63oefficient_info\x18\x02 \x03(\x0b\x32\x1d.niscope_grpc.CoefficientInfo\x12\"\n\x1anumber_of_coefficient_sets\x18\x03 \x01(\x11\"Y\n\x1dGetScalingCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\"\x8d\x01\n\x1eGetScalingCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x37\n\x10\x63oefficient_info\x18\x02 \x03(\x0b\x32\x1d.niscope_grpc.CoefficientInfo\x12\"\n\x1anumber_of_coefficient_sets\x18\x03 \x01(\x11\"Y\n\x1eGetStreamEndpointHandleRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x13\n\x0bstream_name\x18\x02 \x01(\t\"H\n\x1fGetStreamEndpointHandleResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rwriter_handle\x18\x02 \x01(\r\"f\n)ImportAttributeConfigurationBufferRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x15\n\rconfiguration\x18\x02 \x01(\x0c\"<\n*ImportAttributeConfigurationBufferResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"`\n\'ImportAttributeConfigurationFileRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x11\n\tfile_path\x18\x02 \x01(\t\":\n(ImportAttributeConfigurationFileResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb1\x01\n\x0bInitRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x10\n\x08id_query\x18\x03 \x01(\x08\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12M\n\x17initialization_behavior\x18\x05 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"~\n\x0cInitResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"\xd3\x01\n\x16InitWithOptionsRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x10\n\x08id_query\x18\x03 \x01(\x08\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12\x15\n\roption_string\x18\x05 \x01(\t\x12M\n\x17initialization_behavior\x18\x06 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"\x89\x01\n\x17InitWithOptionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"@\n\x1aInitiateAcquisitionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"-\n\x1bInitiateAcquisitionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"I\n#ProbeCompensationSignalStartRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"6\n$ProbeCompensationSignalStartResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"H\n\"ProbeCompensationSignalStopRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"5\n#ProbeCompensationSignalStopResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"m\n\x0bReadRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"^\n\x0cReadResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08waveform\x18\x02 \x03(\x01\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"\xe5\x01\n\x16ReadMeasurementRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12?\n\x14scalar_meas_function\x18\x04 \x01(\x0e\x32\x1f.niscope_grpc.ScalarMeasurementH\x00\x12\"\n\x18scalar_meas_function_raw\x18\x05 \x01(\x11H\x00\x42\x1b\n\x19scalar_meas_function_enum\"9\n\x17ReadMeasurementResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x03(\x01\"2\n\x0cResetRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rResetResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"8\n\x12ResetDeviceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"%\n\x13ResetDeviceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\":\n\x14RevisionQueryRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"[\n\x15RevisionQueryResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x64river_revision\x18\x02 \x01(\t\x12\x19\n\x11\x66irmware_revision\x18\x03 \x01(\t\"7\n\x11SampleModeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"9\n\x12SampleModeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0bsample_mode\x18\x02 \x01(\x11\"7\n\x11SampleRateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"9\n\x12SampleRateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0bsample_rate\x18\x02 \x01(\x01\"5\n\x0fSelfTestRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"W\n\x10SelfTestResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x18\n\x10self_test_result\x18\x02 \x01(\x11\x12\x19\n\x11self_test_message\x18\x03 \x01(\t\"\xac\x01\n\x1eSendSoftwareTriggerEdgeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x33\n\rwhich_trigger\x18\x02 \x01(\x0e\x32\x1a.niscope_grpc.WhichTriggerH\x00\x12\x1b\n\x11which_trigger_raw\x18\x03 \x01(\x11H\x00\x42\x14\n\x12which_trigger_enum\"1\n\x1fSendSoftwareTriggerEdgeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x9d\x01\n\x1cSetAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\r\n\x05value\x18\x04 \x01(\x08\"/\n\x1dSetAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xeb\x01\n\x1aSetAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x13\n\tvalue_raw\x18\x04 \x01(\x11H\x00\x12:\n\x05value\x18\x05 \x01(\x0e\x32).niscope_grpc.NiScopeInt32AttributeValuesH\x00\x42\x0c\n\nvalue_enum\"-\n\x1bSetAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x9f\x01\n\x1aSetAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x11\n\tvalue_raw\x18\x04 \x01(\x03\"-\n\x1bSetAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb7\x02\n\x1bSetAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x13\n\tvalue_raw\x18\x04 \x01(\x01H\x00\x12;\n\x05value\x18\x05 \x01(\x0e\x32*.niscope_grpc.NiScopeReal64AttributeValuesH\x00\x12H\n\x0cvalue_mapped\x18\x06 \x01(\x0e\x32\x30.niscope_grpc.NiScopeReal64AttributeValuesMappedH\x00\x42\x0c\n\nvalue_enum\".\n\x1cSetAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb5\x01\n\x1cSetAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12%\n\x05value\x18\x04 \x01(\x0b\x32\x16.nidevice_grpc.Session\"/\n\x1dSetAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xfa\x01\n\x1bSetAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12H\n\x0cvalue_mapped\x18\x04 \x01(\x0e\x32\x30.niscope_grpc.NiScopeStringAttributeValuesMappedH\x00\x12\x13\n\tvalue_raw\x18\x05 \x01(\tH\x00\x42\x0c\n\nvalue_enum\".\n\x1cSetAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05*\xe0Q\n\x10NiScopeAttribute\x12!\n\x1dNISCOPE_ATTRIBUTE_UNSPECIFIED\x10\x00\x12#\n\x1dNISCOPE_ATTRIBUTE_RANGE_CHECK\x10\x92\x8b@\x12/\n)NISCOPE_ATTRIBUTE_QUERY_INSTRUMENT_STATUS\x10\x93\x8b@\x12\x1d\n\x17NISCOPE_ATTRIBUTE_CACHE\x10\x94\x8b@\x12 \n\x1aNISCOPE_ATTRIBUTE_SIMULATE\x10\x95\x8b@\x12(\n\"NISCOPE_ATTRIBUTE_RECORD_COERCIONS\x10\x96\x8b@\x12$\n\x1eNISCOPE_ATTRIBUTE_DRIVER_SETUP\x10\x97\x8b@\x12)\n#NISCOPE_ATTRIBUTE_INTERCHANGE_CHECK\x10\xa5\x8b@\x12%\n\x1fNISCOPE_ATTRIBUTE_CHANNEL_COUNT\x10\xdb\x8c@\x12.\n(NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_PREFIX\x10\xbe\x8d@\x12.\n(NISCOPE_ATTRIBUTE_IO_RESOURCE_DESCRIPTOR\x10\xc0\x8d@\x12$\n\x1eNISCOPE_ATTRIBUTE_LOGICAL_NAME\x10\xc1\x8d@\x12\x33\n-NISCOPE_ATTRIBUTE_SUPPORTED_INSTRUMENT_MODELS\x10\xd7\x8d@\x12*\n$NISCOPE_ATTRIBUTE_GROUP_CAPABILITIES\x10\xa1\x8e@\x12\x34\n.NISCOPE_ATTRIBUTE_INSTRUMENT_FIRMWARE_REVISION\x10\x8e\x8f@\x12/\n)NISCOPE_ATTRIBUTE_INSTRUMENT_MANUFACTURER\x10\x8f\x8f@\x12(\n\"NISCOPE_ATTRIBUTE_INSTRUMENT_MODEL\x10\x90\x8f@\x12.\n(NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_VENDOR\x10\x91\x8f@\x12\x33\n-NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_DESCRIPTION\x10\x92\x8f@\x12@\n:NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_CLASS_SPEC_MAJOR_VERSION\x10\x93\x8f@\x12@\n:NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_CLASS_SPEC_MINOR_VERSION\x10\x94\x8f@\x12\x30\n*NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_REVISION\x10\xb7\x8f@\x12(\n\"NISCOPE_ATTRIBUTE_HORZ_NUM_RECORDS\x10\xb1\x98\x46\x12*\n$NISCOPE_ATTRIBUTE_INPUT_CLOCK_SOURCE\x10\xb2\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_OUTPUT_CLOCK_SOURCE\x10\xb3\x98\x46\x12-\n\'NISCOPE_ATTRIBUTE_HORZ_ENFORCE_REALTIME\x10\xb4\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_BINARY_SAMPLE_WIDTH\x10\xb5\x98\x46\x12*\n$NISCOPE_ATTRIBUTE_TRIGGER_HYSTERESIS\x10\xb6\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_CLOCK_SYNC_PULSE_SOURCE\x10\xb7\x98\x46\x12%\n\x1fNISCOPE_ATTRIBUTE_MASTER_ENABLE\x10\xb8\x98\x46\x12\'\n!NISCOPE_ATTRIBUTE_MIN_SAMPLE_RATE\x10\xb9\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_TRIGGER_WINDOW_MODE\x10\xbc\x98\x46\x12\x30\n*NISCOPE_ATTRIBUTE_TRIGGER_WINDOW_LOW_LEVEL\x10\xbd\x98\x46\x12\x31\n+NISCOPE_ATTRIBUTE_TRIGGER_WINDOW_HIGH_LEVEL\x10\xbe\x98\x46\x12,\n&NISCOPE_ATTRIBUTE_MEAS_REF_LEVEL_UNITS\x10\xc0\x98\x46\x12*\n$NISCOPE_ATTRIBUTE_MEAS_OTHER_CHANNEL\x10\xc2\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_MEAS_HYSTERESIS_PERCENT\x10\xc3\x98\x46\x12\x34\n.NISCOPE_ATTRIBUTE_MEAS_LAST_ACQ_HISTOGRAM_SIZE\x10\xc4\x98\x46\x12\x33\n-NISCOPE_ATTRIBUTE_MEAS_VOLTAGE_HISTOGRAM_SIZE\x10\xc5\x98\x46\x12\x38\n2NISCOPE_ATTRIBUTE_MEAS_VOLTAGE_HISTOGRAM_LOW_VOLTS\x10\xc6\x98\x46\x12\x39\n3NISCOPE_ATTRIBUTE_MEAS_VOLTAGE_HISTOGRAM_HIGH_VOLTS\x10\xc7\x98\x46\x12\x30\n*NISCOPE_ATTRIBUTE_MEAS_TIME_HISTOGRAM_SIZE\x10\xc8\x98\x46\x12\x35\n/NISCOPE_ATTRIBUTE_MEAS_TIME_HISTOGRAM_LOW_VOLTS\x10\xc9\x98\x46\x12\x36\n0NISCOPE_ATTRIBUTE_MEAS_TIME_HISTOGRAM_HIGH_VOLTS\x10\xca\x98\x46\x12\x34\n.NISCOPE_ATTRIBUTE_MEAS_TIME_HISTOGRAM_LOW_TIME\x10\xcb\x98\x46\x12\x35\n/NISCOPE_ATTRIBUTE_MEAS_TIME_HISTOGRAM_HIGH_TIME\x10\xcc\x98\x46\x12;\n5NISCOPE_ATTRIBUTE_MEAS_POLYNOMIAL_INTERPOLATION_ORDER\x10\xcd\x98\x46\x12:\n4NISCOPE_ATTRIBUTE_MEAS_INTERPOLATION_SAMPLING_FACTOR\x10\xce\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_MEAS_FILTER_CUTOFF_FREQ\x10\xcf\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_MEAS_FILTER_CENTER_FREQ\x10\xd0\x98\x46\x12*\n$NISCOPE_ATTRIBUTE_MEAS_FILTER_RIPPLE\x10\xd1\x98\x46\x12>\n8NISCOPE_ATTRIBUTE_MEAS_FILTER_TRANSIENT_WAVEFORM_PERCENT\x10\xd2\x98\x46\x12(\n\"NISCOPE_ATTRIBUTE_MEAS_FILTER_TYPE\x10\xd3\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_MEAS_FILTER_ORDER\x10\xd4\x98\x46\x12(\n\"NISCOPE_ATTRIBUTE_MEAS_FILTER_TAPS\x10\xd5\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_MEAS_CHAN_LOW_REF_LEVEL\x10\xd6\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_MEAS_CHAN_MID_REF_LEVEL\x10\xd7\x98\x46\x12\x30\n*NISCOPE_ATTRIBUTE_MEAS_CHAN_HIGH_REF_LEVEL\x10\xd8\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_MEAS_FILTER_WIDTH\x10\xd9\x98\x46\x12.\n(NISCOPE_ATTRIBUTE_MEAS_FIR_FILTER_WINDOW\x10\xda\x98\x46\x12\'\n!NISCOPE_ATTRIBUTE_MEAS_ARRAY_GAIN\x10\xdb\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_MEAS_ARRAY_OFFSET\x10\xdc\x98\x46\x12.\n(NISCOPE_ATTRIBUTE_MEAS_PERCENTAGE_METHOD\x10\xdd\x98\x46\x12&\n NISCOPE_ATTRIBUTE_ACQ_ARM_SOURCE\x10\xe5\x98\x46\x12(\n\"NISCOPE_ATTRIBUTE_IS_PROBE_COMP_ON\x10\xf2\x98\x46\x12*\n$NISCOPE_ATTRIBUTE_USE_SPEC_INITIAL_X\x10\xf3\x98\x46\x12\x36\n0NISCOPE_ATTRIBUTE_ALLOW_MORE_RECORDS_THAN_MEMORY\x10\xf4\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_ONBOARD_MEMORY_SIZE\x10\xf5\x98\x46\x12(\n\"NISCOPE_ATTRIBUTE_RIS_NUM_AVERAGES\x10\xf6\x98\x46\x12\"\n\x1cNISCOPE_ATTRIBUTE_RIS_METHOD\x10\xf7\x98\x46\x12.\n(NISCOPE_ATTRIBUTE_FETCH_INTERLEAVED_DATA\x10\xf8\x98\x46\x12\x33\n-NISCOPE_ATTRIBUTE_MAX_REAL_TIME_SAMPLING_RATE\x10\xf9\x98\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_MAX_RIS_RATE\x10\xfa\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_TRIGGER_IMPEDANCE\x10\xfb\x98\x46\x12%\n\x1fNISCOPE_ATTRIBUTE_DEVICE_NUMBER\x10\xfc\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_FETCH_RELATIVE_TO\x10\xfd\x98\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_FETCH_OFFSET\x10\xfe\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_FETCH_RECORD_NUMBER\x10\xff\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_FETCH_NUM_RECORDS\x10\x80\x99\x46\x12.\n(NISCOPE_ATTRIBUTE_FETCH_MEAS_NUM_SAMPLES\x10\x81\x99\x46\x12#\n\x1dNISCOPE_ATTRIBUTE_POINTS_DONE\x10\x82\x99\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_RECORDS_DONE\x10\x83\x99\x46\x12\x1f\n\x19NISCOPE_ATTRIBUTE_BACKLOG\x10\x84\x99\x46\x12*\n$NISCOPE_ATTRIBUTE_DEVICE_TEMPERATURE\x10\x86\x99\x46\x12-\n\'NISCOPE_ATTRIBUTE_SAMP_CLK_TIMEBASE_SRC\x10\x87\x99\x46\x12.\n(NISCOPE_ATTRIBUTE_SAMP_CLK_TIMEBASE_RATE\x10\x88\x99\x46\x12-\n\'NISCOPE_ATTRIBUTE_SAMP_CLK_TIMEBASE_DIV\x10\x89\x99\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_REF_CLK_RATE\x10\x8a\x99\x46\x12=\n7NISCOPE_ATTRIBUTE_EXPORTED_SAMPLE_CLOCK_OUTPUT_TERMINAL\x10\x8b\x99\x46\x12)\n#NISCOPE_ATTRIBUTE_ENABLE_DC_RESTORE\x10\x8d\x99\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_ADV_TRIG_SRC\x10\x8e\x99\x46\x12(\n\"NISCOPE_ATTRIBUTE_ARM_REF_TRIG_SRC\x10\x8f\x99\x46\x12+\n%NISCOPE_ATTRIBUTE_REF_TRIG_TDC_ENABLE\x10\x90\x99\x46\x12>\n8NISCOPE_ATTRIBUTE_EXPORTED_START_TRIGGER_OUTPUT_TERMINAL\x10\x91\x99\x46\x12<\n6NISCOPE_ATTRIBUTE_EXPORTED_REF_TRIGGER_OUTPUT_TERMINAL\x10\x92\x99\x46\x12;\n5NISCOPE_ATTRIBUTE_END_OF_RECORD_EVENT_OUTPUT_TERMINAL\x10\x93\x99\x46\x12%\n\x1fNISCOPE_ATTRIBUTE_POLL_INTERVAL\x10\x94\x99\x46\x12@\n:NISCOPE_ATTRIBUTE_END_OF_ACQUISITION_EVENT_OUTPUT_TERMINAL\x10\x95\x99\x46\x12\"\n\x1cNISCOPE_ATTRIBUTE_RESOLUTION\x10\x96\x99\x46\x12\x34\n.NISCOPE_ATTRIBUTE_START_TO_REF_TRIGGER_HOLDOFF\x10\x97\x99\x46\x12%\n\x1fNISCOPE_ATTRIBUTE_SERIAL_NUMBER\x10\x98\x99\x46\x12\x32\n,NISCOPE_ATTRIBUTE_OSCILLATOR_PHASE_DAC_VALUE\x10\x99\x99\x46\x12\x30\n*NISCOPE_ATTRIBUTE_RIS_IN_AUTO_SETUP_ENABLE\x10\x9a\x99\x46\x12\x36\n0NISCOPE_ATTRIBUTE_CHANNEL_TERMINAL_CONFIGURATION\x10\x9b\x99\x46\x12@\n:NISCOPE_ATTRIBUTE_EXPORTED_ADVANCE_TRIGGER_OUTPUT_TERMINAL\x10\x9d\x99\x46\x12=\n7NISCOPE_ATTRIBUTE_READY_FOR_START_EVENT_OUTPUT_TERMINAL\x10\x9e\x99\x46\x12;\n5NISCOPE_ATTRIBUTE_READY_FOR_REF_EVENT_OUTPUT_TERMINAL\x10\x9f\x99\x46\x12?\n9NISCOPE_ATTRIBUTE_READY_FOR_ADVANCE_EVENT_OUTPUT_TERMINAL\x10\xa0\x99\x46\x12\x38\n2NISCOPE_ATTRIBUTE_ENABLE_TIME_INTERLEAVED_SAMPLING\x10\xb0\x99\x46\x12.\n(NISCOPE_ATTRIBUTE_5V_OUT_OUTPUT_TERMINAL\x10\xb1\x99\x46\x12+\n%NISCOPE_ATTRIBUTE_RUNT_TIME_CONDITION\x10\xb4\x99\x46\x12+\n%NISCOPE_ATTRIBUTE_RUNT_TIME_LOW_LIMIT\x10\xb5\x99\x46\x12,\n&NISCOPE_ATTRIBUTE_RUNT_TIME_HIGH_LIMIT\x10\xb6\x99\x46\x12+\n%NISCOPE_ATTRIBUTE_CABLE_SENSE_VOLTAGE\x10\xb9\x99\x46\x12(\n\"NISCOPE_ATTRIBUTE_CABLE_SENSE_MODE\x10\xba\x99\x46\x12\x31\n+NISCOPE_ATTRIBUTE_CABLE_SENSE_SIGNAL_ENABLE\x10\xbb\x99\x46\x12(\n\"NISCOPE_ATTRIBUTE_ENABLED_CHANNELS\x10\xbc\x99\x46\x12>\n8NISCOPE_ATTRIBUTE_END_OF_ACQUISITION_EVENT_TERMINAL_NAME\x10\xbd\x99\x46\x12\x39\n3NISCOPE_ATTRIBUTE_END_OF_RECORD_EVENT_TERMINAL_NAME\x10\xbe\x99\x46\x12\x35\n/NISCOPE_ATTRIBUTE_ADVANCE_TRIGGER_TERMINAL_NAME\x10\xbf\x99\x46\x12\x31\n+NISCOPE_ATTRIBUTE_REF_TRIGGER_TERMINAL_NAME\x10\xc0\x99\x46\x12\x33\n-NISCOPE_ATTRIBUTE_START_TRIGGER_TERMINAL_NAME\x10\xc1\x99\x46\x12=\n7NISCOPE_ATTRIBUTE_READY_FOR_ADVANCE_EVENT_TERMINAL_NAME\x10\xc2\x99\x46\x12\x39\n3NISCOPE_ATTRIBUTE_READY_FOR_REF_EVENT_TERMINAL_NAME\x10\xc3\x99\x46\x12;\n5NISCOPE_ATTRIBUTE_READY_FOR_START_EVENT_TERMINAL_NAME\x10\xc4\x99\x46\x12\x36\n0NISCOPE_ATTRIBUTE_FLEX_FIR_ANTIALIAS_FILTER_TYPE\x10\xbf\x9a\x46\x12.\n(NISCOPE_ATTRIBUTE_TRIGGER_AUTO_TRIGGERED\x10\xc6\x9a\x46\x12(\n\"NISCOPE_ATTRIBUTE_SIGNAL_COND_GAIN\x10\xc7\x9a\x46\x12*\n$NISCOPE_ATTRIBUTE_SIGNAL_COND_OFFSET\x10\xc8\x9a\x46\x12#\n\x1dNISCOPE_ATTRIBUTE_DDC_ENABLED\x10\xdc\x9a\x46\x12\x39\n3NISCOPE_ATTRIBUTE_DDC_FREQUENCY_TRANSLATION_ENABLED\x10\xde\x9a\x46\x12,\n&NISCOPE_ATTRIBUTE_DDC_CENTER_FREQUENCY\x10\xdf\x9a\x46\x12\x30\n*NISCOPE_ATTRIBUTE_DDC_DATA_PROCESSING_MODE\x10\xe0\x9a\x46\x12\x39\n3NISCOPE_ATTRIBUTE_DDC_FREQUENCY_TRANSLATION_PHASE_I\x10\xe1\x9a\x46\x12\x39\n3NISCOPE_ATTRIBUTE_DDC_FREQUENCY_TRANSLATION_PHASE_Q\x10\xe2\x9a\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_DIGITAL_GAIN\x10\xe3\x9a\x46\x12&\n NISCOPE_ATTRIBUTE_DIGITAL_OFFSET\x10\xe4\x9a\x46\x12\x30\n*NISCOPE_ATTRIBUTE_OVERFLOW_ERROR_REPORTING\x10\xe5\x9a\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_DDC_Q_SOURCE\x10\xe6\x9a\x46\x12\x31\n+NISCOPE_ATTRIBUTE_FETCH_INTERLEAVED_IQ_DATA\x10\xe7\x9a\x46\x12\x35\n/NISCOPE_ATTRIBUTE_EQUALIZATION_NUM_COEFFICIENTS\x10\xe8\x9a\x46\x12\x33\n-NISCOPE_ATTRIBUTE_EQUALIZATION_FILTER_ENABLED\x10\xe9\x9a\x46\x12\x35\n/NISCOPE_ATTRIBUTE_REF_TRIGGER_DETECTOR_LOCATION\x10\xea\x9a\x46\x12\x36\n0NISCOPE_ATTRIBUTE_REF_TRIGGER_MINIMUM_QUIET_TIME\x10\xeb\x9a\x46\x12\x30\n*NISCOPE_ATTRIBUTE_DATA_TRANSFER_BLOCK_SIZE\x10\xec\x9a\x46\x12/\n)NISCOPE_ATTRIBUTE_BANDPASS_FILTER_ENABLED\x10\xee\x9a\x46\x12&\n NISCOPE_ATTRIBUTE_DITHER_ENABLED\x10\xef\x9a\x46\x12\x33\n-NISCOPE_ATTRIBUTE_FRACTIONAL_RESAMPLE_ENABLED\x10\xf0\x9a\x46\x12\x37\n1NISCOPE_ATTRIBUTE_DATA_TRANSFER_MAXIMUM_BANDWIDTH\x10\xf1\x9a\x46\x12;\n5NISCOPE_ATTRIBUTE_DATA_TRANSFER_PREFERRED_PACKET_SIZE\x10\xf2\x9a\x46\x12\x35\n/NISCOPE_ATTRIBUTE_P2P_SAMPLES_AVAIL_IN_ENDPOINT\x10\xf8\x9a\x46\x12\x36\n0NISCOPE_ATTRIBUTE_P2P_DATA_TRANS_PERMISSION_ADDR\x10\xf9\x9a\x46\x12;\n5NISCOPE_ATTRIBUTE_P2P_DATA_TRANS_PERMISSION_ADDR_TYPE\x10\xfa\x9a\x46\x12\x33\n-NISCOPE_ATTRIBUTE_P2P_DESTINATION_WINDOW_ADDR\x10\xfb\x9a\x46\x12\x38\n2NISCOPE_ATTRIBUTE_P2P_DESTINATION_WINDOW_ADDR_TYPE\x10\xfc\x9a\x46\x12\x33\n-NISCOPE_ATTRIBUTE_P2P_DESTINATION_WINDOW_SIZE\x10\xfd\x9a\x46\x12\x32\n,NISCOPE_ATTRIBUTE_P2P_NOTIFY_PUSH_MESSAGE_ON\x10\xfe\x9a\x46\x12\x34\n.NISCOPE_ATTRIBUTE_P2P_NOTIFY_MESSAGE_PUSH_ADDR\x10\xff\x9a\x46\x12\x39\n3NISCOPE_ATTRIBUTE_P2P_NOTIFY_MESSAGE_PUSH_ADDR_TYPE\x10\x80\x9b\x46\x12\x35\n/NISCOPE_ATTRIBUTE_P2P_NOTIFY_MESSAGE_PUSH_VALUE\x10\x81\x9b\x46\x12#\n\x1dNISCOPE_ATTRIBUTE_P2P_ENABLED\x10\x82\x9b\x46\x12.\n(NISCOPE_ATTRIBUTE_P2P_CHANNELS_TO_STREAM\x10\x83\x9b\x46\x12/\n)NISCOPE_ATTRIBUTE_P2P_SAMPLES_TRANSFERRED\x10\x84\x9b\x46\x12:\n4NISCOPE_ATTRIBUTE_P2P_MOST_SAMPLES_AVAIL_IN_ENDPOINT\x10\x85\x9b\x46\x12)\n#NISCOPE_ATTRIBUTE_P2P_ENDPOINT_SIZE\x10\x86\x9b\x46\x12\x38\n2NISCOPE_ATTRIBUTE_P2P_MANUAL_CONFIGURATION_ENABLED\x10\x87\x9b\x46\x12-\n\'NISCOPE_ATTRIBUTE_P2P_ENDPOINT_OVERFLOW\x10\x88\x9b\x46\x12/\n)NISCOPE_ATTRIBUTE_P2P_FIFO_ENDPOINT_COUNT\x10\x89\x9b\x46\x12\x32\n,NISCOPE_ATTRIBUTE_P2P_ONBOARD_MEMORY_ENABLED\x10\x92\x9b\x46\x12@\n:NISCOPE_ATTRIBUTE_END_OF_RECORD_TO_ADVANCE_TRIGGER_HOLDOFF\x10\x9e\x9b\x46\x12.\n(NISCOPE_ATTRIBUTE_SAMP_CLK_TIMEBASE_MULT\x10\x9f\x9b\x46\x12.\n(NISCOPE_ATTRIBUTE_P2P_STREAM_RELATIVE_TO\x10\xa5\x9b\x46\x12\x34\n.NISCOPE_ATTRIBUTE_ABSOLUTE_SAMPLE_CLOCK_OFFSET\x10\xa6\x9b\x46\x12)\n#NISCOPE_ATTRIBUTE_FPGA_BITFILE_PATH\x10\xa7\x9b\x46\x12>\n8NISCOPE_ATTRIBUTE_INTERLEAVING_OFFSET_CORRECTION_ENABLED\x10\xa8\x9b\x46\x12\x32\n,NISCOPE_ATTRIBUTE_HIGH_PASS_FILTER_FREQUENCY\x10\xa9\x9b\x46\x12:\n4NISCOPE_ATTRIBUTE_P2P_SAMPLES_TRANSFERRED_PER_RECORD\x10\xac\x9b\x46\x12\'\n!NISCOPE_ATTRIBUTE_PLL_LOCK_STATUS\x10\xc7\xa2\x46\x12&\n NISCOPE_ATTRIBUTE_VERTICAL_RANGE\x10\xd1\xa5L\x12\'\n!NISCOPE_ATTRIBUTE_VERTICAL_OFFSET\x10\xd2\xa5L\x12)\n#NISCOPE_ATTRIBUTE_VERTICAL_COUPLING\x10\xd3\xa5L\x12)\n#NISCOPE_ATTRIBUTE_PROBE_ATTENUATION\x10\xd4\xa5L\x12\'\n!NISCOPE_ATTRIBUTE_CHANNEL_ENABLED\x10\xd5\xa5L\x12+\n%NISCOPE_ATTRIBUTE_MAX_INPUT_FREQUENCY\x10\xd6\xa5L\x12,\n&NISCOPE_ATTRIBUTE_HORZ_TIME_PER_RECORD\x10\xd7\xa5L\x12*\n$NISCOPE_ATTRIBUTE_HORZ_RECORD_LENGTH\x10\xd8\xa5L\x12(\n\"NISCOPE_ATTRIBUTE_HORZ_MIN_NUM_PTS\x10\xd9\xa5L\x12(\n\"NISCOPE_ATTRIBUTE_HORZ_SAMPLE_RATE\x10\xda\xa5L\x12\x30\n*NISCOPE_ATTRIBUTE_HORZ_RECORD_REF_POSITION\x10\xdb\xa5L\x12$\n\x1eNISCOPE_ATTRIBUTE_TRIGGER_TYPE\x10\xdc\xa5L\x12&\n NISCOPE_ATTRIBUTE_TRIGGER_SOURCE\x10\xdd\xa5L\x12(\n\"NISCOPE_ATTRIBUTE_TRIGGER_COUPLING\x10\xde\xa5L\x12*\n$NISCOPE_ATTRIBUTE_TRIGGER_DELAY_TIME\x10\xdf\xa5L\x12\'\n!NISCOPE_ATTRIBUTE_TRIGGER_HOLDOFF\x10\xe0\xa5L\x12%\n\x1fNISCOPE_ATTRIBUTE_TRIGGER_LEVEL\x10\xe1\xa5L\x12%\n\x1fNISCOPE_ATTRIBUTE_TRIGGER_SLOPE\x10\xe2\xa5L\x12(\n\"NISCOPE_ATTRIBUTE_ACQUISITION_TYPE\x10\xb5\xa6L\x12(\n\"NISCOPE_ATTRIBUTE_TRIGGER_MODIFIER\x10\xb6\xa6L\x12\'\n!NISCOPE_ATTRIBUTE_INPUT_IMPEDANCE\x10\xb7\xa6L\x12#\n\x1dNISCOPE_ATTRIBUTE_SAMPLE_MODE\x10\xba\xa6L\x12.\n(NISCOPE_ATTRIBUTE_ACQUISITION_START_TIME\x10\xbd\xa6L\x12\x30\n*NISCOPE_ATTRIBUTE_TV_TRIGGER_SIGNAL_FORMAT\x10\x99\xa7L\x12+\n%NISCOPE_ATTRIBUTE_TV_TRIGGER_POLARITY\x10\x9c\xa7L\x12(\n\"NISCOPE_ATTRIBUTE_TV_TRIGGER_EVENT\x10\x9d\xa7L\x12.\n(NISCOPE_ATTRIBUTE_TV_TRIGGER_LINE_NUMBER\x10\x9e\xa7L\x12+\n%NISCOPE_ATTRIBUTE_RUNT_HIGH_THRESHOLD\x10\xfd\xa7L\x12*\n$NISCOPE_ATTRIBUTE_RUNT_LOW_THRESHOLD\x10\xfe\xa7L\x12%\n\x1fNISCOPE_ATTRIBUTE_RUNT_POLARITY\x10\xff\xa7L\x12$\n\x1eNISCOPE_ATTRIBUTE_GLITCH_WIDTH\x10\xe1\xa8L\x12\'\n!NISCOPE_ATTRIBUTE_GLITCH_POLARITY\x10\xe2\xa8L\x12(\n\"NISCOPE_ATTRIBUTE_GLITCH_CONDITION\x10\xe3\xa8L\x12+\n%NISCOPE_ATTRIBUTE_WIDTH_LOW_THRESHOLD\x10\xc5\xa9L\x12,\n&NISCOPE_ATTRIBUTE_WIDTH_HIGH_THRESHOLD\x10\xc6\xa9L\x12&\n NISCOPE_ATTRIBUTE_WIDTH_POLARITY\x10\xc7\xa9L\x12\'\n!NISCOPE_ATTRIBUTE_WIDTH_CONDITION\x10\xc8\xa9L\x12%\n\x1fNISCOPE_ATTRIBUTE_MEAS_HIGH_REF\x10\xaf\xaaL\x12$\n\x1eNISCOPE_ATTRIBUTE_MEAS_LOW_REF\x10\xb0\xaaL\x12$\n\x1eNISCOPE_ATTRIBUTE_MEAS_MID_REF\x10\xb1\xaaL*\xb8\x01\n\x11\x41\x63quisitionStatus\x12\x32\n.ACQUISITION_STATUS_NISCOPE_VAL_ACQ_IN_PROGRESS\x10\x00\x12/\n+ACQUISITION_STATUS_NISCOPE_VAL_ACQ_COMPLETE\x10\x01\x12>\n1ACQUISITION_STATUS_NISCOPE_VAL_ACQ_STATUS_UNKNOWN\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01*\xd4\x0b\n\x10\x41rrayMeasurement\x12!\n\x1d\x41RRAY_MEASUREMENT_UNSPECIFIED\x10\x00\x12\x31\n,ARRAY_MEASUREMENT_NISCOPE_VAL_NO_MEASUREMENT\x10\xa0\x1f\x12\x35\n0ARRAY_MEASUREMENT_NISCOPE_VAL_LAST_ACQ_HISTOGRAM\x10\xa1\x1f\x12\x35\n0ARRAY_MEASUREMENT_NISCOPE_VAL_FFT_PHASE_SPECTRUM\x10\xa2\x1f\x12=\n8ARRAY_MEASUREMENT_NISCOPE_VAL_FFT_AMP_SPECTRUM_VOLTS_RMS\x10\xa3\x1f\x12>\n9ARRAY_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_VOLTAGE_HISTOGRAM\x10\xa4\x1f\x12;\n6ARRAY_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_TIME_HISTOGRAM\x10\xa5\x1f\x12\x31\n,ARRAY_MEASUREMENT_NISCOPE_VAL_ARRAY_INTEGRAL\x10\xa6\x1f\x12-\n(ARRAY_MEASUREMENT_NISCOPE_VAL_DERIVATIVE\x10\xa7\x1f\x12*\n%ARRAY_MEASUREMENT_NISCOPE_VAL_INVERSE\x10\xa8\x1f\x12\x31\n,ARRAY_MEASUREMENT_NISCOPE_VAL_HANNING_WINDOW\x10\xa9\x1f\x12\x32\n-ARRAY_MEASUREMENT_NISCOPE_VAL_FLAT_TOP_WINDOW\x10\xaa\x1f\x12;\n6ARRAY_MEASUREMENT_NISCOPE_VAL_POLYNOMIAL_INTERPOLATION\x10\xab\x1f\x12\x34\n/ARRAY_MEASUREMENT_NISCOPE_VAL_MULTIPLY_CHANNELS\x10\xac\x1f\x12/\n*ARRAY_MEASUREMENT_NISCOPE_VAL_ADD_CHANNELS\x10\xad\x1f\x12\x34\n/ARRAY_MEASUREMENT_NISCOPE_VAL_SUBTRACT_CHANNELS\x10\xae\x1f\x12\x32\n-ARRAY_MEASUREMENT_NISCOPE_VAL_DIVIDE_CHANNELS\x10\xaf\x1f\x12\x34\n/ARRAY_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_AVERAGE\x10\xb0\x1f\x12\x35\n0ARRAY_MEASUREMENT_NISCOPE_VAL_BUTTERWORTH_FILTER\x10\xb1\x1f\x12\x33\n.ARRAY_MEASUREMENT_NISCOPE_VAL_CHEBYSHEV_FILTER\x10\xb2\x1f\x12\x36\n1ARRAY_MEASUREMENT_NISCOPE_VAL_FFT_AMP_SPECTRUM_DB\x10\xb3\x1f\x12\x31\n,ARRAY_MEASUREMENT_NISCOPE_VAL_HAMMING_WINDOW\x10\xb4\x1f\x12\x36\n1ARRAY_MEASUREMENT_NISCOPE_VAL_WINDOWED_FIR_FILTER\x10\xb5\x1f\x12\x30\n+ARRAY_MEASUREMENT_NISCOPE_VAL_BESSEL_FILTER\x10\xb6\x1f\x12\x32\n-ARRAY_MEASUREMENT_NISCOPE_VAL_TRIANGLE_WINDOW\x10\xb7\x1f\x12\x32\n-ARRAY_MEASUREMENT_NISCOPE_VAL_BLACKMAN_WINDOW\x10\xb8\x1f\x12/\n*ARRAY_MEASUREMENT_NISCOPE_VAL_ARRAY_OFFSET\x10\xb9\x1f\x12-\n(ARRAY_MEASUREMENT_NISCOPE_VAL_ARRAY_GAIN\x10\xba\x1f*\xa1\x01\n\x10\x43\x61librationTypes\x12.\n*CALIBRATION_TYPES_NISCOPE_VAL_CAL_EXTERNAL\x10\x00\x12*\n&CALIBRATION_TYPES_NISCOPE_VAL_CAL_SELF\x10\x01\x12\x31\n-CALIBRATION_TYPES_NISCOPE_VAL_CAL_MANUFACTURE\x10\x02*\xb3\x1e\n\x14\x43learableMeasurement\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_RISE_TIME\x10\x00\x12\x37\n2CLEARABLE_MEASUREMENT_NISCOPE_VAL_ALL_MEASUREMENTS\x10\x90N\x12\x42\n=CLEARABLE_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_VOLTAGE_HISTOGRAM\x10\xa4\x1f\x12?\n:CLEARABLE_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_TIME_HISTOGRAM\x10\xa5\x1f\x12\x38\n3CLEARABLE_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_AVERAGE\x10\xb0\x1f\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_FREQUENCY\x10\x02\x12\x38\n3CLEARABLE_MEASUREMENT_NISCOPE_VAL_AVERAGE_FREQUENCY\x10\xf8\x07\x12\x34\n/CLEARABLE_MEASUREMENT_NISCOPE_VAL_FFT_FREQUENCY\x10\xf0\x07\x12,\n(CLEARABLE_MEASUREMENT_NISCOPE_VAL_PERIOD\x10\x03\x12\x35\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_AVERAGE_PERIOD\x10\xf7\x07\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_FALL_TIME\x10\x01\x12\x35\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_RISE_SLEW_RATE\x10\xf2\x07\x12\x35\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_FALL_SLEW_RATE\x10\xf3\x07\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_OVERSHOOT\x10\x12\x12.\n*CLEARABLE_MEASUREMENT_NISCOPE_VAL_PRESHOOT\x10\x13\x12\x31\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_RMS\x10\x04\x12\x37\n3CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_CYCLE_RMS\x10\x10\x12\x32\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_AC_ESTIMATE\x10\xf4\x07\x12\x34\n/CLEARABLE_MEASUREMENT_NISCOPE_VAL_FFT_AMPLITUDE\x10\xf1\x07\x12\x35\n1CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_AVERAGE\x10\n\x12;\n7CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_CYCLE_AVERAGE\x10\x11\x12\x32\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_DC_ESTIMATE\x10\xf5\x07\x12\x31\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_MAX\x10\x06\x12\x31\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_MIN\x10\x07\x12:\n6CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_PEAK_TO_PEAK\x10\x05\x12\x32\n.CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HIGH\x10\x08\x12\x31\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_LOW\x10\t\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_AMPLITUDE\x10\x0f\x12\x32\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_TOP\x10\xef\x07\x12\x33\n.CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_BASE\x10\xee\x07\x12:\n5CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_BASE_TO_TOP\x10\xf9\x07\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_WIDTH_NEG\x10\x0b\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_WIDTH_POS\x10\x0c\x12\x34\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_DUTY_CYCLE_NEG\x10\r\x12\x34\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_DUTY_CYCLE_POS\x10\x0e\x12/\n*CLEARABLE_MEASUREMENT_NISCOPE_VAL_INTEGRAL\x10\xed\x07\x12+\n&CLEARABLE_MEASUREMENT_NISCOPE_VAL_AREA\x10\xeb\x07\x12\x31\n,CLEARABLE_MEASUREMENT_NISCOPE_VAL_CYCLE_AREA\x10\xec\x07\x12\x31\n,CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_DELAY\x10\xf6\x07\x12\x32\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_PHASE_DELAY\x10\xfa\x07\x12\x34\n/CLEARABLE_MEASUREMENT_NISCOPE_VAL_LOW_REF_VOLTS\x10\xe8\x07\x12\x34\n/CLEARABLE_MEASUREMENT_NISCOPE_VAL_MID_REF_VOLTS\x10\xe9\x07\x12\x35\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_HIGH_REF_VOLTS\x10\xea\x07\x12=\n8CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MEAN\x10\xd0\x0f\x12>\n9CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_STDEV\x10\xd1\x0f\x12?\n:CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MEDIAN\x10\xd3\x0f\x12=\n8CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MODE\x10\xda\x0f\x12<\n7CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MAX\x10\xd5\x0f\x12<\n7CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MIN\x10\xd6\x0f\x12\x45\n@CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_PEAK_TO_PEAK\x10\xd2\x0f\x12H\nCCLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MEAN_PLUS_STDEV\x10\xd7\x0f\x12J\nECLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MEAN_PLUS_2_STDEV\x10\xd8\x0f\x12J\nECLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MEAN_PLUS_3_STDEV\x10\xd9\x0f\x12=\n8CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_HITS\x10\xd4\x0f\x12\x41\n<CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_NEW_HITS\x10\xdb\x0f\x12:\n5CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MEAN\x10\xb8\x17\x12;\n6CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_STDEV\x10\xb9\x17\x12<\n7CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MEDIAN\x10\xbb\x17\x12:\n5CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MODE\x10\xc2\x17\x12\x39\n4CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MAX\x10\xbd\x17\x12\x39\n4CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MIN\x10\xbe\x17\x12\x42\n=CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_PEAK_TO_PEAK\x10\xba\x17\x12\x45\n@CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MEAN_PLUS_STDEV\x10\xbf\x17\x12G\nBCLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MEAN_PLUS_2_STDEV\x10\xc0\x17\x12G\nBCLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MEAN_PLUS_3_STDEV\x10\xc1\x17\x12:\n5CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_HITS\x10\xbc\x17\x12>\n9CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_NEW_HITS\x10\xc3\x17*\x96\x07\n\x16\x43lockingTerminalValues\x12(\n$CLOCKING_TERMINAL_VALUES_UNSPECIFIED\x10\x00\x12\x32\n.CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_NO_SOURCE\x10\x01\x12\x33\n/CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_RTSI_CLOCK\x10\x02\x12\x31\n-CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_EXTERNAL\x10\x03\x12.\n*CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PFI_0\x10\x04\x12.\n*CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PFI_1\x10\x05\x12.\n*CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PFI_2\x10\x06\x12/\n+CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_CLK_IN\x10\x07\x12\x30\n,CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_CLK_OUT\x10\x08\x12:\n6CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_INTERNAL10MHZ_OSC\x10\t\x12\x30\n,CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PXI_CLK\x10\n\x12\x32\n.CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PXI_CLK10\x10\x0b\x12\x33\n/CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PXI_CLK100\x10\x0c\x12\x35\n1CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PXIE_DSTAR_A\x10\r\x12\x35\n1CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_AUX_0_CLK_IN\x10\x0e\x12\x36\n2CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_AUX_0_CLK_OUT\x10\x0f\x12\x46\nBCLOCKING_TERMINAL_VALUES_NISCOPE_VAL_ONBOARD_CONFIGURABLE_RATE_CLK\x10\x10*\xfa\x04\n\x11\x45xportableSignals\x12\"\n\x1e\x45XPORTABLE_SIGNALS_UNSPECIFIED\x10\x00\x12.\n*EXPORTABLE_SIGNALS_NISCOPE_VAL_REF_TRIGGER\x10\x01\x12\x30\n,EXPORTABLE_SIGNALS_NISCOPE_VAL_START_TRIGGER\x10\x02\x12;\n7EXPORTABLE_SIGNALS_NISCOPE_VAL_END_OF_ACQUISITION_EVENT\x10\x03\x12\x36\n2EXPORTABLE_SIGNALS_NISCOPE_VAL_END_OF_RECORD_EVENT\x10\x04\x12\x32\n.EXPORTABLE_SIGNALS_NISCOPE_VAL_ADVANCE_TRIGGER\x10\x05\x12:\n6EXPORTABLE_SIGNALS_NISCOPE_VAL_READY_FOR_ADVANCE_EVENT\x10\x06\x12\x38\n4EXPORTABLE_SIGNALS_NISCOPE_VAL_READY_FOR_START_EVENT\x10\x07\x12\x36\n2EXPORTABLE_SIGNALS_NISCOPE_VAL_READY_FOR_REF_EVENT\x10\n\x12)\n%EXPORTABLE_SIGNALS_NISCOPE_VAL_5V_OUT\x10\r\x12,\n(EXPORTABLE_SIGNALS_NISCOPE_VAL_REF_CLOCK\x10\x64\x12/\n+EXPORTABLE_SIGNALS_NISCOPE_VAL_SAMPLE_CLOCK\x10\x65*\x9c\x01\n\x0fGlitchCondition\x12 \n\x1cGLITCH_CONDITION_UNSPECIFIED\x10\x00\x12\x34\n0GLITCH_CONDITION_NISCOPE_VAL_GLITCH_GREATER_THAN\x10\x02\x12\x31\n-GLITCH_CONDITION_NISCOPE_VAL_GLITCH_LESS_THAN\x10\x01*\xc2\x01\n\x0eGlitchPolarity\x12\x1f\n\x1bGLITCH_POLARITY_UNSPECIFIED\x10\x00\x12/\n+GLITCH_POLARITY_NISCOPE_VAL_GLITCH_POSITIVE\x10\x01\x12/\n+GLITCH_POLARITY_NISCOPE_VAL_GLITCH_NEGATIVE\x10\x02\x12-\n)GLITCH_POLARITY_NISCOPE_VAL_GLITCH_EITHER\x10\x03*\xad\x35\n\x1bNiScopeInt32AttributeValues\x12\x1d\n\x19NISCOPE_INT32_UNSPECIFIED\x10\x00\x12-\n)NISCOPE_INT32_ACQUISITION_TYPE_VAL_NORMAL\x10\x00\x12/\n*NISCOPE_INT32_ACQUISITION_TYPE_VAL_FLEXRES\x10\xe9\x07\x12+\n&NISCOPE_INT32_ACQUISITION_TYPE_VAL_DDC\x10\xea\x07\x12\x30\n,NISCOPE_INT32_ADDRESS_TYPE_VAL_ADDR_PHYSICAL\x10\x00\x12/\n+NISCOPE_INT32_ADDRESS_TYPE_VAL_ADDR_VIRTUAL\x10\x01\x12/\n+NISCOPE_INT32_DATA_PROCESSING_MODE_VAL_REAL\x10\x00\x12\x32\n.NISCOPE_INT32_DATA_PROCESSING_MODE_VAL_COMPLEX\x10\x01\x12,\n(NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_NONE\x10\x00\x12\x30\n+NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_HANNING\x10\x99\x03\x12\x31\n,NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_FLAT_TOP\x10\x9a\x03\x12\x30\n+NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_HAMMING\x10\xa4\x03\x12\x31\n,NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_TRIANGLE\x10\xa7\x03\x12\x31\n,NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_BLACKMAN\x10\xa8\x03\x12\x35\n0NISCOPE_INT32_FETCH_RELATIVE_TO_VAL_READ_POINTER\x10\x84\x03\x12\x33\n.NISCOPE_INT32_FETCH_RELATIVE_TO_VAL_PRETRIGGER\x10\xdd\x03\x12,\n\'NISCOPE_INT32_FETCH_RELATIVE_TO_VAL_NOW\x10\xe1\x03\x12.\n)NISCOPE_INT32_FETCH_RELATIVE_TO_VAL_START\x10\xe2\x03\x12\x30\n+NISCOPE_INT32_FETCH_RELATIVE_TO_VAL_TRIGGER\x10\xe3\x03\x12\x44\n@NISCOPE_INT32_FLEX_FIR_ANTIALIAS_FILTER_TYPE_VAL_48_TAP_STANDARD\x10\x00\x12\x43\n?NISCOPE_INT32_FLEX_FIR_ANTIALIAS_FILTER_TYPE_VAL_48_TAP_HANNING\x10\x01\x12\x43\n?NISCOPE_INT32_FLEX_FIR_ANTIALIAS_FILTER_TYPE_VAL_16_TAP_HANNING\x10\x02\x12\x42\n>NISCOPE_INT32_FLEX_FIR_ANTIALIAS_FILTER_TYPE_VAL_8_TAP_HANNING\x10\x03\x12:\n6NISCOPE_INT32_GLITCH_CONDITION_VAL_GLITCH_GREATER_THAN\x10\x02\x12\x37\n3NISCOPE_INT32_GLITCH_CONDITION_VAL_GLITCH_LESS_THAN\x10\x01\x12\x35\n1NISCOPE_INT32_GLITCH_POLARITY_VAL_GLITCH_POSITIVE\x10\x01\x12\x35\n1NISCOPE_INT32_GLITCH_POLARITY_VAL_GLITCH_NEGATIVE\x10\x02\x12\x33\n/NISCOPE_INT32_GLITCH_POLARITY_VAL_GLITCH_EITHER\x10\x03\x12\x33\n/NISCOPE_INT32_MEAS_FILTER_TYPE_VAL_MEAS_LOWPASS\x10\x00\x12\x34\n0NISCOPE_INT32_MEAS_FILTER_TYPE_VAL_MEAS_HIGHPASS\x10\x01\x12\x34\n0NISCOPE_INT32_MEAS_FILTER_TYPE_VAL_MEAS_BANDPASS\x10\x02\x12\x34\n0NISCOPE_INT32_MEAS_FILTER_TYPE_VAL_MEAS_BANDSTOP\x10\x03\x12:\n6NISCOPE_INT32_MEAS_PERCENTAGE_METHOD_VAL_MEAS_LOW_HIGH\x10\x00\x12\x39\n5NISCOPE_INT32_MEAS_PERCENTAGE_METHOD_VAL_MEAS_MIN_MAX\x10\x01\x12:\n6NISCOPE_INT32_MEAS_PERCENTAGE_METHOD_VAL_MEAS_BASE_TOP\x10\x02\x12\x37\n3NISCOPE_INT32_MEAS_REF_LEVEL_UNITS_VAL_MEAS_VOLTAGE\x10\x00\x12:\n6NISCOPE_INT32_MEAS_REF_LEVEL_UNITS_VAL_MEAS_PERCENTAGE\x10\x01\x12\x34\n0NISCOPE_INT32_NOTIFICATION_TYPE_VAL_NOTIFY_NEVER\x10\x00\x12\x33\n/NISCOPE_INT32_NOTIFICATION_TYPE_VAL_NOTIFY_DONE\x10\x01\x12\x44\n@NISCOPE_INT32_OVERFLOW_ERROR_REPORTING_VAL_ERROR_REPORTING_ERROR\x10\x00\x12\x46\nBNISCOPE_INT32_OVERFLOW_ERROR_REPORTING_VAL_ERROR_REPORTING_WARNING\x10\x01\x12G\nCNISCOPE_INT32_OVERFLOW_ERROR_REPORTING_VAL_ERROR_REPORTING_DISABLED\x10\x02\x12N\nJNISCOPE_INT32_P2_P_STREAM_RELATIVE_TO_VAL_STREAM_RELATIVE_TO_START_TRIGGER\x10\x00\x12R\nNNISCOPE_INT32_P2_P_STREAM_RELATIVE_TO_VAL_STREAM_RELATIVE_TO_REFERENCE_TRIGGER\x10\x01\x12M\nINISCOPE_INT32_P2_P_STREAM_RELATIVE_TO_VAL_STREAM_RELATIVE_TO_SYNC_TRIGGER\x10\x02\x12\x37\n3NISCOPE_INT32_RIS_METHOD_VAL_RIS_EXACT_NUM_AVERAGES\x10\x01\x12\x35\n1NISCOPE_INT32_RIS_METHOD_VAL_RIS_MIN_NUM_AVERAGES\x10\x02\x12/\n+NISCOPE_INT32_RIS_METHOD_VAL_RIS_INCOMPLETE\x10\x03\x12\x36\n2NISCOPE_INT32_RIS_METHOD_VAL_RIS_LIMITED_BIN_WIDTH\x10\x05\x12L\nHNISCOPE_INT32_REF_TRIGGER_DETECTOR_LOCATION_VAL_ANALOG_DETECTION_CIRCUIT\x10\x00\x12>\n:NISCOPE_INT32_REF_TRIGGER_DETECTOR_LOCATION_VAL_DDC_OUTPUT\x10\x01\x12\x31\n-NISCOPE_INT32_RUNT_POLARITY_VAL_RUNT_POSITIVE\x10\x01\x12\x31\n-NISCOPE_INT32_RUNT_POLARITY_VAL_RUNT_NEGATIVE\x10\x02\x12/\n+NISCOPE_INT32_RUNT_POLARITY_VAL_RUNT_EITHER\x10\x03\x12\x42\n>NISCOPE_INT32_RUNT_TIME_CONDITION_VAL_RUNT_TIME_CONDITION_NONE\x10\x00\x12\x44\n@NISCOPE_INT32_RUNT_TIME_CONDITION_VAL_RUNT_TIME_CONDITION_WITHIN\x10\x01\x12\x45\nANISCOPE_INT32_RUNT_TIME_CONDITION_VAL_RUNT_TIME_CONDITION_OUTSIDE\x10\x02\x12+\n\'NISCOPE_INT32_SAMPLE_MODE_VAL_REAL_TIME\x10\x00\x12\x31\n-NISCOPE_INT32_SAMPLE_MODE_VAL_EQUIVALENT_TIME\x10\x01\x12\x39\n5NISCOPE_INT32_TERMINAL_CONFIGURATION_VAL_SINGLE_ENDED\x10\x00\x12\x44\n@NISCOPE_INT32_TERMINAL_CONFIGURATION_VAL_UNBALANCED_DIFFERENTIAL\x10\x01\x12\x39\n5NISCOPE_INT32_TERMINAL_CONFIGURATION_VAL_DIFFERENTIAL\x10\x02\x12)\n%NISCOPE_INT32_TRIGGER_COUPLING_VAL_AC\x10\x00\x12)\n%NISCOPE_INT32_TRIGGER_COUPLING_VAL_DC\x10\x01\x12\x30\n,NISCOPE_INT32_TRIGGER_COUPLING_VAL_HF_REJECT\x10\x03\x12\x30\n,NISCOPE_INT32_TRIGGER_COUPLING_VAL_LF_REJECT\x10\x04\x12\x39\n4NISCOPE_INT32_TRIGGER_COUPLING_VAL_AC_PLUS_HF_REJECT\x10\xe9\x07\x12\x35\n1NISCOPE_INT32_TRIGGER_MODIFIER_VAL_NO_TRIGGER_MOD\x10\x01\x12+\n\'NISCOPE_INT32_TRIGGER_MODIFIER_VAL_AUTO\x10\x02\x12\x31\n-NISCOPE_INT32_TRIGGER_MODIFIER_VAL_AUTO_LEVEL\x10\x03\x12,\n(NISCOPE_INT32_TRIGGER_SLOPE_VAL_NEGATIVE\x10\x00\x12,\n(NISCOPE_INT32_TRIGGER_SLOPE_VAL_POSITIVE\x10\x01\x12\x30\n,NISCOPE_INT32_TRIGGER_SLOPE_VAL_SLOPE_EITHER\x10\x03\x12/\n+NISCOPE_INT32_TRIGGER_TYPE_VAL_EDGE_TRIGGER\x10\x01\x12\x36\n1NISCOPE_INT32_TRIGGER_TYPE_VAL_HYSTERESIS_TRIGGER\x10\xe9\x07\x12\x33\n.NISCOPE_INT32_TRIGGER_TYPE_VAL_DIGITAL_TRIGGER\x10\xea\x07\x12\x32\n-NISCOPE_INT32_TRIGGER_TYPE_VAL_WINDOW_TRIGGER\x10\xeb\x07\x12\x34\n/NISCOPE_INT32_TRIGGER_TYPE_VAL_SOFTWARE_TRIGGER\x10\xec\x07\x12-\n)NISCOPE_INT32_TRIGGER_TYPE_VAL_TV_TRIGGER\x10\x05\x12\x31\n-NISCOPE_INT32_TRIGGER_TYPE_VAL_GLITCH_TRIGGER\x10\x04\x12\x30\n,NISCOPE_INT32_TRIGGER_TYPE_VAL_WIDTH_TRIGGER\x10\x02\x12/\n+NISCOPE_INT32_TRIGGER_TYPE_VAL_RUNT_TRIGGER\x10\x03\x12\x34\n0NISCOPE_INT32_TRIGGER_TYPE_VAL_IMMEDIATE_TRIGGER\x10\x06\x12\x39\n5NISCOPE_INT32_TRIGGER_WINDOW_MODE_VAL_ENTERING_WINDOW\x10\x00\x12\x38\n4NISCOPE_INT32_TRIGGER_WINDOW_MODE_VAL_LEAVING_WINDOW\x10\x01\x12\x44\n@NISCOPE_INT32_TRIGGER_WINDOW_MODE_VAL_ENTERING_OR_LEAVING_WINDOW\x10\x02\x12*\n&NISCOPE_INT32_VERTICAL_COUPLING_VAL_AC\x10\x00\x12*\n&NISCOPE_INT32_VERTICAL_COUPLING_VAL_DC\x10\x01\x12+\n\'NISCOPE_INT32_VERTICAL_COUPLING_VAL_GND\x10\x02\x12\x30\n,NISCOPE_INT32_VIDEO_POLARITY_VAL_TV_POSITIVE\x10\x01\x12\x30\n,NISCOPE_INT32_VIDEO_POLARITY_VAL_TV_NEGATIVE\x10\x02\x12.\n*NISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_NTSC\x10\x01\x12-\n)NISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_PAL\x10\x02\x12/\n+NISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_SECAM\x10\x03\x12\x30\n+NISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_M_PAL\x10\xe9\x07\x12M\nHNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_480I_59_94_FIELDS_PER_SECOND\x10\xf2\x07\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_480I_60_FIELDS_PER_SECOND\x10\xf3\x07\x12M\nHNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_480P_59_94_FRAMES_PER_SECOND\x10\xf7\x07\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_480P_60_FRAMES_PER_SECOND\x10\xf8\x07\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_576I_50_FIELDS_PER_SECOND\x10\xfc\x07\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_576P_50_FRAMES_PER_SECOND\x10\x81\x08\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_720P_50_FRAMES_PER_SECOND\x10\x87\x08\x12M\nHNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_720P_59_94_FRAMES_PER_SECOND\x10\x88\x08\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_720P_60_FRAMES_PER_SECOND\x10\x89\x08\x12K\nFNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_1080I_50_FIELDS_PER_SECOND\x10\x90\x08\x12N\nINISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_1080I_59_94_FIELDS_PER_SECOND\x10\x91\x08\x12K\nFNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_1080I_60_FIELDS_PER_SECOND\x10\x92\x08\x12K\nFNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_1080P_24_FRAMES_PER_SECOND\x10\x95\x08\x12\x39\n5NISCOPE_INT32_VIDEO_TRIGGER_EVENT_VAL_TV_EVENT_FIELD1\x10\x01\x12\x39\n5NISCOPE_INT32_VIDEO_TRIGGER_EVENT_VAL_TV_EVENT_FIELD2\x10\x02\x12<\n8NISCOPE_INT32_VIDEO_TRIGGER_EVENT_VAL_TV_EVENT_ANY_FIELD\x10\x03\x12;\n7NISCOPE_INT32_VIDEO_TRIGGER_EVENT_VAL_TV_EVENT_ANY_LINE\x10\x04\x12>\n:NISCOPE_INT32_VIDEO_TRIGGER_EVENT_VAL_TV_EVENT_LINE_NUMBER\x10\x05\x12\x32\n.NISCOPE_INT32_WIDTH_CONDITION_VAL_WIDTH_WITHIN\x10\x01\x12\x33\n/NISCOPE_INT32_WIDTH_CONDITION_VAL_WIDTH_OUTSIDE\x10\x02\x12\x33\n/NISCOPE_INT32_WIDTH_POLARITY_VAL_WIDTH_POSITIVE\x10\x01\x12\x33\n/NISCOPE_INT32_WIDTH_POLARITY_VAL_WIDTH_NEGATIVE\x10\x02\x12\x31\n-NISCOPE_INT32_WIDTH_POLARITY_VAL_WIDTH_EITHER\x10\x03\x1a\x02\x10\x01*\xc9\x01\n\x1cNiScopeReal64AttributeValues\x12\x1e\n\x1aNISCOPE_REAL64_UNSPECIFIED\x10\x00\x12\x41\n=NISCOPE_REAL64_CABLE_SENSE_MODE_VAL_CABLE_SENSE_MODE_DISABLED\x10\x00\x12\x42\n>NISCOPE_REAL64_CABLE_SENSE_MODE_VAL_CABLE_SENSE_MODE_ON_DEMAND\x10\x01\x1a\x02\x10\x01*\xe3\x04\n\"NiScopeReal64AttributeValuesMapped\x12%\n!NISCOPE_REAL64_MAPPED_UNSPECIFIED\x10\x00\x12.\n*NISCOPE_REAL64_INPUT_IMPEDANCE_VAL_50_OHMS\x10\x01\x12.\n*NISCOPE_REAL64_INPUT_IMPEDANCE_VAL_75_OHMS\x10\x02\x12\x30\n,NISCOPE_REAL64_INPUT_IMPEDANCE_VAL_1_MEG_OHM\x10\x03\x12\x43\n?NISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_BANDWIDTH_DEVICE_DEFAULT\x10\x04\x12\x39\n5NISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_BANDWIDTH_FULL\x10\x05\x12:\n6NISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_20MHZ_BANDWIDTH\x10\x06\x12;\n7NISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_100MHZ_BANDWIDTH\x10\x07\x12\x44\n@NISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_20MHZ_MAX_INPUT_FREQUENCY\x10\x08\x12\x45\nANISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_100MHZ_MAX_INPUT_FREQUENCY\x10\t*\x9e\x11\n\"NiScopeStringAttributeValuesMapped\x12%\n!NISCOPE_STRING_MAPPED_UNSPECIFIED\x10\x00\x12\x33\n/NISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_CLK_IN\x10\x01\x12\x36\n2NISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_NO_SOURCE\x10\x02\x12\x35\n1NISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_PXI_STAR\x10\x03\x12\x39\n5NISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_PXIE_DSTAR_A\x10\x04\x12\x39\n5NISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_AUX_0_CLK_IN\x10\x05\x12J\nFNISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_ONBOARD_CONFIGURABLE_RATE_CLK\x10\x06\x12/\n+NISCOPE_STRING_TRIGGER_SOURCE_VAL_IMMEDIATE\x10\x07\x12.\n*NISCOPE_STRING_TRIGGER_SOURCE_VAL_EXTERNAL\x10\x08\x12\x32\n.NISCOPE_STRING_TRIGGER_SOURCE_VAL_SW_TRIG_FUNC\x10\t\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL0\x10\n\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL1\x10\x0b\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL2\x10\x0c\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL3\x10\r\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL4\x10\x0e\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL5\x10\x0f\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL6\x10\x10\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL7\x10\x11\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_ECL0\x10\x12\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_ECL1\x10\x13\x12.\n*NISCOPE_STRING_TRIGGER_SOURCE_VAL_PXI_STAR\x10\x14\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_0\x10\x15\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_1\x10\x16\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_2\x10\x17\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_3\x10\x18\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_4\x10\x19\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_5\x10\x1a\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_6\x10\x1b\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_7\x10\x1c\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_0\x10\x1d\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_1\x10\x1e\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_2\x10\x1f\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_3\x10 \x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_4\x10!\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_5\x10\"\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_6\x10#\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_7\x10$\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_0\x10%\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_1\x10&\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_3\x10\'\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_4\x10(\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_5\x10)\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_6\x10*\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_7\x10+\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_2\x10,*q\n\x06Option\x12\x32\n.OPTION_NISCOPE_VAL_SELF_CALIBRATE_ALL_CHANNELS\x10\x00\x12\x33\n/OPTION_NISCOPE_VAL_RESTORE_EXTERNAL_CALIBRATION\x10\x01*\xb2\x01\n\x0cRuntPolarity\x12\x1d\n\x19RUNT_POLARITY_UNSPECIFIED\x10\x00\x12+\n\'RUNT_POLARITY_NISCOPE_VAL_RUNT_POSITIVE\x10\x01\x12+\n\'RUNT_POLARITY_NISCOPE_VAL_RUNT_NEGATIVE\x10\x02\x12)\n%RUNT_POLARITY_NISCOPE_VAL_RUNT_EITHER\x10\x03*\xcf\x0f\n\x11ScalarMeasurement\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_RISE_TIME\x10\x00\x12\x32\n-SCALAR_MEASUREMENT_NISCOPE_VAL_NO_MEASUREMENT\x10\xa0\x1f\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_FALL_TIME\x10\x01\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_FREQUENCY\x10\x02\x12)\n%SCALAR_MEASUREMENT_NISCOPE_VAL_PERIOD\x10\x03\x12.\n*SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_RMS\x10\x04\x12\x37\n3SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_PEAK_TO_PEAK\x10\x05\x12.\n*SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_MAX\x10\x06\x12.\n*SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_MIN\x10\x07\x12/\n+SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HIGH\x10\x08\x12.\n*SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_LOW\x10\t\x12\x32\n.SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_AVERAGE\x10\n\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_WIDTH_NEG\x10\x0b\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_WIDTH_POS\x10\x0c\x12\x31\n-SCALAR_MEASUREMENT_NISCOPE_VAL_DUTY_CYCLE_NEG\x10\r\x12\x31\n-SCALAR_MEASUREMENT_NISCOPE_VAL_DUTY_CYCLE_POS\x10\x0e\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_AMPLITUDE\x10\x0f\x12\x34\n0SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_CYCLE_RMS\x10\x10\x12\x38\n4SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_CYCLE_AVERAGE\x10\x11\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_OVERSHOOT\x10\x12\x12+\n\'SCALAR_MEASUREMENT_NISCOPE_VAL_PRESHOOT\x10\x13\x12\x31\n,SCALAR_MEASUREMENT_NISCOPE_VAL_LOW_REF_VOLTS\x10\xe8\x07\x12\x31\n,SCALAR_MEASUREMENT_NISCOPE_VAL_MID_REF_VOLTS\x10\xe9\x07\x12\x32\n-SCALAR_MEASUREMENT_NISCOPE_VAL_HIGH_REF_VOLTS\x10\xea\x07\x12(\n#SCALAR_MEASUREMENT_NISCOPE_VAL_AREA\x10\xeb\x07\x12.\n)SCALAR_MEASUREMENT_NISCOPE_VAL_CYCLE_AREA\x10\xec\x07\x12,\n\'SCALAR_MEASUREMENT_NISCOPE_VAL_INTEGRAL\x10\xed\x07\x12\x30\n+SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_BASE\x10\xee\x07\x12/\n*SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_TOP\x10\xef\x07\x12\x31\n,SCALAR_MEASUREMENT_NISCOPE_VAL_FFT_FREQUENCY\x10\xf0\x07\x12\x31\n,SCALAR_MEASUREMENT_NISCOPE_VAL_FFT_AMPLITUDE\x10\xf1\x07\x12\x32\n-SCALAR_MEASUREMENT_NISCOPE_VAL_RISE_SLEW_RATE\x10\xf2\x07\x12\x32\n-SCALAR_MEASUREMENT_NISCOPE_VAL_FALL_SLEW_RATE\x10\xf3\x07\x12/\n*SCALAR_MEASUREMENT_NISCOPE_VAL_AC_ESTIMATE\x10\xf4\x07\x12/\n*SCALAR_MEASUREMENT_NISCOPE_VAL_DC_ESTIMATE\x10\xf5\x07\x12.\n)SCALAR_MEASUREMENT_NISCOPE_VAL_TIME_DELAY\x10\xf6\x07\x12\x32\n-SCALAR_MEASUREMENT_NISCOPE_VAL_AVERAGE_PERIOD\x10\xf7\x07\x12\x35\n0SCALAR_MEASUREMENT_NISCOPE_VAL_AVERAGE_FREQUENCY\x10\xf8\x07\x12\x37\n2SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_BASE_TO_TOP\x10\xf9\x07\x12/\n*SCALAR_MEASUREMENT_NISCOPE_VAL_PHASE_DELAY\x10\xfa\x07*\xe8\x01\n\x0fTriggerCoupling\x12#\n\x1fTRIGGER_COUPLING_NISCOPE_VAL_AC\x10\x00\x12#\n\x1fTRIGGER_COUPLING_NISCOPE_VAL_DC\x10\x01\x12*\n&TRIGGER_COUPLING_NISCOPE_VAL_HF_REJECT\x10\x03\x12*\n&TRIGGER_COUPLING_NISCOPE_VAL_LF_REJECT\x10\x04\x12\x33\n.TRIGGER_COUPLING_NISCOPE_VAL_AC_PLUS_HF_REJECT\x10\xe9\x07*\x8a\x01\n\x0cTriggerSlope\x12&\n\"TRIGGER_SLOPE_NISCOPE_VAL_NEGATIVE\x10\x00\x12&\n\"TRIGGER_SLOPE_NISCOPE_VAL_POSITIVE\x10\x01\x12*\n&TRIGGER_SLOPE_NISCOPE_VAL_SLOPE_EITHER\x10\x03*\xbc\x01\n\x11TriggerWindowMode\x12\x33\n/TRIGGER_WINDOW_MODE_NISCOPE_VAL_ENTERING_WINDOW\x10\x00\x12\x32\n.TRIGGER_WINDOW_MODE_NISCOPE_VAL_LEAVING_WINDOW\x10\x01\x12>\n:TRIGGER_WINDOW_MODE_NISCOPE_VAL_ENTERING_OR_LEAVING_WINDOW\x10\x02*\x85\x01\n\x10VerticalCoupling\x12$\n VERTICAL_COUPLING_NISCOPE_VAL_AC\x10\x00\x12$\n VERTICAL_COUPLING_NISCOPE_VAL_DC\x10\x01\x12%\n!VERTICAL_COUPLING_NISCOPE_VAL_GND\x10\x02*\x87\x01\n\rVideoPolarity\x12\x1e\n\x1aVIDEO_POLARITY_UNSPECIFIED\x10\x00\x12*\n&VIDEO_POLARITY_NISCOPE_VAL_TV_POSITIVE\x10\x01\x12*\n&VIDEO_POLARITY_NISCOPE_VAL_TV_NEGATIVE\x10\x02*\x80\t\n\x11VideoSignalFormat\x12#\n\x1fVIDEO_SIGNAL_FORMAT_UNSPECIFIED\x10\x00\x12(\n$VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_NTSC\x10\x01\x12\'\n#VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_PAL\x10\x02\x12)\n%VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_SECAM\x10\x03\x12*\n%VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_M_PAL\x10\xe9\x07\x12G\nBVIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_480I_59_94_FIELDS_PER_SECOND\x10\xf2\x07\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_480I_60_FIELDS_PER_SECOND\x10\xf3\x07\x12G\nBVIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_480P_59_94_FRAMES_PER_SECOND\x10\xf7\x07\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_480P_60_FRAMES_PER_SECOND\x10\xf8\x07\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_576I_50_FIELDS_PER_SECOND\x10\xfc\x07\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_576P_50_FRAMES_PER_SECOND\x10\x81\x08\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_720P_50_FRAMES_PER_SECOND\x10\x87\x08\x12G\nBVIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_720P_59_94_FRAMES_PER_SECOND\x10\x88\x08\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_720P_60_FRAMES_PER_SECOND\x10\x89\x08\x12\x45\n@VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_1080I_50_FIELDS_PER_SECOND\x10\x90\x08\x12H\nCVIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_1080I_59_94_FIELDS_PER_SECOND\x10\x91\x08\x12\x45\n@VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_1080I_60_FIELDS_PER_SECOND\x10\x92\x08\x12\x45\n@VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_1080P_24_FRAMES_PER_SECOND\x10\x95\x08*\xcb\x02\n\x11VideoTriggerEvent\x12#\n\x1fVIDEO_TRIGGER_EVENT_UNSPECIFIED\x10\x00\x12\x33\n/VIDEO_TRIGGER_EVENT_NISCOPE_VAL_TV_EVENT_FIELD1\x10\x01\x12\x33\n/VIDEO_TRIGGER_EVENT_NISCOPE_VAL_TV_EVENT_FIELD2\x10\x02\x12\x36\n2VIDEO_TRIGGER_EVENT_NISCOPE_VAL_TV_EVENT_ANY_FIELD\x10\x03\x12\x35\n1VIDEO_TRIGGER_EVENT_NISCOPE_VAL_TV_EVENT_ANY_LINE\x10\x04\x12\x38\n4VIDEO_TRIGGER_EVENT_NISCOPE_VAL_TV_EVENT_LINE_NUMBER\x10\x05*\xf4\x01\n\x0cWhichTrigger\x12\x34\n0WHICH_TRIGGER_NISCOPE_VAL_SOFTWARE_TRIGGER_START\x10\x00\x12<\n8WHICH_TRIGGER_NISCOPE_VAL_SOFTWARE_TRIGGER_ARM_REFERENCE\x10\x01\x12\x38\n4WHICH_TRIGGER_NISCOPE_VAL_SOFTWARE_TRIGGER_REFERENCE\x10\x02\x12\x36\n2WHICH_TRIGGER_NISCOPE_VAL_SOFTWARE_TRIGGER_ADVANCE\x10\x03*\x8e\x01\n\x0eWidthCondition\x12\x1f\n\x1bWIDTH_CONDITION_UNSPECIFIED\x10\x00\x12,\n(WIDTH_CONDITION_NISCOPE_VAL_WIDTH_WITHIN\x10\x01\x12-\n)WIDTH_CONDITION_NISCOPE_VAL_WIDTH_OUTSIDE\x10\x02*\xba\x01\n\rWidthPolarity\x12\x1e\n\x1aWIDTH_POLARITY_UNSPECIFIED\x10\x00\x12-\n)WIDTH_POLARITY_NISCOPE_VAL_WIDTH_POSITIVE\x10\x01\x12-\n)WIDTH_POLARITY_NISCOPE_VAL_WIDTH_NEGATIVE\x10\x02\x12+\n\'WIDTH_POLARITY_NISCOPE_VAL_WIDTH_EITHER\x10\x03\x32\xe0K\n\x07NiScope\x12@\n\x05\x41\x62ort\x12\x1a.niscope_grpc.AbortRequest\x1a\x1b.niscope_grpc.AbortResponse\x12\x64\n\x11\x41\x63quisitionStatus\x12&.niscope_grpc.AcquisitionStatusRequest\x1a\'.niscope_grpc.AcquisitionStatusResponse\x12\x64\n\x11\x41\x63tualMeasWfmSize\x12&.niscope_grpc.ActualMeasWfmSizeRequest\x1a\'.niscope_grpc.ActualMeasWfmSizeResponse\x12X\n\rActualNumWfms\x12\".niscope_grpc.ActualNumWfmsRequest\x1a#.niscope_grpc.ActualNumWfmsResponse\x12g\n\x12\x41\x63tualRecordLength\x12\'.niscope_grpc.ActualRecordLengthRequest\x1a(.niscope_grpc.ActualRecordLengthResponse\x12p\n\x15\x41\x64\x64WaveformProcessing\x12*.niscope_grpc.AddWaveformProcessingRequest\x1a+.niscope_grpc.AddWaveformProcessingResponse\x12\x8b\x01\n\x1e\x41\x64justSampleClockRelativeDelay\x12\x33.niscope_grpc.AdjustSampleClockRelativeDelayRequest\x1a\x34.niscope_grpc.AdjustSampleClockRelativeDelayResponse\x12L\n\tAutoSetup\x12\x1e.niscope_grpc.AutoSetupRequest\x1a\x1f.niscope_grpc.AutoSetupResponse\x12p\n\x15\x43\x61\x62leSenseSignalStart\x12*.niscope_grpc.CableSenseSignalStartRequest\x1a+.niscope_grpc.CableSenseSignalStartResponse\x12m\n\x14\x43\x61\x62leSenseSignalStop\x12).niscope_grpc.CableSenseSignalStopRequest\x1a*.niscope_grpc.CableSenseSignalStopResponse\x12U\n\x0c\x43\x61lFetchDate\x12!.niscope_grpc.CalFetchDateRequest\x1a\".niscope_grpc.CalFetchDateResponse\x12j\n\x13\x43\x61lFetchTemperature\x12(.niscope_grpc.CalFetchTemperatureRequest\x1a).niscope_grpc.CalFetchTemperatureResponse\x12\x61\n\x10\x43\x61lSelfCalibrate\x12%.niscope_grpc.CalSelfCalibrateRequest\x1a&.niscope_grpc.CalSelfCalibrateResponse\x12v\n\x17\x43heckAttributeViBoolean\x12,.niscope_grpc.CheckAttributeViBooleanRequest\x1a-.niscope_grpc.CheckAttributeViBooleanResponse\x12p\n\x15\x43heckAttributeViInt32\x12*.niscope_grpc.CheckAttributeViInt32Request\x1a+.niscope_grpc.CheckAttributeViInt32Response\x12p\n\x15\x43heckAttributeViInt64\x12*.niscope_grpc.CheckAttributeViInt64Request\x1a+.niscope_grpc.CheckAttributeViInt64Response\x12s\n\x16\x43heckAttributeViReal64\x12+.niscope_grpc.CheckAttributeViReal64Request\x1a,.niscope_grpc.CheckAttributeViReal64Response\x12v\n\x17\x43heckAttributeViSession\x12,.niscope_grpc.CheckAttributeViSessionRequest\x1a-.niscope_grpc.CheckAttributeViSessionResponse\x12s\n\x16\x43heckAttributeViString\x12+.niscope_grpc.CheckAttributeViStringRequest\x1a,.niscope_grpc.CheckAttributeViStringResponse\x12\x88\x01\n\x1d\x43learWaveformMeasurementStats\x12\x32.niscope_grpc.ClearWaveformMeasurementStatsRequest\x1a\x33.niscope_grpc.ClearWaveformMeasurementStatsResponse\x12v\n\x17\x43learWaveformProcessing\x12,.niscope_grpc.ClearWaveformProcessingRequest\x1a-.niscope_grpc.ClearWaveformProcessingResponse\x12@\n\x05\x43lose\x12\x1a.niscope_grpc.CloseRequest\x1a\x1b.niscope_grpc.CloseResponse\x12\x43\n\x06\x43ommit\x12\x1b.niscope_grpc.CommitRequest\x1a\x1c.niscope_grpc.CommitResponse\x12m\n\x14\x43onfigureAcquisition\x12).niscope_grpc.ConfigureAcquisitionRequest\x1a*.niscope_grpc.ConfigureAcquisitionResponse\x12\x85\x01\n\x1c\x43onfigureChanCharacteristics\x12\x31.niscope_grpc.ConfigureChanCharacteristicsRequest\x1a\x32.niscope_grpc.ConfigureChanCharacteristicsResponse\x12[\n\x0e\x43onfigureClock\x12#.niscope_grpc.ConfigureClockRequest\x1a$.niscope_grpc.ConfigureClockResponse\x12\xa6\x01\n\'ConfigureEqualizationFilterCoefficients\x12<.niscope_grpc.ConfigureEqualizationFilterCoefficientsRequest\x1a=.niscope_grpc.ConfigureEqualizationFilterCoefficientsResponse\x12|\n\x19\x43onfigureHorizontalTiming\x12..niscope_grpc.ConfigureHorizontalTimingRequest\x1a/.niscope_grpc.ConfigureHorizontalTimingResponse\x12v\n\x17\x43onfigureTriggerDigital\x12,.niscope_grpc.ConfigureTriggerDigitalRequest\x1a-.niscope_grpc.ConfigureTriggerDigitalResponse\x12m\n\x14\x43onfigureTriggerEdge\x12).niscope_grpc.ConfigureTriggerEdgeRequest\x1a*.niscope_grpc.ConfigureTriggerEdgeResponse\x12s\n\x16\x43onfigureTriggerGlitch\x12+.niscope_grpc.ConfigureTriggerGlitchRequest\x1a,.niscope_grpc.ConfigureTriggerGlitchResponse\x12\x7f\n\x1a\x43onfigureTriggerHysteresis\x12/.niscope_grpc.ConfigureTriggerHysteresisRequest\x1a\x30.niscope_grpc.ConfigureTriggerHysteresisResponse\x12|\n\x19\x43onfigureTriggerImmediate\x12..niscope_grpc.ConfigureTriggerImmediateRequest\x1a/.niscope_grpc.ConfigureTriggerImmediateResponse\x12m\n\x14\x43onfigureTriggerRunt\x12).niscope_grpc.ConfigureTriggerRuntRequest\x1a*.niscope_grpc.ConfigureTriggerRuntResponse\x12y\n\x18\x43onfigureTriggerSoftware\x12-.niscope_grpc.ConfigureTriggerSoftwareRequest\x1a..niscope_grpc.ConfigureTriggerSoftwareResponse\x12p\n\x15\x43onfigureTriggerVideo\x12*.niscope_grpc.ConfigureTriggerVideoRequest\x1a+.niscope_grpc.ConfigureTriggerVideoResponse\x12p\n\x15\x43onfigureTriggerWidth\x12*.niscope_grpc.ConfigureTriggerWidthRequest\x1a+.niscope_grpc.ConfigureTriggerWidthResponse\x12s\n\x16\x43onfigureTriggerWindow\x12+.niscope_grpc.ConfigureTriggerWindowRequest\x1a,.niscope_grpc.ConfigureTriggerWindowResponse\x12\x64\n\x11\x43onfigureVertical\x12&.niscope_grpc.ConfigureVerticalRequest\x1a\'.niscope_grpc.ConfigureVerticalResponse\x12\x46\n\x07\x44isable\x12\x1c.niscope_grpc.DisableRequest\x1a\x1d.niscope_grpc.DisableResponse\x12U\n\x0c\x45rrorHandler\x12!.niscope_grpc.ErrorHandlerRequest\x1a\".niscope_grpc.ErrorHandlerResponse\x12\x97\x01\n\"ExportAttributeConfigurationBuffer\x12\x37.niscope_grpc.ExportAttributeConfigurationBufferRequest\x1a\x38.niscope_grpc.ExportAttributeConfigurationBufferResponse\x12\x91\x01\n ExportAttributeConfigurationFile\x12\x35.niscope_grpc.ExportAttributeConfigurationFileRequest\x1a\x36.niscope_grpc.ExportAttributeConfigurationFileResponse\x12U\n\x0c\x45xportSignal\x12!.niscope_grpc.ExportSignalRequest\x1a\".niscope_grpc.ExportSignalResponse\x12@\n\x05\x46\x65tch\x12\x1a.niscope_grpc.FetchRequest\x1a\x1b.niscope_grpc.FetchResponse\x12p\n\x15\x46\x65tchArrayMeasurement\x12*.niscope_grpc.FetchArrayMeasurementRequest\x1a+.niscope_grpc.FetchArrayMeasurementResponse\x12X\n\rFetchBinary16\x12\".niscope_grpc.FetchBinary16Request\x1a#.niscope_grpc.FetchBinary16Response\x12X\n\rFetchBinary32\x12\".niscope_grpc.FetchBinary32Request\x1a#.niscope_grpc.FetchBinary32Response\x12U\n\x0c\x46\x65tchBinary8\x12!.niscope_grpc.FetchBinary8Request\x1a\".niscope_grpc.FetchBinary8Response\x12U\n\x0c\x46\x65tchComplex\x12!.niscope_grpc.FetchComplexRequest\x1a\".niscope_grpc.FetchComplexResponse\x12m\n\x14\x46\x65tchComplexBinary16\x12).niscope_grpc.FetchComplexBinary16Request\x1a*.niscope_grpc.FetchComplexBinary16Response\x12\x61\n\x10\x46\x65tchMeasurement\x12%.niscope_grpc.FetchMeasurementRequest\x1a&.niscope_grpc.FetchMeasurementResponse\x12p\n\x15\x46\x65tchMeasurementStats\x12*.niscope_grpc.FetchMeasurementStatsRequest\x1a+.niscope_grpc.FetchMeasurementStatsResponse\x12p\n\x15GetAttributeViBoolean\x12*.niscope_grpc.GetAttributeViBooleanRequest\x1a+.niscope_grpc.GetAttributeViBooleanResponse\x12j\n\x13GetAttributeViInt32\x12(.niscope_grpc.GetAttributeViInt32Request\x1a).niscope_grpc.GetAttributeViInt32Response\x12j\n\x13GetAttributeViInt64\x12(.niscope_grpc.GetAttributeViInt64Request\x1a).niscope_grpc.GetAttributeViInt64Response\x12m\n\x14GetAttributeViReal64\x12).niscope_grpc.GetAttributeViReal64Request\x1a*.niscope_grpc.GetAttributeViReal64Response\x12p\n\x15GetAttributeViSession\x12*.niscope_grpc.GetAttributeViSessionRequest\x1a+.niscope_grpc.GetAttributeViSessionResponse\x12m\n\x14GetAttributeViString\x12).niscope_grpc.GetAttributeViStringRequest\x1a*.niscope_grpc.GetAttributeViStringResponse\x12[\n\x0eGetChannelName\x12#.niscope_grpc.GetChannelNameRequest\x1a$.niscope_grpc.GetChannelNameResponse\x12y\n\x18GetChannelNameFromString\x12-.niscope_grpc.GetChannelNameFromStringRequest\x1a..niscope_grpc.GetChannelNameFromStringResponse\x12\x94\x01\n!GetEqualizationFilterCoefficients\x12\x36.niscope_grpc.GetEqualizationFilterCoefficientsRequest\x1a\x37.niscope_grpc.GetEqualizationFilterCoefficientsResponse\x12I\n\x08GetError\x12\x1d.niscope_grpc.GetErrorRequest\x1a\x1e.niscope_grpc.GetErrorResponse\x12^\n\x0fGetErrorMessage\x12$.niscope_grpc.GetErrorMessageRequest\x1a%.niscope_grpc.GetErrorMessageResponse\x12m\n\x14GetFrequencyResponse\x12).niscope_grpc.GetFrequencyResponseRequest\x1a*.niscope_grpc.GetFrequencyResponseResponse\x12\x85\x01\n\x1cGetNormalizationCoefficients\x12\x31.niscope_grpc.GetNormalizationCoefficientsRequest\x1a\x32.niscope_grpc.GetNormalizationCoefficientsResponse\x12s\n\x16GetScalingCoefficients\x12+.niscope_grpc.GetScalingCoefficientsRequest\x1a,.niscope_grpc.GetScalingCoefficientsResponse\x12v\n\x17GetStreamEndpointHandle\x12,.niscope_grpc.GetStreamEndpointHandleRequest\x1a-.niscope_grpc.GetStreamEndpointHandleResponse\x12\x97\x01\n\"ImportAttributeConfigurationBuffer\x12\x37.niscope_grpc.ImportAttributeConfigurationBufferRequest\x1a\x38.niscope_grpc.ImportAttributeConfigurationBufferResponse\x12\x91\x01\n ImportAttributeConfigurationFile\x12\x35.niscope_grpc.ImportAttributeConfigurationFileRequest\x1a\x36.niscope_grpc.ImportAttributeConfigurationFileResponse\x12=\n\x04Init\x12\x19.niscope_grpc.InitRequest\x1a\x1a.niscope_grpc.InitResponse\x12^\n\x0fInitWithOptions\x12$.niscope_grpc.InitWithOptionsRequest\x1a%.niscope_grpc.InitWithOptionsResponse\x12j\n\x13InitiateAcquisition\x12(.niscope_grpc.InitiateAcquisitionRequest\x1a).niscope_grpc.InitiateAcquisitionResponse\x12\x85\x01\n\x1cProbeCompensationSignalStart\x12\x31.niscope_grpc.ProbeCompensationSignalStartRequest\x1a\x32.niscope_grpc.ProbeCompensationSignalStartResponse\x12\x82\x01\n\x1bProbeCompensationSignalStop\x12\x30.niscope_grpc.ProbeCompensationSignalStopRequest\x1a\x31.niscope_grpc.ProbeCompensationSignalStopResponse\x12=\n\x04Read\x12\x19.niscope_grpc.ReadRequest\x1a\x1a.niscope_grpc.ReadResponse\x12^\n\x0fReadMeasurement\x12$.niscope_grpc.ReadMeasurementRequest\x1a%.niscope_grpc.ReadMeasurementResponse\x12@\n\x05Reset\x12\x1a.niscope_grpc.ResetRequest\x1a\x1b.niscope_grpc.ResetResponse\x12R\n\x0bResetDevice\x12 .niscope_grpc.ResetDeviceRequest\x1a!.niscope_grpc.ResetDeviceResponse\x12X\n\rRevisionQuery\x12\".niscope_grpc.RevisionQueryRequest\x1a#.niscope_grpc.RevisionQueryResponse\x12O\n\nSampleMode\x12\x1f.niscope_grpc.SampleModeRequest\x1a .niscope_grpc.SampleModeResponse\x12O\n\nSampleRate\x12\x1f.niscope_grpc.SampleRateRequest\x1a .niscope_grpc.SampleRateResponse\x12I\n\x08SelfTest\x12\x1d.niscope_grpc.SelfTestRequest\x1a\x1e.niscope_grpc.SelfTestResponse\x12v\n\x17SendSoftwareTriggerEdge\x12,.niscope_grpc.SendSoftwareTriggerEdgeRequest\x1a-.niscope_grpc.SendSoftwareTriggerEdgeResponse\x12p\n\x15SetAttributeViBoolean\x12*.niscope_grpc.SetAttributeViBooleanRequest\x1a+.niscope_grpc.SetAttributeViBooleanResponse\x12j\n\x13SetAttributeViInt32\x12(.niscope_grpc.SetAttributeViInt32Request\x1a).niscope_grpc.SetAttributeViInt32Response\x12j\n\x13SetAttributeViInt64\x12(.niscope_grpc.SetAttributeViInt64Request\x1a).niscope_grpc.SetAttributeViInt64Response\x12m\n\x14SetAttributeViReal64\x12).niscope_grpc.SetAttributeViReal64Request\x1a*.niscope_grpc.SetAttributeViReal64Response\x12p\n\x15SetAttributeViSession\x12*.niscope_grpc.SetAttributeViSessionRequest\x1a+.niscope_grpc.SetAttributeViSessionResponse\x12m\n\x14SetAttributeViString\x12).niscope_grpc.SetAttributeViStringRequest\x1a*.niscope_grpc.SetAttributeViStringResponseB?\n\x11\x63om.ni.grpc.scopeB\x07NiScopeP\x01\xaa\x02\x1eNationalInstruments.Grpc.Scopeb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rniscope.proto\x12\x0cniscope_grpc\x1a\x0enidevice.proto\x1a\rsession.proto\"\xb7\x01\n\x0cWaveformInfo\x12\x1a\n\x12\x61\x62solute_initial_x\x18\x01 \x01(\x01\x12\x1a\n\x12relative_initial_x\x18\x02 \x01(\x01\x12\x13\n\x0bx_increment\x18\x03 \x01(\x01\x12\x16\n\x0e\x61\x63tual_samples\x18\x04 \x01(\x11\x12\x0e\n\x06offset\x18\x05 \x01(\x01\x12\x0c\n\x04gain\x18\x06 \x01(\x01\x12\x11\n\treserved1\x18\x07 \x01(\x01\x12\x11\n\treserved2\x18\x08 \x01(\x01\"U\n\x0f\x43oefficientInfo\x12\x0e\n\x06offset\x18\x01 \x01(\x01\x12\x0c\n\x04gain\x18\x02 \x01(\x01\x12\x11\n\treserved1\x18\x03 \x01(\x01\x12\x11\n\treserved2\x18\x04 \x01(\x01\"\xb1\x01\n\x0bInitRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x10\n\x08id_query\x18\x03 \x01(\x08\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12M\n\x17initialization_behavior\x18\x05 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"~\n\x0cInitResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"\xd3\x01\n\x16InitWithOptionsRequest\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x10\n\x08id_query\x18\x03 \x01(\x08\x12\x14\n\x0creset_device\x18\x04 \x01(\x08\x12\x15\n\roption_string\x18\x05 \x01(\t\x12M\n\x17initialization_behavior\x18\x06 \x01(\x0e\x32,.nidevice_grpc.SessionInitializationBehavior\"\x89\x01\n\x17InitWithOptionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\"\n\x02vi\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x19\n\rerror_message\x18\x03 \x01(\tB\x02\x18\x01\x12\x1f\n\x17new_session_initialized\x18\x04 \x01(\x08\"2\n\x0c\x43loseRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rCloseResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"6\n\x10\x41utoSetupRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"#\n\x11\x41utoSetupResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xfc\x01\n\x18\x43onfigureVerticalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\r\n\x05range\x18\x03 \x01(\x01\x12\x0e\n\x06offset\x18\x04 \x01(\x01\x12\x32\n\x08\x63oupling\x18\x05 \x01(\x0e\x32\x1e.niscope_grpc.VerticalCouplingH\x00\x12\x16\n\x0c\x63oupling_raw\x18\x06 \x01(\x11H\x00\x12\x19\n\x11probe_attenuation\x18\x07 \x01(\x01\x12\x0f\n\x07\x65nabled\x18\x08 \x01(\x08\x42\x0f\n\rcoupling_enum\"+\n\x19\x43onfigureVerticalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x95\x01\n#ConfigureChanCharacteristicsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x17\n\x0finput_impedance\x18\x03 \x01(\x01\x12\x1b\n\x13max_input_frequency\x18\x04 \x01(\x01\"6\n$ConfigureChanCharacteristicsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb9\x01\n ConfigureHorizontalTimingRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x17\n\x0fmin_sample_rate\x18\x02 \x01(\x01\x12\x13\n\x0bmin_num_pts\x18\x03 \x01(\x11\x12\x14\n\x0cref_position\x18\x04 \x01(\x01\x12\x13\n\x0bnum_records\x18\x05 \x01(\x11\x12\x18\n\x10\x65nforce_realtime\x18\x06 \x01(\x08\"3\n!ConfigureHorizontalTimingResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xfd\x03\n\x15\x43onfigureClockRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12 \n\x16input_clock_source_raw\x18\x02 \x01(\tH\x00\x12I\n\x19input_clock_source_mapped\x18\x06 \x01(\x0e\x32$.niscope_grpc.ClockingTerminalValuesH\x00\x12!\n\x17output_clock_source_raw\x18\x03 \x01(\tH\x01\x12J\n\x1aoutput_clock_source_mapped\x18\x07 \x01(\x0e\x32$.niscope_grpc.ClockingTerminalValuesH\x01\x12%\n\x1b\x63lock_sync_pulse_source_raw\x18\x04 \x01(\tH\x02\x12N\n\x1e\x63lock_sync_pulse_source_mapped\x18\x08 \x01(\x0e\x32$.niscope_grpc.ClockingTerminalValuesH\x02\x12\x16\n\x0emaster_enabled\x18\x05 \x01(\x08\x42\x19\n\x17input_clock_source_enumB\x1a\n\x18output_clock_source_enumB\x1e\n\x1c\x63lock_sync_pulse_source_enum\"(\n\x16\x43onfigureClockResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xab\x02\n\x13\x45xportSignalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x31\n\x06signal\x18\x02 \x01(\x0e\x32\x1f.niscope_grpc.ExportableSignalsH\x00\x12\x14\n\nsignal_raw\x18\x03 \x01(\x11H\x00\x12\x19\n\x11signal_identifier\x18\x04 \x01(\t\x12\x46\n\x16output_terminal_mapped\x18\x05 \x01(\x0e\x32$.niscope_grpc.ClockingTerminalValuesH\x01\x12\x1d\n\x13output_terminal_raw\x18\x06 \x01(\tH\x01\x42\r\n\x0bsignal_enumB\x16\n\x14output_terminal_enum\"&\n\x14\x45xportSignalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"Z\n%AdjustSampleClockRelativeDelayRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\r\n\x05\x64\x65lay\x18\x02 \x01(\x01\"8\n&AdjustSampleClockRelativeDelayResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xcc\x02\n\x1b\x43onfigureTriggerEdgeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\x01\x12+\n\x05slope\x18\x04 \x01(\x0e\x32\x1a.niscope_grpc.TriggerSlopeH\x00\x12\x13\n\tslope_raw\x18\x05 \x01(\x11H\x00\x12\x39\n\x10trigger_coupling\x18\x06 \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x01\x12\x1e\n\x14trigger_coupling_raw\x18\x07 \x01(\x11H\x01\x12\x0f\n\x07holdoff\x18\x08 \x01(\x01\x12\r\n\x05\x64\x65lay\x18\t \x01(\x01\x42\x0c\n\nslope_enumB\x17\n\x15trigger_coupling_enum\".\n\x1c\x43onfigureTriggerEdgeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xdc\x03\n\x1d\x43onfigureTriggerGlitchRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\x01\x12\r\n\x05width\x18\x04 \x01(\x01\x12\x30\n\x08polarity\x18\x05 \x01(\x0e\x32\x1c.niscope_grpc.GlitchPolarityH\x00\x12\x16\n\x0cpolarity_raw\x18\x06 \x01(\x11H\x00\x12\x39\n\x10glitch_condition\x18\x07 \x01(\x0e\x32\x1d.niscope_grpc.GlitchConditionH\x01\x12\x1e\n\x14glitch_condition_raw\x18\x08 \x01(\x11H\x01\x12\x39\n\x10trigger_coupling\x18\t \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x02\x12\x1e\n\x14trigger_coupling_raw\x18\n \x01(\x11H\x02\x12\x0f\n\x07holdoff\x18\x0b \x01(\x01\x12\r\n\x05\x64\x65lay\x18\x0c \x01(\x01\x42\x0f\n\rpolarity_enumB\x17\n\x15glitch_condition_enumB\x17\n\x15trigger_coupling_enum\"0\n\x1e\x43onfigureTriggerGlitchResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xe6\x02\n!ConfigureTriggerHysteresisRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\x01\x12\x12\n\nhysteresis\x18\x04 \x01(\x01\x12+\n\x05slope\x18\x05 \x01(\x0e\x32\x1a.niscope_grpc.TriggerSlopeH\x00\x12\x13\n\tslope_raw\x18\x06 \x01(\x11H\x00\x12\x39\n\x10trigger_coupling\x18\x07 \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x01\x12\x1e\n\x14trigger_coupling_raw\x18\x08 \x01(\x11H\x01\x12\x0f\n\x07holdoff\x18\t \x01(\x01\x12\r\n\x05\x64\x65lay\x18\n \x01(\x01\x42\x0c\n\nslope_enumB\x17\n\x15trigger_coupling_enum\"4\n\"ConfigureTriggerHysteresisResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xfd\x02\n\x1d\x43onfigureTriggerWindowRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\x11\n\tlow_level\x18\x03 \x01(\x01\x12\x12\n\nhigh_level\x18\x04 \x01(\x01\x12\x36\n\x0bwindow_mode\x18\x05 \x01(\x0e\x32\x1f.niscope_grpc.TriggerWindowModeH\x00\x12\x19\n\x0fwindow_mode_raw\x18\x06 \x01(\x11H\x00\x12\x39\n\x10trigger_coupling\x18\x07 \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x01\x12\x1e\n\x14trigger_coupling_raw\x18\x08 \x01(\x11H\x01\x12\x0f\n\x07holdoff\x18\t \x01(\x01\x12\r\n\x05\x64\x65lay\x18\n \x01(\x01\x42\x12\n\x10window_mode_enumB\x17\n\x15trigger_coupling_enum\"0\n\x1e\x43onfigureTriggerWindowResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"e\n\x1f\x43onfigureTriggerSoftwareRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x0f\n\x07holdoff\x18\x02 \x01(\x01\x12\r\n\x05\x64\x65lay\x18\x03 \x01(\x01\"2\n ConfigureTriggerSoftwareResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xac\x01\n\x1eSendSoftwareTriggerEdgeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x33\n\rwhich_trigger\x18\x02 \x01(\x0e\x32\x1a.niscope_grpc.WhichTriggerH\x00\x12\x1b\n\x11which_trigger_raw\x18\x03 \x01(\x11H\x00\x42\x14\n\x12which_trigger_enum\"1\n\x1fSendSoftwareTriggerEdgeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"F\n ConfigureTriggerImmediateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"3\n!ConfigureTriggerImmediateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xf5\x02\n\x1b\x43onfigureTriggerRuntRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\x15\n\rlow_threshold\x18\x03 \x01(\x01\x12\x16\n\x0ehigh_threshold\x18\x04 \x01(\x01\x12.\n\x08polarity\x18\x05 \x01(\x0e\x32\x1a.niscope_grpc.RuntPolarityH\x00\x12\x16\n\x0cpolarity_raw\x18\x06 \x01(\x11H\x00\x12\x39\n\x10trigger_coupling\x18\x07 \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x01\x12\x1e\n\x14trigger_coupling_raw\x18\x08 \x01(\x11H\x01\x12\x0f\n\x07holdoff\x18\t \x01(\x01\x12\r\n\x05\x64\x65lay\x18\n \x01(\x01\x42\x0f\n\rpolarity_enumB\x17\n\x15trigger_coupling_enum\".\n\x1c\x43onfigureTriggerRuntResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xcc\x01\n\x1e\x43onfigureTriggerDigitalRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12+\n\x05slope\x18\x03 \x01(\x0e\x32\x1a.niscope_grpc.TriggerSlopeH\x00\x12\x13\n\tslope_raw\x18\x04 \x01(\x11H\x00\x12\x0f\n\x07holdoff\x18\x05 \x01(\x01\x12\r\n\x05\x64\x65lay\x18\x06 \x01(\x01\x42\x0c\n\nslope_enum\"1\n\x1f\x43onfigureTriggerDigitalResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xba\x04\n\x1c\x43onfigureTriggerVideoRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\x19\n\x11\x65nable_dc_restore\x18\x03 \x01(\x08\x12\x38\n\rsignal_format\x18\x04 \x01(\x0e\x32\x1f.niscope_grpc.VideoSignalFormatH\x00\x12\x1b\n\x11signal_format_raw\x18\x05 \x01(\x11H\x00\x12\x30\n\x05\x65vent\x18\x06 \x01(\x0e\x32\x1f.niscope_grpc.VideoTriggerEventH\x01\x12\x13\n\tevent_raw\x18\x07 \x01(\x11H\x01\x12\x13\n\x0bline_number\x18\x08 \x01(\x11\x12/\n\x08polarity\x18\t \x01(\x0e\x32\x1b.niscope_grpc.VideoPolarityH\x02\x12\x16\n\x0cpolarity_raw\x18\n \x01(\x11H\x02\x12\x39\n\x10trigger_coupling\x18\x0b \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x03\x12\x1e\n\x14trigger_coupling_raw\x18\x0c \x01(\x11H\x03\x12\x0f\n\x07holdoff\x18\r \x01(\x01\x12\r\n\x05\x64\x65lay\x18\x0e \x01(\x01\x42\x14\n\x12signal_format_enumB\x0c\n\nevent_enumB\x0f\n\rpolarity_enumB\x17\n\x15trigger_coupling_enum\"/\n\x1d\x43onfigureTriggerVideoResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xe4\x03\n\x1c\x43onfigureTriggerWidthRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x16\n\x0etrigger_source\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\x01\x12\x15\n\rlow_threshold\x18\x04 \x01(\x01\x12\x16\n\x0ehigh_threshold\x18\x05 \x01(\x01\x12/\n\x08polarity\x18\x06 \x01(\x0e\x32\x1b.niscope_grpc.WidthPolarityH\x00\x12\x16\n\x0cpolarity_raw\x18\x07 \x01(\x11H\x00\x12\x31\n\tcondition\x18\x08 \x01(\x0e\x32\x1c.niscope_grpc.WidthConditionH\x01\x12\x17\n\rcondition_raw\x18\t \x01(\x11H\x01\x12\x39\n\x10trigger_coupling\x18\n \x01(\x0e\x32\x1d.niscope_grpc.TriggerCouplingH\x02\x12\x1e\n\x14trigger_coupling_raw\x18\x0b \x01(\x11H\x02\x12\x0f\n\x07holdoff\x18\x0c \x01(\x01\x12\r\n\x05\x64\x65lay\x18\r \x01(\x01\x42\x0f\n\rpolarity_enumB\x10\n\x0e\x63ondition_enumB\x17\n\x15trigger_coupling_enum\"/\n\x1d\x43onfigureTriggerWidthResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x80\x01\n.ConfigureEqualizationFilterCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x14\n\x0c\x63oefficients\x18\x03 \x03(\x01\"A\n/ConfigureEqualizationFilterCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x7f\n(GetEqualizationFilterCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\t\x12\x1e\n\x16number_of_coefficients\x18\x03 \x01(\x11\"Q\n)GetEqualizationFilterCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x14\n\x0c\x63oefficients\x18\x02 \x03(\x01\"g\n\x1bGetFrequencyResponseRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\t\x12\x13\n\x0b\x62uffer_size\x18\x03 \x01(\x11\"\x86\x01\n\x1cGetFrequencyResponseResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0b\x66requencies\x18\x02 \x03(\x01\x12\x12\n\namplitudes\x18\x03 \x03(\x01\x12\x0e\n\x06phases\x18\x04 \x03(\x01\x12\x1d\n\x15number_of_frequencies\x18\x05 \x01(\x11\"[\n\x1b\x43onfigureAcquisitionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x18\n\x10\x61\x63quisition_type\x18\x02 \x01(\x11\".\n\x1c\x43onfigureAcquisitionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"@\n\x1aInitiateAcquisitionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"-\n\x1bInitiateAcquisitionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"2\n\x0c\x41\x62ortRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rAbortResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"3\n\rCommitRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\" \n\x0e\x43ommitResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"m\n\x0bReadRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"^\n\x0cReadResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08waveform\x18\x02 \x03(\x01\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"n\n\x0c\x46\x65tchRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"_\n\rFetchResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08waveform\x18\x02 \x03(\x01\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"u\n\x13\x46\x65tchBinary8Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"f\n\x14\x46\x65tchBinary8Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08waveform\x18\x02 \x01(\x0c\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"v\n\x14\x46\x65tchBinary16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"g\n\x15\x46\x65tchBinary16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08waveform\x18\x02 \x03(\x11\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"v\n\x14\x46\x65tchBinary32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"g\n\x15\x46\x65tchBinary32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08waveform\x18\x02 \x03(\x11\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"u\n\x13\x46\x65tchComplexRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"\x81\x01\n\x14\x46\x65tchComplexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12+\n\x03wfm\x18\x02 \x03(\x0b\x32\x1e.nidevice_grpc.NIComplexNumber\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"}\n\x1b\x46\x65tchComplexBinary16Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x11\"\x86\x01\n\x1c\x46\x65tchComplexBinary16Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12(\n\x03wfm\x18\x02 \x03(\x0b\x32\x1b.nidevice_grpc.NIComplexI16\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\">\n\x18\x41\x63quisitionStatusRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x88\x01\n\x19\x41\x63quisitionStatusResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12;\n\x12\x61\x63quisition_status\x18\x02 \x01(\x0e\x32\x1f.niscope_grpc.AcquisitionStatus\x12\x1e\n\x16\x61\x63quisition_status_raw\x18\x03 \x01(\x11\"P\n\x14\x41\x63tualNumWfmsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\"9\n\x15\x41\x63tualNumWfmsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08num_wfms\x18\x02 \x01(\x11\"\xbc\x01\n\x18\x41\x63tualMeasWfmSizeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12=\n\x13\x61rray_meas_function\x18\x02 \x01(\x0e\x32\x1e.niscope_grpc.ArrayMeasurementH\x00\x12!\n\x17\x61rray_meas_function_raw\x18\x03 \x01(\x11H\x00\x42\x1a\n\x18\x61rray_meas_function_enum\"G\n\x19\x41\x63tualMeasWfmSizeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x1a\n\x12meas_waveform_size\x18\x02 \x01(\x11\"?\n\x19\x41\x63tualRecordLengthRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"C\n\x1a\x41\x63tualRecordLengthResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rrecord_length\x18\x02 \x01(\x11\"7\n\x11SampleRateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"9\n\x12SampleRateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0bsample_rate\x18\x02 \x01(\x01\"7\n\x11SampleModeRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"9\n\x12SampleModeResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0bsample_mode\x18\x02 \x01(\x11\"\xc4\x01\n\x1c\x41\x64\x64WaveformProcessingRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x37\n\rmeas_function\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.ArrayMeasurementH\x00\x12\x1b\n\x11meas_function_raw\x18\x04 \x01(\x11H\x00\x42\x14\n\x12meas_function_enum\"/\n\x1d\x41\x64\x64WaveformProcessingResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"Z\n\x1e\x43learWaveformProcessingRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\"1\n\x1f\x43learWaveformProcessingResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x83\x02\n$ClearWaveformMeasurementStatsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12L\n\x1e\x63learable_measurement_function\x18\x03 \x01(\x0e\x32\".niscope_grpc.ClearableMeasurementH\x00\x12,\n\"clearable_measurement_function_raw\x18\x04 \x01(\x11H\x00\x42%\n#clearable_measurement_function_enum\"7\n%ClearWaveformMeasurementStatsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xe5\x01\n\x16ReadMeasurementRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12?\n\x14scalar_meas_function\x18\x04 \x01(\x0e\x32\x1f.niscope_grpc.ScalarMeasurementH\x00\x12\"\n\x18scalar_meas_function_raw\x18\x05 \x01(\x11H\x00\x42\x1b\n\x19scalar_meas_function_enum\"9\n\x17ReadMeasurementResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x03(\x01\"\xe6\x01\n\x17\x46\x65tchMeasurementRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12?\n\x14scalar_meas_function\x18\x04 \x01(\x0e\x32\x1f.niscope_grpc.ScalarMeasurementH\x00\x12\"\n\x18scalar_meas_function_raw\x18\x05 \x01(\x11H\x00\x42\x1b\n\x19scalar_meas_function_enum\":\n\x18\x46\x65tchMeasurementResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x03(\x01\"\xeb\x01\n\x1c\x46\x65tchMeasurementStatsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12?\n\x14scalar_meas_function\x18\x04 \x01(\x0e\x32\x1f.niscope_grpc.ScalarMeasurementH\x00\x12\"\n\x18scalar_meas_function_raw\x18\x05 \x01(\x11H\x00\x42\x1b\n\x19scalar_meas_function_enum\"\x8c\x01\n\x1d\x46\x65tchMeasurementStatsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x03(\x01\x12\x0c\n\x04mean\x18\x03 \x03(\x01\x12\r\n\x05stdev\x18\x04 \x03(\x01\x12\x0b\n\x03min\x18\x05 \x03(\x01\x12\x0b\n\x03max\x18\x06 \x03(\x01\x12\x14\n\x0cnum_in_stats\x18\x07 \x03(\x11\"\x95\x02\n\x1c\x46\x65tchArrayMeasurementRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12=\n\x13\x61rray_meas_function\x18\x04 \x01(\x0e\x32\x1e.niscope_grpc.ArrayMeasurementH\x00\x12!\n\x17\x61rray_meas_function_raw\x18\x05 \x01(\x11H\x00\x12\x1a\n\rmeas_wfm_size\x18\x06 \x01(\x11H\x01\x88\x01\x01\x42\x1a\n\x18\x61rray_meas_function_enumB\x10\n\x0e_meas_wfm_size\"o\n\x1d\x46\x65tchArrayMeasurementResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x10\n\x08meas_wfm\x18\x02 \x03(\x01\x12,\n\x08wfm_info\x18\x03 \x03(\x0b\x32\x1a.niscope_grpc.WaveformInfo\"2\n\x0cResetRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\x1f\n\rResetResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"5\n\x0fSelfTestRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"W\n\x10SelfTestResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x18\n\x10self_test_result\x18\x02 \x01(\x11\x12\x19\n\x11self_test_message\x18\x03 \x01(\t\"4\n\x0e\x44isableRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"!\n\x0f\x44isableResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"8\n\x12ResetDeviceRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"%\n\x13ResetDeviceResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa0\x01\n\x17\x43\x61lSelfCalibrateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12&\n\x06option\x18\x03 \x01(\x0e\x32\x14.niscope_grpc.OptionH\x00\x12\x14\n\noption_raw\x18\x04 \x01(\x11H\x00\x42\r\n\x0boption_enum\"*\n\x18\x43\x61lSelfCalibrateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\":\n\x14RevisionQueryRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"[\n\x15RevisionQueryResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x17\n\x0f\x64river_revision\x18\x02 \x01(\t\x12\x19\n\x11\x66irmware_revision\x18\x03 \x01(\t\"I\n#ProbeCompensationSignalStartRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"6\n$ProbeCompensationSignalStartResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"H\n\"ProbeCompensationSignalStopRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"5\n#ProbeCompensationSignalStopResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"B\n\x1c\x43\x61\x62leSenseSignalStartRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"/\n\x1d\x43\x61\x62leSenseSignalStartResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"A\n\x1b\x43\x61\x62leSenseSignalStopRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\".\n\x1c\x43\x61\x62leSenseSignalStopResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"J\n\x15GetChannelNameRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\r\n\x05index\x18\x02 \x01(\x11\"@\n\x16GetChannelNameResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x16\n\x0e\x63hannel_string\x18\x02 \x01(\t\"T\n\x1fGetChannelNameFromStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\r\n\x05index\x18\x02 \x01(\t\"@\n GetChannelNameFromStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"c\n\x13\x45rrorHandlerRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nerror_code\x18\x02 \x01(\x11\x12\x14\n\x0c\x65rror_source\x18\x03 \x01(\t\"A\n\x14\x45rrorHandlerResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x19\n\x11\x65rror_description\x18\x02 \x01(\t\"5\n\x0fGetErrorRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"K\n\x10GetErrorResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x12\n\nerror_code\x18\x02 \x01(\x11\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\"P\n\x16GetErrorMessageRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x12\n\nerror_code\x18\x02 \x01(\x11\"@\n\x17GetErrorMessageResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"\x8c\x01\n\x1aGetAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\"<\n\x1bGetAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x11\"\xeb\x01\n\x1aSetAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x13\n\tvalue_raw\x18\x04 \x01(\x11H\x00\x12:\n\x05value\x18\x05 \x01(\x0e\x32).niscope_grpc.NiScopeInt32AttributeValuesH\x00\x42\x0c\n\nvalue_enum\"-\n\x1bSetAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xed\x01\n\x1c\x43heckAttributeViInt32Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x13\n\tvalue_raw\x18\x04 \x01(\x11H\x00\x12:\n\x05value\x18\x05 \x01(\x0e\x32).niscope_grpc.NiScopeInt32AttributeValuesH\x00\x42\x0c\n\nvalue_enum\"/\n\x1d\x43heckAttributeViInt32Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8c\x01\n\x1aGetAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\"<\n\x1bGetAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x03\"\x9f\x01\n\x1aSetAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x11\n\tvalue_raw\x18\x04 \x01(\x03\"-\n\x1bSetAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xa1\x01\n\x1c\x43heckAttributeViInt64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x11\n\tvalue_raw\x18\x04 \x01(\x03\"/\n\x1d\x43heckAttributeViInt64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8d\x01\n\x1bGetAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\"=\n\x1cGetAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x01\"\xb7\x02\n\x1bSetAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x13\n\tvalue_raw\x18\x04 \x01(\x01H\x00\x12;\n\x05value\x18\x05 \x01(\x0e\x32*.niscope_grpc.NiScopeReal64AttributeValuesH\x00\x12H\n\x0cvalue_mapped\x18\x06 \x01(\x0e\x32\x30.niscope_grpc.NiScopeReal64AttributeValuesMappedH\x00\x42\x0c\n\nvalue_enum\".\n\x1cSetAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb9\x02\n\x1d\x43heckAttributeViReal64Request\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\x13\n\tvalue_raw\x18\x04 \x01(\x01H\x00\x12;\n\x05value\x18\x05 \x01(\x0e\x32*.niscope_grpc.NiScopeReal64AttributeValuesH\x00\x12H\n\x0cvalue_mapped\x18\x06 \x01(\x0e\x32\x30.niscope_grpc.NiScopeReal64AttributeValuesMappedH\x00\x42\x0c\n\nvalue_enum\"0\n\x1e\x43heckAttributeViReal64Response\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8d\x01\n\x1bGetAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\"=\n\x1cGetAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t\"\xfa\x01\n\x1bSetAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12H\n\x0cvalue_mapped\x18\x04 \x01(\x0e\x32\x30.niscope_grpc.NiScopeStringAttributeValuesMappedH\x00\x12\x13\n\tvalue_raw\x18\x05 \x01(\tH\x00\x42\x0c\n\nvalue_enum\".\n\x1cSetAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xfc\x01\n\x1d\x43heckAttributeViStringRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12H\n\x0cvalue_mapped\x18\x04 \x01(\x0e\x32\x30.niscope_grpc.NiScopeStringAttributeValuesMappedH\x00\x12\x13\n\tvalue_raw\x18\x05 \x01(\tH\x00\x42\x0c\n\nvalue_enum\"0\n\x1e\x43heckAttributeViStringResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8e\x01\n\x1cGetAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\"V\n\x1dGetAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.nidevice_grpc.Session\"\xb5\x01\n\x1cSetAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12%\n\x05value\x18\x04 \x01(\x0b\x32\x16.nidevice_grpc.Session\"/\n\x1dSetAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\xb7\x01\n\x1e\x43heckAttributeViSessionRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12%\n\x05value\x18\x04 \x01(\x0b\x32\x16.nidevice_grpc.Session\"1\n\x1f\x43heckAttributeViSessionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x8e\x01\n\x1cGetAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\">\n\x1dGetAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x08\"\x9d\x01\n\x1cSetAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\r\n\x05value\x18\x04 \x01(\x08\"/\n\x1dSetAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"\x9f\x01\n\x1e\x43heckAttributeViBooleanRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x34\n\x0c\x61ttribute_id\x18\x03 \x01(\x0e\x32\x1e.niscope_grpc.NiScopeAttribute\x12\r\n\x05value\x18\x04 \x01(\x08\"1\n\x1f\x43heckAttributeViBooleanResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"f\n)ImportAttributeConfigurationBufferRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x15\n\rconfiguration\x18\x02 \x01(\x0c\"<\n*ImportAttributeConfigurationBufferResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"O\n)ExportAttributeConfigurationBufferRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\"S\n*ExportAttributeConfigurationBufferResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rconfiguration\x18\x02 \x01(\x0c\"`\n\'ImportAttributeConfigurationFileRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x11\n\tfile_path\x18\x02 \x01(\t\":\n(ImportAttributeConfigurationFileResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"`\n\'ExportAttributeConfigurationFileRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x11\n\tfile_path\x18\x02 \x01(\t\":\n(ExportAttributeConfigurationFileResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\"Y\n\x1dGetScalingCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\"\x8d\x01\n\x1eGetScalingCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x37\n\x10\x63oefficient_info\x18\x02 \x03(\x0b\x32\x1d.niscope_grpc.CoefficientInfo\x12\"\n\x1anumber_of_coefficient_sets\x18\x03 \x01(\x11\"_\n#GetNormalizationCoefficientsRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\"\x93\x01\n$GetNormalizationCoefficientsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x37\n\x10\x63oefficient_info\x18\x02 \x03(\x0b\x32\x1d.niscope_grpc.CoefficientInfo\x12\"\n\x1anumber_of_coefficient_sets\x18\x03 \x01(\x11\"Y\n\x1eGetStreamEndpointHandleRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x13\n\x0bstream_name\x18\x02 \x01(\t\"H\n\x1fGetStreamEndpointHandleResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x15\n\rwriter_handle\x18\x02 \x01(\r\"\x99\x01\n\x13\x43\x61lFetchDateRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x33\n\twhich_one\x18\x02 \x01(\x0e\x32\x1e.niscope_grpc.CalibrationTypesH\x00\x12\x17\n\rwhich_one_raw\x18\x03 \x01(\x11H\x00\x42\x10\n\x0ewhich_one_enum\"P\n\x14\x43\x61lFetchDateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0c\n\x04year\x18\x02 \x01(\x11\x12\r\n\x05month\x18\x03 \x01(\x11\x12\x0b\n\x03\x64\x61y\x18\x04 \x01(\x11\"\xa0\x01\n\x1a\x43\x61lFetchTemperatureRequest\x12\"\n\x02vi\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x33\n\twhich_one\x18\x02 \x01(\x0e\x32\x1e.niscope_grpc.CalibrationTypesH\x00\x12\x17\n\rwhich_one_raw\x18\x03 \x01(\x11H\x00\x42\x10\n\x0ewhich_one_enum\"B\n\x1b\x43\x61lFetchTemperatureResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01*\xe0Q\n\x10NiScopeAttribute\x12!\n\x1dNISCOPE_ATTRIBUTE_UNSPECIFIED\x10\x00\x12%\n\x1fNISCOPE_ATTRIBUTE_MEAS_HIGH_REF\x10\xaf\xaaL\x12$\n\x1eNISCOPE_ATTRIBUTE_MEAS_LOW_REF\x10\xb0\xaaL\x12\x1d\n\x17NISCOPE_ATTRIBUTE_CACHE\x10\x94\x8b@\x12$\n\x1eNISCOPE_ATTRIBUTE_MEAS_MID_REF\x10\xb1\xaaL\x12#\n\x1dNISCOPE_ATTRIBUTE_RANGE_CHECK\x10\x92\x8b@\x12/\n)NISCOPE_ATTRIBUTE_QUERY_INSTRUMENT_STATUS\x10\x93\x8b@\x12(\n\"NISCOPE_ATTRIBUTE_RECORD_COERCIONS\x10\x96\x8b@\x12 \n\x1aNISCOPE_ATTRIBUTE_SIMULATE\x10\x95\x8b@\x12)\n#NISCOPE_ATTRIBUTE_INTERCHANGE_CHECK\x10\xa5\x8b@\x12%\n\x1fNISCOPE_ATTRIBUTE_CHANNEL_COUNT\x10\xdb\x8c@\x12\x33\n-NISCOPE_ATTRIBUTE_SUPPORTED_INSTRUMENT_MODELS\x10\xd7\x8d@\x12*\n$NISCOPE_ATTRIBUTE_GROUP_CAPABILITIES\x10\xa1\x8e@\x12\x33\n-NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_DESCRIPTION\x10\x92\x8f@\x12.\n(NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_PREFIX\x10\xbe\x8d@\x12.\n(NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_VENDOR\x10\x91\x8f@\x12@\n:NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_CLASS_SPEC_MAJOR_VERSION\x10\x93\x8f@\x12@\n:NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_CLASS_SPEC_MINOR_VERSION\x10\x94\x8f@\x12\x30\n*NISCOPE_ATTRIBUTE_SPECIFIC_DRIVER_REVISION\x10\xb7\x8f@\x12/\n)NISCOPE_ATTRIBUTE_INSTRUMENT_MANUFACTURER\x10\x8f\x8f@\x12(\n\"NISCOPE_ATTRIBUTE_INSTRUMENT_MODEL\x10\x90\x8f@\x12\x34\n.NISCOPE_ATTRIBUTE_INSTRUMENT_FIRMWARE_REVISION\x10\x8e\x8f@\x12.\n(NISCOPE_ATTRIBUTE_IO_RESOURCE_DESCRIPTOR\x10\xc0\x8d@\x12$\n\x1eNISCOPE_ATTRIBUTE_LOGICAL_NAME\x10\xc1\x8d@\x12$\n\x1eNISCOPE_ATTRIBUTE_DRIVER_SETUP\x10\x97\x8b@\x12(\n\"NISCOPE_ATTRIBUTE_ACQUISITION_TYPE\x10\xb5\xa6L\x12#\n\x1dNISCOPE_ATTRIBUTE_SAMPLE_MODE\x10\xba\xa6L\x12\'\n!NISCOPE_ATTRIBUTE_CHANNEL_ENABLED\x10\xd5\xa5L\x12)\n#NISCOPE_ATTRIBUTE_PROBE_ATTENUATION\x10\xd4\xa5L\x12&\n NISCOPE_ATTRIBUTE_VERTICAL_RANGE\x10\xd1\xa5L\x12\'\n!NISCOPE_ATTRIBUTE_VERTICAL_OFFSET\x10\xd2\xa5L\x12\'\n!NISCOPE_ATTRIBUTE_WIDTH_CONDITION\x10\xc8\xa9L\x12+\n%NISCOPE_ATTRIBUTE_WIDTH_LOW_THRESHOLD\x10\xc5\xa9L\x12,\n&NISCOPE_ATTRIBUTE_WIDTH_HIGH_THRESHOLD\x10\xc6\xa9L\x12&\n NISCOPE_ATTRIBUTE_WIDTH_POLARITY\x10\xc7\xa9L\x12)\n#NISCOPE_ATTRIBUTE_VERTICAL_COUPLING\x10\xd3\xa5L\x12+\n%NISCOPE_ATTRIBUTE_MAX_INPUT_FREQUENCY\x10\xd6\xa5L\x12\'\n!NISCOPE_ATTRIBUTE_INPUT_IMPEDANCE\x10\xb7\xa6L\x12,\n&NISCOPE_ATTRIBUTE_HORZ_TIME_PER_RECORD\x10\xd7\xa5L\x12.\n(NISCOPE_ATTRIBUTE_ACQUISITION_START_TIME\x10\xbd\xa6L\x12(\n\"NISCOPE_ATTRIBUTE_HORZ_MIN_NUM_PTS\x10\xd9\xa5L\x12*\n$NISCOPE_ATTRIBUTE_HORZ_RECORD_LENGTH\x10\xd8\xa5L\x12\x30\n*NISCOPE_ATTRIBUTE_HORZ_RECORD_REF_POSITION\x10\xdb\xa5L\x12(\n\"NISCOPE_ATTRIBUTE_HORZ_SAMPLE_RATE\x10\xda\xa5L\x12$\n\x1eNISCOPE_ATTRIBUTE_TRIGGER_TYPE\x10\xdc\xa5L\x12&\n NISCOPE_ATTRIBUTE_TRIGGER_SOURCE\x10\xdd\xa5L\x12%\n\x1fNISCOPE_ATTRIBUTE_TRIGGER_LEVEL\x10\xe1\xa5L\x12*\n$NISCOPE_ATTRIBUTE_TRIGGER_DELAY_TIME\x10\xdf\xa5L\x12\'\n!NISCOPE_ATTRIBUTE_TRIGGER_HOLDOFF\x10\xe0\xa5L\x12(\n\"NISCOPE_ATTRIBUTE_TRIGGER_COUPLING\x10\xde\xa5L\x12%\n\x1fNISCOPE_ATTRIBUTE_TRIGGER_SLOPE\x10\xe2\xa5L\x12(\n\"NISCOPE_ATTRIBUTE_TV_TRIGGER_EVENT\x10\x9d\xa7L\x12.\n(NISCOPE_ATTRIBUTE_TV_TRIGGER_LINE_NUMBER\x10\x9e\xa7L\x12\x30\n*NISCOPE_ATTRIBUTE_TV_TRIGGER_SIGNAL_FORMAT\x10\x99\xa7L\x12+\n%NISCOPE_ATTRIBUTE_TV_TRIGGER_POLARITY\x10\x9c\xa7L\x12(\n\"NISCOPE_ATTRIBUTE_HORZ_NUM_RECORDS\x10\xb1\x98\x46\x12*\n$NISCOPE_ATTRIBUTE_INPUT_CLOCK_SOURCE\x10\xb2\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_OUTPUT_CLOCK_SOURCE\x10\xb3\x98\x46\x12-\n\'NISCOPE_ATTRIBUTE_HORZ_ENFORCE_REALTIME\x10\xb4\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_BINARY_SAMPLE_WIDTH\x10\xb5\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_CABLE_SENSE_VOLTAGE\x10\xb9\x99\x46\x12(\n\"NISCOPE_ATTRIBUTE_CABLE_SENSE_MODE\x10\xba\x99\x46\x12\x31\n+NISCOPE_ATTRIBUTE_CABLE_SENSE_SIGNAL_ENABLE\x10\xbb\x99\x46\x12*\n$NISCOPE_ATTRIBUTE_TRIGGER_HYSTERESIS\x10\xb6\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_CLOCK_SYNC_PULSE_SOURCE\x10\xb7\x98\x46\x12%\n\x1fNISCOPE_ATTRIBUTE_MASTER_ENABLE\x10\xb8\x98\x46\x12\'\n!NISCOPE_ATTRIBUTE_MIN_SAMPLE_RATE\x10\xb9\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_TRIGGER_WINDOW_MODE\x10\xbc\x98\x46\x12\x30\n*NISCOPE_ATTRIBUTE_TRIGGER_WINDOW_LOW_LEVEL\x10\xbd\x98\x46\x12\x31\n+NISCOPE_ATTRIBUTE_TRIGGER_WINDOW_HIGH_LEVEL\x10\xbe\x98\x46\x12,\n&NISCOPE_ATTRIBUTE_MEAS_REF_LEVEL_UNITS\x10\xc0\x98\x46\x12*\n$NISCOPE_ATTRIBUTE_MEAS_OTHER_CHANNEL\x10\xc2\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_MEAS_HYSTERESIS_PERCENT\x10\xc3\x98\x46\x12\x34\n.NISCOPE_ATTRIBUTE_MEAS_LAST_ACQ_HISTOGRAM_SIZE\x10\xc4\x98\x46\x12\x33\n-NISCOPE_ATTRIBUTE_MEAS_VOLTAGE_HISTOGRAM_SIZE\x10\xc5\x98\x46\x12\x38\n2NISCOPE_ATTRIBUTE_MEAS_VOLTAGE_HISTOGRAM_LOW_VOLTS\x10\xc6\x98\x46\x12\x39\n3NISCOPE_ATTRIBUTE_MEAS_VOLTAGE_HISTOGRAM_HIGH_VOLTS\x10\xc7\x98\x46\x12\x30\n*NISCOPE_ATTRIBUTE_MEAS_TIME_HISTOGRAM_SIZE\x10\xc8\x98\x46\x12\x35\n/NISCOPE_ATTRIBUTE_MEAS_TIME_HISTOGRAM_LOW_VOLTS\x10\xc9\x98\x46\x12\x36\n0NISCOPE_ATTRIBUTE_MEAS_TIME_HISTOGRAM_HIGH_VOLTS\x10\xca\x98\x46\x12\x34\n.NISCOPE_ATTRIBUTE_MEAS_TIME_HISTOGRAM_LOW_TIME\x10\xcb\x98\x46\x12\x35\n/NISCOPE_ATTRIBUTE_MEAS_TIME_HISTOGRAM_HIGH_TIME\x10\xcc\x98\x46\x12;\n5NISCOPE_ATTRIBUTE_MEAS_POLYNOMIAL_INTERPOLATION_ORDER\x10\xcd\x98\x46\x12:\n4NISCOPE_ATTRIBUTE_MEAS_INTERPOLATION_SAMPLING_FACTOR\x10\xce\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_MEAS_FILTER_CUTOFF_FREQ\x10\xcf\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_MEAS_FILTER_CENTER_FREQ\x10\xd0\x98\x46\x12*\n$NISCOPE_ATTRIBUTE_MEAS_FILTER_RIPPLE\x10\xd1\x98\x46\x12>\n8NISCOPE_ATTRIBUTE_MEAS_FILTER_TRANSIENT_WAVEFORM_PERCENT\x10\xd2\x98\x46\x12(\n\"NISCOPE_ATTRIBUTE_MEAS_FILTER_TYPE\x10\xd3\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_MEAS_FILTER_ORDER\x10\xd4\x98\x46\x12(\n\"NISCOPE_ATTRIBUTE_MEAS_FILTER_TAPS\x10\xd5\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_MEAS_CHAN_LOW_REF_LEVEL\x10\xd6\x98\x46\x12/\n)NISCOPE_ATTRIBUTE_MEAS_CHAN_MID_REF_LEVEL\x10\xd7\x98\x46\x12\x30\n*NISCOPE_ATTRIBUTE_MEAS_CHAN_HIGH_REF_LEVEL\x10\xd8\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_MEAS_FILTER_WIDTH\x10\xd9\x98\x46\x12.\n(NISCOPE_ATTRIBUTE_MEAS_FIR_FILTER_WINDOW\x10\xda\x98\x46\x12\'\n!NISCOPE_ATTRIBUTE_MEAS_ARRAY_GAIN\x10\xdb\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_MEAS_ARRAY_OFFSET\x10\xdc\x98\x46\x12.\n(NISCOPE_ATTRIBUTE_MEAS_PERCENTAGE_METHOD\x10\xdd\x98\x46\x12&\n NISCOPE_ATTRIBUTE_ACQ_ARM_SOURCE\x10\xe5\x98\x46\x12(\n\"NISCOPE_ATTRIBUTE_IS_PROBE_COMP_ON\x10\xf2\x98\x46\x12*\n$NISCOPE_ATTRIBUTE_USE_SPEC_INITIAL_X\x10\xf3\x98\x46\x12\x36\n0NISCOPE_ATTRIBUTE_ALLOW_MORE_RECORDS_THAN_MEMORY\x10\xf4\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_ONBOARD_MEMORY_SIZE\x10\xf5\x98\x46\x12(\n\"NISCOPE_ATTRIBUTE_RIS_NUM_AVERAGES\x10\xf6\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_RUNT_TIME_CONDITION\x10\xb4\x99\x46\x12+\n%NISCOPE_ATTRIBUTE_RUNT_TIME_LOW_LIMIT\x10\xb5\x99\x46\x12,\n&NISCOPE_ATTRIBUTE_RUNT_TIME_HIGH_LIMIT\x10\xb6\x99\x46\x12%\n\x1fNISCOPE_ATTRIBUTE_RUNT_POLARITY\x10\xff\xa7L\x12*\n$NISCOPE_ATTRIBUTE_RUNT_LOW_THRESHOLD\x10\xfe\xa7L\x12+\n%NISCOPE_ATTRIBUTE_RUNT_HIGH_THRESHOLD\x10\xfd\xa7L\x12\"\n\x1cNISCOPE_ATTRIBUTE_RIS_METHOD\x10\xf7\x98\x46\x12.\n(NISCOPE_ATTRIBUTE_FETCH_INTERLEAVED_DATA\x10\xf8\x98\x46\x12\x33\n-NISCOPE_ATTRIBUTE_MAX_REAL_TIME_SAMPLING_RATE\x10\xf9\x98\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_MAX_RIS_RATE\x10\xfa\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_TRIGGER_IMPEDANCE\x10\xfb\x98\x46\x12%\n\x1fNISCOPE_ATTRIBUTE_DEVICE_NUMBER\x10\xfc\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_FETCH_RELATIVE_TO\x10\xfd\x98\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_FETCH_OFFSET\x10\xfe\x98\x46\x12+\n%NISCOPE_ATTRIBUTE_FETCH_RECORD_NUMBER\x10\xff\x98\x46\x12)\n#NISCOPE_ATTRIBUTE_FETCH_NUM_RECORDS\x10\x80\x99\x46\x12.\n(NISCOPE_ATTRIBUTE_FETCH_MEAS_NUM_SAMPLES\x10\x81\x99\x46\x12#\n\x1dNISCOPE_ATTRIBUTE_POINTS_DONE\x10\x82\x99\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_RECORDS_DONE\x10\x83\x99\x46\x12\x1f\n\x19NISCOPE_ATTRIBUTE_BACKLOG\x10\x84\x99\x46\x12%\n\x1fNISCOPE_ATTRIBUTE_POLL_INTERVAL\x10\x94\x99\x46\x12\'\n!NISCOPE_ATTRIBUTE_PLL_LOCK_STATUS\x10\xc7\xa2\x46\x12*\n$NISCOPE_ATTRIBUTE_DEVICE_TEMPERATURE\x10\x86\x99\x46\x12-\n\'NISCOPE_ATTRIBUTE_SAMP_CLK_TIMEBASE_SRC\x10\x87\x99\x46\x12.\n(NISCOPE_ATTRIBUTE_SAMP_CLK_TIMEBASE_RATE\x10\x88\x99\x46\x12-\n\'NISCOPE_ATTRIBUTE_SAMP_CLK_TIMEBASE_DIV\x10\x89\x99\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_REF_CLK_RATE\x10\x8a\x99\x46\x12=\n7NISCOPE_ATTRIBUTE_EXPORTED_SAMPLE_CLOCK_OUTPUT_TERMINAL\x10\x8b\x99\x46\x12)\n#NISCOPE_ATTRIBUTE_ENABLE_DC_RESTORE\x10\x8d\x99\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_ADV_TRIG_SRC\x10\x8e\x99\x46\x12(\n\"NISCOPE_ATTRIBUTE_ARM_REF_TRIG_SRC\x10\x8f\x99\x46\x12+\n%NISCOPE_ATTRIBUTE_REF_TRIG_TDC_ENABLE\x10\x90\x99\x46\x12\"\n\x1cNISCOPE_ATTRIBUTE_RESOLUTION\x10\x96\x99\x46\x12\x34\n.NISCOPE_ATTRIBUTE_START_TO_REF_TRIGGER_HOLDOFF\x10\x97\x99\x46\x12%\n\x1fNISCOPE_ATTRIBUTE_SERIAL_NUMBER\x10\x98\x99\x46\x12\x32\n,NISCOPE_ATTRIBUTE_OSCILLATOR_PHASE_DAC_VALUE\x10\x99\x99\x46\x12\x30\n*NISCOPE_ATTRIBUTE_RIS_IN_AUTO_SETUP_ENABLE\x10\x9a\x99\x46\x12\x36\n0NISCOPE_ATTRIBUTE_CHANNEL_TERMINAL_CONFIGURATION\x10\x9b\x99\x46\x12@\n:NISCOPE_ATTRIBUTE_EXPORTED_ADVANCE_TRIGGER_OUTPUT_TERMINAL\x10\x9d\x99\x46\x12=\n7NISCOPE_ATTRIBUTE_READY_FOR_START_EVENT_OUTPUT_TERMINAL\x10\x9e\x99\x46\x12;\n5NISCOPE_ATTRIBUTE_READY_FOR_REF_EVENT_OUTPUT_TERMINAL\x10\x9f\x99\x46\x12?\n9NISCOPE_ATTRIBUTE_READY_FOR_ADVANCE_EVENT_OUTPUT_TERMINAL\x10\xa0\x99\x46\x12\x36\n0NISCOPE_ATTRIBUTE_FLEX_FIR_ANTIALIAS_FILTER_TYPE\x10\xbf\x9a\x46\x12#\n\x1dNISCOPE_ATTRIBUTE_DDC_ENABLED\x10\xdc\x9a\x46\x12\x39\n3NISCOPE_ATTRIBUTE_DDC_FREQUENCY_TRANSLATION_ENABLED\x10\xde\x9a\x46\x12,\n&NISCOPE_ATTRIBUTE_DDC_CENTER_FREQUENCY\x10\xdf\x9a\x46\x12\x30\n*NISCOPE_ATTRIBUTE_DDC_DATA_PROCESSING_MODE\x10\xe0\x9a\x46\x12\x39\n3NISCOPE_ATTRIBUTE_DDC_FREQUENCY_TRANSLATION_PHASE_I\x10\xe1\x9a\x46\x12\x39\n3NISCOPE_ATTRIBUTE_DDC_FREQUENCY_TRANSLATION_PHASE_Q\x10\xe2\x9a\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_DIGITAL_GAIN\x10\xe3\x9a\x46\x12&\n NISCOPE_ATTRIBUTE_DIGITAL_OFFSET\x10\xe4\x9a\x46\x12\x30\n*NISCOPE_ATTRIBUTE_OVERFLOW_ERROR_REPORTING\x10\xe5\x9a\x46\x12$\n\x1eNISCOPE_ATTRIBUTE_DDC_Q_SOURCE\x10\xe6\x9a\x46\x12\x31\n+NISCOPE_ATTRIBUTE_FETCH_INTERLEAVED_IQ_DATA\x10\xe7\x9a\x46\x12\x35\n/NISCOPE_ATTRIBUTE_EQUALIZATION_NUM_COEFFICIENTS\x10\xe8\x9a\x46\x12\x33\n-NISCOPE_ATTRIBUTE_EQUALIZATION_FILTER_ENABLED\x10\xe9\x9a\x46\x12\x35\n/NISCOPE_ATTRIBUTE_REF_TRIGGER_DETECTOR_LOCATION\x10\xea\x9a\x46\x12\x36\n0NISCOPE_ATTRIBUTE_REF_TRIGGER_MINIMUM_QUIET_TIME\x10\xeb\x9a\x46\x12\x38\n2NISCOPE_ATTRIBUTE_ENABLE_TIME_INTERLEAVED_SAMPLING\x10\xb0\x99\x46\x12(\n\"NISCOPE_ATTRIBUTE_ENABLED_CHANNELS\x10\xbc\x99\x46\x12\x30\n*NISCOPE_ATTRIBUTE_DATA_TRANSFER_BLOCK_SIZE\x10\xec\x9a\x46\x12(\n\"NISCOPE_ATTRIBUTE_TRIGGER_MODIFIER\x10\xb6\xa6L\x12.\n(NISCOPE_ATTRIBUTE_TRIGGER_AUTO_TRIGGERED\x10\xc6\x9a\x46\x12>\n8NISCOPE_ATTRIBUTE_EXPORTED_START_TRIGGER_OUTPUT_TERMINAL\x10\x91\x99\x46\x12<\n6NISCOPE_ATTRIBUTE_EXPORTED_REF_TRIGGER_OUTPUT_TERMINAL\x10\x92\x99\x46\x12;\n5NISCOPE_ATTRIBUTE_END_OF_RECORD_EVENT_OUTPUT_TERMINAL\x10\x93\x99\x46\x12@\n:NISCOPE_ATTRIBUTE_END_OF_ACQUISITION_EVENT_OUTPUT_TERMINAL\x10\x95\x99\x46\x12.\n(NISCOPE_ATTRIBUTE_5V_OUT_OUTPUT_TERMINAL\x10\xb1\x99\x46\x12/\n)NISCOPE_ATTRIBUTE_BANDPASS_FILTER_ENABLED\x10\xee\x9a\x46\x12&\n NISCOPE_ATTRIBUTE_DITHER_ENABLED\x10\xef\x9a\x46\x12\x33\n-NISCOPE_ATTRIBUTE_FRACTIONAL_RESAMPLE_ENABLED\x10\xf0\x9a\x46\x12(\n\"NISCOPE_ATTRIBUTE_GLITCH_CONDITION\x10\xe3\xa8L\x12$\n\x1eNISCOPE_ATTRIBUTE_GLITCH_WIDTH\x10\xe1\xa8L\x12\'\n!NISCOPE_ATTRIBUTE_GLITCH_POLARITY\x10\xe2\xa8L\x12\x37\n1NISCOPE_ATTRIBUTE_DATA_TRANSFER_MAXIMUM_BANDWIDTH\x10\xf1\x9a\x46\x12;\n5NISCOPE_ATTRIBUTE_DATA_TRANSFER_PREFERRED_PACKET_SIZE\x10\xf2\x9a\x46\x12(\n\"NISCOPE_ATTRIBUTE_SIGNAL_COND_GAIN\x10\xc7\x9a\x46\x12*\n$NISCOPE_ATTRIBUTE_SIGNAL_COND_OFFSET\x10\xc8\x9a\x46\x12#\n\x1dNISCOPE_ATTRIBUTE_P2P_ENABLED\x10\x82\x9b\x46\x12.\n(NISCOPE_ATTRIBUTE_P2P_CHANNELS_TO_STREAM\x10\x83\x9b\x46\x12)\n#NISCOPE_ATTRIBUTE_P2P_ENDPOINT_SIZE\x10\x86\x9b\x46\x12\x35\n/NISCOPE_ATTRIBUTE_P2P_SAMPLES_AVAIL_IN_ENDPOINT\x10\xf8\x9a\x46\x12:\n4NISCOPE_ATTRIBUTE_P2P_MOST_SAMPLES_AVAIL_IN_ENDPOINT\x10\x85\x9b\x46\x12/\n)NISCOPE_ATTRIBUTE_P2P_SAMPLES_TRANSFERRED\x10\x84\x9b\x46\x12-\n\'NISCOPE_ATTRIBUTE_P2P_ENDPOINT_OVERFLOW\x10\x88\x9b\x46\x12/\n)NISCOPE_ATTRIBUTE_P2P_FIFO_ENDPOINT_COUNT\x10\x89\x9b\x46\x12\x32\n,NISCOPE_ATTRIBUTE_P2P_ONBOARD_MEMORY_ENABLED\x10\x92\x9b\x46\x12\x38\n2NISCOPE_ATTRIBUTE_P2P_MANUAL_CONFIGURATION_ENABLED\x10\x87\x9b\x46\x12\x36\n0NISCOPE_ATTRIBUTE_P2P_DATA_TRANS_PERMISSION_ADDR\x10\xf9\x9a\x46\x12;\n5NISCOPE_ATTRIBUTE_P2P_DATA_TRANS_PERMISSION_ADDR_TYPE\x10\xfa\x9a\x46\x12\x33\n-NISCOPE_ATTRIBUTE_P2P_DESTINATION_WINDOW_ADDR\x10\xfb\x9a\x46\x12\x38\n2NISCOPE_ATTRIBUTE_P2P_DESTINATION_WINDOW_ADDR_TYPE\x10\xfc\x9a\x46\x12\x33\n-NISCOPE_ATTRIBUTE_P2P_DESTINATION_WINDOW_SIZE\x10\xfd\x9a\x46\x12\x32\n,NISCOPE_ATTRIBUTE_P2P_NOTIFY_PUSH_MESSAGE_ON\x10\xfe\x9a\x46\x12\x34\n.NISCOPE_ATTRIBUTE_P2P_NOTIFY_MESSAGE_PUSH_ADDR\x10\xff\x9a\x46\x12\x39\n3NISCOPE_ATTRIBUTE_P2P_NOTIFY_MESSAGE_PUSH_ADDR_TYPE\x10\x80\x9b\x46\x12\x35\n/NISCOPE_ATTRIBUTE_P2P_NOTIFY_MESSAGE_PUSH_VALUE\x10\x81\x9b\x46\x12.\n(NISCOPE_ATTRIBUTE_SAMP_CLK_TIMEBASE_MULT\x10\x9f\x9b\x46\x12.\n(NISCOPE_ATTRIBUTE_P2P_STREAM_RELATIVE_TO\x10\xa5\x9b\x46\x12:\n4NISCOPE_ATTRIBUTE_P2P_SAMPLES_TRANSFERRED_PER_RECORD\x10\xac\x9b\x46\x12@\n:NISCOPE_ATTRIBUTE_END_OF_RECORD_TO_ADVANCE_TRIGGER_HOLDOFF\x10\x9e\x9b\x46\x12\x34\n.NISCOPE_ATTRIBUTE_ABSOLUTE_SAMPLE_CLOCK_OFFSET\x10\xa6\x9b\x46\x12)\n#NISCOPE_ATTRIBUTE_FPGA_BITFILE_PATH\x10\xa7\x9b\x46\x12>\n8NISCOPE_ATTRIBUTE_INTERLEAVING_OFFSET_CORRECTION_ENABLED\x10\xa8\x9b\x46\x12\x32\n,NISCOPE_ATTRIBUTE_HIGH_PASS_FILTER_FREQUENCY\x10\xa9\x9b\x46\x12>\n8NISCOPE_ATTRIBUTE_END_OF_ACQUISITION_EVENT_TERMINAL_NAME\x10\xbd\x99\x46\x12\x39\n3NISCOPE_ATTRIBUTE_END_OF_RECORD_EVENT_TERMINAL_NAME\x10\xbe\x99\x46\x12\x35\n/NISCOPE_ATTRIBUTE_ADVANCE_TRIGGER_TERMINAL_NAME\x10\xbf\x99\x46\x12\x31\n+NISCOPE_ATTRIBUTE_REF_TRIGGER_TERMINAL_NAME\x10\xc0\x99\x46\x12\x33\n-NISCOPE_ATTRIBUTE_START_TRIGGER_TERMINAL_NAME\x10\xc1\x99\x46\x12=\n7NISCOPE_ATTRIBUTE_READY_FOR_ADVANCE_EVENT_TERMINAL_NAME\x10\xc2\x99\x46\x12\x39\n3NISCOPE_ATTRIBUTE_READY_FOR_REF_EVENT_TERMINAL_NAME\x10\xc3\x99\x46\x12;\n5NISCOPE_ATTRIBUTE_READY_FOR_START_EVENT_TERMINAL_NAME\x10\xc4\x99\x46*\xf4\x01\n\x0cWhichTrigger\x12\x34\n0WHICH_TRIGGER_NISCOPE_VAL_SOFTWARE_TRIGGER_START\x10\x00\x12<\n8WHICH_TRIGGER_NISCOPE_VAL_SOFTWARE_TRIGGER_ARM_REFERENCE\x10\x01\x12\x38\n4WHICH_TRIGGER_NISCOPE_VAL_SOFTWARE_TRIGGER_REFERENCE\x10\x02\x12\x36\n2WHICH_TRIGGER_NISCOPE_VAL_SOFTWARE_TRIGGER_ADVANCE\x10\x03*\x85\x01\n\x10VerticalCoupling\x12$\n VERTICAL_COUPLING_NISCOPE_VAL_AC\x10\x00\x12$\n VERTICAL_COUPLING_NISCOPE_VAL_DC\x10\x01\x12%\n!VERTICAL_COUPLING_NISCOPE_VAL_GND\x10\x02*\xe8\x01\n\x0fTriggerCoupling\x12#\n\x1fTRIGGER_COUPLING_NISCOPE_VAL_AC\x10\x00\x12#\n\x1fTRIGGER_COUPLING_NISCOPE_VAL_DC\x10\x01\x12*\n&TRIGGER_COUPLING_NISCOPE_VAL_HF_REJECT\x10\x03\x12*\n&TRIGGER_COUPLING_NISCOPE_VAL_LF_REJECT\x10\x04\x12\x33\n.TRIGGER_COUPLING_NISCOPE_VAL_AC_PLUS_HF_REJECT\x10\xe9\x07*\x8a\x01\n\x0cTriggerSlope\x12&\n\"TRIGGER_SLOPE_NISCOPE_VAL_NEGATIVE\x10\x00\x12&\n\"TRIGGER_SLOPE_NISCOPE_VAL_POSITIVE\x10\x01\x12*\n&TRIGGER_SLOPE_NISCOPE_VAL_SLOPE_EITHER\x10\x03*\x87\x01\n\rVideoPolarity\x12\x1e\n\x1aVIDEO_POLARITY_UNSPECIFIED\x10\x00\x12*\n&VIDEO_POLARITY_NISCOPE_VAL_TV_POSITIVE\x10\x01\x12*\n&VIDEO_POLARITY_NISCOPE_VAL_TV_NEGATIVE\x10\x02*\xcb\x02\n\x11VideoTriggerEvent\x12#\n\x1fVIDEO_TRIGGER_EVENT_UNSPECIFIED\x10\x00\x12\x33\n/VIDEO_TRIGGER_EVENT_NISCOPE_VAL_TV_EVENT_FIELD1\x10\x01\x12\x33\n/VIDEO_TRIGGER_EVENT_NISCOPE_VAL_TV_EVENT_FIELD2\x10\x02\x12\x36\n2VIDEO_TRIGGER_EVENT_NISCOPE_VAL_TV_EVENT_ANY_FIELD\x10\x03\x12\x35\n1VIDEO_TRIGGER_EVENT_NISCOPE_VAL_TV_EVENT_ANY_LINE\x10\x04\x12\x38\n4VIDEO_TRIGGER_EVENT_NISCOPE_VAL_TV_EVENT_LINE_NUMBER\x10\x05*\x9c\x01\n\x0fGlitchCondition\x12 \n\x1cGLITCH_CONDITION_UNSPECIFIED\x10\x00\x12\x34\n0GLITCH_CONDITION_NISCOPE_VAL_GLITCH_GREATER_THAN\x10\x02\x12\x31\n-GLITCH_CONDITION_NISCOPE_VAL_GLITCH_LESS_THAN\x10\x01*\xc2\x01\n\x0eGlitchPolarity\x12\x1f\n\x1bGLITCH_POLARITY_UNSPECIFIED\x10\x00\x12/\n+GLITCH_POLARITY_NISCOPE_VAL_GLITCH_POSITIVE\x10\x01\x12/\n+GLITCH_POLARITY_NISCOPE_VAL_GLITCH_NEGATIVE\x10\x02\x12-\n)GLITCH_POLARITY_NISCOPE_VAL_GLITCH_EITHER\x10\x03*\x8e\x01\n\x0eWidthCondition\x12\x1f\n\x1bWIDTH_CONDITION_UNSPECIFIED\x10\x00\x12,\n(WIDTH_CONDITION_NISCOPE_VAL_WIDTH_WITHIN\x10\x01\x12-\n)WIDTH_CONDITION_NISCOPE_VAL_WIDTH_OUTSIDE\x10\x02*\xba\x01\n\rWidthPolarity\x12\x1e\n\x1aWIDTH_POLARITY_UNSPECIFIED\x10\x00\x12-\n)WIDTH_POLARITY_NISCOPE_VAL_WIDTH_POSITIVE\x10\x01\x12-\n)WIDTH_POLARITY_NISCOPE_VAL_WIDTH_NEGATIVE\x10\x02\x12+\n\'WIDTH_POLARITY_NISCOPE_VAL_WIDTH_EITHER\x10\x03*\xb2\x01\n\x0cRuntPolarity\x12\x1d\n\x19RUNT_POLARITY_UNSPECIFIED\x10\x00\x12+\n\'RUNT_POLARITY_NISCOPE_VAL_RUNT_POSITIVE\x10\x01\x12+\n\'RUNT_POLARITY_NISCOPE_VAL_RUNT_NEGATIVE\x10\x02\x12)\n%RUNT_POLARITY_NISCOPE_VAL_RUNT_EITHER\x10\x03*\x96\x07\n\x16\x43lockingTerminalValues\x12(\n$CLOCKING_TERMINAL_VALUES_UNSPECIFIED\x10\x00\x12\x32\n.CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_NO_SOURCE\x10\x01\x12\x33\n/CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_RTSI_CLOCK\x10\x02\x12\x31\n-CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_EXTERNAL\x10\x03\x12.\n*CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PFI_0\x10\x04\x12.\n*CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PFI_1\x10\x05\x12.\n*CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PFI_2\x10\x06\x12/\n+CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_CLK_IN\x10\x07\x12\x30\n,CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_CLK_OUT\x10\x08\x12:\n6CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_INTERNAL10MHZ_OSC\x10\t\x12\x30\n,CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PXI_CLK\x10\n\x12\x32\n.CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PXI_CLK10\x10\x0b\x12\x33\n/CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PXI_CLK100\x10\x0c\x12\x35\n1CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_PXIE_DSTAR_A\x10\r\x12\x35\n1CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_AUX_0_CLK_IN\x10\x0e\x12\x36\n2CLOCKING_TERMINAL_VALUES_NISCOPE_VAL_AUX_0_CLK_OUT\x10\x0f\x12\x46\nBCLOCKING_TERMINAL_VALUES_NISCOPE_VAL_ONBOARD_CONFIGURABLE_RATE_CLK\x10\x10*\xfa\x04\n\x11\x45xportableSignals\x12\"\n\x1e\x45XPORTABLE_SIGNALS_UNSPECIFIED\x10\x00\x12.\n*EXPORTABLE_SIGNALS_NISCOPE_VAL_REF_TRIGGER\x10\x01\x12\x30\n,EXPORTABLE_SIGNALS_NISCOPE_VAL_START_TRIGGER\x10\x02\x12;\n7EXPORTABLE_SIGNALS_NISCOPE_VAL_END_OF_ACQUISITION_EVENT\x10\x03\x12\x36\n2EXPORTABLE_SIGNALS_NISCOPE_VAL_END_OF_RECORD_EVENT\x10\x04\x12\x32\n.EXPORTABLE_SIGNALS_NISCOPE_VAL_ADVANCE_TRIGGER\x10\x05\x12:\n6EXPORTABLE_SIGNALS_NISCOPE_VAL_READY_FOR_ADVANCE_EVENT\x10\x06\x12\x38\n4EXPORTABLE_SIGNALS_NISCOPE_VAL_READY_FOR_START_EVENT\x10\x07\x12\x36\n2EXPORTABLE_SIGNALS_NISCOPE_VAL_READY_FOR_REF_EVENT\x10\n\x12)\n%EXPORTABLE_SIGNALS_NISCOPE_VAL_5V_OUT\x10\r\x12,\n(EXPORTABLE_SIGNALS_NISCOPE_VAL_REF_CLOCK\x10\x64\x12/\n+EXPORTABLE_SIGNALS_NISCOPE_VAL_SAMPLE_CLOCK\x10\x65*\xbc\x01\n\x11TriggerWindowMode\x12\x33\n/TRIGGER_WINDOW_MODE_NISCOPE_VAL_ENTERING_WINDOW\x10\x00\x12\x32\n.TRIGGER_WINDOW_MODE_NISCOPE_VAL_LEAVING_WINDOW\x10\x01\x12>\n:TRIGGER_WINDOW_MODE_NISCOPE_VAL_ENTERING_OR_LEAVING_WINDOW\x10\x02*\xb8\x01\n\x11\x41\x63quisitionStatus\x12\x32\n.ACQUISITION_STATUS_NISCOPE_VAL_ACQ_IN_PROGRESS\x10\x00\x12/\n+ACQUISITION_STATUS_NISCOPE_VAL_ACQ_COMPLETE\x10\x01\x12>\n1ACQUISITION_STATUS_NISCOPE_VAL_ACQ_STATUS_UNKNOWN\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01*\xcf\x0f\n\x11ScalarMeasurement\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_RISE_TIME\x10\x00\x12\x32\n-SCALAR_MEASUREMENT_NISCOPE_VAL_NO_MEASUREMENT\x10\xa0\x1f\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_FALL_TIME\x10\x01\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_FREQUENCY\x10\x02\x12)\n%SCALAR_MEASUREMENT_NISCOPE_VAL_PERIOD\x10\x03\x12.\n*SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_RMS\x10\x04\x12\x37\n3SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_PEAK_TO_PEAK\x10\x05\x12.\n*SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_MAX\x10\x06\x12.\n*SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_MIN\x10\x07\x12/\n+SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HIGH\x10\x08\x12.\n*SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_LOW\x10\t\x12\x32\n.SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_AVERAGE\x10\n\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_WIDTH_NEG\x10\x0b\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_WIDTH_POS\x10\x0c\x12\x31\n-SCALAR_MEASUREMENT_NISCOPE_VAL_DUTY_CYCLE_NEG\x10\r\x12\x31\n-SCALAR_MEASUREMENT_NISCOPE_VAL_DUTY_CYCLE_POS\x10\x0e\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_AMPLITUDE\x10\x0f\x12\x34\n0SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_CYCLE_RMS\x10\x10\x12\x38\n4SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_CYCLE_AVERAGE\x10\x11\x12,\n(SCALAR_MEASUREMENT_NISCOPE_VAL_OVERSHOOT\x10\x12\x12+\n\'SCALAR_MEASUREMENT_NISCOPE_VAL_PRESHOOT\x10\x13\x12\x31\n,SCALAR_MEASUREMENT_NISCOPE_VAL_LOW_REF_VOLTS\x10\xe8\x07\x12\x31\n,SCALAR_MEASUREMENT_NISCOPE_VAL_MID_REF_VOLTS\x10\xe9\x07\x12\x32\n-SCALAR_MEASUREMENT_NISCOPE_VAL_HIGH_REF_VOLTS\x10\xea\x07\x12(\n#SCALAR_MEASUREMENT_NISCOPE_VAL_AREA\x10\xeb\x07\x12.\n)SCALAR_MEASUREMENT_NISCOPE_VAL_CYCLE_AREA\x10\xec\x07\x12,\n\'SCALAR_MEASUREMENT_NISCOPE_VAL_INTEGRAL\x10\xed\x07\x12\x30\n+SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_BASE\x10\xee\x07\x12/\n*SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_TOP\x10\xef\x07\x12\x31\n,SCALAR_MEASUREMENT_NISCOPE_VAL_FFT_FREQUENCY\x10\xf0\x07\x12\x31\n,SCALAR_MEASUREMENT_NISCOPE_VAL_FFT_AMPLITUDE\x10\xf1\x07\x12\x32\n-SCALAR_MEASUREMENT_NISCOPE_VAL_RISE_SLEW_RATE\x10\xf2\x07\x12\x32\n-SCALAR_MEASUREMENT_NISCOPE_VAL_FALL_SLEW_RATE\x10\xf3\x07\x12/\n*SCALAR_MEASUREMENT_NISCOPE_VAL_AC_ESTIMATE\x10\xf4\x07\x12/\n*SCALAR_MEASUREMENT_NISCOPE_VAL_DC_ESTIMATE\x10\xf5\x07\x12.\n)SCALAR_MEASUREMENT_NISCOPE_VAL_TIME_DELAY\x10\xf6\x07\x12\x32\n-SCALAR_MEASUREMENT_NISCOPE_VAL_AVERAGE_PERIOD\x10\xf7\x07\x12\x35\n0SCALAR_MEASUREMENT_NISCOPE_VAL_AVERAGE_FREQUENCY\x10\xf8\x07\x12\x37\n2SCALAR_MEASUREMENT_NISCOPE_VAL_VOLTAGE_BASE_TO_TOP\x10\xf9\x07\x12/\n*SCALAR_MEASUREMENT_NISCOPE_VAL_PHASE_DELAY\x10\xfa\x07*\xd4\x0b\n\x10\x41rrayMeasurement\x12!\n\x1d\x41RRAY_MEASUREMENT_UNSPECIFIED\x10\x00\x12\x31\n,ARRAY_MEASUREMENT_NISCOPE_VAL_NO_MEASUREMENT\x10\xa0\x1f\x12\x35\n0ARRAY_MEASUREMENT_NISCOPE_VAL_LAST_ACQ_HISTOGRAM\x10\xa1\x1f\x12\x35\n0ARRAY_MEASUREMENT_NISCOPE_VAL_FFT_PHASE_SPECTRUM\x10\xa2\x1f\x12=\n8ARRAY_MEASUREMENT_NISCOPE_VAL_FFT_AMP_SPECTRUM_VOLTS_RMS\x10\xa3\x1f\x12>\n9ARRAY_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_VOLTAGE_HISTOGRAM\x10\xa4\x1f\x12;\n6ARRAY_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_TIME_HISTOGRAM\x10\xa5\x1f\x12\x31\n,ARRAY_MEASUREMENT_NISCOPE_VAL_ARRAY_INTEGRAL\x10\xa6\x1f\x12-\n(ARRAY_MEASUREMENT_NISCOPE_VAL_DERIVATIVE\x10\xa7\x1f\x12*\n%ARRAY_MEASUREMENT_NISCOPE_VAL_INVERSE\x10\xa8\x1f\x12\x31\n,ARRAY_MEASUREMENT_NISCOPE_VAL_HANNING_WINDOW\x10\xa9\x1f\x12\x32\n-ARRAY_MEASUREMENT_NISCOPE_VAL_FLAT_TOP_WINDOW\x10\xaa\x1f\x12;\n6ARRAY_MEASUREMENT_NISCOPE_VAL_POLYNOMIAL_INTERPOLATION\x10\xab\x1f\x12\x34\n/ARRAY_MEASUREMENT_NISCOPE_VAL_MULTIPLY_CHANNELS\x10\xac\x1f\x12/\n*ARRAY_MEASUREMENT_NISCOPE_VAL_ADD_CHANNELS\x10\xad\x1f\x12\x34\n/ARRAY_MEASUREMENT_NISCOPE_VAL_SUBTRACT_CHANNELS\x10\xae\x1f\x12\x32\n-ARRAY_MEASUREMENT_NISCOPE_VAL_DIVIDE_CHANNELS\x10\xaf\x1f\x12\x34\n/ARRAY_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_AVERAGE\x10\xb0\x1f\x12\x35\n0ARRAY_MEASUREMENT_NISCOPE_VAL_BUTTERWORTH_FILTER\x10\xb1\x1f\x12\x33\n.ARRAY_MEASUREMENT_NISCOPE_VAL_CHEBYSHEV_FILTER\x10\xb2\x1f\x12\x36\n1ARRAY_MEASUREMENT_NISCOPE_VAL_FFT_AMP_SPECTRUM_DB\x10\xb3\x1f\x12\x31\n,ARRAY_MEASUREMENT_NISCOPE_VAL_HAMMING_WINDOW\x10\xb4\x1f\x12\x36\n1ARRAY_MEASUREMENT_NISCOPE_VAL_WINDOWED_FIR_FILTER\x10\xb5\x1f\x12\x30\n+ARRAY_MEASUREMENT_NISCOPE_VAL_BESSEL_FILTER\x10\xb6\x1f\x12\x32\n-ARRAY_MEASUREMENT_NISCOPE_VAL_TRIANGLE_WINDOW\x10\xb7\x1f\x12\x32\n-ARRAY_MEASUREMENT_NISCOPE_VAL_BLACKMAN_WINDOW\x10\xb8\x1f\x12/\n*ARRAY_MEASUREMENT_NISCOPE_VAL_ARRAY_OFFSET\x10\xb9\x1f\x12-\n(ARRAY_MEASUREMENT_NISCOPE_VAL_ARRAY_GAIN\x10\xba\x1f*\xa1\x01\n\x10\x43\x61librationTypes\x12.\n*CALIBRATION_TYPES_NISCOPE_VAL_CAL_EXTERNAL\x10\x00\x12*\n&CALIBRATION_TYPES_NISCOPE_VAL_CAL_SELF\x10\x01\x12\x31\n-CALIBRATION_TYPES_NISCOPE_VAL_CAL_MANUFACTURE\x10\x02*\xb3\x1e\n\x14\x43learableMeasurement\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_RISE_TIME\x10\x00\x12\x37\n2CLEARABLE_MEASUREMENT_NISCOPE_VAL_ALL_MEASUREMENTS\x10\x90N\x12\x42\n=CLEARABLE_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_VOLTAGE_HISTOGRAM\x10\xa4\x1f\x12?\n:CLEARABLE_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_TIME_HISTOGRAM\x10\xa5\x1f\x12\x38\n3CLEARABLE_MEASUREMENT_NISCOPE_VAL_MULTI_ACQ_AVERAGE\x10\xb0\x1f\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_FREQUENCY\x10\x02\x12\x38\n3CLEARABLE_MEASUREMENT_NISCOPE_VAL_AVERAGE_FREQUENCY\x10\xf8\x07\x12\x34\n/CLEARABLE_MEASUREMENT_NISCOPE_VAL_FFT_FREQUENCY\x10\xf0\x07\x12,\n(CLEARABLE_MEASUREMENT_NISCOPE_VAL_PERIOD\x10\x03\x12\x35\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_AVERAGE_PERIOD\x10\xf7\x07\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_FALL_TIME\x10\x01\x12\x35\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_RISE_SLEW_RATE\x10\xf2\x07\x12\x35\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_FALL_SLEW_RATE\x10\xf3\x07\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_OVERSHOOT\x10\x12\x12.\n*CLEARABLE_MEASUREMENT_NISCOPE_VAL_PRESHOOT\x10\x13\x12\x31\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_RMS\x10\x04\x12\x37\n3CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_CYCLE_RMS\x10\x10\x12\x32\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_AC_ESTIMATE\x10\xf4\x07\x12\x34\n/CLEARABLE_MEASUREMENT_NISCOPE_VAL_FFT_AMPLITUDE\x10\xf1\x07\x12\x35\n1CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_AVERAGE\x10\n\x12;\n7CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_CYCLE_AVERAGE\x10\x11\x12\x32\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_DC_ESTIMATE\x10\xf5\x07\x12\x31\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_MAX\x10\x06\x12\x31\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_MIN\x10\x07\x12:\n6CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_PEAK_TO_PEAK\x10\x05\x12\x32\n.CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HIGH\x10\x08\x12\x31\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_LOW\x10\t\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_AMPLITUDE\x10\x0f\x12\x32\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_TOP\x10\xef\x07\x12\x33\n.CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_BASE\x10\xee\x07\x12:\n5CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_BASE_TO_TOP\x10\xf9\x07\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_WIDTH_NEG\x10\x0b\x12/\n+CLEARABLE_MEASUREMENT_NISCOPE_VAL_WIDTH_POS\x10\x0c\x12\x34\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_DUTY_CYCLE_NEG\x10\r\x12\x34\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_DUTY_CYCLE_POS\x10\x0e\x12/\n*CLEARABLE_MEASUREMENT_NISCOPE_VAL_INTEGRAL\x10\xed\x07\x12+\n&CLEARABLE_MEASUREMENT_NISCOPE_VAL_AREA\x10\xeb\x07\x12\x31\n,CLEARABLE_MEASUREMENT_NISCOPE_VAL_CYCLE_AREA\x10\xec\x07\x12\x31\n,CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_DELAY\x10\xf6\x07\x12\x32\n-CLEARABLE_MEASUREMENT_NISCOPE_VAL_PHASE_DELAY\x10\xfa\x07\x12\x34\n/CLEARABLE_MEASUREMENT_NISCOPE_VAL_LOW_REF_VOLTS\x10\xe8\x07\x12\x34\n/CLEARABLE_MEASUREMENT_NISCOPE_VAL_MID_REF_VOLTS\x10\xe9\x07\x12\x35\n0CLEARABLE_MEASUREMENT_NISCOPE_VAL_HIGH_REF_VOLTS\x10\xea\x07\x12=\n8CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MEAN\x10\xd0\x0f\x12>\n9CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_STDEV\x10\xd1\x0f\x12?\n:CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MEDIAN\x10\xd3\x0f\x12=\n8CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MODE\x10\xda\x0f\x12<\n7CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MAX\x10\xd5\x0f\x12<\n7CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MIN\x10\xd6\x0f\x12\x45\n@CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_PEAK_TO_PEAK\x10\xd2\x0f\x12H\nCCLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MEAN_PLUS_STDEV\x10\xd7\x0f\x12J\nECLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MEAN_PLUS_2_STDEV\x10\xd8\x0f\x12J\nECLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_MEAN_PLUS_3_STDEV\x10\xd9\x0f\x12=\n8CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_HITS\x10\xd4\x0f\x12\x41\n<CLEARABLE_MEASUREMENT_NISCOPE_VAL_VOLTAGE_HISTOGRAM_NEW_HITS\x10\xdb\x0f\x12:\n5CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MEAN\x10\xb8\x17\x12;\n6CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_STDEV\x10\xb9\x17\x12<\n7CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MEDIAN\x10\xbb\x17\x12:\n5CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MODE\x10\xc2\x17\x12\x39\n4CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MAX\x10\xbd\x17\x12\x39\n4CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MIN\x10\xbe\x17\x12\x42\n=CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_PEAK_TO_PEAK\x10\xba\x17\x12\x45\n@CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MEAN_PLUS_STDEV\x10\xbf\x17\x12G\nBCLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MEAN_PLUS_2_STDEV\x10\xc0\x17\x12G\nBCLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_MEAN_PLUS_3_STDEV\x10\xc1\x17\x12:\n5CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_HITS\x10\xbc\x17\x12>\n9CLEARABLE_MEASUREMENT_NISCOPE_VAL_TIME_HISTOGRAM_NEW_HITS\x10\xc3\x17*q\n\x06Option\x12\x32\n.OPTION_NISCOPE_VAL_SELF_CALIBRATE_ALL_CHANNELS\x10\x00\x12\x33\n/OPTION_NISCOPE_VAL_RESTORE_EXTERNAL_CALIBRATION\x10\x01*\x80\t\n\x11VideoSignalFormat\x12#\n\x1fVIDEO_SIGNAL_FORMAT_UNSPECIFIED\x10\x00\x12(\n$VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_NTSC\x10\x01\x12\'\n#VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_PAL\x10\x02\x12)\n%VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_SECAM\x10\x03\x12*\n%VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_M_PAL\x10\xe9\x07\x12G\nBVIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_480I_59_94_FIELDS_PER_SECOND\x10\xf2\x07\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_480I_60_FIELDS_PER_SECOND\x10\xf3\x07\x12G\nBVIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_480P_59_94_FRAMES_PER_SECOND\x10\xf7\x07\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_480P_60_FRAMES_PER_SECOND\x10\xf8\x07\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_576I_50_FIELDS_PER_SECOND\x10\xfc\x07\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_576P_50_FRAMES_PER_SECOND\x10\x81\x08\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_720P_50_FRAMES_PER_SECOND\x10\x87\x08\x12G\nBVIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_720P_59_94_FRAMES_PER_SECOND\x10\x88\x08\x12\x44\n?VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_720P_60_FRAMES_PER_SECOND\x10\x89\x08\x12\x45\n@VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_1080I_50_FIELDS_PER_SECOND\x10\x90\x08\x12H\nCVIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_1080I_59_94_FIELDS_PER_SECOND\x10\x91\x08\x12\x45\n@VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_1080I_60_FIELDS_PER_SECOND\x10\x92\x08\x12\x45\n@VIDEO_SIGNAL_FORMAT_NISCOPE_VAL_VIDEO_1080P_24_FRAMES_PER_SECOND\x10\x95\x08*\xad\x35\n\x1bNiScopeInt32AttributeValues\x12\x1d\n\x19NISCOPE_INT32_UNSPECIFIED\x10\x00\x12-\n)NISCOPE_INT32_ACQUISITION_TYPE_VAL_NORMAL\x10\x00\x12/\n*NISCOPE_INT32_ACQUISITION_TYPE_VAL_FLEXRES\x10\xe9\x07\x12+\n&NISCOPE_INT32_ACQUISITION_TYPE_VAL_DDC\x10\xea\x07\x12\x30\n,NISCOPE_INT32_ADDRESS_TYPE_VAL_ADDR_PHYSICAL\x10\x00\x12/\n+NISCOPE_INT32_ADDRESS_TYPE_VAL_ADDR_VIRTUAL\x10\x01\x12/\n+NISCOPE_INT32_DATA_PROCESSING_MODE_VAL_REAL\x10\x00\x12\x32\n.NISCOPE_INT32_DATA_PROCESSING_MODE_VAL_COMPLEX\x10\x01\x12,\n(NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_NONE\x10\x00\x12\x30\n+NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_HANNING\x10\x99\x03\x12\x31\n,NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_FLAT_TOP\x10\x9a\x03\x12\x30\n+NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_HAMMING\x10\xa4\x03\x12\x31\n,NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_TRIANGLE\x10\xa7\x03\x12\x31\n,NISCOPE_INT32_FIR_FILTER_WINDOW_VAL_BLACKMAN\x10\xa8\x03\x12\x35\n0NISCOPE_INT32_FETCH_RELATIVE_TO_VAL_READ_POINTER\x10\x84\x03\x12\x33\n.NISCOPE_INT32_FETCH_RELATIVE_TO_VAL_PRETRIGGER\x10\xdd\x03\x12,\n\'NISCOPE_INT32_FETCH_RELATIVE_TO_VAL_NOW\x10\xe1\x03\x12.\n)NISCOPE_INT32_FETCH_RELATIVE_TO_VAL_START\x10\xe2\x03\x12\x30\n+NISCOPE_INT32_FETCH_RELATIVE_TO_VAL_TRIGGER\x10\xe3\x03\x12\x44\n@NISCOPE_INT32_FLEX_FIR_ANTIALIAS_FILTER_TYPE_VAL_48_TAP_STANDARD\x10\x00\x12\x43\n?NISCOPE_INT32_FLEX_FIR_ANTIALIAS_FILTER_TYPE_VAL_48_TAP_HANNING\x10\x01\x12\x43\n?NISCOPE_INT32_FLEX_FIR_ANTIALIAS_FILTER_TYPE_VAL_16_TAP_HANNING\x10\x02\x12\x42\n>NISCOPE_INT32_FLEX_FIR_ANTIALIAS_FILTER_TYPE_VAL_8_TAP_HANNING\x10\x03\x12:\n6NISCOPE_INT32_GLITCH_CONDITION_VAL_GLITCH_GREATER_THAN\x10\x02\x12\x37\n3NISCOPE_INT32_GLITCH_CONDITION_VAL_GLITCH_LESS_THAN\x10\x01\x12\x35\n1NISCOPE_INT32_GLITCH_POLARITY_VAL_GLITCH_POSITIVE\x10\x01\x12\x35\n1NISCOPE_INT32_GLITCH_POLARITY_VAL_GLITCH_NEGATIVE\x10\x02\x12\x33\n/NISCOPE_INT32_GLITCH_POLARITY_VAL_GLITCH_EITHER\x10\x03\x12\x33\n/NISCOPE_INT32_MEAS_FILTER_TYPE_VAL_MEAS_LOWPASS\x10\x00\x12\x34\n0NISCOPE_INT32_MEAS_FILTER_TYPE_VAL_MEAS_HIGHPASS\x10\x01\x12\x34\n0NISCOPE_INT32_MEAS_FILTER_TYPE_VAL_MEAS_BANDPASS\x10\x02\x12\x34\n0NISCOPE_INT32_MEAS_FILTER_TYPE_VAL_MEAS_BANDSTOP\x10\x03\x12:\n6NISCOPE_INT32_MEAS_PERCENTAGE_METHOD_VAL_MEAS_LOW_HIGH\x10\x00\x12\x39\n5NISCOPE_INT32_MEAS_PERCENTAGE_METHOD_VAL_MEAS_MIN_MAX\x10\x01\x12:\n6NISCOPE_INT32_MEAS_PERCENTAGE_METHOD_VAL_MEAS_BASE_TOP\x10\x02\x12\x37\n3NISCOPE_INT32_MEAS_REF_LEVEL_UNITS_VAL_MEAS_VOLTAGE\x10\x00\x12:\n6NISCOPE_INT32_MEAS_REF_LEVEL_UNITS_VAL_MEAS_PERCENTAGE\x10\x01\x12\x34\n0NISCOPE_INT32_NOTIFICATION_TYPE_VAL_NOTIFY_NEVER\x10\x00\x12\x33\n/NISCOPE_INT32_NOTIFICATION_TYPE_VAL_NOTIFY_DONE\x10\x01\x12\x44\n@NISCOPE_INT32_OVERFLOW_ERROR_REPORTING_VAL_ERROR_REPORTING_ERROR\x10\x00\x12\x46\nBNISCOPE_INT32_OVERFLOW_ERROR_REPORTING_VAL_ERROR_REPORTING_WARNING\x10\x01\x12G\nCNISCOPE_INT32_OVERFLOW_ERROR_REPORTING_VAL_ERROR_REPORTING_DISABLED\x10\x02\x12N\nJNISCOPE_INT32_P2_P_STREAM_RELATIVE_TO_VAL_STREAM_RELATIVE_TO_START_TRIGGER\x10\x00\x12R\nNNISCOPE_INT32_P2_P_STREAM_RELATIVE_TO_VAL_STREAM_RELATIVE_TO_REFERENCE_TRIGGER\x10\x01\x12M\nINISCOPE_INT32_P2_P_STREAM_RELATIVE_TO_VAL_STREAM_RELATIVE_TO_SYNC_TRIGGER\x10\x02\x12\x37\n3NISCOPE_INT32_RIS_METHOD_VAL_RIS_EXACT_NUM_AVERAGES\x10\x01\x12\x35\n1NISCOPE_INT32_RIS_METHOD_VAL_RIS_MIN_NUM_AVERAGES\x10\x02\x12/\n+NISCOPE_INT32_RIS_METHOD_VAL_RIS_INCOMPLETE\x10\x03\x12\x36\n2NISCOPE_INT32_RIS_METHOD_VAL_RIS_LIMITED_BIN_WIDTH\x10\x05\x12L\nHNISCOPE_INT32_REF_TRIGGER_DETECTOR_LOCATION_VAL_ANALOG_DETECTION_CIRCUIT\x10\x00\x12>\n:NISCOPE_INT32_REF_TRIGGER_DETECTOR_LOCATION_VAL_DDC_OUTPUT\x10\x01\x12\x31\n-NISCOPE_INT32_RUNT_POLARITY_VAL_RUNT_POSITIVE\x10\x01\x12\x31\n-NISCOPE_INT32_RUNT_POLARITY_VAL_RUNT_NEGATIVE\x10\x02\x12/\n+NISCOPE_INT32_RUNT_POLARITY_VAL_RUNT_EITHER\x10\x03\x12\x42\n>NISCOPE_INT32_RUNT_TIME_CONDITION_VAL_RUNT_TIME_CONDITION_NONE\x10\x00\x12\x44\n@NISCOPE_INT32_RUNT_TIME_CONDITION_VAL_RUNT_TIME_CONDITION_WITHIN\x10\x01\x12\x45\nANISCOPE_INT32_RUNT_TIME_CONDITION_VAL_RUNT_TIME_CONDITION_OUTSIDE\x10\x02\x12+\n\'NISCOPE_INT32_SAMPLE_MODE_VAL_REAL_TIME\x10\x00\x12\x31\n-NISCOPE_INT32_SAMPLE_MODE_VAL_EQUIVALENT_TIME\x10\x01\x12\x39\n5NISCOPE_INT32_TERMINAL_CONFIGURATION_VAL_SINGLE_ENDED\x10\x00\x12\x44\n@NISCOPE_INT32_TERMINAL_CONFIGURATION_VAL_UNBALANCED_DIFFERENTIAL\x10\x01\x12\x39\n5NISCOPE_INT32_TERMINAL_CONFIGURATION_VAL_DIFFERENTIAL\x10\x02\x12)\n%NISCOPE_INT32_TRIGGER_COUPLING_VAL_AC\x10\x00\x12)\n%NISCOPE_INT32_TRIGGER_COUPLING_VAL_DC\x10\x01\x12\x30\n,NISCOPE_INT32_TRIGGER_COUPLING_VAL_HF_REJECT\x10\x03\x12\x30\n,NISCOPE_INT32_TRIGGER_COUPLING_VAL_LF_REJECT\x10\x04\x12\x39\n4NISCOPE_INT32_TRIGGER_COUPLING_VAL_AC_PLUS_HF_REJECT\x10\xe9\x07\x12\x35\n1NISCOPE_INT32_TRIGGER_MODIFIER_VAL_NO_TRIGGER_MOD\x10\x01\x12+\n\'NISCOPE_INT32_TRIGGER_MODIFIER_VAL_AUTO\x10\x02\x12\x31\n-NISCOPE_INT32_TRIGGER_MODIFIER_VAL_AUTO_LEVEL\x10\x03\x12,\n(NISCOPE_INT32_TRIGGER_SLOPE_VAL_NEGATIVE\x10\x00\x12,\n(NISCOPE_INT32_TRIGGER_SLOPE_VAL_POSITIVE\x10\x01\x12\x30\n,NISCOPE_INT32_TRIGGER_SLOPE_VAL_SLOPE_EITHER\x10\x03\x12/\n+NISCOPE_INT32_TRIGGER_TYPE_VAL_EDGE_TRIGGER\x10\x01\x12\x36\n1NISCOPE_INT32_TRIGGER_TYPE_VAL_HYSTERESIS_TRIGGER\x10\xe9\x07\x12\x33\n.NISCOPE_INT32_TRIGGER_TYPE_VAL_DIGITAL_TRIGGER\x10\xea\x07\x12\x32\n-NISCOPE_INT32_TRIGGER_TYPE_VAL_WINDOW_TRIGGER\x10\xeb\x07\x12\x34\n/NISCOPE_INT32_TRIGGER_TYPE_VAL_SOFTWARE_TRIGGER\x10\xec\x07\x12-\n)NISCOPE_INT32_TRIGGER_TYPE_VAL_TV_TRIGGER\x10\x05\x12\x31\n-NISCOPE_INT32_TRIGGER_TYPE_VAL_GLITCH_TRIGGER\x10\x04\x12\x30\n,NISCOPE_INT32_TRIGGER_TYPE_VAL_WIDTH_TRIGGER\x10\x02\x12/\n+NISCOPE_INT32_TRIGGER_TYPE_VAL_RUNT_TRIGGER\x10\x03\x12\x34\n0NISCOPE_INT32_TRIGGER_TYPE_VAL_IMMEDIATE_TRIGGER\x10\x06\x12\x39\n5NISCOPE_INT32_TRIGGER_WINDOW_MODE_VAL_ENTERING_WINDOW\x10\x00\x12\x38\n4NISCOPE_INT32_TRIGGER_WINDOW_MODE_VAL_LEAVING_WINDOW\x10\x01\x12\x44\n@NISCOPE_INT32_TRIGGER_WINDOW_MODE_VAL_ENTERING_OR_LEAVING_WINDOW\x10\x02\x12*\n&NISCOPE_INT32_VERTICAL_COUPLING_VAL_AC\x10\x00\x12*\n&NISCOPE_INT32_VERTICAL_COUPLING_VAL_DC\x10\x01\x12+\n\'NISCOPE_INT32_VERTICAL_COUPLING_VAL_GND\x10\x02\x12\x30\n,NISCOPE_INT32_VIDEO_POLARITY_VAL_TV_POSITIVE\x10\x01\x12\x30\n,NISCOPE_INT32_VIDEO_POLARITY_VAL_TV_NEGATIVE\x10\x02\x12.\n*NISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_NTSC\x10\x01\x12-\n)NISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_PAL\x10\x02\x12/\n+NISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_SECAM\x10\x03\x12\x30\n+NISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_M_PAL\x10\xe9\x07\x12M\nHNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_480I_59_94_FIELDS_PER_SECOND\x10\xf2\x07\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_480I_60_FIELDS_PER_SECOND\x10\xf3\x07\x12M\nHNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_480P_59_94_FRAMES_PER_SECOND\x10\xf7\x07\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_480P_60_FRAMES_PER_SECOND\x10\xf8\x07\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_576I_50_FIELDS_PER_SECOND\x10\xfc\x07\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_576P_50_FRAMES_PER_SECOND\x10\x81\x08\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_720P_50_FRAMES_PER_SECOND\x10\x87\x08\x12M\nHNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_720P_59_94_FRAMES_PER_SECOND\x10\x88\x08\x12J\nENISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_720P_60_FRAMES_PER_SECOND\x10\x89\x08\x12K\nFNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_1080I_50_FIELDS_PER_SECOND\x10\x90\x08\x12N\nINISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_1080I_59_94_FIELDS_PER_SECOND\x10\x91\x08\x12K\nFNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_1080I_60_FIELDS_PER_SECOND\x10\x92\x08\x12K\nFNISCOPE_INT32_VIDEO_SIGNAL_FORMAT_VAL_VIDEO_1080P_24_FRAMES_PER_SECOND\x10\x95\x08\x12\x39\n5NISCOPE_INT32_VIDEO_TRIGGER_EVENT_VAL_TV_EVENT_FIELD1\x10\x01\x12\x39\n5NISCOPE_INT32_VIDEO_TRIGGER_EVENT_VAL_TV_EVENT_FIELD2\x10\x02\x12<\n8NISCOPE_INT32_VIDEO_TRIGGER_EVENT_VAL_TV_EVENT_ANY_FIELD\x10\x03\x12;\n7NISCOPE_INT32_VIDEO_TRIGGER_EVENT_VAL_TV_EVENT_ANY_LINE\x10\x04\x12>\n:NISCOPE_INT32_VIDEO_TRIGGER_EVENT_VAL_TV_EVENT_LINE_NUMBER\x10\x05\x12\x32\n.NISCOPE_INT32_WIDTH_CONDITION_VAL_WIDTH_WITHIN\x10\x01\x12\x33\n/NISCOPE_INT32_WIDTH_CONDITION_VAL_WIDTH_OUTSIDE\x10\x02\x12\x33\n/NISCOPE_INT32_WIDTH_POLARITY_VAL_WIDTH_POSITIVE\x10\x01\x12\x33\n/NISCOPE_INT32_WIDTH_POLARITY_VAL_WIDTH_NEGATIVE\x10\x02\x12\x31\n-NISCOPE_INT32_WIDTH_POLARITY_VAL_WIDTH_EITHER\x10\x03\x1a\x02\x10\x01*\xc9\x01\n\x1cNiScopeReal64AttributeValues\x12\x1e\n\x1aNISCOPE_REAL64_UNSPECIFIED\x10\x00\x12\x41\n=NISCOPE_REAL64_CABLE_SENSE_MODE_VAL_CABLE_SENSE_MODE_DISABLED\x10\x00\x12\x42\n>NISCOPE_REAL64_CABLE_SENSE_MODE_VAL_CABLE_SENSE_MODE_ON_DEMAND\x10\x01\x1a\x02\x10\x01*\xe3\x04\n\"NiScopeReal64AttributeValuesMapped\x12%\n!NISCOPE_REAL64_MAPPED_UNSPECIFIED\x10\x00\x12.\n*NISCOPE_REAL64_INPUT_IMPEDANCE_VAL_50_OHMS\x10\x01\x12.\n*NISCOPE_REAL64_INPUT_IMPEDANCE_VAL_75_OHMS\x10\x02\x12\x30\n,NISCOPE_REAL64_INPUT_IMPEDANCE_VAL_1_MEG_OHM\x10\x03\x12\x43\n?NISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_BANDWIDTH_DEVICE_DEFAULT\x10\x04\x12\x39\n5NISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_BANDWIDTH_FULL\x10\x05\x12:\n6NISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_20MHZ_BANDWIDTH\x10\x06\x12;\n7NISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_100MHZ_BANDWIDTH\x10\x07\x12\x44\n@NISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_20MHZ_MAX_INPUT_FREQUENCY\x10\x08\x12\x45\nANISCOPE_REAL64_MAX_INPUT_FREQUENCY_VAL_100MHZ_MAX_INPUT_FREQUENCY\x10\t*\x9e\x11\n\"NiScopeStringAttributeValuesMapped\x12%\n!NISCOPE_STRING_MAPPED_UNSPECIFIED\x10\x00\x12\x33\n/NISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_CLK_IN\x10\x01\x12\x36\n2NISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_NO_SOURCE\x10\x02\x12\x35\n1NISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_PXI_STAR\x10\x03\x12\x39\n5NISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_PXIE_DSTAR_A\x10\x04\x12\x39\n5NISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_AUX_0_CLK_IN\x10\x05\x12J\nFNISCOPE_STRING_SAMP_CLK_TIMEPACE_SRC_VAL_ONBOARD_CONFIGURABLE_RATE_CLK\x10\x06\x12/\n+NISCOPE_STRING_TRIGGER_SOURCE_VAL_IMMEDIATE\x10\x07\x12.\n*NISCOPE_STRING_TRIGGER_SOURCE_VAL_EXTERNAL\x10\x08\x12\x32\n.NISCOPE_STRING_TRIGGER_SOURCE_VAL_SW_TRIG_FUNC\x10\t\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL0\x10\n\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL1\x10\x0b\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL2\x10\x0c\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL3\x10\r\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL4\x10\x0e\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL5\x10\x0f\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL6\x10\x10\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_TTL7\x10\x11\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_ECL0\x10\x12\x12*\n&NISCOPE_STRING_TRIGGER_SOURCE_VAL_ECL1\x10\x13\x12.\n*NISCOPE_STRING_TRIGGER_SOURCE_VAL_PXI_STAR\x10\x14\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_0\x10\x15\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_1\x10\x16\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_2\x10\x17\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_3\x10\x18\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_4\x10\x19\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_5\x10\x1a\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_6\x10\x1b\x12,\n(NISCOPE_STRING_TRIGGER_SOURCE_VAL_RTSI_7\x10\x1c\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_0\x10\x1d\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_1\x10\x1e\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_2\x10\x1f\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_3\x10 \x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_4\x10!\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_5\x10\"\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_6\x10#\x12+\n\'NISCOPE_STRING_TRIGGER_SOURCE_VAL_PFI_7\x10$\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_0\x10%\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_1\x10&\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_3\x10\'\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_4\x10(\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_5\x10)\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_6\x10*\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_7\x10+\x12\x31\n-NISCOPE_STRING_TRIGGER_SOURCE_VAL_AUX_0_PFI_2\x10,2\xe0K\n\x07NiScope\x12=\n\x04Init\x12\x19.niscope_grpc.InitRequest\x1a\x1a.niscope_grpc.InitResponse\x12^\n\x0fInitWithOptions\x12$.niscope_grpc.InitWithOptionsRequest\x1a%.niscope_grpc.InitWithOptionsResponse\x12@\n\x05\x43lose\x12\x1a.niscope_grpc.CloseRequest\x1a\x1b.niscope_grpc.CloseResponse\x12L\n\tAutoSetup\x12\x1e.niscope_grpc.AutoSetupRequest\x1a\x1f.niscope_grpc.AutoSetupResponse\x12\x64\n\x11\x43onfigureVertical\x12&.niscope_grpc.ConfigureVerticalRequest\x1a\'.niscope_grpc.ConfigureVerticalResponse\x12\x85\x01\n\x1c\x43onfigureChanCharacteristics\x12\x31.niscope_grpc.ConfigureChanCharacteristicsRequest\x1a\x32.niscope_grpc.ConfigureChanCharacteristicsResponse\x12|\n\x19\x43onfigureHorizontalTiming\x12..niscope_grpc.ConfigureHorizontalTimingRequest\x1a/.niscope_grpc.ConfigureHorizontalTimingResponse\x12[\n\x0e\x43onfigureClock\x12#.niscope_grpc.ConfigureClockRequest\x1a$.niscope_grpc.ConfigureClockResponse\x12U\n\x0c\x45xportSignal\x12!.niscope_grpc.ExportSignalRequest\x1a\".niscope_grpc.ExportSignalResponse\x12\x8b\x01\n\x1e\x41\x64justSampleClockRelativeDelay\x12\x33.niscope_grpc.AdjustSampleClockRelativeDelayRequest\x1a\x34.niscope_grpc.AdjustSampleClockRelativeDelayResponse\x12m\n\x14\x43onfigureTriggerEdge\x12).niscope_grpc.ConfigureTriggerEdgeRequest\x1a*.niscope_grpc.ConfigureTriggerEdgeResponse\x12s\n\x16\x43onfigureTriggerGlitch\x12+.niscope_grpc.ConfigureTriggerGlitchRequest\x1a,.niscope_grpc.ConfigureTriggerGlitchResponse\x12\x7f\n\x1a\x43onfigureTriggerHysteresis\x12/.niscope_grpc.ConfigureTriggerHysteresisRequest\x1a\x30.niscope_grpc.ConfigureTriggerHysteresisResponse\x12s\n\x16\x43onfigureTriggerWindow\x12+.niscope_grpc.ConfigureTriggerWindowRequest\x1a,.niscope_grpc.ConfigureTriggerWindowResponse\x12y\n\x18\x43onfigureTriggerSoftware\x12-.niscope_grpc.ConfigureTriggerSoftwareRequest\x1a..niscope_grpc.ConfigureTriggerSoftwareResponse\x12v\n\x17SendSoftwareTriggerEdge\x12,.niscope_grpc.SendSoftwareTriggerEdgeRequest\x1a-.niscope_grpc.SendSoftwareTriggerEdgeResponse\x12|\n\x19\x43onfigureTriggerImmediate\x12..niscope_grpc.ConfigureTriggerImmediateRequest\x1a/.niscope_grpc.ConfigureTriggerImmediateResponse\x12m\n\x14\x43onfigureTriggerRunt\x12).niscope_grpc.ConfigureTriggerRuntRequest\x1a*.niscope_grpc.ConfigureTriggerRuntResponse\x12v\n\x17\x43onfigureTriggerDigital\x12,.niscope_grpc.ConfigureTriggerDigitalRequest\x1a-.niscope_grpc.ConfigureTriggerDigitalResponse\x12p\n\x15\x43onfigureTriggerVideo\x12*.niscope_grpc.ConfigureTriggerVideoRequest\x1a+.niscope_grpc.ConfigureTriggerVideoResponse\x12p\n\x15\x43onfigureTriggerWidth\x12*.niscope_grpc.ConfigureTriggerWidthRequest\x1a+.niscope_grpc.ConfigureTriggerWidthResponse\x12\xa6\x01\n\'ConfigureEqualizationFilterCoefficients\x12<.niscope_grpc.ConfigureEqualizationFilterCoefficientsRequest\x1a=.niscope_grpc.ConfigureEqualizationFilterCoefficientsResponse\x12\x94\x01\n!GetEqualizationFilterCoefficients\x12\x36.niscope_grpc.GetEqualizationFilterCoefficientsRequest\x1a\x37.niscope_grpc.GetEqualizationFilterCoefficientsResponse\x12m\n\x14GetFrequencyResponse\x12).niscope_grpc.GetFrequencyResponseRequest\x1a*.niscope_grpc.GetFrequencyResponseResponse\x12m\n\x14\x43onfigureAcquisition\x12).niscope_grpc.ConfigureAcquisitionRequest\x1a*.niscope_grpc.ConfigureAcquisitionResponse\x12j\n\x13InitiateAcquisition\x12(.niscope_grpc.InitiateAcquisitionRequest\x1a).niscope_grpc.InitiateAcquisitionResponse\x12@\n\x05\x41\x62ort\x12\x1a.niscope_grpc.AbortRequest\x1a\x1b.niscope_grpc.AbortResponse\x12\x43\n\x06\x43ommit\x12\x1b.niscope_grpc.CommitRequest\x1a\x1c.niscope_grpc.CommitResponse\x12=\n\x04Read\x12\x19.niscope_grpc.ReadRequest\x1a\x1a.niscope_grpc.ReadResponse\x12@\n\x05\x46\x65tch\x12\x1a.niscope_grpc.FetchRequest\x1a\x1b.niscope_grpc.FetchResponse\x12U\n\x0c\x46\x65tchBinary8\x12!.niscope_grpc.FetchBinary8Request\x1a\".niscope_grpc.FetchBinary8Response\x12X\n\rFetchBinary16\x12\".niscope_grpc.FetchBinary16Request\x1a#.niscope_grpc.FetchBinary16Response\x12X\n\rFetchBinary32\x12\".niscope_grpc.FetchBinary32Request\x1a#.niscope_grpc.FetchBinary32Response\x12U\n\x0c\x46\x65tchComplex\x12!.niscope_grpc.FetchComplexRequest\x1a\".niscope_grpc.FetchComplexResponse\x12m\n\x14\x46\x65tchComplexBinary16\x12).niscope_grpc.FetchComplexBinary16Request\x1a*.niscope_grpc.FetchComplexBinary16Response\x12\x64\n\x11\x41\x63quisitionStatus\x12&.niscope_grpc.AcquisitionStatusRequest\x1a\'.niscope_grpc.AcquisitionStatusResponse\x12X\n\rActualNumWfms\x12\".niscope_grpc.ActualNumWfmsRequest\x1a#.niscope_grpc.ActualNumWfmsResponse\x12\x64\n\x11\x41\x63tualMeasWfmSize\x12&.niscope_grpc.ActualMeasWfmSizeRequest\x1a\'.niscope_grpc.ActualMeasWfmSizeResponse\x12g\n\x12\x41\x63tualRecordLength\x12\'.niscope_grpc.ActualRecordLengthRequest\x1a(.niscope_grpc.ActualRecordLengthResponse\x12O\n\nSampleRate\x12\x1f.niscope_grpc.SampleRateRequest\x1a .niscope_grpc.SampleRateResponse\x12O\n\nSampleMode\x12\x1f.niscope_grpc.SampleModeRequest\x1a .niscope_grpc.SampleModeResponse\x12p\n\x15\x41\x64\x64WaveformProcessing\x12*.niscope_grpc.AddWaveformProcessingRequest\x1a+.niscope_grpc.AddWaveformProcessingResponse\x12v\n\x17\x43learWaveformProcessing\x12,.niscope_grpc.ClearWaveformProcessingRequest\x1a-.niscope_grpc.ClearWaveformProcessingResponse\x12\x88\x01\n\x1d\x43learWaveformMeasurementStats\x12\x32.niscope_grpc.ClearWaveformMeasurementStatsRequest\x1a\x33.niscope_grpc.ClearWaveformMeasurementStatsResponse\x12^\n\x0fReadMeasurement\x12$.niscope_grpc.ReadMeasurementRequest\x1a%.niscope_grpc.ReadMeasurementResponse\x12\x61\n\x10\x46\x65tchMeasurement\x12%.niscope_grpc.FetchMeasurementRequest\x1a&.niscope_grpc.FetchMeasurementResponse\x12p\n\x15\x46\x65tchMeasurementStats\x12*.niscope_grpc.FetchMeasurementStatsRequest\x1a+.niscope_grpc.FetchMeasurementStatsResponse\x12p\n\x15\x46\x65tchArrayMeasurement\x12*.niscope_grpc.FetchArrayMeasurementRequest\x1a+.niscope_grpc.FetchArrayMeasurementResponse\x12@\n\x05Reset\x12\x1a.niscope_grpc.ResetRequest\x1a\x1b.niscope_grpc.ResetResponse\x12I\n\x08SelfTest\x12\x1d.niscope_grpc.SelfTestRequest\x1a\x1e.niscope_grpc.SelfTestResponse\x12\x46\n\x07\x44isable\x12\x1c.niscope_grpc.DisableRequest\x1a\x1d.niscope_grpc.DisableResponse\x12R\n\x0bResetDevice\x12 .niscope_grpc.ResetDeviceRequest\x1a!.niscope_grpc.ResetDeviceResponse\x12\x61\n\x10\x43\x61lSelfCalibrate\x12%.niscope_grpc.CalSelfCalibrateRequest\x1a&.niscope_grpc.CalSelfCalibrateResponse\x12X\n\rRevisionQuery\x12\".niscope_grpc.RevisionQueryRequest\x1a#.niscope_grpc.RevisionQueryResponse\x12\x85\x01\n\x1cProbeCompensationSignalStart\x12\x31.niscope_grpc.ProbeCompensationSignalStartRequest\x1a\x32.niscope_grpc.ProbeCompensationSignalStartResponse\x12\x82\x01\n\x1bProbeCompensationSignalStop\x12\x30.niscope_grpc.ProbeCompensationSignalStopRequest\x1a\x31.niscope_grpc.ProbeCompensationSignalStopResponse\x12p\n\x15\x43\x61\x62leSenseSignalStart\x12*.niscope_grpc.CableSenseSignalStartRequest\x1a+.niscope_grpc.CableSenseSignalStartResponse\x12m\n\x14\x43\x61\x62leSenseSignalStop\x12).niscope_grpc.CableSenseSignalStopRequest\x1a*.niscope_grpc.CableSenseSignalStopResponse\x12[\n\x0eGetChannelName\x12#.niscope_grpc.GetChannelNameRequest\x1a$.niscope_grpc.GetChannelNameResponse\x12y\n\x18GetChannelNameFromString\x12-.niscope_grpc.GetChannelNameFromStringRequest\x1a..niscope_grpc.GetChannelNameFromStringResponse\x12U\n\x0c\x45rrorHandler\x12!.niscope_grpc.ErrorHandlerRequest\x1a\".niscope_grpc.ErrorHandlerResponse\x12I\n\x08GetError\x12\x1d.niscope_grpc.GetErrorRequest\x1a\x1e.niscope_grpc.GetErrorResponse\x12^\n\x0fGetErrorMessage\x12$.niscope_grpc.GetErrorMessageRequest\x1a%.niscope_grpc.GetErrorMessageResponse\x12j\n\x13GetAttributeViInt32\x12(.niscope_grpc.GetAttributeViInt32Request\x1a).niscope_grpc.GetAttributeViInt32Response\x12j\n\x13SetAttributeViInt32\x12(.niscope_grpc.SetAttributeViInt32Request\x1a).niscope_grpc.SetAttributeViInt32Response\x12p\n\x15\x43heckAttributeViInt32\x12*.niscope_grpc.CheckAttributeViInt32Request\x1a+.niscope_grpc.CheckAttributeViInt32Response\x12j\n\x13GetAttributeViInt64\x12(.niscope_grpc.GetAttributeViInt64Request\x1a).niscope_grpc.GetAttributeViInt64Response\x12j\n\x13SetAttributeViInt64\x12(.niscope_grpc.SetAttributeViInt64Request\x1a).niscope_grpc.SetAttributeViInt64Response\x12p\n\x15\x43heckAttributeViInt64\x12*.niscope_grpc.CheckAttributeViInt64Request\x1a+.niscope_grpc.CheckAttributeViInt64Response\x12m\n\x14GetAttributeViReal64\x12).niscope_grpc.GetAttributeViReal64Request\x1a*.niscope_grpc.GetAttributeViReal64Response\x12m\n\x14SetAttributeViReal64\x12).niscope_grpc.SetAttributeViReal64Request\x1a*.niscope_grpc.SetAttributeViReal64Response\x12s\n\x16\x43heckAttributeViReal64\x12+.niscope_grpc.CheckAttributeViReal64Request\x1a,.niscope_grpc.CheckAttributeViReal64Response\x12m\n\x14GetAttributeViString\x12).niscope_grpc.GetAttributeViStringRequest\x1a*.niscope_grpc.GetAttributeViStringResponse\x12m\n\x14SetAttributeViString\x12).niscope_grpc.SetAttributeViStringRequest\x1a*.niscope_grpc.SetAttributeViStringResponse\x12s\n\x16\x43heckAttributeViString\x12+.niscope_grpc.CheckAttributeViStringRequest\x1a,.niscope_grpc.CheckAttributeViStringResponse\x12p\n\x15GetAttributeViSession\x12*.niscope_grpc.GetAttributeViSessionRequest\x1a+.niscope_grpc.GetAttributeViSessionResponse\x12p\n\x15SetAttributeViSession\x12*.niscope_grpc.SetAttributeViSessionRequest\x1a+.niscope_grpc.SetAttributeViSessionResponse\x12v\n\x17\x43heckAttributeViSession\x12,.niscope_grpc.CheckAttributeViSessionRequest\x1a-.niscope_grpc.CheckAttributeViSessionResponse\x12p\n\x15GetAttributeViBoolean\x12*.niscope_grpc.GetAttributeViBooleanRequest\x1a+.niscope_grpc.GetAttributeViBooleanResponse\x12p\n\x15SetAttributeViBoolean\x12*.niscope_grpc.SetAttributeViBooleanRequest\x1a+.niscope_grpc.SetAttributeViBooleanResponse\x12v\n\x17\x43heckAttributeViBoolean\x12,.niscope_grpc.CheckAttributeViBooleanRequest\x1a-.niscope_grpc.CheckAttributeViBooleanResponse\x12\x97\x01\n\"ImportAttributeConfigurationBuffer\x12\x37.niscope_grpc.ImportAttributeConfigurationBufferRequest\x1a\x38.niscope_grpc.ImportAttributeConfigurationBufferResponse\x12\x97\x01\n\"ExportAttributeConfigurationBuffer\x12\x37.niscope_grpc.ExportAttributeConfigurationBufferRequest\x1a\x38.niscope_grpc.ExportAttributeConfigurationBufferResponse\x12\x91\x01\n ImportAttributeConfigurationFile\x12\x35.niscope_grpc.ImportAttributeConfigurationFileRequest\x1a\x36.niscope_grpc.ImportAttributeConfigurationFileResponse\x12\x91\x01\n ExportAttributeConfigurationFile\x12\x35.niscope_grpc.ExportAttributeConfigurationFileRequest\x1a\x36.niscope_grpc.ExportAttributeConfigurationFileResponse\x12s\n\x16GetScalingCoefficients\x12+.niscope_grpc.GetScalingCoefficientsRequest\x1a,.niscope_grpc.GetScalingCoefficientsResponse\x12\x85\x01\n\x1cGetNormalizationCoefficients\x12\x31.niscope_grpc.GetNormalizationCoefficientsRequest\x1a\x32.niscope_grpc.GetNormalizationCoefficientsResponse\x12v\n\x17GetStreamEndpointHandle\x12,.niscope_grpc.GetStreamEndpointHandleRequest\x1a-.niscope_grpc.GetStreamEndpointHandleResponse\x12U\n\x0c\x43\x61lFetchDate\x12!.niscope_grpc.CalFetchDateRequest\x1a\".niscope_grpc.CalFetchDateResponse\x12j\n\x13\x43\x61lFetchTemperature\x12(.niscope_grpc.CalFetchTemperatureRequest\x1a).niscope_grpc.CalFetchTemperatureResponseB?\n\x11\x63om.ni.grpc.scopeB\x07NiScopeP\x01\xaa\x02\x1eNationalInstruments.Grpc.Scopeb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'niscope_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'niscope_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021com.ni.grpc.scopeB\007NiScopeP\001\252\002\036NationalInstruments.Grpc.Scope'
   _NISCOPEINT32ATTRIBUTEVALUES._options = None
   _NISCOPEINT32ATTRIBUTEVALUES._serialized_options = b'\020\001'
   _NISCOPEREAL64ATTRIBUTEVALUES._options = None
   _NISCOPEREAL64ATTRIBUTEVALUES._serialized_options = b'\020\001'
   _INITRESPONSE.fields_by_name['error_message']._options = None
   _INITRESPONSE.fields_by_name['error_message']._serialized_options = b'\030\001'
   _INITWITHOPTIONSRESPONSE.fields_by_name['error_message']._options = None
   _INITWITHOPTIONSRESPONSE.fields_by_name['error_message']._serialized_options = b'\030\001'
-  _NISCOPEATTRIBUTE._serialized_start=21063
-  _NISCOPEATTRIBUTE._serialized_end=31527
-  _ACQUISITIONSTATUS._serialized_start=31530
-  _ACQUISITIONSTATUS._serialized_end=31714
-  _ARRAYMEASUREMENT._serialized_start=31717
-  _ARRAYMEASUREMENT._serialized_end=33209
-  _CALIBRATIONTYPES._serialized_start=33212
-  _CALIBRATIONTYPES._serialized_end=33373
-  _CLEARABLEMEASUREMENT._serialized_start=33376
-  _CLEARABLEMEASUREMENT._serialized_end=37267
-  _CLOCKINGTERMINALVALUES._serialized_start=37270
-  _CLOCKINGTERMINALVALUES._serialized_end=38188
-  _EXPORTABLESIGNALS._serialized_start=38191
-  _EXPORTABLESIGNALS._serialized_end=38825
-  _GLITCHCONDITION._serialized_start=38828
-  _GLITCHCONDITION._serialized_end=38984
-  _GLITCHPOLARITY._serialized_start=38987
-  _GLITCHPOLARITY._serialized_end=39181
-  _NISCOPEINT32ATTRIBUTEVALUES._serialized_start=39184
-  _NISCOPEINT32ATTRIBUTEVALUES._serialized_end=46013
-  _NISCOPEREAL64ATTRIBUTEVALUES._serialized_start=46016
-  _NISCOPEREAL64ATTRIBUTEVALUES._serialized_end=46217
-  _NISCOPEREAL64ATTRIBUTEVALUESMAPPED._serialized_start=46220
-  _NISCOPEREAL64ATTRIBUTEVALUESMAPPED._serialized_end=46831
-  _NISCOPESTRINGATTRIBUTEVALUESMAPPED._serialized_start=46834
-  _NISCOPESTRINGATTRIBUTEVALUESMAPPED._serialized_end=49040
-  _OPTION._serialized_start=49042
-  _OPTION._serialized_end=49155
-  _RUNTPOLARITY._serialized_start=49158
-  _RUNTPOLARITY._serialized_end=49336
-  _SCALARMEASUREMENT._serialized_start=49339
-  _SCALARMEASUREMENT._serialized_end=51338
-  _TRIGGERCOUPLING._serialized_start=51341
-  _TRIGGERCOUPLING._serialized_end=51573
-  _TRIGGERSLOPE._serialized_start=51576
-  _TRIGGERSLOPE._serialized_end=51714
-  _TRIGGERWINDOWMODE._serialized_start=51717
-  _TRIGGERWINDOWMODE._serialized_end=51905
-  _VERTICALCOUPLING._serialized_start=51908
-  _VERTICALCOUPLING._serialized_end=52041
-  _VIDEOPOLARITY._serialized_start=52044
-  _VIDEOPOLARITY._serialized_end=52179
-  _VIDEOSIGNALFORMAT._serialized_start=52182
-  _VIDEOSIGNALFORMAT._serialized_end=53334
-  _VIDEOTRIGGEREVENT._serialized_start=53337
-  _VIDEOTRIGGEREVENT._serialized_end=53668
-  _WHICHTRIGGER._serialized_start=53671
-  _WHICHTRIGGER._serialized_end=53915
-  _WIDTHCONDITION._serialized_start=53918
-  _WIDTHCONDITION._serialized_end=54060
-  _WIDTHPOLARITY._serialized_start=54063
-  _WIDTHPOLARITY._serialized_end=54249
-  _COEFFICIENTINFO._serialized_start=62
-  _COEFFICIENTINFO._serialized_end=147
-  _WAVEFORMINFO._serialized_start=150
-  _WAVEFORMINFO._serialized_end=333
-  _ABORTREQUEST._serialized_start=335
-  _ABORTREQUEST._serialized_end=385
-  _ABORTRESPONSE._serialized_start=387
-  _ABORTRESPONSE._serialized_end=418
-  _ACQUISITIONSTATUSREQUEST._serialized_start=420
-  _ACQUISITIONSTATUSREQUEST._serialized_end=482
-  _ACQUISITIONSTATUSRESPONSE._serialized_start=485
-  _ACQUISITIONSTATUSRESPONSE._serialized_end=621
-  _ACTUALMEASWFMSIZEREQUEST._serialized_start=624
-  _ACTUALMEASWFMSIZEREQUEST._serialized_end=812
-  _ACTUALMEASWFMSIZERESPONSE._serialized_start=814
-  _ACTUALMEASWFMSIZERESPONSE._serialized_end=885
-  _ACTUALNUMWFMSREQUEST._serialized_start=887
-  _ACTUALNUMWFMSREQUEST._serialized_end=967
-  _ACTUALNUMWFMSRESPONSE._serialized_start=969
-  _ACTUALNUMWFMSRESPONSE._serialized_end=1026
-  _ACTUALRECORDLENGTHREQUEST._serialized_start=1028
-  _ACTUALRECORDLENGTHREQUEST._serialized_end=1091
-  _ACTUALRECORDLENGTHRESPONSE._serialized_start=1093
-  _ACTUALRECORDLENGTHRESPONSE._serialized_end=1160
-  _ADDWAVEFORMPROCESSINGREQUEST._serialized_start=1163
-  _ADDWAVEFORMPROCESSINGREQUEST._serialized_end=1359
-  _ADDWAVEFORMPROCESSINGRESPONSE._serialized_start=1361
-  _ADDWAVEFORMPROCESSINGRESPONSE._serialized_end=1408
-  _ADJUSTSAMPLECLOCKRELATIVEDELAYREQUEST._serialized_start=1410
-  _ADJUSTSAMPLECLOCKRELATIVEDELAYREQUEST._serialized_end=1500
-  _ADJUSTSAMPLECLOCKRELATIVEDELAYRESPONSE._serialized_start=1502
-  _ADJUSTSAMPLECLOCKRELATIVEDELAYRESPONSE._serialized_end=1558
-  _AUTOSETUPREQUEST._serialized_start=1560
-  _AUTOSETUPREQUEST._serialized_end=1614
-  _AUTOSETUPRESPONSE._serialized_start=1616
-  _AUTOSETUPRESPONSE._serialized_end=1651
-  _CABLESENSESIGNALSTARTREQUEST._serialized_start=1653
-  _CABLESENSESIGNALSTARTREQUEST._serialized_end=1719
-  _CABLESENSESIGNALSTARTRESPONSE._serialized_start=1721
-  _CABLESENSESIGNALSTARTRESPONSE._serialized_end=1768
-  _CABLESENSESIGNALSTOPREQUEST._serialized_start=1770
-  _CABLESENSESIGNALSTOPREQUEST._serialized_end=1835
-  _CABLESENSESIGNALSTOPRESPONSE._serialized_start=1837
-  _CABLESENSESIGNALSTOPRESPONSE._serialized_end=1883
-  _CALFETCHDATEREQUEST._serialized_start=1886
-  _CALFETCHDATEREQUEST._serialized_end=2039
-  _CALFETCHDATERESPONSE._serialized_start=2041
-  _CALFETCHDATERESPONSE._serialized_end=2121
-  _CALFETCHTEMPERATUREREQUEST._serialized_start=2124
-  _CALFETCHTEMPERATUREREQUEST._serialized_end=2284
-  _CALFETCHTEMPERATURERESPONSE._serialized_start=2286
-  _CALFETCHTEMPERATURERESPONSE._serialized_end=2352
-  _CALSELFCALIBRATEREQUEST._serialized_start=2355
-  _CALSELFCALIBRATEREQUEST._serialized_end=2515
-  _CALSELFCALIBRATERESPONSE._serialized_start=2517
-  _CALSELFCALIBRATERESPONSE._serialized_end=2559
-  _CHECKATTRIBUTEVIBOOLEANREQUEST._serialized_start=2562
-  _CHECKATTRIBUTEVIBOOLEANREQUEST._serialized_end=2721
-  _CHECKATTRIBUTEVIBOOLEANRESPONSE._serialized_start=2723
-  _CHECKATTRIBUTEVIBOOLEANRESPONSE._serialized_end=2772
-  _CHECKATTRIBUTEVIINT32REQUEST._serialized_start=2775
-  _CHECKATTRIBUTEVIINT32REQUEST._serialized_end=3012
-  _CHECKATTRIBUTEVIINT32RESPONSE._serialized_start=3014
-  _CHECKATTRIBUTEVIINT32RESPONSE._serialized_end=3061
-  _CHECKATTRIBUTEVIINT64REQUEST._serialized_start=3064
-  _CHECKATTRIBUTEVIINT64REQUEST._serialized_end=3225
-  _CHECKATTRIBUTEVIINT64RESPONSE._serialized_start=3227
-  _CHECKATTRIBUTEVIINT64RESPONSE._serialized_end=3274
-  _CHECKATTRIBUTEVIREAL64REQUEST._serialized_start=3277
-  _CHECKATTRIBUTEVIREAL64REQUEST._serialized_end=3590
-  _CHECKATTRIBUTEVIREAL64RESPONSE._serialized_start=3592
-  _CHECKATTRIBUTEVIREAL64RESPONSE._serialized_end=3640
-  _CHECKATTRIBUTEVISESSIONREQUEST._serialized_start=3643
-  _CHECKATTRIBUTEVISESSIONREQUEST._serialized_end=3826
-  _CHECKATTRIBUTEVISESSIONRESPONSE._serialized_start=3828
-  _CHECKATTRIBUTEVISESSIONRESPONSE._serialized_end=3877
-  _CHECKATTRIBUTEVISTRINGREQUEST._serialized_start=3880
-  _CHECKATTRIBUTEVISTRINGREQUEST._serialized_end=4132
-  _CHECKATTRIBUTEVISTRINGRESPONSE._serialized_start=4134
-  _CHECKATTRIBUTEVISTRINGRESPONSE._serialized_end=4182
-  _CLEARWAVEFORMMEASUREMENTSTATSREQUEST._serialized_start=4185
-  _CLEARWAVEFORMMEASUREMENTSTATSREQUEST._serialized_end=4444
-  _CLEARWAVEFORMMEASUREMENTSTATSRESPONSE._serialized_start=4446
-  _CLEARWAVEFORMMEASUREMENTSTATSRESPONSE._serialized_end=4501
-  _CLEARWAVEFORMPROCESSINGREQUEST._serialized_start=4503
-  _CLEARWAVEFORMPROCESSINGREQUEST._serialized_end=4593
-  _CLEARWAVEFORMPROCESSINGRESPONSE._serialized_start=4595
-  _CLEARWAVEFORMPROCESSINGRESPONSE._serialized_end=4644
-  _CLOSEREQUEST._serialized_start=4646
-  _CLOSEREQUEST._serialized_end=4696
-  _CLOSERESPONSE._serialized_start=4698
-  _CLOSERESPONSE._serialized_end=4729
-  _COMMITREQUEST._serialized_start=4731
-  _COMMITREQUEST._serialized_end=4782
-  _COMMITRESPONSE._serialized_start=4784
-  _COMMITRESPONSE._serialized_end=4816
-  _CONFIGUREACQUISITIONREQUEST._serialized_start=4818
-  _CONFIGUREACQUISITIONREQUEST._serialized_end=4909
-  _CONFIGUREACQUISITIONRESPONSE._serialized_start=4911
-  _CONFIGUREACQUISITIONRESPONSE._serialized_end=4957
-  _CONFIGURECHANCHARACTERISTICSREQUEST._serialized_start=4960
-  _CONFIGURECHANCHARACTERISTICSREQUEST._serialized_end=5109
-  _CONFIGURECHANCHARACTERISTICSRESPONSE._serialized_start=5111
-  _CONFIGURECHANCHARACTERISTICSRESPONSE._serialized_end=5165
-  _CONFIGURECLOCKREQUEST._serialized_start=5168
-  _CONFIGURECLOCKREQUEST._serialized_end=5677
-  _CONFIGURECLOCKRESPONSE._serialized_start=5679
-  _CONFIGURECLOCKRESPONSE._serialized_end=5719
-  _CONFIGUREEQUALIZATIONFILTERCOEFFICIENTSREQUEST._serialized_start=5722
-  _CONFIGUREEQUALIZATIONFILTERCOEFFICIENTSREQUEST._serialized_end=5850
-  _CONFIGUREEQUALIZATIONFILTERCOEFFICIENTSRESPONSE._serialized_start=5852
-  _CONFIGUREEQUALIZATIONFILTERCOEFFICIENTSRESPONSE._serialized_end=5917
-  _CONFIGUREHORIZONTALTIMINGREQUEST._serialized_start=5920
-  _CONFIGUREHORIZONTALTIMINGREQUEST._serialized_end=6105
-  _CONFIGUREHORIZONTALTIMINGRESPONSE._serialized_start=6107
-  _CONFIGUREHORIZONTALTIMINGRESPONSE._serialized_end=6158
-  _CONFIGURETRIGGERDIGITALREQUEST._serialized_start=6161
-  _CONFIGURETRIGGERDIGITALREQUEST._serialized_end=6365
-  _CONFIGURETRIGGERDIGITALRESPONSE._serialized_start=6367
-  _CONFIGURETRIGGERDIGITALRESPONSE._serialized_end=6416
-  _CONFIGURETRIGGEREDGEREQUEST._serialized_start=6419
-  _CONFIGURETRIGGEREDGEREQUEST._serialized_end=6751
-  _CONFIGURETRIGGEREDGERESPONSE._serialized_start=6753
-  _CONFIGURETRIGGEREDGERESPONSE._serialized_end=6799
-  _CONFIGURETRIGGERGLITCHREQUEST._serialized_start=6802
-  _CONFIGURETRIGGERGLITCHREQUEST._serialized_end=7278
-  _CONFIGURETRIGGERGLITCHRESPONSE._serialized_start=7280
-  _CONFIGURETRIGGERGLITCHRESPONSE._serialized_end=7328
-  _CONFIGURETRIGGERHYSTERESISREQUEST._serialized_start=7331
-  _CONFIGURETRIGGERHYSTERESISREQUEST._serialized_end=7689
-  _CONFIGURETRIGGERHYSTERESISRESPONSE._serialized_start=7691
-  _CONFIGURETRIGGERHYSTERESISRESPONSE._serialized_end=7743
-  _CONFIGURETRIGGERIMMEDIATEREQUEST._serialized_start=7745
-  _CONFIGURETRIGGERIMMEDIATEREQUEST._serialized_end=7815
-  _CONFIGURETRIGGERIMMEDIATERESPONSE._serialized_start=7817
-  _CONFIGURETRIGGERIMMEDIATERESPONSE._serialized_end=7868
-  _CONFIGURETRIGGERRUNTREQUEST._serialized_start=7871
-  _CONFIGURETRIGGERRUNTREQUEST._serialized_end=8244
-  _CONFIGURETRIGGERRUNTRESPONSE._serialized_start=8246
-  _CONFIGURETRIGGERRUNTRESPONSE._serialized_end=8292
-  _CONFIGURETRIGGERSOFTWAREREQUEST._serialized_start=8294
-  _CONFIGURETRIGGERSOFTWAREREQUEST._serialized_end=8395
-  _CONFIGURETRIGGERSOFTWARERESPONSE._serialized_start=8397
-  _CONFIGURETRIGGERSOFTWARERESPONSE._serialized_end=8447
-  _CONFIGURETRIGGERVIDEOREQUEST._serialized_start=8450
-  _CONFIGURETRIGGERVIDEOREQUEST._serialized_end=9020
-  _CONFIGURETRIGGERVIDEORESPONSE._serialized_start=9022
-  _CONFIGURETRIGGERVIDEORESPONSE._serialized_end=9069
-  _CONFIGURETRIGGERWIDTHREQUEST._serialized_start=9072
-  _CONFIGURETRIGGERWIDTHREQUEST._serialized_end=9556
-  _CONFIGURETRIGGERWIDTHRESPONSE._serialized_start=9558
-  _CONFIGURETRIGGERWIDTHRESPONSE._serialized_end=9605
-  _CONFIGURETRIGGERWINDOWREQUEST._serialized_start=9608
-  _CONFIGURETRIGGERWINDOWREQUEST._serialized_end=9989
-  _CONFIGURETRIGGERWINDOWRESPONSE._serialized_start=9991
-  _CONFIGURETRIGGERWINDOWRESPONSE._serialized_end=10039
-  _CONFIGUREVERTICALREQUEST._serialized_start=10042
-  _CONFIGUREVERTICALREQUEST._serialized_end=10294
-  _CONFIGUREVERTICALRESPONSE._serialized_start=10296
-  _CONFIGUREVERTICALRESPONSE._serialized_end=10339
-  _DISABLEREQUEST._serialized_start=10341
-  _DISABLEREQUEST._serialized_end=10393
-  _DISABLERESPONSE._serialized_start=10395
-  _DISABLERESPONSE._serialized_end=10428
-  _ERRORHANDLERREQUEST._serialized_start=10430
-  _ERRORHANDLERREQUEST._serialized_end=10529
-  _ERRORHANDLERRESPONSE._serialized_start=10531
-  _ERRORHANDLERRESPONSE._serialized_end=10596
-  _EXPORTATTRIBUTECONFIGURATIONBUFFERREQUEST._serialized_start=10598
-  _EXPORTATTRIBUTECONFIGURATIONBUFFERREQUEST._serialized_end=10677
-  _EXPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE._serialized_start=10679
-  _EXPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE._serialized_end=10762
-  _EXPORTATTRIBUTECONFIGURATIONFILEREQUEST._serialized_start=10764
-  _EXPORTATTRIBUTECONFIGURATIONFILEREQUEST._serialized_end=10860
-  _EXPORTATTRIBUTECONFIGURATIONFILERESPONSE._serialized_start=10862
-  _EXPORTATTRIBUTECONFIGURATIONFILERESPONSE._serialized_end=10920
-  _EXPORTSIGNALREQUEST._serialized_start=10923
-  _EXPORTSIGNALREQUEST._serialized_end=11222
-  _EXPORTSIGNALRESPONSE._serialized_start=11224
-  _EXPORTSIGNALRESPONSE._serialized_end=11262
-  _FETCHREQUEST._serialized_start=11264
-  _FETCHREQUEST._serialized_end=11374
-  _FETCHRESPONSE._serialized_start=11376
-  _FETCHRESPONSE._serialized_end=11471
-  _FETCHARRAYMEASUREMENTREQUEST._serialized_start=11474
-  _FETCHARRAYMEASUREMENTREQUEST._serialized_end=11751
-  _FETCHARRAYMEASUREMENTRESPONSE._serialized_start=11753
-  _FETCHARRAYMEASUREMENTRESPONSE._serialized_end=11864
-  _FETCHBINARY16REQUEST._serialized_start=11866
-  _FETCHBINARY16REQUEST._serialized_end=11984
-  _FETCHBINARY16RESPONSE._serialized_start=11986
-  _FETCHBINARY16RESPONSE._serialized_end=12089
-  _FETCHBINARY32REQUEST._serialized_start=12091
-  _FETCHBINARY32REQUEST._serialized_end=12209
-  _FETCHBINARY32RESPONSE._serialized_start=12211
-  _FETCHBINARY32RESPONSE._serialized_end=12314
-  _FETCHBINARY8REQUEST._serialized_start=12316
-  _FETCHBINARY8REQUEST._serialized_end=12433
-  _FETCHBINARY8RESPONSE._serialized_start=12435
-  _FETCHBINARY8RESPONSE._serialized_end=12537
-  _FETCHCOMPLEXREQUEST._serialized_start=12539
-  _FETCHCOMPLEXREQUEST._serialized_end=12656
-  _FETCHCOMPLEXRESPONSE._serialized_start=12659
-  _FETCHCOMPLEXRESPONSE._serialized_end=12788
-  _FETCHCOMPLEXBINARY16REQUEST._serialized_start=12790
-  _FETCHCOMPLEXBINARY16REQUEST._serialized_end=12915
-  _FETCHCOMPLEXBINARY16RESPONSE._serialized_start=12918
-  _FETCHCOMPLEXBINARY16RESPONSE._serialized_end=13052
-  _FETCHMEASUREMENTREQUEST._serialized_start=13055
-  _FETCHMEASUREMENTREQUEST._serialized_end=13285
-  _FETCHMEASUREMENTRESPONSE._serialized_start=13287
-  _FETCHMEASUREMENTRESPONSE._serialized_end=13345
-  _FETCHMEASUREMENTSTATSREQUEST._serialized_start=13348
-  _FETCHMEASUREMENTSTATSREQUEST._serialized_end=13583
-  _FETCHMEASUREMENTSTATSRESPONSE._serialized_start=13586
-  _FETCHMEASUREMENTSTATSRESPONSE._serialized_end=13726
-  _GETATTRIBUTEVIBOOLEANREQUEST._serialized_start=13729
-  _GETATTRIBUTEVIBOOLEANREQUEST._serialized_end=13871
-  _GETATTRIBUTEVIBOOLEANRESPONSE._serialized_start=13873
-  _GETATTRIBUTEVIBOOLEANRESPONSE._serialized_end=13935
-  _GETATTRIBUTEVIINT32REQUEST._serialized_start=13938
-  _GETATTRIBUTEVIINT32REQUEST._serialized_end=14078
-  _GETATTRIBUTEVIINT32RESPONSE._serialized_start=14080
-  _GETATTRIBUTEVIINT32RESPONSE._serialized_end=14140
-  _GETATTRIBUTEVIINT64REQUEST._serialized_start=14143
-  _GETATTRIBUTEVIINT64REQUEST._serialized_end=14283
-  _GETATTRIBUTEVIINT64RESPONSE._serialized_start=14285
-  _GETATTRIBUTEVIINT64RESPONSE._serialized_end=14345
-  _GETATTRIBUTEVIREAL64REQUEST._serialized_start=14348
-  _GETATTRIBUTEVIREAL64REQUEST._serialized_end=14489
-  _GETATTRIBUTEVIREAL64RESPONSE._serialized_start=14491
-  _GETATTRIBUTEVIREAL64RESPONSE._serialized_end=14552
-  _GETATTRIBUTEVISESSIONREQUEST._serialized_start=14555
-  _GETATTRIBUTEVISESSIONREQUEST._serialized_end=14697
-  _GETATTRIBUTEVISESSIONRESPONSE._serialized_start=14699
-  _GETATTRIBUTEVISESSIONRESPONSE._serialized_end=14785
-  _GETATTRIBUTEVISTRINGREQUEST._serialized_start=14788
-  _GETATTRIBUTEVISTRINGREQUEST._serialized_end=14929
-  _GETATTRIBUTEVISTRINGRESPONSE._serialized_start=14931
-  _GETATTRIBUTEVISTRINGRESPONSE._serialized_end=14992
-  _GETCHANNELNAMEREQUEST._serialized_start=14994
-  _GETCHANNELNAMEREQUEST._serialized_end=15068
-  _GETCHANNELNAMERESPONSE._serialized_start=15070
-  _GETCHANNELNAMERESPONSE._serialized_end=15134
-  _GETCHANNELNAMEFROMSTRINGREQUEST._serialized_start=15136
-  _GETCHANNELNAMEFROMSTRINGREQUEST._serialized_end=15220
-  _GETCHANNELNAMEFROMSTRINGRESPONSE._serialized_start=15222
-  _GETCHANNELNAMEFROMSTRINGRESPONSE._serialized_end=15286
-  _GETEQUALIZATIONFILTERCOEFFICIENTSREQUEST._serialized_start=15288
-  _GETEQUALIZATIONFILTERCOEFFICIENTSREQUEST._serialized_end=15415
-  _GETEQUALIZATIONFILTERCOEFFICIENTSRESPONSE._serialized_start=15417
-  _GETEQUALIZATIONFILTERCOEFFICIENTSRESPONSE._serialized_end=15498
-  _GETERRORREQUEST._serialized_start=15500
-  _GETERRORREQUEST._serialized_end=15553
-  _GETERRORRESPONSE._serialized_start=15555
-  _GETERRORRESPONSE._serialized_end=15630
-  _GETERRORMESSAGEREQUEST._serialized_start=15632
-  _GETERRORMESSAGEREQUEST._serialized_end=15712
-  _GETERRORMESSAGERESPONSE._serialized_start=15714
-  _GETERRORMESSAGERESPONSE._serialized_end=15778
-  _GETFREQUENCYRESPONSEREQUEST._serialized_start=15780
-  _GETFREQUENCYRESPONSEREQUEST._serialized_end=15883
-  _GETFREQUENCYRESPONSERESPONSE._serialized_start=15886
-  _GETFREQUENCYRESPONSERESPONSE._serialized_end=16020
-  _GETNORMALIZATIONCOEFFICIENTSREQUEST._serialized_start=16022
-  _GETNORMALIZATIONCOEFFICIENTSREQUEST._serialized_end=16117
-  _GETNORMALIZATIONCOEFFICIENTSRESPONSE._serialized_start=16120
-  _GETNORMALIZATIONCOEFFICIENTSRESPONSE._serialized_end=16267
-  _GETSCALINGCOEFFICIENTSREQUEST._serialized_start=16269
-  _GETSCALINGCOEFFICIENTSREQUEST._serialized_end=16358
-  _GETSCALINGCOEFFICIENTSRESPONSE._serialized_start=16361
-  _GETSCALINGCOEFFICIENTSRESPONSE._serialized_end=16502
-  _GETSTREAMENDPOINTHANDLEREQUEST._serialized_start=16504
-  _GETSTREAMENDPOINTHANDLEREQUEST._serialized_end=16593
-  _GETSTREAMENDPOINTHANDLERESPONSE._serialized_start=16595
-  _GETSTREAMENDPOINTHANDLERESPONSE._serialized_end=16667
-  _IMPORTATTRIBUTECONFIGURATIONBUFFERREQUEST._serialized_start=16669
-  _IMPORTATTRIBUTECONFIGURATIONBUFFERREQUEST._serialized_end=16771
-  _IMPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE._serialized_start=16773
-  _IMPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE._serialized_end=16833
-  _IMPORTATTRIBUTECONFIGURATIONFILEREQUEST._serialized_start=16835
-  _IMPORTATTRIBUTECONFIGURATIONFILEREQUEST._serialized_end=16931
-  _IMPORTATTRIBUTECONFIGURATIONFILERESPONSE._serialized_start=16933
-  _IMPORTATTRIBUTECONFIGURATIONFILERESPONSE._serialized_end=16991
-  _INITREQUEST._serialized_start=16994
-  _INITREQUEST._serialized_end=17171
-  _INITRESPONSE._serialized_start=17173
-  _INITRESPONSE._serialized_end=17299
-  _INITWITHOPTIONSREQUEST._serialized_start=17302
-  _INITWITHOPTIONSREQUEST._serialized_end=17513
-  _INITWITHOPTIONSRESPONSE._serialized_start=17516
-  _INITWITHOPTIONSRESPONSE._serialized_end=17653
-  _INITIATEACQUISITIONREQUEST._serialized_start=17655
-  _INITIATEACQUISITIONREQUEST._serialized_end=17719
-  _INITIATEACQUISITIONRESPONSE._serialized_start=17721
-  _INITIATEACQUISITIONRESPONSE._serialized_end=17766
-  _PROBECOMPENSATIONSIGNALSTARTREQUEST._serialized_start=17768
-  _PROBECOMPENSATIONSIGNALSTARTREQUEST._serialized_end=17841
-  _PROBECOMPENSATIONSIGNALSTARTRESPONSE._serialized_start=17843
-  _PROBECOMPENSATIONSIGNALSTARTRESPONSE._serialized_end=17897
-  _PROBECOMPENSATIONSIGNALSTOPREQUEST._serialized_start=17899
-  _PROBECOMPENSATIONSIGNALSTOPREQUEST._serialized_end=17971
-  _PROBECOMPENSATIONSIGNALSTOPRESPONSE._serialized_start=17973
-  _PROBECOMPENSATIONSIGNALSTOPRESPONSE._serialized_end=18026
-  _READREQUEST._serialized_start=18028
-  _READREQUEST._serialized_end=18137
-  _READRESPONSE._serialized_start=18139
-  _READRESPONSE._serialized_end=18233
-  _READMEASUREMENTREQUEST._serialized_start=18236
-  _READMEASUREMENTREQUEST._serialized_end=18465
-  _READMEASUREMENTRESPONSE._serialized_start=18467
-  _READMEASUREMENTRESPONSE._serialized_end=18524
-  _RESETREQUEST._serialized_start=18526
-  _RESETREQUEST._serialized_end=18576
-  _RESETRESPONSE._serialized_start=18578
-  _RESETRESPONSE._serialized_end=18609
-  _RESETDEVICEREQUEST._serialized_start=18611
-  _RESETDEVICEREQUEST._serialized_end=18667
-  _RESETDEVICERESPONSE._serialized_start=18669
-  _RESETDEVICERESPONSE._serialized_end=18706
-  _REVISIONQUERYREQUEST._serialized_start=18708
-  _REVISIONQUERYREQUEST._serialized_end=18766
-  _REVISIONQUERYRESPONSE._serialized_start=18768
-  _REVISIONQUERYRESPONSE._serialized_end=18859
-  _SAMPLEMODEREQUEST._serialized_start=18861
-  _SAMPLEMODEREQUEST._serialized_end=18916
-  _SAMPLEMODERESPONSE._serialized_start=18918
-  _SAMPLEMODERESPONSE._serialized_end=18975
-  _SAMPLERATEREQUEST._serialized_start=18977
-  _SAMPLERATEREQUEST._serialized_end=19032
-  _SAMPLERATERESPONSE._serialized_start=19034
-  _SAMPLERATERESPONSE._serialized_end=19091
-  _SELFTESTREQUEST._serialized_start=19093
-  _SELFTESTREQUEST._serialized_end=19146
-  _SELFTESTRESPONSE._serialized_start=19148
-  _SELFTESTRESPONSE._serialized_end=19235
-  _SENDSOFTWARETRIGGEREDGEREQUEST._serialized_start=19238
-  _SENDSOFTWARETRIGGEREDGEREQUEST._serialized_end=19410
-  _SENDSOFTWARETRIGGEREDGERESPONSE._serialized_start=19412
-  _SENDSOFTWARETRIGGEREDGERESPONSE._serialized_end=19461
-  _SETATTRIBUTEVIBOOLEANREQUEST._serialized_start=19464
-  _SETATTRIBUTEVIBOOLEANREQUEST._serialized_end=19621
-  _SETATTRIBUTEVIBOOLEANRESPONSE._serialized_start=19623
-  _SETATTRIBUTEVIBOOLEANRESPONSE._serialized_end=19670
-  _SETATTRIBUTEVIINT32REQUEST._serialized_start=19673
-  _SETATTRIBUTEVIINT32REQUEST._serialized_end=19908
-  _SETATTRIBUTEVIINT32RESPONSE._serialized_start=19910
-  _SETATTRIBUTEVIINT32RESPONSE._serialized_end=19955
-  _SETATTRIBUTEVIINT64REQUEST._serialized_start=19958
-  _SETATTRIBUTEVIINT64REQUEST._serialized_end=20117
-  _SETATTRIBUTEVIINT64RESPONSE._serialized_start=20119
-  _SETATTRIBUTEVIINT64RESPONSE._serialized_end=20164
-  _SETATTRIBUTEVIREAL64REQUEST._serialized_start=20167
-  _SETATTRIBUTEVIREAL64REQUEST._serialized_end=20478
-  _SETATTRIBUTEVIREAL64RESPONSE._serialized_start=20480
-  _SETATTRIBUTEVIREAL64RESPONSE._serialized_end=20526
-  _SETATTRIBUTEVISESSIONREQUEST._serialized_start=20529
-  _SETATTRIBUTEVISESSIONREQUEST._serialized_end=20710
-  _SETATTRIBUTEVISESSIONRESPONSE._serialized_start=20712
-  _SETATTRIBUTEVISESSIONRESPONSE._serialized_end=20759
-  _SETATTRIBUTEVISTRINGREQUEST._serialized_start=20762
-  _SETATTRIBUTEVISTRINGREQUEST._serialized_end=21012
-  _SETATTRIBUTEVISTRINGRESPONSE._serialized_start=21014
-  _SETATTRIBUTEVISTRINGRESPONSE._serialized_end=21060
-  _NISCOPE._serialized_start=54252
-  _NISCOPE._serialized_end=63948
+  _globals['_NISCOPEATTRIBUTE']._serialized_start=21063
+  _globals['_NISCOPEATTRIBUTE']._serialized_end=31527
+  _globals['_WHICHTRIGGER']._serialized_start=31530
+  _globals['_WHICHTRIGGER']._serialized_end=31774
+  _globals['_VERTICALCOUPLING']._serialized_start=31777
+  _globals['_VERTICALCOUPLING']._serialized_end=31910
+  _globals['_TRIGGERCOUPLING']._serialized_start=31913
+  _globals['_TRIGGERCOUPLING']._serialized_end=32145
+  _globals['_TRIGGERSLOPE']._serialized_start=32148
+  _globals['_TRIGGERSLOPE']._serialized_end=32286
+  _globals['_VIDEOPOLARITY']._serialized_start=32289
+  _globals['_VIDEOPOLARITY']._serialized_end=32424
+  _globals['_VIDEOTRIGGEREVENT']._serialized_start=32427
+  _globals['_VIDEOTRIGGEREVENT']._serialized_end=32758
+  _globals['_GLITCHCONDITION']._serialized_start=32761
+  _globals['_GLITCHCONDITION']._serialized_end=32917
+  _globals['_GLITCHPOLARITY']._serialized_start=32920
+  _globals['_GLITCHPOLARITY']._serialized_end=33114
+  _globals['_WIDTHCONDITION']._serialized_start=33117
+  _globals['_WIDTHCONDITION']._serialized_end=33259
+  _globals['_WIDTHPOLARITY']._serialized_start=33262
+  _globals['_WIDTHPOLARITY']._serialized_end=33448
+  _globals['_RUNTPOLARITY']._serialized_start=33451
+  _globals['_RUNTPOLARITY']._serialized_end=33629
+  _globals['_CLOCKINGTERMINALVALUES']._serialized_start=33632
+  _globals['_CLOCKINGTERMINALVALUES']._serialized_end=34550
+  _globals['_EXPORTABLESIGNALS']._serialized_start=34553
+  _globals['_EXPORTABLESIGNALS']._serialized_end=35187
+  _globals['_TRIGGERWINDOWMODE']._serialized_start=35190
+  _globals['_TRIGGERWINDOWMODE']._serialized_end=35378
+  _globals['_ACQUISITIONSTATUS']._serialized_start=35381
+  _globals['_ACQUISITIONSTATUS']._serialized_end=35565
+  _globals['_SCALARMEASUREMENT']._serialized_start=35568
+  _globals['_SCALARMEASUREMENT']._serialized_end=37567
+  _globals['_ARRAYMEASUREMENT']._serialized_start=37570
+  _globals['_ARRAYMEASUREMENT']._serialized_end=39062
+  _globals['_CALIBRATIONTYPES']._serialized_start=39065
+  _globals['_CALIBRATIONTYPES']._serialized_end=39226
+  _globals['_CLEARABLEMEASUREMENT']._serialized_start=39229
+  _globals['_CLEARABLEMEASUREMENT']._serialized_end=43120
+  _globals['_OPTION']._serialized_start=43122
+  _globals['_OPTION']._serialized_end=43235
+  _globals['_VIDEOSIGNALFORMAT']._serialized_start=43238
+  _globals['_VIDEOSIGNALFORMAT']._serialized_end=44390
+  _globals['_NISCOPEINT32ATTRIBUTEVALUES']._serialized_start=44393
+  _globals['_NISCOPEINT32ATTRIBUTEVALUES']._serialized_end=51222
+  _globals['_NISCOPEREAL64ATTRIBUTEVALUES']._serialized_start=51225
+  _globals['_NISCOPEREAL64ATTRIBUTEVALUES']._serialized_end=51426
+  _globals['_NISCOPEREAL64ATTRIBUTEVALUESMAPPED']._serialized_start=51429
+  _globals['_NISCOPEREAL64ATTRIBUTEVALUESMAPPED']._serialized_end=52040
+  _globals['_NISCOPESTRINGATTRIBUTEVALUESMAPPED']._serialized_start=52043
+  _globals['_NISCOPESTRINGATTRIBUTEVALUESMAPPED']._serialized_end=54249
+  _globals['_WAVEFORMINFO']._serialized_start=63
+  _globals['_WAVEFORMINFO']._serialized_end=246
+  _globals['_COEFFICIENTINFO']._serialized_start=248
+  _globals['_COEFFICIENTINFO']._serialized_end=333
+  _globals['_INITREQUEST']._serialized_start=336
+  _globals['_INITREQUEST']._serialized_end=513
+  _globals['_INITRESPONSE']._serialized_start=515
+  _globals['_INITRESPONSE']._serialized_end=641
+  _globals['_INITWITHOPTIONSREQUEST']._serialized_start=644
+  _globals['_INITWITHOPTIONSREQUEST']._serialized_end=855
+  _globals['_INITWITHOPTIONSRESPONSE']._serialized_start=858
+  _globals['_INITWITHOPTIONSRESPONSE']._serialized_end=995
+  _globals['_CLOSEREQUEST']._serialized_start=997
+  _globals['_CLOSEREQUEST']._serialized_end=1047
+  _globals['_CLOSERESPONSE']._serialized_start=1049
+  _globals['_CLOSERESPONSE']._serialized_end=1080
+  _globals['_AUTOSETUPREQUEST']._serialized_start=1082
+  _globals['_AUTOSETUPREQUEST']._serialized_end=1136
+  _globals['_AUTOSETUPRESPONSE']._serialized_start=1138
+  _globals['_AUTOSETUPRESPONSE']._serialized_end=1173
+  _globals['_CONFIGUREVERTICALREQUEST']._serialized_start=1176
+  _globals['_CONFIGUREVERTICALREQUEST']._serialized_end=1428
+  _globals['_CONFIGUREVERTICALRESPONSE']._serialized_start=1430
+  _globals['_CONFIGUREVERTICALRESPONSE']._serialized_end=1473
+  _globals['_CONFIGURECHANCHARACTERISTICSREQUEST']._serialized_start=1476
+  _globals['_CONFIGURECHANCHARACTERISTICSREQUEST']._serialized_end=1625
+  _globals['_CONFIGURECHANCHARACTERISTICSRESPONSE']._serialized_start=1627
+  _globals['_CONFIGURECHANCHARACTERISTICSRESPONSE']._serialized_end=1681
+  _globals['_CONFIGUREHORIZONTALTIMINGREQUEST']._serialized_start=1684
+  _globals['_CONFIGUREHORIZONTALTIMINGREQUEST']._serialized_end=1869
+  _globals['_CONFIGUREHORIZONTALTIMINGRESPONSE']._serialized_start=1871
+  _globals['_CONFIGUREHORIZONTALTIMINGRESPONSE']._serialized_end=1922
+  _globals['_CONFIGURECLOCKREQUEST']._serialized_start=1925
+  _globals['_CONFIGURECLOCKREQUEST']._serialized_end=2434
+  _globals['_CONFIGURECLOCKRESPONSE']._serialized_start=2436
+  _globals['_CONFIGURECLOCKRESPONSE']._serialized_end=2476
+  _globals['_EXPORTSIGNALREQUEST']._serialized_start=2479
+  _globals['_EXPORTSIGNALREQUEST']._serialized_end=2778
+  _globals['_EXPORTSIGNALRESPONSE']._serialized_start=2780
+  _globals['_EXPORTSIGNALRESPONSE']._serialized_end=2818
+  _globals['_ADJUSTSAMPLECLOCKRELATIVEDELAYREQUEST']._serialized_start=2820
+  _globals['_ADJUSTSAMPLECLOCKRELATIVEDELAYREQUEST']._serialized_end=2910
+  _globals['_ADJUSTSAMPLECLOCKRELATIVEDELAYRESPONSE']._serialized_start=2912
+  _globals['_ADJUSTSAMPLECLOCKRELATIVEDELAYRESPONSE']._serialized_end=2968
+  _globals['_CONFIGURETRIGGEREDGEREQUEST']._serialized_start=2971
+  _globals['_CONFIGURETRIGGEREDGEREQUEST']._serialized_end=3303
+  _globals['_CONFIGURETRIGGEREDGERESPONSE']._serialized_start=3305
+  _globals['_CONFIGURETRIGGEREDGERESPONSE']._serialized_end=3351
+  _globals['_CONFIGURETRIGGERGLITCHREQUEST']._serialized_start=3354
+  _globals['_CONFIGURETRIGGERGLITCHREQUEST']._serialized_end=3830
+  _globals['_CONFIGURETRIGGERGLITCHRESPONSE']._serialized_start=3832
+  _globals['_CONFIGURETRIGGERGLITCHRESPONSE']._serialized_end=3880
+  _globals['_CONFIGURETRIGGERHYSTERESISREQUEST']._serialized_start=3883
+  _globals['_CONFIGURETRIGGERHYSTERESISREQUEST']._serialized_end=4241
+  _globals['_CONFIGURETRIGGERHYSTERESISRESPONSE']._serialized_start=4243
+  _globals['_CONFIGURETRIGGERHYSTERESISRESPONSE']._serialized_end=4295
+  _globals['_CONFIGURETRIGGERWINDOWREQUEST']._serialized_start=4298
+  _globals['_CONFIGURETRIGGERWINDOWREQUEST']._serialized_end=4679
+  _globals['_CONFIGURETRIGGERWINDOWRESPONSE']._serialized_start=4681
+  _globals['_CONFIGURETRIGGERWINDOWRESPONSE']._serialized_end=4729
+  _globals['_CONFIGURETRIGGERSOFTWAREREQUEST']._serialized_start=4731
+  _globals['_CONFIGURETRIGGERSOFTWAREREQUEST']._serialized_end=4832
+  _globals['_CONFIGURETRIGGERSOFTWARERESPONSE']._serialized_start=4834
+  _globals['_CONFIGURETRIGGERSOFTWARERESPONSE']._serialized_end=4884
+  _globals['_SENDSOFTWARETRIGGEREDGEREQUEST']._serialized_start=4887
+  _globals['_SENDSOFTWARETRIGGEREDGEREQUEST']._serialized_end=5059
+  _globals['_SENDSOFTWARETRIGGEREDGERESPONSE']._serialized_start=5061
+  _globals['_SENDSOFTWARETRIGGEREDGERESPONSE']._serialized_end=5110
+  _globals['_CONFIGURETRIGGERIMMEDIATEREQUEST']._serialized_start=5112
+  _globals['_CONFIGURETRIGGERIMMEDIATEREQUEST']._serialized_end=5182
+  _globals['_CONFIGURETRIGGERIMMEDIATERESPONSE']._serialized_start=5184
+  _globals['_CONFIGURETRIGGERIMMEDIATERESPONSE']._serialized_end=5235
+  _globals['_CONFIGURETRIGGERRUNTREQUEST']._serialized_start=5238
+  _globals['_CONFIGURETRIGGERRUNTREQUEST']._serialized_end=5611
+  _globals['_CONFIGURETRIGGERRUNTRESPONSE']._serialized_start=5613
+  _globals['_CONFIGURETRIGGERRUNTRESPONSE']._serialized_end=5659
+  _globals['_CONFIGURETRIGGERDIGITALREQUEST']._serialized_start=5662
+  _globals['_CONFIGURETRIGGERDIGITALREQUEST']._serialized_end=5866
+  _globals['_CONFIGURETRIGGERDIGITALRESPONSE']._serialized_start=5868
+  _globals['_CONFIGURETRIGGERDIGITALRESPONSE']._serialized_end=5917
+  _globals['_CONFIGURETRIGGERVIDEOREQUEST']._serialized_start=5920
+  _globals['_CONFIGURETRIGGERVIDEOREQUEST']._serialized_end=6490
+  _globals['_CONFIGURETRIGGERVIDEORESPONSE']._serialized_start=6492
+  _globals['_CONFIGURETRIGGERVIDEORESPONSE']._serialized_end=6539
+  _globals['_CONFIGURETRIGGERWIDTHREQUEST']._serialized_start=6542
+  _globals['_CONFIGURETRIGGERWIDTHREQUEST']._serialized_end=7026
+  _globals['_CONFIGURETRIGGERWIDTHRESPONSE']._serialized_start=7028
+  _globals['_CONFIGURETRIGGERWIDTHRESPONSE']._serialized_end=7075
+  _globals['_CONFIGUREEQUALIZATIONFILTERCOEFFICIENTSREQUEST']._serialized_start=7078
+  _globals['_CONFIGUREEQUALIZATIONFILTERCOEFFICIENTSREQUEST']._serialized_end=7206
+  _globals['_CONFIGUREEQUALIZATIONFILTERCOEFFICIENTSRESPONSE']._serialized_start=7208
+  _globals['_CONFIGUREEQUALIZATIONFILTERCOEFFICIENTSRESPONSE']._serialized_end=7273
+  _globals['_GETEQUALIZATIONFILTERCOEFFICIENTSREQUEST']._serialized_start=7275
+  _globals['_GETEQUALIZATIONFILTERCOEFFICIENTSREQUEST']._serialized_end=7402
+  _globals['_GETEQUALIZATIONFILTERCOEFFICIENTSRESPONSE']._serialized_start=7404
+  _globals['_GETEQUALIZATIONFILTERCOEFFICIENTSRESPONSE']._serialized_end=7485
+  _globals['_GETFREQUENCYRESPONSEREQUEST']._serialized_start=7487
+  _globals['_GETFREQUENCYRESPONSEREQUEST']._serialized_end=7590
+  _globals['_GETFREQUENCYRESPONSERESPONSE']._serialized_start=7593
+  _globals['_GETFREQUENCYRESPONSERESPONSE']._serialized_end=7727
+  _globals['_CONFIGUREACQUISITIONREQUEST']._serialized_start=7729
+  _globals['_CONFIGUREACQUISITIONREQUEST']._serialized_end=7820
+  _globals['_CONFIGUREACQUISITIONRESPONSE']._serialized_start=7822
+  _globals['_CONFIGUREACQUISITIONRESPONSE']._serialized_end=7868
+  _globals['_INITIATEACQUISITIONREQUEST']._serialized_start=7870
+  _globals['_INITIATEACQUISITIONREQUEST']._serialized_end=7934
+  _globals['_INITIATEACQUISITIONRESPONSE']._serialized_start=7936
+  _globals['_INITIATEACQUISITIONRESPONSE']._serialized_end=7981
+  _globals['_ABORTREQUEST']._serialized_start=7983
+  _globals['_ABORTREQUEST']._serialized_end=8033
+  _globals['_ABORTRESPONSE']._serialized_start=8035
+  _globals['_ABORTRESPONSE']._serialized_end=8066
+  _globals['_COMMITREQUEST']._serialized_start=8068
+  _globals['_COMMITREQUEST']._serialized_end=8119
+  _globals['_COMMITRESPONSE']._serialized_start=8121
+  _globals['_COMMITRESPONSE']._serialized_end=8153
+  _globals['_READREQUEST']._serialized_start=8155
+  _globals['_READREQUEST']._serialized_end=8264
+  _globals['_READRESPONSE']._serialized_start=8266
+  _globals['_READRESPONSE']._serialized_end=8360
+  _globals['_FETCHREQUEST']._serialized_start=8362
+  _globals['_FETCHREQUEST']._serialized_end=8472
+  _globals['_FETCHRESPONSE']._serialized_start=8474
+  _globals['_FETCHRESPONSE']._serialized_end=8569
+  _globals['_FETCHBINARY8REQUEST']._serialized_start=8571
+  _globals['_FETCHBINARY8REQUEST']._serialized_end=8688
+  _globals['_FETCHBINARY8RESPONSE']._serialized_start=8690
+  _globals['_FETCHBINARY8RESPONSE']._serialized_end=8792
+  _globals['_FETCHBINARY16REQUEST']._serialized_start=8794
+  _globals['_FETCHBINARY16REQUEST']._serialized_end=8912
+  _globals['_FETCHBINARY16RESPONSE']._serialized_start=8914
+  _globals['_FETCHBINARY16RESPONSE']._serialized_end=9017
+  _globals['_FETCHBINARY32REQUEST']._serialized_start=9019
+  _globals['_FETCHBINARY32REQUEST']._serialized_end=9137
+  _globals['_FETCHBINARY32RESPONSE']._serialized_start=9139
+  _globals['_FETCHBINARY32RESPONSE']._serialized_end=9242
+  _globals['_FETCHCOMPLEXREQUEST']._serialized_start=9244
+  _globals['_FETCHCOMPLEXREQUEST']._serialized_end=9361
+  _globals['_FETCHCOMPLEXRESPONSE']._serialized_start=9364
+  _globals['_FETCHCOMPLEXRESPONSE']._serialized_end=9493
+  _globals['_FETCHCOMPLEXBINARY16REQUEST']._serialized_start=9495
+  _globals['_FETCHCOMPLEXBINARY16REQUEST']._serialized_end=9620
+  _globals['_FETCHCOMPLEXBINARY16RESPONSE']._serialized_start=9623
+  _globals['_FETCHCOMPLEXBINARY16RESPONSE']._serialized_end=9757
+  _globals['_ACQUISITIONSTATUSREQUEST']._serialized_start=9759
+  _globals['_ACQUISITIONSTATUSREQUEST']._serialized_end=9821
+  _globals['_ACQUISITIONSTATUSRESPONSE']._serialized_start=9824
+  _globals['_ACQUISITIONSTATUSRESPONSE']._serialized_end=9960
+  _globals['_ACTUALNUMWFMSREQUEST']._serialized_start=9962
+  _globals['_ACTUALNUMWFMSREQUEST']._serialized_end=10042
+  _globals['_ACTUALNUMWFMSRESPONSE']._serialized_start=10044
+  _globals['_ACTUALNUMWFMSRESPONSE']._serialized_end=10101
+  _globals['_ACTUALMEASWFMSIZEREQUEST']._serialized_start=10104
+  _globals['_ACTUALMEASWFMSIZEREQUEST']._serialized_end=10292
+  _globals['_ACTUALMEASWFMSIZERESPONSE']._serialized_start=10294
+  _globals['_ACTUALMEASWFMSIZERESPONSE']._serialized_end=10365
+  _globals['_ACTUALRECORDLENGTHREQUEST']._serialized_start=10367
+  _globals['_ACTUALRECORDLENGTHREQUEST']._serialized_end=10430
+  _globals['_ACTUALRECORDLENGTHRESPONSE']._serialized_start=10432
+  _globals['_ACTUALRECORDLENGTHRESPONSE']._serialized_end=10499
+  _globals['_SAMPLERATEREQUEST']._serialized_start=10501
+  _globals['_SAMPLERATEREQUEST']._serialized_end=10556
+  _globals['_SAMPLERATERESPONSE']._serialized_start=10558
+  _globals['_SAMPLERATERESPONSE']._serialized_end=10615
+  _globals['_SAMPLEMODEREQUEST']._serialized_start=10617
+  _globals['_SAMPLEMODEREQUEST']._serialized_end=10672
+  _globals['_SAMPLEMODERESPONSE']._serialized_start=10674
+  _globals['_SAMPLEMODERESPONSE']._serialized_end=10731
+  _globals['_ADDWAVEFORMPROCESSINGREQUEST']._serialized_start=10734
+  _globals['_ADDWAVEFORMPROCESSINGREQUEST']._serialized_end=10930
+  _globals['_ADDWAVEFORMPROCESSINGRESPONSE']._serialized_start=10932
+  _globals['_ADDWAVEFORMPROCESSINGRESPONSE']._serialized_end=10979
+  _globals['_CLEARWAVEFORMPROCESSINGREQUEST']._serialized_start=10981
+  _globals['_CLEARWAVEFORMPROCESSINGREQUEST']._serialized_end=11071
+  _globals['_CLEARWAVEFORMPROCESSINGRESPONSE']._serialized_start=11073
+  _globals['_CLEARWAVEFORMPROCESSINGRESPONSE']._serialized_end=11122
+  _globals['_CLEARWAVEFORMMEASUREMENTSTATSREQUEST']._serialized_start=11125
+  _globals['_CLEARWAVEFORMMEASUREMENTSTATSREQUEST']._serialized_end=11384
+  _globals['_CLEARWAVEFORMMEASUREMENTSTATSRESPONSE']._serialized_start=11386
+  _globals['_CLEARWAVEFORMMEASUREMENTSTATSRESPONSE']._serialized_end=11441
+  _globals['_READMEASUREMENTREQUEST']._serialized_start=11444
+  _globals['_READMEASUREMENTREQUEST']._serialized_end=11673
+  _globals['_READMEASUREMENTRESPONSE']._serialized_start=11675
+  _globals['_READMEASUREMENTRESPONSE']._serialized_end=11732
+  _globals['_FETCHMEASUREMENTREQUEST']._serialized_start=11735
+  _globals['_FETCHMEASUREMENTREQUEST']._serialized_end=11965
+  _globals['_FETCHMEASUREMENTRESPONSE']._serialized_start=11967
+  _globals['_FETCHMEASUREMENTRESPONSE']._serialized_end=12025
+  _globals['_FETCHMEASUREMENTSTATSREQUEST']._serialized_start=12028
+  _globals['_FETCHMEASUREMENTSTATSREQUEST']._serialized_end=12263
+  _globals['_FETCHMEASUREMENTSTATSRESPONSE']._serialized_start=12266
+  _globals['_FETCHMEASUREMENTSTATSRESPONSE']._serialized_end=12406
+  _globals['_FETCHARRAYMEASUREMENTREQUEST']._serialized_start=12409
+  _globals['_FETCHARRAYMEASUREMENTREQUEST']._serialized_end=12686
+  _globals['_FETCHARRAYMEASUREMENTRESPONSE']._serialized_start=12688
+  _globals['_FETCHARRAYMEASUREMENTRESPONSE']._serialized_end=12799
+  _globals['_RESETREQUEST']._serialized_start=12801
+  _globals['_RESETREQUEST']._serialized_end=12851
+  _globals['_RESETRESPONSE']._serialized_start=12853
+  _globals['_RESETRESPONSE']._serialized_end=12884
+  _globals['_SELFTESTREQUEST']._serialized_start=12886
+  _globals['_SELFTESTREQUEST']._serialized_end=12939
+  _globals['_SELFTESTRESPONSE']._serialized_start=12941
+  _globals['_SELFTESTRESPONSE']._serialized_end=13028
+  _globals['_DISABLEREQUEST']._serialized_start=13030
+  _globals['_DISABLEREQUEST']._serialized_end=13082
+  _globals['_DISABLERESPONSE']._serialized_start=13084
+  _globals['_DISABLERESPONSE']._serialized_end=13117
+  _globals['_RESETDEVICEREQUEST']._serialized_start=13119
+  _globals['_RESETDEVICEREQUEST']._serialized_end=13175
+  _globals['_RESETDEVICERESPONSE']._serialized_start=13177
+  _globals['_RESETDEVICERESPONSE']._serialized_end=13214
+  _globals['_CALSELFCALIBRATEREQUEST']._serialized_start=13217
+  _globals['_CALSELFCALIBRATEREQUEST']._serialized_end=13377
+  _globals['_CALSELFCALIBRATERESPONSE']._serialized_start=13379
+  _globals['_CALSELFCALIBRATERESPONSE']._serialized_end=13421
+  _globals['_REVISIONQUERYREQUEST']._serialized_start=13423
+  _globals['_REVISIONQUERYREQUEST']._serialized_end=13481
+  _globals['_REVISIONQUERYRESPONSE']._serialized_start=13483
+  _globals['_REVISIONQUERYRESPONSE']._serialized_end=13574
+  _globals['_PROBECOMPENSATIONSIGNALSTARTREQUEST']._serialized_start=13576
+  _globals['_PROBECOMPENSATIONSIGNALSTARTREQUEST']._serialized_end=13649
+  _globals['_PROBECOMPENSATIONSIGNALSTARTRESPONSE']._serialized_start=13651
+  _globals['_PROBECOMPENSATIONSIGNALSTARTRESPONSE']._serialized_end=13705
+  _globals['_PROBECOMPENSATIONSIGNALSTOPREQUEST']._serialized_start=13707
+  _globals['_PROBECOMPENSATIONSIGNALSTOPREQUEST']._serialized_end=13779
+  _globals['_PROBECOMPENSATIONSIGNALSTOPRESPONSE']._serialized_start=13781
+  _globals['_PROBECOMPENSATIONSIGNALSTOPRESPONSE']._serialized_end=13834
+  _globals['_CABLESENSESIGNALSTARTREQUEST']._serialized_start=13836
+  _globals['_CABLESENSESIGNALSTARTREQUEST']._serialized_end=13902
+  _globals['_CABLESENSESIGNALSTARTRESPONSE']._serialized_start=13904
+  _globals['_CABLESENSESIGNALSTARTRESPONSE']._serialized_end=13951
+  _globals['_CABLESENSESIGNALSTOPREQUEST']._serialized_start=13953
+  _globals['_CABLESENSESIGNALSTOPREQUEST']._serialized_end=14018
+  _globals['_CABLESENSESIGNALSTOPRESPONSE']._serialized_start=14020
+  _globals['_CABLESENSESIGNALSTOPRESPONSE']._serialized_end=14066
+  _globals['_GETCHANNELNAMEREQUEST']._serialized_start=14068
+  _globals['_GETCHANNELNAMEREQUEST']._serialized_end=14142
+  _globals['_GETCHANNELNAMERESPONSE']._serialized_start=14144
+  _globals['_GETCHANNELNAMERESPONSE']._serialized_end=14208
+  _globals['_GETCHANNELNAMEFROMSTRINGREQUEST']._serialized_start=14210
+  _globals['_GETCHANNELNAMEFROMSTRINGREQUEST']._serialized_end=14294
+  _globals['_GETCHANNELNAMEFROMSTRINGRESPONSE']._serialized_start=14296
+  _globals['_GETCHANNELNAMEFROMSTRINGRESPONSE']._serialized_end=14360
+  _globals['_ERRORHANDLERREQUEST']._serialized_start=14362
+  _globals['_ERRORHANDLERREQUEST']._serialized_end=14461
+  _globals['_ERRORHANDLERRESPONSE']._serialized_start=14463
+  _globals['_ERRORHANDLERRESPONSE']._serialized_end=14528
+  _globals['_GETERRORREQUEST']._serialized_start=14530
+  _globals['_GETERRORREQUEST']._serialized_end=14583
+  _globals['_GETERRORRESPONSE']._serialized_start=14585
+  _globals['_GETERRORRESPONSE']._serialized_end=14660
+  _globals['_GETERRORMESSAGEREQUEST']._serialized_start=14662
+  _globals['_GETERRORMESSAGEREQUEST']._serialized_end=14742
+  _globals['_GETERRORMESSAGERESPONSE']._serialized_start=14744
+  _globals['_GETERRORMESSAGERESPONSE']._serialized_end=14808
+  _globals['_GETATTRIBUTEVIINT32REQUEST']._serialized_start=14811
+  _globals['_GETATTRIBUTEVIINT32REQUEST']._serialized_end=14951
+  _globals['_GETATTRIBUTEVIINT32RESPONSE']._serialized_start=14953
+  _globals['_GETATTRIBUTEVIINT32RESPONSE']._serialized_end=15013
+  _globals['_SETATTRIBUTEVIINT32REQUEST']._serialized_start=15016
+  _globals['_SETATTRIBUTEVIINT32REQUEST']._serialized_end=15251
+  _globals['_SETATTRIBUTEVIINT32RESPONSE']._serialized_start=15253
+  _globals['_SETATTRIBUTEVIINT32RESPONSE']._serialized_end=15298
+  _globals['_CHECKATTRIBUTEVIINT32REQUEST']._serialized_start=15301
+  _globals['_CHECKATTRIBUTEVIINT32REQUEST']._serialized_end=15538
+  _globals['_CHECKATTRIBUTEVIINT32RESPONSE']._serialized_start=15540
+  _globals['_CHECKATTRIBUTEVIINT32RESPONSE']._serialized_end=15587
+  _globals['_GETATTRIBUTEVIINT64REQUEST']._serialized_start=15590
+  _globals['_GETATTRIBUTEVIINT64REQUEST']._serialized_end=15730
+  _globals['_GETATTRIBUTEVIINT64RESPONSE']._serialized_start=15732
+  _globals['_GETATTRIBUTEVIINT64RESPONSE']._serialized_end=15792
+  _globals['_SETATTRIBUTEVIINT64REQUEST']._serialized_start=15795
+  _globals['_SETATTRIBUTEVIINT64REQUEST']._serialized_end=15954
+  _globals['_SETATTRIBUTEVIINT64RESPONSE']._serialized_start=15956
+  _globals['_SETATTRIBUTEVIINT64RESPONSE']._serialized_end=16001
+  _globals['_CHECKATTRIBUTEVIINT64REQUEST']._serialized_start=16004
+  _globals['_CHECKATTRIBUTEVIINT64REQUEST']._serialized_end=16165
+  _globals['_CHECKATTRIBUTEVIINT64RESPONSE']._serialized_start=16167
+  _globals['_CHECKATTRIBUTEVIINT64RESPONSE']._serialized_end=16214
+  _globals['_GETATTRIBUTEVIREAL64REQUEST']._serialized_start=16217
+  _globals['_GETATTRIBUTEVIREAL64REQUEST']._serialized_end=16358
+  _globals['_GETATTRIBUTEVIREAL64RESPONSE']._serialized_start=16360
+  _globals['_GETATTRIBUTEVIREAL64RESPONSE']._serialized_end=16421
+  _globals['_SETATTRIBUTEVIREAL64REQUEST']._serialized_start=16424
+  _globals['_SETATTRIBUTEVIREAL64REQUEST']._serialized_end=16735
+  _globals['_SETATTRIBUTEVIREAL64RESPONSE']._serialized_start=16737
+  _globals['_SETATTRIBUTEVIREAL64RESPONSE']._serialized_end=16783
+  _globals['_CHECKATTRIBUTEVIREAL64REQUEST']._serialized_start=16786
+  _globals['_CHECKATTRIBUTEVIREAL64REQUEST']._serialized_end=17099
+  _globals['_CHECKATTRIBUTEVIREAL64RESPONSE']._serialized_start=17101
+  _globals['_CHECKATTRIBUTEVIREAL64RESPONSE']._serialized_end=17149
+  _globals['_GETATTRIBUTEVISTRINGREQUEST']._serialized_start=17152
+  _globals['_GETATTRIBUTEVISTRINGREQUEST']._serialized_end=17293
+  _globals['_GETATTRIBUTEVISTRINGRESPONSE']._serialized_start=17295
+  _globals['_GETATTRIBUTEVISTRINGRESPONSE']._serialized_end=17356
+  _globals['_SETATTRIBUTEVISTRINGREQUEST']._serialized_start=17359
+  _globals['_SETATTRIBUTEVISTRINGREQUEST']._serialized_end=17609
+  _globals['_SETATTRIBUTEVISTRINGRESPONSE']._serialized_start=17611
+  _globals['_SETATTRIBUTEVISTRINGRESPONSE']._serialized_end=17657
+  _globals['_CHECKATTRIBUTEVISTRINGREQUEST']._serialized_start=17660
+  _globals['_CHECKATTRIBUTEVISTRINGREQUEST']._serialized_end=17912
+  _globals['_CHECKATTRIBUTEVISTRINGRESPONSE']._serialized_start=17914
+  _globals['_CHECKATTRIBUTEVISTRINGRESPONSE']._serialized_end=17962
+  _globals['_GETATTRIBUTEVISESSIONREQUEST']._serialized_start=17965
+  _globals['_GETATTRIBUTEVISESSIONREQUEST']._serialized_end=18107
+  _globals['_GETATTRIBUTEVISESSIONRESPONSE']._serialized_start=18109
+  _globals['_GETATTRIBUTEVISESSIONRESPONSE']._serialized_end=18195
+  _globals['_SETATTRIBUTEVISESSIONREQUEST']._serialized_start=18198
+  _globals['_SETATTRIBUTEVISESSIONREQUEST']._serialized_end=18379
+  _globals['_SETATTRIBUTEVISESSIONRESPONSE']._serialized_start=18381
+  _globals['_SETATTRIBUTEVISESSIONRESPONSE']._serialized_end=18428
+  _globals['_CHECKATTRIBUTEVISESSIONREQUEST']._serialized_start=18431
+  _globals['_CHECKATTRIBUTEVISESSIONREQUEST']._serialized_end=18614
+  _globals['_CHECKATTRIBUTEVISESSIONRESPONSE']._serialized_start=18616
+  _globals['_CHECKATTRIBUTEVISESSIONRESPONSE']._serialized_end=18665
+  _globals['_GETATTRIBUTEVIBOOLEANREQUEST']._serialized_start=18668
+  _globals['_GETATTRIBUTEVIBOOLEANREQUEST']._serialized_end=18810
+  _globals['_GETATTRIBUTEVIBOOLEANRESPONSE']._serialized_start=18812
+  _globals['_GETATTRIBUTEVIBOOLEANRESPONSE']._serialized_end=18874
+  _globals['_SETATTRIBUTEVIBOOLEANREQUEST']._serialized_start=18877
+  _globals['_SETATTRIBUTEVIBOOLEANREQUEST']._serialized_end=19034
+  _globals['_SETATTRIBUTEVIBOOLEANRESPONSE']._serialized_start=19036
+  _globals['_SETATTRIBUTEVIBOOLEANRESPONSE']._serialized_end=19083
+  _globals['_CHECKATTRIBUTEVIBOOLEANREQUEST']._serialized_start=19086
+  _globals['_CHECKATTRIBUTEVIBOOLEANREQUEST']._serialized_end=19245
+  _globals['_CHECKATTRIBUTEVIBOOLEANRESPONSE']._serialized_start=19247
+  _globals['_CHECKATTRIBUTEVIBOOLEANRESPONSE']._serialized_end=19296
+  _globals['_IMPORTATTRIBUTECONFIGURATIONBUFFERREQUEST']._serialized_start=19298
+  _globals['_IMPORTATTRIBUTECONFIGURATIONBUFFERREQUEST']._serialized_end=19400
+  _globals['_IMPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE']._serialized_start=19402
+  _globals['_IMPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE']._serialized_end=19462
+  _globals['_EXPORTATTRIBUTECONFIGURATIONBUFFERREQUEST']._serialized_start=19464
+  _globals['_EXPORTATTRIBUTECONFIGURATIONBUFFERREQUEST']._serialized_end=19543
+  _globals['_EXPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE']._serialized_start=19545
+  _globals['_EXPORTATTRIBUTECONFIGURATIONBUFFERRESPONSE']._serialized_end=19628
+  _globals['_IMPORTATTRIBUTECONFIGURATIONFILEREQUEST']._serialized_start=19630
+  _globals['_IMPORTATTRIBUTECONFIGURATIONFILEREQUEST']._serialized_end=19726
+  _globals['_IMPORTATTRIBUTECONFIGURATIONFILERESPONSE']._serialized_start=19728
+  _globals['_IMPORTATTRIBUTECONFIGURATIONFILERESPONSE']._serialized_end=19786
+  _globals['_EXPORTATTRIBUTECONFIGURATIONFILEREQUEST']._serialized_start=19788
+  _globals['_EXPORTATTRIBUTECONFIGURATIONFILEREQUEST']._serialized_end=19884
+  _globals['_EXPORTATTRIBUTECONFIGURATIONFILERESPONSE']._serialized_start=19886
+  _globals['_EXPORTATTRIBUTECONFIGURATIONFILERESPONSE']._serialized_end=19944
+  _globals['_GETSCALINGCOEFFICIENTSREQUEST']._serialized_start=19946
+  _globals['_GETSCALINGCOEFFICIENTSREQUEST']._serialized_end=20035
+  _globals['_GETSCALINGCOEFFICIENTSRESPONSE']._serialized_start=20038
+  _globals['_GETSCALINGCOEFFICIENTSRESPONSE']._serialized_end=20179
+  _globals['_GETNORMALIZATIONCOEFFICIENTSREQUEST']._serialized_start=20181
+  _globals['_GETNORMALIZATIONCOEFFICIENTSREQUEST']._serialized_end=20276
+  _globals['_GETNORMALIZATIONCOEFFICIENTSRESPONSE']._serialized_start=20279
+  _globals['_GETNORMALIZATIONCOEFFICIENTSRESPONSE']._serialized_end=20426
+  _globals['_GETSTREAMENDPOINTHANDLEREQUEST']._serialized_start=20428
+  _globals['_GETSTREAMENDPOINTHANDLEREQUEST']._serialized_end=20517
+  _globals['_GETSTREAMENDPOINTHANDLERESPONSE']._serialized_start=20519
+  _globals['_GETSTREAMENDPOINTHANDLERESPONSE']._serialized_end=20591
+  _globals['_CALFETCHDATEREQUEST']._serialized_start=20594
+  _globals['_CALFETCHDATEREQUEST']._serialized_end=20747
+  _globals['_CALFETCHDATERESPONSE']._serialized_start=20749
+  _globals['_CALFETCHDATERESPONSE']._serialized_end=20829
+  _globals['_CALFETCHTEMPERATUREREQUEST']._serialized_start=20832
+  _globals['_CALFETCHTEMPERATUREREQUEST']._serialized_end=20992
+  _globals['_CALFETCHTEMPERATURERESPONSE']._serialized_start=20994
+  _globals['_CALFETCHTEMPERATURERESPONSE']._serialized_end=21060
+  _globals['_NISCOPE']._serialized_start=54252
+  _globals['_NISCOPE']._serialized_end=63948
 # @@protoc_insertion_point(module_scope)
```

### Comparing `niscope-1.4.7/niscope/niscope_pb2_grpc.py` & `niscope-1.4.8/niscope/niscope_pb2_grpc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,158 +10,63 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.Abort = channel.unary_unary(
-                '/niscope_grpc.NiScope/Abort',
-                request_serializer=niscope__pb2.AbortRequest.SerializeToString,
-                response_deserializer=niscope__pb2.AbortResponse.FromString,
-                )
-        self.AcquisitionStatus = channel.unary_unary(
-                '/niscope_grpc.NiScope/AcquisitionStatus',
-                request_serializer=niscope__pb2.AcquisitionStatusRequest.SerializeToString,
-                response_deserializer=niscope__pb2.AcquisitionStatusResponse.FromString,
-                )
-        self.ActualMeasWfmSize = channel.unary_unary(
-                '/niscope_grpc.NiScope/ActualMeasWfmSize',
-                request_serializer=niscope__pb2.ActualMeasWfmSizeRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ActualMeasWfmSizeResponse.FromString,
-                )
-        self.ActualNumWfms = channel.unary_unary(
-                '/niscope_grpc.NiScope/ActualNumWfms',
-                request_serializer=niscope__pb2.ActualNumWfmsRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ActualNumWfmsResponse.FromString,
-                )
-        self.ActualRecordLength = channel.unary_unary(
-                '/niscope_grpc.NiScope/ActualRecordLength',
-                request_serializer=niscope__pb2.ActualRecordLengthRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ActualRecordLengthResponse.FromString,
-                )
-        self.AddWaveformProcessing = channel.unary_unary(
-                '/niscope_grpc.NiScope/AddWaveformProcessing',
-                request_serializer=niscope__pb2.AddWaveformProcessingRequest.SerializeToString,
-                response_deserializer=niscope__pb2.AddWaveformProcessingResponse.FromString,
-                )
-        self.AdjustSampleClockRelativeDelay = channel.unary_unary(
-                '/niscope_grpc.NiScope/AdjustSampleClockRelativeDelay',
-                request_serializer=niscope__pb2.AdjustSampleClockRelativeDelayRequest.SerializeToString,
-                response_deserializer=niscope__pb2.AdjustSampleClockRelativeDelayResponse.FromString,
-                )
-        self.AutoSetup = channel.unary_unary(
-                '/niscope_grpc.NiScope/AutoSetup',
-                request_serializer=niscope__pb2.AutoSetupRequest.SerializeToString,
-                response_deserializer=niscope__pb2.AutoSetupResponse.FromString,
-                )
-        self.CableSenseSignalStart = channel.unary_unary(
-                '/niscope_grpc.NiScope/CableSenseSignalStart',
-                request_serializer=niscope__pb2.CableSenseSignalStartRequest.SerializeToString,
-                response_deserializer=niscope__pb2.CableSenseSignalStartResponse.FromString,
-                )
-        self.CableSenseSignalStop = channel.unary_unary(
-                '/niscope_grpc.NiScope/CableSenseSignalStop',
-                request_serializer=niscope__pb2.CableSenseSignalStopRequest.SerializeToString,
-                response_deserializer=niscope__pb2.CableSenseSignalStopResponse.FromString,
-                )
-        self.CalFetchDate = channel.unary_unary(
-                '/niscope_grpc.NiScope/CalFetchDate',
-                request_serializer=niscope__pb2.CalFetchDateRequest.SerializeToString,
-                response_deserializer=niscope__pb2.CalFetchDateResponse.FromString,
-                )
-        self.CalFetchTemperature = channel.unary_unary(
-                '/niscope_grpc.NiScope/CalFetchTemperature',
-                request_serializer=niscope__pb2.CalFetchTemperatureRequest.SerializeToString,
-                response_deserializer=niscope__pb2.CalFetchTemperatureResponse.FromString,
-                )
-        self.CalSelfCalibrate = channel.unary_unary(
-                '/niscope_grpc.NiScope/CalSelfCalibrate',
-                request_serializer=niscope__pb2.CalSelfCalibrateRequest.SerializeToString,
-                response_deserializer=niscope__pb2.CalSelfCalibrateResponse.FromString,
-                )
-        self.CheckAttributeViBoolean = channel.unary_unary(
-                '/niscope_grpc.NiScope/CheckAttributeViBoolean',
-                request_serializer=niscope__pb2.CheckAttributeViBooleanRequest.SerializeToString,
-                response_deserializer=niscope__pb2.CheckAttributeViBooleanResponse.FromString,
-                )
-        self.CheckAttributeViInt32 = channel.unary_unary(
-                '/niscope_grpc.NiScope/CheckAttributeViInt32',
-                request_serializer=niscope__pb2.CheckAttributeViInt32Request.SerializeToString,
-                response_deserializer=niscope__pb2.CheckAttributeViInt32Response.FromString,
-                )
-        self.CheckAttributeViInt64 = channel.unary_unary(
-                '/niscope_grpc.NiScope/CheckAttributeViInt64',
-                request_serializer=niscope__pb2.CheckAttributeViInt64Request.SerializeToString,
-                response_deserializer=niscope__pb2.CheckAttributeViInt64Response.FromString,
-                )
-        self.CheckAttributeViReal64 = channel.unary_unary(
-                '/niscope_grpc.NiScope/CheckAttributeViReal64',
-                request_serializer=niscope__pb2.CheckAttributeViReal64Request.SerializeToString,
-                response_deserializer=niscope__pb2.CheckAttributeViReal64Response.FromString,
-                )
-        self.CheckAttributeViSession = channel.unary_unary(
-                '/niscope_grpc.NiScope/CheckAttributeViSession',
-                request_serializer=niscope__pb2.CheckAttributeViSessionRequest.SerializeToString,
-                response_deserializer=niscope__pb2.CheckAttributeViSessionResponse.FromString,
-                )
-        self.CheckAttributeViString = channel.unary_unary(
-                '/niscope_grpc.NiScope/CheckAttributeViString',
-                request_serializer=niscope__pb2.CheckAttributeViStringRequest.SerializeToString,
-                response_deserializer=niscope__pb2.CheckAttributeViStringResponse.FromString,
-                )
-        self.ClearWaveformMeasurementStats = channel.unary_unary(
-                '/niscope_grpc.NiScope/ClearWaveformMeasurementStats',
-                request_serializer=niscope__pb2.ClearWaveformMeasurementStatsRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ClearWaveformMeasurementStatsResponse.FromString,
+        self.Init = channel.unary_unary(
+                '/niscope_grpc.NiScope/Init',
+                request_serializer=niscope__pb2.InitRequest.SerializeToString,
+                response_deserializer=niscope__pb2.InitResponse.FromString,
                 )
-        self.ClearWaveformProcessing = channel.unary_unary(
-                '/niscope_grpc.NiScope/ClearWaveformProcessing',
-                request_serializer=niscope__pb2.ClearWaveformProcessingRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ClearWaveformProcessingResponse.FromString,
+        self.InitWithOptions = channel.unary_unary(
+                '/niscope_grpc.NiScope/InitWithOptions',
+                request_serializer=niscope__pb2.InitWithOptionsRequest.SerializeToString,
+                response_deserializer=niscope__pb2.InitWithOptionsResponse.FromString,
                 )
         self.Close = channel.unary_unary(
                 '/niscope_grpc.NiScope/Close',
                 request_serializer=niscope__pb2.CloseRequest.SerializeToString,
                 response_deserializer=niscope__pb2.CloseResponse.FromString,
                 )
-        self.Commit = channel.unary_unary(
-                '/niscope_grpc.NiScope/Commit',
-                request_serializer=niscope__pb2.CommitRequest.SerializeToString,
-                response_deserializer=niscope__pb2.CommitResponse.FromString,
+        self.AutoSetup = channel.unary_unary(
+                '/niscope_grpc.NiScope/AutoSetup',
+                request_serializer=niscope__pb2.AutoSetupRequest.SerializeToString,
+                response_deserializer=niscope__pb2.AutoSetupResponse.FromString,
                 )
-        self.ConfigureAcquisition = channel.unary_unary(
-                '/niscope_grpc.NiScope/ConfigureAcquisition',
-                request_serializer=niscope__pb2.ConfigureAcquisitionRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ConfigureAcquisitionResponse.FromString,
+        self.ConfigureVertical = channel.unary_unary(
+                '/niscope_grpc.NiScope/ConfigureVertical',
+                request_serializer=niscope__pb2.ConfigureVerticalRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ConfigureVerticalResponse.FromString,
                 )
         self.ConfigureChanCharacteristics = channel.unary_unary(
                 '/niscope_grpc.NiScope/ConfigureChanCharacteristics',
                 request_serializer=niscope__pb2.ConfigureChanCharacteristicsRequest.SerializeToString,
                 response_deserializer=niscope__pb2.ConfigureChanCharacteristicsResponse.FromString,
                 )
+        self.ConfigureHorizontalTiming = channel.unary_unary(
+                '/niscope_grpc.NiScope/ConfigureHorizontalTiming',
+                request_serializer=niscope__pb2.ConfigureHorizontalTimingRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ConfigureHorizontalTimingResponse.FromString,
+                )
         self.ConfigureClock = channel.unary_unary(
                 '/niscope_grpc.NiScope/ConfigureClock',
                 request_serializer=niscope__pb2.ConfigureClockRequest.SerializeToString,
                 response_deserializer=niscope__pb2.ConfigureClockResponse.FromString,
                 )
-        self.ConfigureEqualizationFilterCoefficients = channel.unary_unary(
-                '/niscope_grpc.NiScope/ConfigureEqualizationFilterCoefficients',
-                request_serializer=niscope__pb2.ConfigureEqualizationFilterCoefficientsRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ConfigureEqualizationFilterCoefficientsResponse.FromString,
-                )
-        self.ConfigureHorizontalTiming = channel.unary_unary(
-                '/niscope_grpc.NiScope/ConfigureHorizontalTiming',
-                request_serializer=niscope__pb2.ConfigureHorizontalTimingRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ConfigureHorizontalTimingResponse.FromString,
+        self.ExportSignal = channel.unary_unary(
+                '/niscope_grpc.NiScope/ExportSignal',
+                request_serializer=niscope__pb2.ExportSignalRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ExportSignalResponse.FromString,
                 )
-        self.ConfigureTriggerDigital = channel.unary_unary(
-                '/niscope_grpc.NiScope/ConfigureTriggerDigital',
-                request_serializer=niscope__pb2.ConfigureTriggerDigitalRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ConfigureTriggerDigitalResponse.FromString,
+        self.AdjustSampleClockRelativeDelay = channel.unary_unary(
+                '/niscope_grpc.NiScope/AdjustSampleClockRelativeDelay',
+                request_serializer=niscope__pb2.AdjustSampleClockRelativeDelayRequest.SerializeToString,
+                response_deserializer=niscope__pb2.AdjustSampleClockRelativeDelayResponse.FromString,
                 )
         self.ConfigureTriggerEdge = channel.unary_unary(
                 '/niscope_grpc.NiScope/ConfigureTriggerEdge',
                 request_serializer=niscope__pb2.ConfigureTriggerEdgeRequest.SerializeToString,
                 response_deserializer=niscope__pb2.ConfigureTriggerEdgeResponse.FromString,
                 )
         self.ConfigureTriggerGlitch = channel.unary_unary(
@@ -170,996 +75,996 @@
                 response_deserializer=niscope__pb2.ConfigureTriggerGlitchResponse.FromString,
                 )
         self.ConfigureTriggerHysteresis = channel.unary_unary(
                 '/niscope_grpc.NiScope/ConfigureTriggerHysteresis',
                 request_serializer=niscope__pb2.ConfigureTriggerHysteresisRequest.SerializeToString,
                 response_deserializer=niscope__pb2.ConfigureTriggerHysteresisResponse.FromString,
                 )
+        self.ConfigureTriggerWindow = channel.unary_unary(
+                '/niscope_grpc.NiScope/ConfigureTriggerWindow',
+                request_serializer=niscope__pb2.ConfigureTriggerWindowRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ConfigureTriggerWindowResponse.FromString,
+                )
+        self.ConfigureTriggerSoftware = channel.unary_unary(
+                '/niscope_grpc.NiScope/ConfigureTriggerSoftware',
+                request_serializer=niscope__pb2.ConfigureTriggerSoftwareRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ConfigureTriggerSoftwareResponse.FromString,
+                )
+        self.SendSoftwareTriggerEdge = channel.unary_unary(
+                '/niscope_grpc.NiScope/SendSoftwareTriggerEdge',
+                request_serializer=niscope__pb2.SendSoftwareTriggerEdgeRequest.SerializeToString,
+                response_deserializer=niscope__pb2.SendSoftwareTriggerEdgeResponse.FromString,
+                )
         self.ConfigureTriggerImmediate = channel.unary_unary(
                 '/niscope_grpc.NiScope/ConfigureTriggerImmediate',
                 request_serializer=niscope__pb2.ConfigureTriggerImmediateRequest.SerializeToString,
                 response_deserializer=niscope__pb2.ConfigureTriggerImmediateResponse.FromString,
                 )
         self.ConfigureTriggerRunt = channel.unary_unary(
                 '/niscope_grpc.NiScope/ConfigureTriggerRunt',
                 request_serializer=niscope__pb2.ConfigureTriggerRuntRequest.SerializeToString,
                 response_deserializer=niscope__pb2.ConfigureTriggerRuntResponse.FromString,
                 )
-        self.ConfigureTriggerSoftware = channel.unary_unary(
-                '/niscope_grpc.NiScope/ConfigureTriggerSoftware',
-                request_serializer=niscope__pb2.ConfigureTriggerSoftwareRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ConfigureTriggerSoftwareResponse.FromString,
+        self.ConfigureTriggerDigital = channel.unary_unary(
+                '/niscope_grpc.NiScope/ConfigureTriggerDigital',
+                request_serializer=niscope__pb2.ConfigureTriggerDigitalRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ConfigureTriggerDigitalResponse.FromString,
                 )
         self.ConfigureTriggerVideo = channel.unary_unary(
                 '/niscope_grpc.NiScope/ConfigureTriggerVideo',
                 request_serializer=niscope__pb2.ConfigureTriggerVideoRequest.SerializeToString,
                 response_deserializer=niscope__pb2.ConfigureTriggerVideoResponse.FromString,
                 )
         self.ConfigureTriggerWidth = channel.unary_unary(
                 '/niscope_grpc.NiScope/ConfigureTriggerWidth',
                 request_serializer=niscope__pb2.ConfigureTriggerWidthRequest.SerializeToString,
                 response_deserializer=niscope__pb2.ConfigureTriggerWidthResponse.FromString,
                 )
-        self.ConfigureTriggerWindow = channel.unary_unary(
-                '/niscope_grpc.NiScope/ConfigureTriggerWindow',
-                request_serializer=niscope__pb2.ConfigureTriggerWindowRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ConfigureTriggerWindowResponse.FromString,
+        self.ConfigureEqualizationFilterCoefficients = channel.unary_unary(
+                '/niscope_grpc.NiScope/ConfigureEqualizationFilterCoefficients',
+                request_serializer=niscope__pb2.ConfigureEqualizationFilterCoefficientsRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ConfigureEqualizationFilterCoefficientsResponse.FromString,
                 )
-        self.ConfigureVertical = channel.unary_unary(
-                '/niscope_grpc.NiScope/ConfigureVertical',
-                request_serializer=niscope__pb2.ConfigureVerticalRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ConfigureVerticalResponse.FromString,
+        self.GetEqualizationFilterCoefficients = channel.unary_unary(
+                '/niscope_grpc.NiScope/GetEqualizationFilterCoefficients',
+                request_serializer=niscope__pb2.GetEqualizationFilterCoefficientsRequest.SerializeToString,
+                response_deserializer=niscope__pb2.GetEqualizationFilterCoefficientsResponse.FromString,
                 )
-        self.Disable = channel.unary_unary(
-                '/niscope_grpc.NiScope/Disable',
-                request_serializer=niscope__pb2.DisableRequest.SerializeToString,
-                response_deserializer=niscope__pb2.DisableResponse.FromString,
+        self.GetFrequencyResponse = channel.unary_unary(
+                '/niscope_grpc.NiScope/GetFrequencyResponse',
+                request_serializer=niscope__pb2.GetFrequencyResponseRequest.SerializeToString,
+                response_deserializer=niscope__pb2.GetFrequencyResponseResponse.FromString,
                 )
-        self.ErrorHandler = channel.unary_unary(
-                '/niscope_grpc.NiScope/ErrorHandler',
-                request_serializer=niscope__pb2.ErrorHandlerRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ErrorHandlerResponse.FromString,
+        self.ConfigureAcquisition = channel.unary_unary(
+                '/niscope_grpc.NiScope/ConfigureAcquisition',
+                request_serializer=niscope__pb2.ConfigureAcquisitionRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ConfigureAcquisitionResponse.FromString,
                 )
-        self.ExportAttributeConfigurationBuffer = channel.unary_unary(
-                '/niscope_grpc.NiScope/ExportAttributeConfigurationBuffer',
-                request_serializer=niscope__pb2.ExportAttributeConfigurationBufferRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ExportAttributeConfigurationBufferResponse.FromString,
+        self.InitiateAcquisition = channel.unary_unary(
+                '/niscope_grpc.NiScope/InitiateAcquisition',
+                request_serializer=niscope__pb2.InitiateAcquisitionRequest.SerializeToString,
+                response_deserializer=niscope__pb2.InitiateAcquisitionResponse.FromString,
                 )
-        self.ExportAttributeConfigurationFile = channel.unary_unary(
-                '/niscope_grpc.NiScope/ExportAttributeConfigurationFile',
-                request_serializer=niscope__pb2.ExportAttributeConfigurationFileRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ExportAttributeConfigurationFileResponse.FromString,
+        self.Abort = channel.unary_unary(
+                '/niscope_grpc.NiScope/Abort',
+                request_serializer=niscope__pb2.AbortRequest.SerializeToString,
+                response_deserializer=niscope__pb2.AbortResponse.FromString,
                 )
-        self.ExportSignal = channel.unary_unary(
-                '/niscope_grpc.NiScope/ExportSignal',
-                request_serializer=niscope__pb2.ExportSignalRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ExportSignalResponse.FromString,
+        self.Commit = channel.unary_unary(
+                '/niscope_grpc.NiScope/Commit',
+                request_serializer=niscope__pb2.CommitRequest.SerializeToString,
+                response_deserializer=niscope__pb2.CommitResponse.FromString,
+                )
+        self.Read = channel.unary_unary(
+                '/niscope_grpc.NiScope/Read',
+                request_serializer=niscope__pb2.ReadRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ReadResponse.FromString,
                 )
         self.Fetch = channel.unary_unary(
                 '/niscope_grpc.NiScope/Fetch',
                 request_serializer=niscope__pb2.FetchRequest.SerializeToString,
                 response_deserializer=niscope__pb2.FetchResponse.FromString,
                 )
-        self.FetchArrayMeasurement = channel.unary_unary(
-                '/niscope_grpc.NiScope/FetchArrayMeasurement',
-                request_serializer=niscope__pb2.FetchArrayMeasurementRequest.SerializeToString,
-                response_deserializer=niscope__pb2.FetchArrayMeasurementResponse.FromString,
+        self.FetchBinary8 = channel.unary_unary(
+                '/niscope_grpc.NiScope/FetchBinary8',
+                request_serializer=niscope__pb2.FetchBinary8Request.SerializeToString,
+                response_deserializer=niscope__pb2.FetchBinary8Response.FromString,
                 )
         self.FetchBinary16 = channel.unary_unary(
                 '/niscope_grpc.NiScope/FetchBinary16',
                 request_serializer=niscope__pb2.FetchBinary16Request.SerializeToString,
                 response_deserializer=niscope__pb2.FetchBinary16Response.FromString,
                 )
         self.FetchBinary32 = channel.unary_unary(
                 '/niscope_grpc.NiScope/FetchBinary32',
                 request_serializer=niscope__pb2.FetchBinary32Request.SerializeToString,
                 response_deserializer=niscope__pb2.FetchBinary32Response.FromString,
                 )
-        self.FetchBinary8 = channel.unary_unary(
-                '/niscope_grpc.NiScope/FetchBinary8',
-                request_serializer=niscope__pb2.FetchBinary8Request.SerializeToString,
-                response_deserializer=niscope__pb2.FetchBinary8Response.FromString,
-                )
         self.FetchComplex = channel.unary_unary(
                 '/niscope_grpc.NiScope/FetchComplex',
                 request_serializer=niscope__pb2.FetchComplexRequest.SerializeToString,
                 response_deserializer=niscope__pb2.FetchComplexResponse.FromString,
                 )
         self.FetchComplexBinary16 = channel.unary_unary(
                 '/niscope_grpc.NiScope/FetchComplexBinary16',
                 request_serializer=niscope__pb2.FetchComplexBinary16Request.SerializeToString,
                 response_deserializer=niscope__pb2.FetchComplexBinary16Response.FromString,
                 )
+        self.AcquisitionStatus = channel.unary_unary(
+                '/niscope_grpc.NiScope/AcquisitionStatus',
+                request_serializer=niscope__pb2.AcquisitionStatusRequest.SerializeToString,
+                response_deserializer=niscope__pb2.AcquisitionStatusResponse.FromString,
+                )
+        self.ActualNumWfms = channel.unary_unary(
+                '/niscope_grpc.NiScope/ActualNumWfms',
+                request_serializer=niscope__pb2.ActualNumWfmsRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ActualNumWfmsResponse.FromString,
+                )
+        self.ActualMeasWfmSize = channel.unary_unary(
+                '/niscope_grpc.NiScope/ActualMeasWfmSize',
+                request_serializer=niscope__pb2.ActualMeasWfmSizeRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ActualMeasWfmSizeResponse.FromString,
+                )
+        self.ActualRecordLength = channel.unary_unary(
+                '/niscope_grpc.NiScope/ActualRecordLength',
+                request_serializer=niscope__pb2.ActualRecordLengthRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ActualRecordLengthResponse.FromString,
+                )
+        self.SampleRate = channel.unary_unary(
+                '/niscope_grpc.NiScope/SampleRate',
+                request_serializer=niscope__pb2.SampleRateRequest.SerializeToString,
+                response_deserializer=niscope__pb2.SampleRateResponse.FromString,
+                )
+        self.SampleMode = channel.unary_unary(
+                '/niscope_grpc.NiScope/SampleMode',
+                request_serializer=niscope__pb2.SampleModeRequest.SerializeToString,
+                response_deserializer=niscope__pb2.SampleModeResponse.FromString,
+                )
+        self.AddWaveformProcessing = channel.unary_unary(
+                '/niscope_grpc.NiScope/AddWaveformProcessing',
+                request_serializer=niscope__pb2.AddWaveformProcessingRequest.SerializeToString,
+                response_deserializer=niscope__pb2.AddWaveformProcessingResponse.FromString,
+                )
+        self.ClearWaveformProcessing = channel.unary_unary(
+                '/niscope_grpc.NiScope/ClearWaveformProcessing',
+                request_serializer=niscope__pb2.ClearWaveformProcessingRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ClearWaveformProcessingResponse.FromString,
+                )
+        self.ClearWaveformMeasurementStats = channel.unary_unary(
+                '/niscope_grpc.NiScope/ClearWaveformMeasurementStats',
+                request_serializer=niscope__pb2.ClearWaveformMeasurementStatsRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ClearWaveformMeasurementStatsResponse.FromString,
+                )
+        self.ReadMeasurement = channel.unary_unary(
+                '/niscope_grpc.NiScope/ReadMeasurement',
+                request_serializer=niscope__pb2.ReadMeasurementRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ReadMeasurementResponse.FromString,
+                )
         self.FetchMeasurement = channel.unary_unary(
                 '/niscope_grpc.NiScope/FetchMeasurement',
                 request_serializer=niscope__pb2.FetchMeasurementRequest.SerializeToString,
                 response_deserializer=niscope__pb2.FetchMeasurementResponse.FromString,
                 )
         self.FetchMeasurementStats = channel.unary_unary(
                 '/niscope_grpc.NiScope/FetchMeasurementStats',
                 request_serializer=niscope__pb2.FetchMeasurementStatsRequest.SerializeToString,
                 response_deserializer=niscope__pb2.FetchMeasurementStatsResponse.FromString,
                 )
-        self.GetAttributeViBoolean = channel.unary_unary(
-                '/niscope_grpc.NiScope/GetAttributeViBoolean',
-                request_serializer=niscope__pb2.GetAttributeViBooleanRequest.SerializeToString,
-                response_deserializer=niscope__pb2.GetAttributeViBooleanResponse.FromString,
+        self.FetchArrayMeasurement = channel.unary_unary(
+                '/niscope_grpc.NiScope/FetchArrayMeasurement',
+                request_serializer=niscope__pb2.FetchArrayMeasurementRequest.SerializeToString,
+                response_deserializer=niscope__pb2.FetchArrayMeasurementResponse.FromString,
                 )
-        self.GetAttributeViInt32 = channel.unary_unary(
-                '/niscope_grpc.NiScope/GetAttributeViInt32',
-                request_serializer=niscope__pb2.GetAttributeViInt32Request.SerializeToString,
-                response_deserializer=niscope__pb2.GetAttributeViInt32Response.FromString,
+        self.Reset = channel.unary_unary(
+                '/niscope_grpc.NiScope/Reset',
+                request_serializer=niscope__pb2.ResetRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ResetResponse.FromString,
                 )
-        self.GetAttributeViInt64 = channel.unary_unary(
-                '/niscope_grpc.NiScope/GetAttributeViInt64',
-                request_serializer=niscope__pb2.GetAttributeViInt64Request.SerializeToString,
-                response_deserializer=niscope__pb2.GetAttributeViInt64Response.FromString,
+        self.SelfTest = channel.unary_unary(
+                '/niscope_grpc.NiScope/SelfTest',
+                request_serializer=niscope__pb2.SelfTestRequest.SerializeToString,
+                response_deserializer=niscope__pb2.SelfTestResponse.FromString,
                 )
-        self.GetAttributeViReal64 = channel.unary_unary(
-                '/niscope_grpc.NiScope/GetAttributeViReal64',
-                request_serializer=niscope__pb2.GetAttributeViReal64Request.SerializeToString,
-                response_deserializer=niscope__pb2.GetAttributeViReal64Response.FromString,
+        self.Disable = channel.unary_unary(
+                '/niscope_grpc.NiScope/Disable',
+                request_serializer=niscope__pb2.DisableRequest.SerializeToString,
+                response_deserializer=niscope__pb2.DisableResponse.FromString,
                 )
-        self.GetAttributeViSession = channel.unary_unary(
-                '/niscope_grpc.NiScope/GetAttributeViSession',
-                request_serializer=niscope__pb2.GetAttributeViSessionRequest.SerializeToString,
-                response_deserializer=niscope__pb2.GetAttributeViSessionResponse.FromString,
+        self.ResetDevice = channel.unary_unary(
+                '/niscope_grpc.NiScope/ResetDevice',
+                request_serializer=niscope__pb2.ResetDeviceRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ResetDeviceResponse.FromString,
                 )
-        self.GetAttributeViString = channel.unary_unary(
-                '/niscope_grpc.NiScope/GetAttributeViString',
-                request_serializer=niscope__pb2.GetAttributeViStringRequest.SerializeToString,
-                response_deserializer=niscope__pb2.GetAttributeViStringResponse.FromString,
+        self.CalSelfCalibrate = channel.unary_unary(
+                '/niscope_grpc.NiScope/CalSelfCalibrate',
+                request_serializer=niscope__pb2.CalSelfCalibrateRequest.SerializeToString,
+                response_deserializer=niscope__pb2.CalSelfCalibrateResponse.FromString,
+                )
+        self.RevisionQuery = channel.unary_unary(
+                '/niscope_grpc.NiScope/RevisionQuery',
+                request_serializer=niscope__pb2.RevisionQueryRequest.SerializeToString,
+                response_deserializer=niscope__pb2.RevisionQueryResponse.FromString,
+                )
+        self.ProbeCompensationSignalStart = channel.unary_unary(
+                '/niscope_grpc.NiScope/ProbeCompensationSignalStart',
+                request_serializer=niscope__pb2.ProbeCompensationSignalStartRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ProbeCompensationSignalStartResponse.FromString,
+                )
+        self.ProbeCompensationSignalStop = channel.unary_unary(
+                '/niscope_grpc.NiScope/ProbeCompensationSignalStop',
+                request_serializer=niscope__pb2.ProbeCompensationSignalStopRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ProbeCompensationSignalStopResponse.FromString,
+                )
+        self.CableSenseSignalStart = channel.unary_unary(
+                '/niscope_grpc.NiScope/CableSenseSignalStart',
+                request_serializer=niscope__pb2.CableSenseSignalStartRequest.SerializeToString,
+                response_deserializer=niscope__pb2.CableSenseSignalStartResponse.FromString,
+                )
+        self.CableSenseSignalStop = channel.unary_unary(
+                '/niscope_grpc.NiScope/CableSenseSignalStop',
+                request_serializer=niscope__pb2.CableSenseSignalStopRequest.SerializeToString,
+                response_deserializer=niscope__pb2.CableSenseSignalStopResponse.FromString,
                 )
         self.GetChannelName = channel.unary_unary(
                 '/niscope_grpc.NiScope/GetChannelName',
                 request_serializer=niscope__pb2.GetChannelNameRequest.SerializeToString,
                 response_deserializer=niscope__pb2.GetChannelNameResponse.FromString,
                 )
         self.GetChannelNameFromString = channel.unary_unary(
                 '/niscope_grpc.NiScope/GetChannelNameFromString',
                 request_serializer=niscope__pb2.GetChannelNameFromStringRequest.SerializeToString,
                 response_deserializer=niscope__pb2.GetChannelNameFromStringResponse.FromString,
                 )
-        self.GetEqualizationFilterCoefficients = channel.unary_unary(
-                '/niscope_grpc.NiScope/GetEqualizationFilterCoefficients',
-                request_serializer=niscope__pb2.GetEqualizationFilterCoefficientsRequest.SerializeToString,
-                response_deserializer=niscope__pb2.GetEqualizationFilterCoefficientsResponse.FromString,
+        self.ErrorHandler = channel.unary_unary(
+                '/niscope_grpc.NiScope/ErrorHandler',
+                request_serializer=niscope__pb2.ErrorHandlerRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ErrorHandlerResponse.FromString,
                 )
         self.GetError = channel.unary_unary(
                 '/niscope_grpc.NiScope/GetError',
                 request_serializer=niscope__pb2.GetErrorRequest.SerializeToString,
                 response_deserializer=niscope__pb2.GetErrorResponse.FromString,
                 )
         self.GetErrorMessage = channel.unary_unary(
                 '/niscope_grpc.NiScope/GetErrorMessage',
                 request_serializer=niscope__pb2.GetErrorMessageRequest.SerializeToString,
                 response_deserializer=niscope__pb2.GetErrorMessageResponse.FromString,
                 )
-        self.GetFrequencyResponse = channel.unary_unary(
-                '/niscope_grpc.NiScope/GetFrequencyResponse',
-                request_serializer=niscope__pb2.GetFrequencyResponseRequest.SerializeToString,
-                response_deserializer=niscope__pb2.GetFrequencyResponseResponse.FromString,
-                )
-        self.GetNormalizationCoefficients = channel.unary_unary(
-                '/niscope_grpc.NiScope/GetNormalizationCoefficients',
-                request_serializer=niscope__pb2.GetNormalizationCoefficientsRequest.SerializeToString,
-                response_deserializer=niscope__pb2.GetNormalizationCoefficientsResponse.FromString,
-                )
-        self.GetScalingCoefficients = channel.unary_unary(
-                '/niscope_grpc.NiScope/GetScalingCoefficients',
-                request_serializer=niscope__pb2.GetScalingCoefficientsRequest.SerializeToString,
-                response_deserializer=niscope__pb2.GetScalingCoefficientsResponse.FromString,
-                )
-        self.GetStreamEndpointHandle = channel.unary_unary(
-                '/niscope_grpc.NiScope/GetStreamEndpointHandle',
-                request_serializer=niscope__pb2.GetStreamEndpointHandleRequest.SerializeToString,
-                response_deserializer=niscope__pb2.GetStreamEndpointHandleResponse.FromString,
-                )
-        self.ImportAttributeConfigurationBuffer = channel.unary_unary(
-                '/niscope_grpc.NiScope/ImportAttributeConfigurationBuffer',
-                request_serializer=niscope__pb2.ImportAttributeConfigurationBufferRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ImportAttributeConfigurationBufferResponse.FromString,
+        self.GetAttributeViInt32 = channel.unary_unary(
+                '/niscope_grpc.NiScope/GetAttributeViInt32',
+                request_serializer=niscope__pb2.GetAttributeViInt32Request.SerializeToString,
+                response_deserializer=niscope__pb2.GetAttributeViInt32Response.FromString,
                 )
-        self.ImportAttributeConfigurationFile = channel.unary_unary(
-                '/niscope_grpc.NiScope/ImportAttributeConfigurationFile',
-                request_serializer=niscope__pb2.ImportAttributeConfigurationFileRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ImportAttributeConfigurationFileResponse.FromString,
+        self.SetAttributeViInt32 = channel.unary_unary(
+                '/niscope_grpc.NiScope/SetAttributeViInt32',
+                request_serializer=niscope__pb2.SetAttributeViInt32Request.SerializeToString,
+                response_deserializer=niscope__pb2.SetAttributeViInt32Response.FromString,
                 )
-        self.Init = channel.unary_unary(
-                '/niscope_grpc.NiScope/Init',
-                request_serializer=niscope__pb2.InitRequest.SerializeToString,
-                response_deserializer=niscope__pb2.InitResponse.FromString,
+        self.CheckAttributeViInt32 = channel.unary_unary(
+                '/niscope_grpc.NiScope/CheckAttributeViInt32',
+                request_serializer=niscope__pb2.CheckAttributeViInt32Request.SerializeToString,
+                response_deserializer=niscope__pb2.CheckAttributeViInt32Response.FromString,
                 )
-        self.InitWithOptions = channel.unary_unary(
-                '/niscope_grpc.NiScope/InitWithOptions',
-                request_serializer=niscope__pb2.InitWithOptionsRequest.SerializeToString,
-                response_deserializer=niscope__pb2.InitWithOptionsResponse.FromString,
+        self.GetAttributeViInt64 = channel.unary_unary(
+                '/niscope_grpc.NiScope/GetAttributeViInt64',
+                request_serializer=niscope__pb2.GetAttributeViInt64Request.SerializeToString,
+                response_deserializer=niscope__pb2.GetAttributeViInt64Response.FromString,
                 )
-        self.InitiateAcquisition = channel.unary_unary(
-                '/niscope_grpc.NiScope/InitiateAcquisition',
-                request_serializer=niscope__pb2.InitiateAcquisitionRequest.SerializeToString,
-                response_deserializer=niscope__pb2.InitiateAcquisitionResponse.FromString,
+        self.SetAttributeViInt64 = channel.unary_unary(
+                '/niscope_grpc.NiScope/SetAttributeViInt64',
+                request_serializer=niscope__pb2.SetAttributeViInt64Request.SerializeToString,
+                response_deserializer=niscope__pb2.SetAttributeViInt64Response.FromString,
                 )
-        self.ProbeCompensationSignalStart = channel.unary_unary(
-                '/niscope_grpc.NiScope/ProbeCompensationSignalStart',
-                request_serializer=niscope__pb2.ProbeCompensationSignalStartRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ProbeCompensationSignalStartResponse.FromString,
+        self.CheckAttributeViInt64 = channel.unary_unary(
+                '/niscope_grpc.NiScope/CheckAttributeViInt64',
+                request_serializer=niscope__pb2.CheckAttributeViInt64Request.SerializeToString,
+                response_deserializer=niscope__pb2.CheckAttributeViInt64Response.FromString,
                 )
-        self.ProbeCompensationSignalStop = channel.unary_unary(
-                '/niscope_grpc.NiScope/ProbeCompensationSignalStop',
-                request_serializer=niscope__pb2.ProbeCompensationSignalStopRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ProbeCompensationSignalStopResponse.FromString,
+        self.GetAttributeViReal64 = channel.unary_unary(
+                '/niscope_grpc.NiScope/GetAttributeViReal64',
+                request_serializer=niscope__pb2.GetAttributeViReal64Request.SerializeToString,
+                response_deserializer=niscope__pb2.GetAttributeViReal64Response.FromString,
                 )
-        self.Read = channel.unary_unary(
-                '/niscope_grpc.NiScope/Read',
-                request_serializer=niscope__pb2.ReadRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ReadResponse.FromString,
+        self.SetAttributeViReal64 = channel.unary_unary(
+                '/niscope_grpc.NiScope/SetAttributeViReal64',
+                request_serializer=niscope__pb2.SetAttributeViReal64Request.SerializeToString,
+                response_deserializer=niscope__pb2.SetAttributeViReal64Response.FromString,
                 )
-        self.ReadMeasurement = channel.unary_unary(
-                '/niscope_grpc.NiScope/ReadMeasurement',
-                request_serializer=niscope__pb2.ReadMeasurementRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ReadMeasurementResponse.FromString,
+        self.CheckAttributeViReal64 = channel.unary_unary(
+                '/niscope_grpc.NiScope/CheckAttributeViReal64',
+                request_serializer=niscope__pb2.CheckAttributeViReal64Request.SerializeToString,
+                response_deserializer=niscope__pb2.CheckAttributeViReal64Response.FromString,
                 )
-        self.Reset = channel.unary_unary(
-                '/niscope_grpc.NiScope/Reset',
-                request_serializer=niscope__pb2.ResetRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ResetResponse.FromString,
+        self.GetAttributeViString = channel.unary_unary(
+                '/niscope_grpc.NiScope/GetAttributeViString',
+                request_serializer=niscope__pb2.GetAttributeViStringRequest.SerializeToString,
+                response_deserializer=niscope__pb2.GetAttributeViStringResponse.FromString,
                 )
-        self.ResetDevice = channel.unary_unary(
-                '/niscope_grpc.NiScope/ResetDevice',
-                request_serializer=niscope__pb2.ResetDeviceRequest.SerializeToString,
-                response_deserializer=niscope__pb2.ResetDeviceResponse.FromString,
+        self.SetAttributeViString = channel.unary_unary(
+                '/niscope_grpc.NiScope/SetAttributeViString',
+                request_serializer=niscope__pb2.SetAttributeViStringRequest.SerializeToString,
+                response_deserializer=niscope__pb2.SetAttributeViStringResponse.FromString,
                 )
-        self.RevisionQuery = channel.unary_unary(
-                '/niscope_grpc.NiScope/RevisionQuery',
-                request_serializer=niscope__pb2.RevisionQueryRequest.SerializeToString,
-                response_deserializer=niscope__pb2.RevisionQueryResponse.FromString,
+        self.CheckAttributeViString = channel.unary_unary(
+                '/niscope_grpc.NiScope/CheckAttributeViString',
+                request_serializer=niscope__pb2.CheckAttributeViStringRequest.SerializeToString,
+                response_deserializer=niscope__pb2.CheckAttributeViStringResponse.FromString,
                 )
-        self.SampleMode = channel.unary_unary(
-                '/niscope_grpc.NiScope/SampleMode',
-                request_serializer=niscope__pb2.SampleModeRequest.SerializeToString,
-                response_deserializer=niscope__pb2.SampleModeResponse.FromString,
+        self.GetAttributeViSession = channel.unary_unary(
+                '/niscope_grpc.NiScope/GetAttributeViSession',
+                request_serializer=niscope__pb2.GetAttributeViSessionRequest.SerializeToString,
+                response_deserializer=niscope__pb2.GetAttributeViSessionResponse.FromString,
                 )
-        self.SampleRate = channel.unary_unary(
-                '/niscope_grpc.NiScope/SampleRate',
-                request_serializer=niscope__pb2.SampleRateRequest.SerializeToString,
-                response_deserializer=niscope__pb2.SampleRateResponse.FromString,
+        self.SetAttributeViSession = channel.unary_unary(
+                '/niscope_grpc.NiScope/SetAttributeViSession',
+                request_serializer=niscope__pb2.SetAttributeViSessionRequest.SerializeToString,
+                response_deserializer=niscope__pb2.SetAttributeViSessionResponse.FromString,
                 )
-        self.SelfTest = channel.unary_unary(
-                '/niscope_grpc.NiScope/SelfTest',
-                request_serializer=niscope__pb2.SelfTestRequest.SerializeToString,
-                response_deserializer=niscope__pb2.SelfTestResponse.FromString,
+        self.CheckAttributeViSession = channel.unary_unary(
+                '/niscope_grpc.NiScope/CheckAttributeViSession',
+                request_serializer=niscope__pb2.CheckAttributeViSessionRequest.SerializeToString,
+                response_deserializer=niscope__pb2.CheckAttributeViSessionResponse.FromString,
                 )
-        self.SendSoftwareTriggerEdge = channel.unary_unary(
-                '/niscope_grpc.NiScope/SendSoftwareTriggerEdge',
-                request_serializer=niscope__pb2.SendSoftwareTriggerEdgeRequest.SerializeToString,
-                response_deserializer=niscope__pb2.SendSoftwareTriggerEdgeResponse.FromString,
+        self.GetAttributeViBoolean = channel.unary_unary(
+                '/niscope_grpc.NiScope/GetAttributeViBoolean',
+                request_serializer=niscope__pb2.GetAttributeViBooleanRequest.SerializeToString,
+                response_deserializer=niscope__pb2.GetAttributeViBooleanResponse.FromString,
                 )
         self.SetAttributeViBoolean = channel.unary_unary(
                 '/niscope_grpc.NiScope/SetAttributeViBoolean',
                 request_serializer=niscope__pb2.SetAttributeViBooleanRequest.SerializeToString,
                 response_deserializer=niscope__pb2.SetAttributeViBooleanResponse.FromString,
                 )
-        self.SetAttributeViInt32 = channel.unary_unary(
-                '/niscope_grpc.NiScope/SetAttributeViInt32',
-                request_serializer=niscope__pb2.SetAttributeViInt32Request.SerializeToString,
-                response_deserializer=niscope__pb2.SetAttributeViInt32Response.FromString,
+        self.CheckAttributeViBoolean = channel.unary_unary(
+                '/niscope_grpc.NiScope/CheckAttributeViBoolean',
+                request_serializer=niscope__pb2.CheckAttributeViBooleanRequest.SerializeToString,
+                response_deserializer=niscope__pb2.CheckAttributeViBooleanResponse.FromString,
                 )
-        self.SetAttributeViInt64 = channel.unary_unary(
-                '/niscope_grpc.NiScope/SetAttributeViInt64',
-                request_serializer=niscope__pb2.SetAttributeViInt64Request.SerializeToString,
-                response_deserializer=niscope__pb2.SetAttributeViInt64Response.FromString,
+        self.ImportAttributeConfigurationBuffer = channel.unary_unary(
+                '/niscope_grpc.NiScope/ImportAttributeConfigurationBuffer',
+                request_serializer=niscope__pb2.ImportAttributeConfigurationBufferRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ImportAttributeConfigurationBufferResponse.FromString,
                 )
-        self.SetAttributeViReal64 = channel.unary_unary(
-                '/niscope_grpc.NiScope/SetAttributeViReal64',
-                request_serializer=niscope__pb2.SetAttributeViReal64Request.SerializeToString,
-                response_deserializer=niscope__pb2.SetAttributeViReal64Response.FromString,
+        self.ExportAttributeConfigurationBuffer = channel.unary_unary(
+                '/niscope_grpc.NiScope/ExportAttributeConfigurationBuffer',
+                request_serializer=niscope__pb2.ExportAttributeConfigurationBufferRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ExportAttributeConfigurationBufferResponse.FromString,
                 )
-        self.SetAttributeViSession = channel.unary_unary(
-                '/niscope_grpc.NiScope/SetAttributeViSession',
-                request_serializer=niscope__pb2.SetAttributeViSessionRequest.SerializeToString,
-                response_deserializer=niscope__pb2.SetAttributeViSessionResponse.FromString,
+        self.ImportAttributeConfigurationFile = channel.unary_unary(
+                '/niscope_grpc.NiScope/ImportAttributeConfigurationFile',
+                request_serializer=niscope__pb2.ImportAttributeConfigurationFileRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ImportAttributeConfigurationFileResponse.FromString,
                 )
-        self.SetAttributeViString = channel.unary_unary(
-                '/niscope_grpc.NiScope/SetAttributeViString',
-                request_serializer=niscope__pb2.SetAttributeViStringRequest.SerializeToString,
-                response_deserializer=niscope__pb2.SetAttributeViStringResponse.FromString,
+        self.ExportAttributeConfigurationFile = channel.unary_unary(
+                '/niscope_grpc.NiScope/ExportAttributeConfigurationFile',
+                request_serializer=niscope__pb2.ExportAttributeConfigurationFileRequest.SerializeToString,
+                response_deserializer=niscope__pb2.ExportAttributeConfigurationFileResponse.FromString,
+                )
+        self.GetScalingCoefficients = channel.unary_unary(
+                '/niscope_grpc.NiScope/GetScalingCoefficients',
+                request_serializer=niscope__pb2.GetScalingCoefficientsRequest.SerializeToString,
+                response_deserializer=niscope__pb2.GetScalingCoefficientsResponse.FromString,
+                )
+        self.GetNormalizationCoefficients = channel.unary_unary(
+                '/niscope_grpc.NiScope/GetNormalizationCoefficients',
+                request_serializer=niscope__pb2.GetNormalizationCoefficientsRequest.SerializeToString,
+                response_deserializer=niscope__pb2.GetNormalizationCoefficientsResponse.FromString,
+                )
+        self.GetStreamEndpointHandle = channel.unary_unary(
+                '/niscope_grpc.NiScope/GetStreamEndpointHandle',
+                request_serializer=niscope__pb2.GetStreamEndpointHandleRequest.SerializeToString,
+                response_deserializer=niscope__pb2.GetStreamEndpointHandleResponse.FromString,
+                )
+        self.CalFetchDate = channel.unary_unary(
+                '/niscope_grpc.NiScope/CalFetchDate',
+                request_serializer=niscope__pb2.CalFetchDateRequest.SerializeToString,
+                response_deserializer=niscope__pb2.CalFetchDateResponse.FromString,
+                )
+        self.CalFetchTemperature = channel.unary_unary(
+                '/niscope_grpc.NiScope/CalFetchTemperature',
+                request_serializer=niscope__pb2.CalFetchTemperatureRequest.SerializeToString,
+                response_deserializer=niscope__pb2.CalFetchTemperatureResponse.FromString,
                 )
 
 
 class NiScopeServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def Abort(self, request, context):
+    def Init(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def AcquisitionStatus(self, request, context):
+    def InitWithOptions(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ActualMeasWfmSize(self, request, context):
+    def Close(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ActualNumWfms(self, request, context):
+    def AutoSetup(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ActualRecordLength(self, request, context):
+    def ConfigureVertical(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def AddWaveformProcessing(self, request, context):
+    def ConfigureChanCharacteristics(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def AdjustSampleClockRelativeDelay(self, request, context):
+    def ConfigureHorizontalTiming(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def AutoSetup(self, request, context):
+    def ConfigureClock(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CableSenseSignalStart(self, request, context):
+    def ExportSignal(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CableSenseSignalStop(self, request, context):
+    def AdjustSampleClockRelativeDelay(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CalFetchDate(self, request, context):
+    def ConfigureTriggerEdge(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CalFetchTemperature(self, request, context):
+    def ConfigureTriggerGlitch(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CalSelfCalibrate(self, request, context):
+    def ConfigureTriggerHysteresis(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CheckAttributeViBoolean(self, request, context):
+    def ConfigureTriggerWindow(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CheckAttributeViInt32(self, request, context):
+    def ConfigureTriggerSoftware(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CheckAttributeViInt64(self, request, context):
+    def SendSoftwareTriggerEdge(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CheckAttributeViReal64(self, request, context):
+    def ConfigureTriggerImmediate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CheckAttributeViSession(self, request, context):
+    def ConfigureTriggerRunt(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CheckAttributeViString(self, request, context):
+    def ConfigureTriggerDigital(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ClearWaveformMeasurementStats(self, request, context):
+    def ConfigureTriggerVideo(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ClearWaveformProcessing(self, request, context):
+    def ConfigureTriggerWidth(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Close(self, request, context):
+    def ConfigureEqualizationFilterCoefficients(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Commit(self, request, context):
+    def GetEqualizationFilterCoefficients(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureAcquisition(self, request, context):
+    def GetFrequencyResponse(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureChanCharacteristics(self, request, context):
+    def ConfigureAcquisition(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureClock(self, request, context):
+    def InitiateAcquisition(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureEqualizationFilterCoefficients(self, request, context):
+    def Abort(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureHorizontalTiming(self, request, context):
+    def Commit(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureTriggerDigital(self, request, context):
+    def Read(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureTriggerEdge(self, request, context):
+    def Fetch(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureTriggerGlitch(self, request, context):
+    def FetchBinary8(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureTriggerHysteresis(self, request, context):
+    def FetchBinary16(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureTriggerImmediate(self, request, context):
+    def FetchBinary32(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureTriggerRunt(self, request, context):
+    def FetchComplex(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureTriggerSoftware(self, request, context):
+    def FetchComplexBinary16(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureTriggerVideo(self, request, context):
+    def AcquisitionStatus(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureTriggerWidth(self, request, context):
+    def ActualNumWfms(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureTriggerWindow(self, request, context):
+    def ActualMeasWfmSize(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ConfigureVertical(self, request, context):
+    def ActualRecordLength(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Disable(self, request, context):
+    def SampleRate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ErrorHandler(self, request, context):
+    def SampleMode(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ExportAttributeConfigurationBuffer(self, request, context):
+    def AddWaveformProcessing(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ExportAttributeConfigurationFile(self, request, context):
+    def ClearWaveformProcessing(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ExportSignal(self, request, context):
+    def ClearWaveformMeasurementStats(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Fetch(self, request, context):
+    def ReadMeasurement(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def FetchArrayMeasurement(self, request, context):
+    def FetchMeasurement(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def FetchBinary16(self, request, context):
+    def FetchMeasurementStats(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def FetchBinary32(self, request, context):
+    def FetchArrayMeasurement(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def FetchBinary8(self, request, context):
+    def Reset(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def FetchComplex(self, request, context):
+    def SelfTest(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def FetchComplexBinary16(self, request, context):
+    def Disable(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def FetchMeasurement(self, request, context):
+    def ResetDevice(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def FetchMeasurementStats(self, request, context):
+    def CalSelfCalibrate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetAttributeViBoolean(self, request, context):
+    def RevisionQuery(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetAttributeViInt32(self, request, context):
+    def ProbeCompensationSignalStart(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetAttributeViInt64(self, request, context):
+    def ProbeCompensationSignalStop(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetAttributeViReal64(self, request, context):
+    def CableSenseSignalStart(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetAttributeViSession(self, request, context):
+    def CableSenseSignalStop(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetAttributeViString(self, request, context):
+    def GetChannelName(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetChannelName(self, request, context):
+    def GetChannelNameFromString(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetChannelNameFromString(self, request, context):
+    def ErrorHandler(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetEqualizationFilterCoefficients(self, request, context):
+    def GetError(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetError(self, request, context):
+    def GetErrorMessage(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetErrorMessage(self, request, context):
+    def GetAttributeViInt32(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetFrequencyResponse(self, request, context):
+    def SetAttributeViInt32(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetNormalizationCoefficients(self, request, context):
+    def CheckAttributeViInt32(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetScalingCoefficients(self, request, context):
+    def GetAttributeViInt64(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetStreamEndpointHandle(self, request, context):
+    def SetAttributeViInt64(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ImportAttributeConfigurationBuffer(self, request, context):
+    def CheckAttributeViInt64(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ImportAttributeConfigurationFile(self, request, context):
+    def GetAttributeViReal64(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Init(self, request, context):
+    def SetAttributeViReal64(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def InitWithOptions(self, request, context):
+    def CheckAttributeViReal64(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def InitiateAcquisition(self, request, context):
+    def GetAttributeViString(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ProbeCompensationSignalStart(self, request, context):
+    def SetAttributeViString(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ProbeCompensationSignalStop(self, request, context):
+    def CheckAttributeViString(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Read(self, request, context):
+    def GetAttributeViSession(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ReadMeasurement(self, request, context):
+    def SetAttributeViSession(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Reset(self, request, context):
+    def CheckAttributeViSession(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ResetDevice(self, request, context):
+    def GetAttributeViBoolean(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def RevisionQuery(self, request, context):
+    def SetAttributeViBoolean(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SampleMode(self, request, context):
+    def CheckAttributeViBoolean(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SampleRate(self, request, context):
+    def ImportAttributeConfigurationBuffer(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SelfTest(self, request, context):
+    def ExportAttributeConfigurationBuffer(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SendSoftwareTriggerEdge(self, request, context):
+    def ImportAttributeConfigurationFile(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetAttributeViBoolean(self, request, context):
+    def ExportAttributeConfigurationFile(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetAttributeViInt32(self, request, context):
+    def GetScalingCoefficients(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetAttributeViInt64(self, request, context):
+    def GetNormalizationCoefficients(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetAttributeViReal64(self, request, context):
+    def GetStreamEndpointHandle(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetAttributeViSession(self, request, context):
+    def CalFetchDate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetAttributeViString(self, request, context):
+    def CalFetchTemperature(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_NiScopeServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'Abort': grpc.unary_unary_rpc_method_handler(
-                    servicer.Abort,
-                    request_deserializer=niscope__pb2.AbortRequest.FromString,
-                    response_serializer=niscope__pb2.AbortResponse.SerializeToString,
-            ),
-            'AcquisitionStatus': grpc.unary_unary_rpc_method_handler(
-                    servicer.AcquisitionStatus,
-                    request_deserializer=niscope__pb2.AcquisitionStatusRequest.FromString,
-                    response_serializer=niscope__pb2.AcquisitionStatusResponse.SerializeToString,
-            ),
-            'ActualMeasWfmSize': grpc.unary_unary_rpc_method_handler(
-                    servicer.ActualMeasWfmSize,
-                    request_deserializer=niscope__pb2.ActualMeasWfmSizeRequest.FromString,
-                    response_serializer=niscope__pb2.ActualMeasWfmSizeResponse.SerializeToString,
-            ),
-            'ActualNumWfms': grpc.unary_unary_rpc_method_handler(
-                    servicer.ActualNumWfms,
-                    request_deserializer=niscope__pb2.ActualNumWfmsRequest.FromString,
-                    response_serializer=niscope__pb2.ActualNumWfmsResponse.SerializeToString,
-            ),
-            'ActualRecordLength': grpc.unary_unary_rpc_method_handler(
-                    servicer.ActualRecordLength,
-                    request_deserializer=niscope__pb2.ActualRecordLengthRequest.FromString,
-                    response_serializer=niscope__pb2.ActualRecordLengthResponse.SerializeToString,
-            ),
-            'AddWaveformProcessing': grpc.unary_unary_rpc_method_handler(
-                    servicer.AddWaveformProcessing,
-                    request_deserializer=niscope__pb2.AddWaveformProcessingRequest.FromString,
-                    response_serializer=niscope__pb2.AddWaveformProcessingResponse.SerializeToString,
-            ),
-            'AdjustSampleClockRelativeDelay': grpc.unary_unary_rpc_method_handler(
-                    servicer.AdjustSampleClockRelativeDelay,
-                    request_deserializer=niscope__pb2.AdjustSampleClockRelativeDelayRequest.FromString,
-                    response_serializer=niscope__pb2.AdjustSampleClockRelativeDelayResponse.SerializeToString,
-            ),
-            'AutoSetup': grpc.unary_unary_rpc_method_handler(
-                    servicer.AutoSetup,
-                    request_deserializer=niscope__pb2.AutoSetupRequest.FromString,
-                    response_serializer=niscope__pb2.AutoSetupResponse.SerializeToString,
-            ),
-            'CableSenseSignalStart': grpc.unary_unary_rpc_method_handler(
-                    servicer.CableSenseSignalStart,
-                    request_deserializer=niscope__pb2.CableSenseSignalStartRequest.FromString,
-                    response_serializer=niscope__pb2.CableSenseSignalStartResponse.SerializeToString,
-            ),
-            'CableSenseSignalStop': grpc.unary_unary_rpc_method_handler(
-                    servicer.CableSenseSignalStop,
-                    request_deserializer=niscope__pb2.CableSenseSignalStopRequest.FromString,
-                    response_serializer=niscope__pb2.CableSenseSignalStopResponse.SerializeToString,
-            ),
-            'CalFetchDate': grpc.unary_unary_rpc_method_handler(
-                    servicer.CalFetchDate,
-                    request_deserializer=niscope__pb2.CalFetchDateRequest.FromString,
-                    response_serializer=niscope__pb2.CalFetchDateResponse.SerializeToString,
-            ),
-            'CalFetchTemperature': grpc.unary_unary_rpc_method_handler(
-                    servicer.CalFetchTemperature,
-                    request_deserializer=niscope__pb2.CalFetchTemperatureRequest.FromString,
-                    response_serializer=niscope__pb2.CalFetchTemperatureResponse.SerializeToString,
-            ),
-            'CalSelfCalibrate': grpc.unary_unary_rpc_method_handler(
-                    servicer.CalSelfCalibrate,
-                    request_deserializer=niscope__pb2.CalSelfCalibrateRequest.FromString,
-                    response_serializer=niscope__pb2.CalSelfCalibrateResponse.SerializeToString,
-            ),
-            'CheckAttributeViBoolean': grpc.unary_unary_rpc_method_handler(
-                    servicer.CheckAttributeViBoolean,
-                    request_deserializer=niscope__pb2.CheckAttributeViBooleanRequest.FromString,
-                    response_serializer=niscope__pb2.CheckAttributeViBooleanResponse.SerializeToString,
-            ),
-            'CheckAttributeViInt32': grpc.unary_unary_rpc_method_handler(
-                    servicer.CheckAttributeViInt32,
-                    request_deserializer=niscope__pb2.CheckAttributeViInt32Request.FromString,
-                    response_serializer=niscope__pb2.CheckAttributeViInt32Response.SerializeToString,
-            ),
-            'CheckAttributeViInt64': grpc.unary_unary_rpc_method_handler(
-                    servicer.CheckAttributeViInt64,
-                    request_deserializer=niscope__pb2.CheckAttributeViInt64Request.FromString,
-                    response_serializer=niscope__pb2.CheckAttributeViInt64Response.SerializeToString,
-            ),
-            'CheckAttributeViReal64': grpc.unary_unary_rpc_method_handler(
-                    servicer.CheckAttributeViReal64,
-                    request_deserializer=niscope__pb2.CheckAttributeViReal64Request.FromString,
-                    response_serializer=niscope__pb2.CheckAttributeViReal64Response.SerializeToString,
-            ),
-            'CheckAttributeViSession': grpc.unary_unary_rpc_method_handler(
-                    servicer.CheckAttributeViSession,
-                    request_deserializer=niscope__pb2.CheckAttributeViSessionRequest.FromString,
-                    response_serializer=niscope__pb2.CheckAttributeViSessionResponse.SerializeToString,
-            ),
-            'CheckAttributeViString': grpc.unary_unary_rpc_method_handler(
-                    servicer.CheckAttributeViString,
-                    request_deserializer=niscope__pb2.CheckAttributeViStringRequest.FromString,
-                    response_serializer=niscope__pb2.CheckAttributeViStringResponse.SerializeToString,
-            ),
-            'ClearWaveformMeasurementStats': grpc.unary_unary_rpc_method_handler(
-                    servicer.ClearWaveformMeasurementStats,
-                    request_deserializer=niscope__pb2.ClearWaveformMeasurementStatsRequest.FromString,
-                    response_serializer=niscope__pb2.ClearWaveformMeasurementStatsResponse.SerializeToString,
+            'Init': grpc.unary_unary_rpc_method_handler(
+                    servicer.Init,
+                    request_deserializer=niscope__pb2.InitRequest.FromString,
+                    response_serializer=niscope__pb2.InitResponse.SerializeToString,
             ),
-            'ClearWaveformProcessing': grpc.unary_unary_rpc_method_handler(
-                    servicer.ClearWaveformProcessing,
-                    request_deserializer=niscope__pb2.ClearWaveformProcessingRequest.FromString,
-                    response_serializer=niscope__pb2.ClearWaveformProcessingResponse.SerializeToString,
+            'InitWithOptions': grpc.unary_unary_rpc_method_handler(
+                    servicer.InitWithOptions,
+                    request_deserializer=niscope__pb2.InitWithOptionsRequest.FromString,
+                    response_serializer=niscope__pb2.InitWithOptionsResponse.SerializeToString,
             ),
             'Close': grpc.unary_unary_rpc_method_handler(
                     servicer.Close,
                     request_deserializer=niscope__pb2.CloseRequest.FromString,
                     response_serializer=niscope__pb2.CloseResponse.SerializeToString,
             ),
-            'Commit': grpc.unary_unary_rpc_method_handler(
-                    servicer.Commit,
-                    request_deserializer=niscope__pb2.CommitRequest.FromString,
-                    response_serializer=niscope__pb2.CommitResponse.SerializeToString,
+            'AutoSetup': grpc.unary_unary_rpc_method_handler(
+                    servicer.AutoSetup,
+                    request_deserializer=niscope__pb2.AutoSetupRequest.FromString,
+                    response_serializer=niscope__pb2.AutoSetupResponse.SerializeToString,
             ),
-            'ConfigureAcquisition': grpc.unary_unary_rpc_method_handler(
-                    servicer.ConfigureAcquisition,
-                    request_deserializer=niscope__pb2.ConfigureAcquisitionRequest.FromString,
-                    response_serializer=niscope__pb2.ConfigureAcquisitionResponse.SerializeToString,
+            'ConfigureVertical': grpc.unary_unary_rpc_method_handler(
+                    servicer.ConfigureVertical,
+                    request_deserializer=niscope__pb2.ConfigureVerticalRequest.FromString,
+                    response_serializer=niscope__pb2.ConfigureVerticalResponse.SerializeToString,
             ),
             'ConfigureChanCharacteristics': grpc.unary_unary_rpc_method_handler(
                     servicer.ConfigureChanCharacteristics,
                     request_deserializer=niscope__pb2.ConfigureChanCharacteristicsRequest.FromString,
                     response_serializer=niscope__pb2.ConfigureChanCharacteristicsResponse.SerializeToString,
             ),
+            'ConfigureHorizontalTiming': grpc.unary_unary_rpc_method_handler(
+                    servicer.ConfigureHorizontalTiming,
+                    request_deserializer=niscope__pb2.ConfigureHorizontalTimingRequest.FromString,
+                    response_serializer=niscope__pb2.ConfigureHorizontalTimingResponse.SerializeToString,
+            ),
             'ConfigureClock': grpc.unary_unary_rpc_method_handler(
                     servicer.ConfigureClock,
                     request_deserializer=niscope__pb2.ConfigureClockRequest.FromString,
                     response_serializer=niscope__pb2.ConfigureClockResponse.SerializeToString,
             ),
-            'ConfigureEqualizationFilterCoefficients': grpc.unary_unary_rpc_method_handler(
-                    servicer.ConfigureEqualizationFilterCoefficients,
-                    request_deserializer=niscope__pb2.ConfigureEqualizationFilterCoefficientsRequest.FromString,
-                    response_serializer=niscope__pb2.ConfigureEqualizationFilterCoefficientsResponse.SerializeToString,
-            ),
-            'ConfigureHorizontalTiming': grpc.unary_unary_rpc_method_handler(
-                    servicer.ConfigureHorizontalTiming,
-                    request_deserializer=niscope__pb2.ConfigureHorizontalTimingRequest.FromString,
-                    response_serializer=niscope__pb2.ConfigureHorizontalTimingResponse.SerializeToString,
+            'ExportSignal': grpc.unary_unary_rpc_method_handler(
+                    servicer.ExportSignal,
+                    request_deserializer=niscope__pb2.ExportSignalRequest.FromString,
+                    response_serializer=niscope__pb2.ExportSignalResponse.SerializeToString,
             ),
-            'ConfigureTriggerDigital': grpc.unary_unary_rpc_method_handler(
-                    servicer.ConfigureTriggerDigital,
-                    request_deserializer=niscope__pb2.ConfigureTriggerDigitalRequest.FromString,
-                    response_serializer=niscope__pb2.ConfigureTriggerDigitalResponse.SerializeToString,
+            'AdjustSampleClockRelativeDelay': grpc.unary_unary_rpc_method_handler(
+                    servicer.AdjustSampleClockRelativeDelay,
+                    request_deserializer=niscope__pb2.AdjustSampleClockRelativeDelayRequest.FromString,
+                    response_serializer=niscope__pb2.AdjustSampleClockRelativeDelayResponse.SerializeToString,
             ),
             'ConfigureTriggerEdge': grpc.unary_unary_rpc_method_handler(
                     servicer.ConfigureTriggerEdge,
                     request_deserializer=niscope__pb2.ConfigureTriggerEdgeRequest.FromString,
                     response_serializer=niscope__pb2.ConfigureTriggerEdgeResponse.SerializeToString,
             ),
             'ConfigureTriggerGlitch': grpc.unary_unary_rpc_method_handler(
@@ -1168,1314 +1073,1392 @@
                     response_serializer=niscope__pb2.ConfigureTriggerGlitchResponse.SerializeToString,
             ),
             'ConfigureTriggerHysteresis': grpc.unary_unary_rpc_method_handler(
                     servicer.ConfigureTriggerHysteresis,
                     request_deserializer=niscope__pb2.ConfigureTriggerHysteresisRequest.FromString,
                     response_serializer=niscope__pb2.ConfigureTriggerHysteresisResponse.SerializeToString,
             ),
+            'ConfigureTriggerWindow': grpc.unary_unary_rpc_method_handler(
+                    servicer.ConfigureTriggerWindow,
+                    request_deserializer=niscope__pb2.ConfigureTriggerWindowRequest.FromString,
+                    response_serializer=niscope__pb2.ConfigureTriggerWindowResponse.SerializeToString,
+            ),
+            'ConfigureTriggerSoftware': grpc.unary_unary_rpc_method_handler(
+                    servicer.ConfigureTriggerSoftware,
+                    request_deserializer=niscope__pb2.ConfigureTriggerSoftwareRequest.FromString,
+                    response_serializer=niscope__pb2.ConfigureTriggerSoftwareResponse.SerializeToString,
+            ),
+            'SendSoftwareTriggerEdge': grpc.unary_unary_rpc_method_handler(
+                    servicer.SendSoftwareTriggerEdge,
+                    request_deserializer=niscope__pb2.SendSoftwareTriggerEdgeRequest.FromString,
+                    response_serializer=niscope__pb2.SendSoftwareTriggerEdgeResponse.SerializeToString,
+            ),
             'ConfigureTriggerImmediate': grpc.unary_unary_rpc_method_handler(
                     servicer.ConfigureTriggerImmediate,
                     request_deserializer=niscope__pb2.ConfigureTriggerImmediateRequest.FromString,
                     response_serializer=niscope__pb2.ConfigureTriggerImmediateResponse.SerializeToString,
             ),
             'ConfigureTriggerRunt': grpc.unary_unary_rpc_method_handler(
                     servicer.ConfigureTriggerRunt,
                     request_deserializer=niscope__pb2.ConfigureTriggerRuntRequest.FromString,
                     response_serializer=niscope__pb2.ConfigureTriggerRuntResponse.SerializeToString,
             ),
-            'ConfigureTriggerSoftware': grpc.unary_unary_rpc_method_handler(
-                    servicer.ConfigureTriggerSoftware,
-                    request_deserializer=niscope__pb2.ConfigureTriggerSoftwareRequest.FromString,
-                    response_serializer=niscope__pb2.ConfigureTriggerSoftwareResponse.SerializeToString,
+            'ConfigureTriggerDigital': grpc.unary_unary_rpc_method_handler(
+                    servicer.ConfigureTriggerDigital,
+                    request_deserializer=niscope__pb2.ConfigureTriggerDigitalRequest.FromString,
+                    response_serializer=niscope__pb2.ConfigureTriggerDigitalResponse.SerializeToString,
             ),
             'ConfigureTriggerVideo': grpc.unary_unary_rpc_method_handler(
                     servicer.ConfigureTriggerVideo,
                     request_deserializer=niscope__pb2.ConfigureTriggerVideoRequest.FromString,
                     response_serializer=niscope__pb2.ConfigureTriggerVideoResponse.SerializeToString,
             ),
             'ConfigureTriggerWidth': grpc.unary_unary_rpc_method_handler(
                     servicer.ConfigureTriggerWidth,
                     request_deserializer=niscope__pb2.ConfigureTriggerWidthRequest.FromString,
                     response_serializer=niscope__pb2.ConfigureTriggerWidthResponse.SerializeToString,
             ),
-            'ConfigureTriggerWindow': grpc.unary_unary_rpc_method_handler(
-                    servicer.ConfigureTriggerWindow,
-                    request_deserializer=niscope__pb2.ConfigureTriggerWindowRequest.FromString,
-                    response_serializer=niscope__pb2.ConfigureTriggerWindowResponse.SerializeToString,
+            'ConfigureEqualizationFilterCoefficients': grpc.unary_unary_rpc_method_handler(
+                    servicer.ConfigureEqualizationFilterCoefficients,
+                    request_deserializer=niscope__pb2.ConfigureEqualizationFilterCoefficientsRequest.FromString,
+                    response_serializer=niscope__pb2.ConfigureEqualizationFilterCoefficientsResponse.SerializeToString,
             ),
-            'ConfigureVertical': grpc.unary_unary_rpc_method_handler(
-                    servicer.ConfigureVertical,
-                    request_deserializer=niscope__pb2.ConfigureVerticalRequest.FromString,
-                    response_serializer=niscope__pb2.ConfigureVerticalResponse.SerializeToString,
+            'GetEqualizationFilterCoefficients': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetEqualizationFilterCoefficients,
+                    request_deserializer=niscope__pb2.GetEqualizationFilterCoefficientsRequest.FromString,
+                    response_serializer=niscope__pb2.GetEqualizationFilterCoefficientsResponse.SerializeToString,
             ),
-            'Disable': grpc.unary_unary_rpc_method_handler(
-                    servicer.Disable,
-                    request_deserializer=niscope__pb2.DisableRequest.FromString,
-                    response_serializer=niscope__pb2.DisableResponse.SerializeToString,
+            'GetFrequencyResponse': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetFrequencyResponse,
+                    request_deserializer=niscope__pb2.GetFrequencyResponseRequest.FromString,
+                    response_serializer=niscope__pb2.GetFrequencyResponseResponse.SerializeToString,
             ),
-            'ErrorHandler': grpc.unary_unary_rpc_method_handler(
-                    servicer.ErrorHandler,
-                    request_deserializer=niscope__pb2.ErrorHandlerRequest.FromString,
-                    response_serializer=niscope__pb2.ErrorHandlerResponse.SerializeToString,
+            'ConfigureAcquisition': grpc.unary_unary_rpc_method_handler(
+                    servicer.ConfigureAcquisition,
+                    request_deserializer=niscope__pb2.ConfigureAcquisitionRequest.FromString,
+                    response_serializer=niscope__pb2.ConfigureAcquisitionResponse.SerializeToString,
             ),
-            'ExportAttributeConfigurationBuffer': grpc.unary_unary_rpc_method_handler(
-                    servicer.ExportAttributeConfigurationBuffer,
-                    request_deserializer=niscope__pb2.ExportAttributeConfigurationBufferRequest.FromString,
-                    response_serializer=niscope__pb2.ExportAttributeConfigurationBufferResponse.SerializeToString,
+            'InitiateAcquisition': grpc.unary_unary_rpc_method_handler(
+                    servicer.InitiateAcquisition,
+                    request_deserializer=niscope__pb2.InitiateAcquisitionRequest.FromString,
+                    response_serializer=niscope__pb2.InitiateAcquisitionResponse.SerializeToString,
             ),
-            'ExportAttributeConfigurationFile': grpc.unary_unary_rpc_method_handler(
-                    servicer.ExportAttributeConfigurationFile,
-                    request_deserializer=niscope__pb2.ExportAttributeConfigurationFileRequest.FromString,
-                    response_serializer=niscope__pb2.ExportAttributeConfigurationFileResponse.SerializeToString,
+            'Abort': grpc.unary_unary_rpc_method_handler(
+                    servicer.Abort,
+                    request_deserializer=niscope__pb2.AbortRequest.FromString,
+                    response_serializer=niscope__pb2.AbortResponse.SerializeToString,
             ),
-            'ExportSignal': grpc.unary_unary_rpc_method_handler(
-                    servicer.ExportSignal,
-                    request_deserializer=niscope__pb2.ExportSignalRequest.FromString,
-                    response_serializer=niscope__pb2.ExportSignalResponse.SerializeToString,
+            'Commit': grpc.unary_unary_rpc_method_handler(
+                    servicer.Commit,
+                    request_deserializer=niscope__pb2.CommitRequest.FromString,
+                    response_serializer=niscope__pb2.CommitResponse.SerializeToString,
+            ),
+            'Read': grpc.unary_unary_rpc_method_handler(
+                    servicer.Read,
+                    request_deserializer=niscope__pb2.ReadRequest.FromString,
+                    response_serializer=niscope__pb2.ReadResponse.SerializeToString,
             ),
             'Fetch': grpc.unary_unary_rpc_method_handler(
                     servicer.Fetch,
                     request_deserializer=niscope__pb2.FetchRequest.FromString,
                     response_serializer=niscope__pb2.FetchResponse.SerializeToString,
             ),
-            'FetchArrayMeasurement': grpc.unary_unary_rpc_method_handler(
-                    servicer.FetchArrayMeasurement,
-                    request_deserializer=niscope__pb2.FetchArrayMeasurementRequest.FromString,
-                    response_serializer=niscope__pb2.FetchArrayMeasurementResponse.SerializeToString,
+            'FetchBinary8': grpc.unary_unary_rpc_method_handler(
+                    servicer.FetchBinary8,
+                    request_deserializer=niscope__pb2.FetchBinary8Request.FromString,
+                    response_serializer=niscope__pb2.FetchBinary8Response.SerializeToString,
             ),
             'FetchBinary16': grpc.unary_unary_rpc_method_handler(
                     servicer.FetchBinary16,
                     request_deserializer=niscope__pb2.FetchBinary16Request.FromString,
                     response_serializer=niscope__pb2.FetchBinary16Response.SerializeToString,
             ),
             'FetchBinary32': grpc.unary_unary_rpc_method_handler(
                     servicer.FetchBinary32,
                     request_deserializer=niscope__pb2.FetchBinary32Request.FromString,
                     response_serializer=niscope__pb2.FetchBinary32Response.SerializeToString,
             ),
-            'FetchBinary8': grpc.unary_unary_rpc_method_handler(
-                    servicer.FetchBinary8,
-                    request_deserializer=niscope__pb2.FetchBinary8Request.FromString,
-                    response_serializer=niscope__pb2.FetchBinary8Response.SerializeToString,
-            ),
             'FetchComplex': grpc.unary_unary_rpc_method_handler(
                     servicer.FetchComplex,
                     request_deserializer=niscope__pb2.FetchComplexRequest.FromString,
                     response_serializer=niscope__pb2.FetchComplexResponse.SerializeToString,
             ),
             'FetchComplexBinary16': grpc.unary_unary_rpc_method_handler(
                     servicer.FetchComplexBinary16,
                     request_deserializer=niscope__pb2.FetchComplexBinary16Request.FromString,
                     response_serializer=niscope__pb2.FetchComplexBinary16Response.SerializeToString,
             ),
+            'AcquisitionStatus': grpc.unary_unary_rpc_method_handler(
+                    servicer.AcquisitionStatus,
+                    request_deserializer=niscope__pb2.AcquisitionStatusRequest.FromString,
+                    response_serializer=niscope__pb2.AcquisitionStatusResponse.SerializeToString,
+            ),
+            'ActualNumWfms': grpc.unary_unary_rpc_method_handler(
+                    servicer.ActualNumWfms,
+                    request_deserializer=niscope__pb2.ActualNumWfmsRequest.FromString,
+                    response_serializer=niscope__pb2.ActualNumWfmsResponse.SerializeToString,
+            ),
+            'ActualMeasWfmSize': grpc.unary_unary_rpc_method_handler(
+                    servicer.ActualMeasWfmSize,
+                    request_deserializer=niscope__pb2.ActualMeasWfmSizeRequest.FromString,
+                    response_serializer=niscope__pb2.ActualMeasWfmSizeResponse.SerializeToString,
+            ),
+            'ActualRecordLength': grpc.unary_unary_rpc_method_handler(
+                    servicer.ActualRecordLength,
+                    request_deserializer=niscope__pb2.ActualRecordLengthRequest.FromString,
+                    response_serializer=niscope__pb2.ActualRecordLengthResponse.SerializeToString,
+            ),
+            'SampleRate': grpc.unary_unary_rpc_method_handler(
+                    servicer.SampleRate,
+                    request_deserializer=niscope__pb2.SampleRateRequest.FromString,
+                    response_serializer=niscope__pb2.SampleRateResponse.SerializeToString,
+            ),
+            'SampleMode': grpc.unary_unary_rpc_method_handler(
+                    servicer.SampleMode,
+                    request_deserializer=niscope__pb2.SampleModeRequest.FromString,
+                    response_serializer=niscope__pb2.SampleModeResponse.SerializeToString,
+            ),
+            'AddWaveformProcessing': grpc.unary_unary_rpc_method_handler(
+                    servicer.AddWaveformProcessing,
+                    request_deserializer=niscope__pb2.AddWaveformProcessingRequest.FromString,
+                    response_serializer=niscope__pb2.AddWaveformProcessingResponse.SerializeToString,
+            ),
+            'ClearWaveformProcessing': grpc.unary_unary_rpc_method_handler(
+                    servicer.ClearWaveformProcessing,
+                    request_deserializer=niscope__pb2.ClearWaveformProcessingRequest.FromString,
+                    response_serializer=niscope__pb2.ClearWaveformProcessingResponse.SerializeToString,
+            ),
+            'ClearWaveformMeasurementStats': grpc.unary_unary_rpc_method_handler(
+                    servicer.ClearWaveformMeasurementStats,
+                    request_deserializer=niscope__pb2.ClearWaveformMeasurementStatsRequest.FromString,
+                    response_serializer=niscope__pb2.ClearWaveformMeasurementStatsResponse.SerializeToString,
+            ),
+            'ReadMeasurement': grpc.unary_unary_rpc_method_handler(
+                    servicer.ReadMeasurement,
+                    request_deserializer=niscope__pb2.ReadMeasurementRequest.FromString,
+                    response_serializer=niscope__pb2.ReadMeasurementResponse.SerializeToString,
+            ),
             'FetchMeasurement': grpc.unary_unary_rpc_method_handler(
                     servicer.FetchMeasurement,
                     request_deserializer=niscope__pb2.FetchMeasurementRequest.FromString,
                     response_serializer=niscope__pb2.FetchMeasurementResponse.SerializeToString,
             ),
             'FetchMeasurementStats': grpc.unary_unary_rpc_method_handler(
                     servicer.FetchMeasurementStats,
                     request_deserializer=niscope__pb2.FetchMeasurementStatsRequest.FromString,
                     response_serializer=niscope__pb2.FetchMeasurementStatsResponse.SerializeToString,
             ),
-            'GetAttributeViBoolean': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAttributeViBoolean,
-                    request_deserializer=niscope__pb2.GetAttributeViBooleanRequest.FromString,
-                    response_serializer=niscope__pb2.GetAttributeViBooleanResponse.SerializeToString,
+            'FetchArrayMeasurement': grpc.unary_unary_rpc_method_handler(
+                    servicer.FetchArrayMeasurement,
+                    request_deserializer=niscope__pb2.FetchArrayMeasurementRequest.FromString,
+                    response_serializer=niscope__pb2.FetchArrayMeasurementResponse.SerializeToString,
             ),
-            'GetAttributeViInt32': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAttributeViInt32,
-                    request_deserializer=niscope__pb2.GetAttributeViInt32Request.FromString,
-                    response_serializer=niscope__pb2.GetAttributeViInt32Response.SerializeToString,
+            'Reset': grpc.unary_unary_rpc_method_handler(
+                    servicer.Reset,
+                    request_deserializer=niscope__pb2.ResetRequest.FromString,
+                    response_serializer=niscope__pb2.ResetResponse.SerializeToString,
             ),
-            'GetAttributeViInt64': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAttributeViInt64,
-                    request_deserializer=niscope__pb2.GetAttributeViInt64Request.FromString,
-                    response_serializer=niscope__pb2.GetAttributeViInt64Response.SerializeToString,
+            'SelfTest': grpc.unary_unary_rpc_method_handler(
+                    servicer.SelfTest,
+                    request_deserializer=niscope__pb2.SelfTestRequest.FromString,
+                    response_serializer=niscope__pb2.SelfTestResponse.SerializeToString,
             ),
-            'GetAttributeViReal64': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAttributeViReal64,
-                    request_deserializer=niscope__pb2.GetAttributeViReal64Request.FromString,
-                    response_serializer=niscope__pb2.GetAttributeViReal64Response.SerializeToString,
+            'Disable': grpc.unary_unary_rpc_method_handler(
+                    servicer.Disable,
+                    request_deserializer=niscope__pb2.DisableRequest.FromString,
+                    response_serializer=niscope__pb2.DisableResponse.SerializeToString,
             ),
-            'GetAttributeViSession': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAttributeViSession,
-                    request_deserializer=niscope__pb2.GetAttributeViSessionRequest.FromString,
-                    response_serializer=niscope__pb2.GetAttributeViSessionResponse.SerializeToString,
+            'ResetDevice': grpc.unary_unary_rpc_method_handler(
+                    servicer.ResetDevice,
+                    request_deserializer=niscope__pb2.ResetDeviceRequest.FromString,
+                    response_serializer=niscope__pb2.ResetDeviceResponse.SerializeToString,
             ),
-            'GetAttributeViString': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAttributeViString,
-                    request_deserializer=niscope__pb2.GetAttributeViStringRequest.FromString,
-                    response_serializer=niscope__pb2.GetAttributeViStringResponse.SerializeToString,
+            'CalSelfCalibrate': grpc.unary_unary_rpc_method_handler(
+                    servicer.CalSelfCalibrate,
+                    request_deserializer=niscope__pb2.CalSelfCalibrateRequest.FromString,
+                    response_serializer=niscope__pb2.CalSelfCalibrateResponse.SerializeToString,
+            ),
+            'RevisionQuery': grpc.unary_unary_rpc_method_handler(
+                    servicer.RevisionQuery,
+                    request_deserializer=niscope__pb2.RevisionQueryRequest.FromString,
+                    response_serializer=niscope__pb2.RevisionQueryResponse.SerializeToString,
+            ),
+            'ProbeCompensationSignalStart': grpc.unary_unary_rpc_method_handler(
+                    servicer.ProbeCompensationSignalStart,
+                    request_deserializer=niscope__pb2.ProbeCompensationSignalStartRequest.FromString,
+                    response_serializer=niscope__pb2.ProbeCompensationSignalStartResponse.SerializeToString,
+            ),
+            'ProbeCompensationSignalStop': grpc.unary_unary_rpc_method_handler(
+                    servicer.ProbeCompensationSignalStop,
+                    request_deserializer=niscope__pb2.ProbeCompensationSignalStopRequest.FromString,
+                    response_serializer=niscope__pb2.ProbeCompensationSignalStopResponse.SerializeToString,
+            ),
+            'CableSenseSignalStart': grpc.unary_unary_rpc_method_handler(
+                    servicer.CableSenseSignalStart,
+                    request_deserializer=niscope__pb2.CableSenseSignalStartRequest.FromString,
+                    response_serializer=niscope__pb2.CableSenseSignalStartResponse.SerializeToString,
+            ),
+            'CableSenseSignalStop': grpc.unary_unary_rpc_method_handler(
+                    servicer.CableSenseSignalStop,
+                    request_deserializer=niscope__pb2.CableSenseSignalStopRequest.FromString,
+                    response_serializer=niscope__pb2.CableSenseSignalStopResponse.SerializeToString,
             ),
             'GetChannelName': grpc.unary_unary_rpc_method_handler(
                     servicer.GetChannelName,
                     request_deserializer=niscope__pb2.GetChannelNameRequest.FromString,
                     response_serializer=niscope__pb2.GetChannelNameResponse.SerializeToString,
             ),
             'GetChannelNameFromString': grpc.unary_unary_rpc_method_handler(
                     servicer.GetChannelNameFromString,
                     request_deserializer=niscope__pb2.GetChannelNameFromStringRequest.FromString,
                     response_serializer=niscope__pb2.GetChannelNameFromStringResponse.SerializeToString,
             ),
-            'GetEqualizationFilterCoefficients': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetEqualizationFilterCoefficients,
-                    request_deserializer=niscope__pb2.GetEqualizationFilterCoefficientsRequest.FromString,
-                    response_serializer=niscope__pb2.GetEqualizationFilterCoefficientsResponse.SerializeToString,
+            'ErrorHandler': grpc.unary_unary_rpc_method_handler(
+                    servicer.ErrorHandler,
+                    request_deserializer=niscope__pb2.ErrorHandlerRequest.FromString,
+                    response_serializer=niscope__pb2.ErrorHandlerResponse.SerializeToString,
             ),
             'GetError': grpc.unary_unary_rpc_method_handler(
                     servicer.GetError,
                     request_deserializer=niscope__pb2.GetErrorRequest.FromString,
                     response_serializer=niscope__pb2.GetErrorResponse.SerializeToString,
             ),
             'GetErrorMessage': grpc.unary_unary_rpc_method_handler(
                     servicer.GetErrorMessage,
                     request_deserializer=niscope__pb2.GetErrorMessageRequest.FromString,
                     response_serializer=niscope__pb2.GetErrorMessageResponse.SerializeToString,
             ),
-            'GetFrequencyResponse': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetFrequencyResponse,
-                    request_deserializer=niscope__pb2.GetFrequencyResponseRequest.FromString,
-                    response_serializer=niscope__pb2.GetFrequencyResponseResponse.SerializeToString,
-            ),
-            'GetNormalizationCoefficients': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetNormalizationCoefficients,
-                    request_deserializer=niscope__pb2.GetNormalizationCoefficientsRequest.FromString,
-                    response_serializer=niscope__pb2.GetNormalizationCoefficientsResponse.SerializeToString,
-            ),
-            'GetScalingCoefficients': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetScalingCoefficients,
-                    request_deserializer=niscope__pb2.GetScalingCoefficientsRequest.FromString,
-                    response_serializer=niscope__pb2.GetScalingCoefficientsResponse.SerializeToString,
-            ),
-            'GetStreamEndpointHandle': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetStreamEndpointHandle,
-                    request_deserializer=niscope__pb2.GetStreamEndpointHandleRequest.FromString,
-                    response_serializer=niscope__pb2.GetStreamEndpointHandleResponse.SerializeToString,
-            ),
-            'ImportAttributeConfigurationBuffer': grpc.unary_unary_rpc_method_handler(
-                    servicer.ImportAttributeConfigurationBuffer,
-                    request_deserializer=niscope__pb2.ImportAttributeConfigurationBufferRequest.FromString,
-                    response_serializer=niscope__pb2.ImportAttributeConfigurationBufferResponse.SerializeToString,
+            'GetAttributeViInt32': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAttributeViInt32,
+                    request_deserializer=niscope__pb2.GetAttributeViInt32Request.FromString,
+                    response_serializer=niscope__pb2.GetAttributeViInt32Response.SerializeToString,
             ),
-            'ImportAttributeConfigurationFile': grpc.unary_unary_rpc_method_handler(
-                    servicer.ImportAttributeConfigurationFile,
-                    request_deserializer=niscope__pb2.ImportAttributeConfigurationFileRequest.FromString,
-                    response_serializer=niscope__pb2.ImportAttributeConfigurationFileResponse.SerializeToString,
+            'SetAttributeViInt32': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetAttributeViInt32,
+                    request_deserializer=niscope__pb2.SetAttributeViInt32Request.FromString,
+                    response_serializer=niscope__pb2.SetAttributeViInt32Response.SerializeToString,
             ),
-            'Init': grpc.unary_unary_rpc_method_handler(
-                    servicer.Init,
-                    request_deserializer=niscope__pb2.InitRequest.FromString,
-                    response_serializer=niscope__pb2.InitResponse.SerializeToString,
+            'CheckAttributeViInt32': grpc.unary_unary_rpc_method_handler(
+                    servicer.CheckAttributeViInt32,
+                    request_deserializer=niscope__pb2.CheckAttributeViInt32Request.FromString,
+                    response_serializer=niscope__pb2.CheckAttributeViInt32Response.SerializeToString,
             ),
-            'InitWithOptions': grpc.unary_unary_rpc_method_handler(
-                    servicer.InitWithOptions,
-                    request_deserializer=niscope__pb2.InitWithOptionsRequest.FromString,
-                    response_serializer=niscope__pb2.InitWithOptionsResponse.SerializeToString,
+            'GetAttributeViInt64': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAttributeViInt64,
+                    request_deserializer=niscope__pb2.GetAttributeViInt64Request.FromString,
+                    response_serializer=niscope__pb2.GetAttributeViInt64Response.SerializeToString,
             ),
-            'InitiateAcquisition': grpc.unary_unary_rpc_method_handler(
-                    servicer.InitiateAcquisition,
-                    request_deserializer=niscope__pb2.InitiateAcquisitionRequest.FromString,
-                    response_serializer=niscope__pb2.InitiateAcquisitionResponse.SerializeToString,
+            'SetAttributeViInt64': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetAttributeViInt64,
+                    request_deserializer=niscope__pb2.SetAttributeViInt64Request.FromString,
+                    response_serializer=niscope__pb2.SetAttributeViInt64Response.SerializeToString,
             ),
-            'ProbeCompensationSignalStart': grpc.unary_unary_rpc_method_handler(
-                    servicer.ProbeCompensationSignalStart,
-                    request_deserializer=niscope__pb2.ProbeCompensationSignalStartRequest.FromString,
-                    response_serializer=niscope__pb2.ProbeCompensationSignalStartResponse.SerializeToString,
+            'CheckAttributeViInt64': grpc.unary_unary_rpc_method_handler(
+                    servicer.CheckAttributeViInt64,
+                    request_deserializer=niscope__pb2.CheckAttributeViInt64Request.FromString,
+                    response_serializer=niscope__pb2.CheckAttributeViInt64Response.SerializeToString,
             ),
-            'ProbeCompensationSignalStop': grpc.unary_unary_rpc_method_handler(
-                    servicer.ProbeCompensationSignalStop,
-                    request_deserializer=niscope__pb2.ProbeCompensationSignalStopRequest.FromString,
-                    response_serializer=niscope__pb2.ProbeCompensationSignalStopResponse.SerializeToString,
+            'GetAttributeViReal64': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAttributeViReal64,
+                    request_deserializer=niscope__pb2.GetAttributeViReal64Request.FromString,
+                    response_serializer=niscope__pb2.GetAttributeViReal64Response.SerializeToString,
             ),
-            'Read': grpc.unary_unary_rpc_method_handler(
-                    servicer.Read,
-                    request_deserializer=niscope__pb2.ReadRequest.FromString,
-                    response_serializer=niscope__pb2.ReadResponse.SerializeToString,
+            'SetAttributeViReal64': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetAttributeViReal64,
+                    request_deserializer=niscope__pb2.SetAttributeViReal64Request.FromString,
+                    response_serializer=niscope__pb2.SetAttributeViReal64Response.SerializeToString,
             ),
-            'ReadMeasurement': grpc.unary_unary_rpc_method_handler(
-                    servicer.ReadMeasurement,
-                    request_deserializer=niscope__pb2.ReadMeasurementRequest.FromString,
-                    response_serializer=niscope__pb2.ReadMeasurementResponse.SerializeToString,
+            'CheckAttributeViReal64': grpc.unary_unary_rpc_method_handler(
+                    servicer.CheckAttributeViReal64,
+                    request_deserializer=niscope__pb2.CheckAttributeViReal64Request.FromString,
+                    response_serializer=niscope__pb2.CheckAttributeViReal64Response.SerializeToString,
             ),
-            'Reset': grpc.unary_unary_rpc_method_handler(
-                    servicer.Reset,
-                    request_deserializer=niscope__pb2.ResetRequest.FromString,
-                    response_serializer=niscope__pb2.ResetResponse.SerializeToString,
+            'GetAttributeViString': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAttributeViString,
+                    request_deserializer=niscope__pb2.GetAttributeViStringRequest.FromString,
+                    response_serializer=niscope__pb2.GetAttributeViStringResponse.SerializeToString,
             ),
-            'ResetDevice': grpc.unary_unary_rpc_method_handler(
-                    servicer.ResetDevice,
-                    request_deserializer=niscope__pb2.ResetDeviceRequest.FromString,
-                    response_serializer=niscope__pb2.ResetDeviceResponse.SerializeToString,
+            'SetAttributeViString': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetAttributeViString,
+                    request_deserializer=niscope__pb2.SetAttributeViStringRequest.FromString,
+                    response_serializer=niscope__pb2.SetAttributeViStringResponse.SerializeToString,
             ),
-            'RevisionQuery': grpc.unary_unary_rpc_method_handler(
-                    servicer.RevisionQuery,
-                    request_deserializer=niscope__pb2.RevisionQueryRequest.FromString,
-                    response_serializer=niscope__pb2.RevisionQueryResponse.SerializeToString,
+            'CheckAttributeViString': grpc.unary_unary_rpc_method_handler(
+                    servicer.CheckAttributeViString,
+                    request_deserializer=niscope__pb2.CheckAttributeViStringRequest.FromString,
+                    response_serializer=niscope__pb2.CheckAttributeViStringResponse.SerializeToString,
             ),
-            'SampleMode': grpc.unary_unary_rpc_method_handler(
-                    servicer.SampleMode,
-                    request_deserializer=niscope__pb2.SampleModeRequest.FromString,
-                    response_serializer=niscope__pb2.SampleModeResponse.SerializeToString,
+            'GetAttributeViSession': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAttributeViSession,
+                    request_deserializer=niscope__pb2.GetAttributeViSessionRequest.FromString,
+                    response_serializer=niscope__pb2.GetAttributeViSessionResponse.SerializeToString,
             ),
-            'SampleRate': grpc.unary_unary_rpc_method_handler(
-                    servicer.SampleRate,
-                    request_deserializer=niscope__pb2.SampleRateRequest.FromString,
-                    response_serializer=niscope__pb2.SampleRateResponse.SerializeToString,
+            'SetAttributeViSession': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetAttributeViSession,
+                    request_deserializer=niscope__pb2.SetAttributeViSessionRequest.FromString,
+                    response_serializer=niscope__pb2.SetAttributeViSessionResponse.SerializeToString,
             ),
-            'SelfTest': grpc.unary_unary_rpc_method_handler(
-                    servicer.SelfTest,
-                    request_deserializer=niscope__pb2.SelfTestRequest.FromString,
-                    response_serializer=niscope__pb2.SelfTestResponse.SerializeToString,
+            'CheckAttributeViSession': grpc.unary_unary_rpc_method_handler(
+                    servicer.CheckAttributeViSession,
+                    request_deserializer=niscope__pb2.CheckAttributeViSessionRequest.FromString,
+                    response_serializer=niscope__pb2.CheckAttributeViSessionResponse.SerializeToString,
             ),
-            'SendSoftwareTriggerEdge': grpc.unary_unary_rpc_method_handler(
-                    servicer.SendSoftwareTriggerEdge,
-                    request_deserializer=niscope__pb2.SendSoftwareTriggerEdgeRequest.FromString,
-                    response_serializer=niscope__pb2.SendSoftwareTriggerEdgeResponse.SerializeToString,
+            'GetAttributeViBoolean': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAttributeViBoolean,
+                    request_deserializer=niscope__pb2.GetAttributeViBooleanRequest.FromString,
+                    response_serializer=niscope__pb2.GetAttributeViBooleanResponse.SerializeToString,
             ),
             'SetAttributeViBoolean': grpc.unary_unary_rpc_method_handler(
                     servicer.SetAttributeViBoolean,
                     request_deserializer=niscope__pb2.SetAttributeViBooleanRequest.FromString,
                     response_serializer=niscope__pb2.SetAttributeViBooleanResponse.SerializeToString,
             ),
-            'SetAttributeViInt32': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetAttributeViInt32,
-                    request_deserializer=niscope__pb2.SetAttributeViInt32Request.FromString,
-                    response_serializer=niscope__pb2.SetAttributeViInt32Response.SerializeToString,
+            'CheckAttributeViBoolean': grpc.unary_unary_rpc_method_handler(
+                    servicer.CheckAttributeViBoolean,
+                    request_deserializer=niscope__pb2.CheckAttributeViBooleanRequest.FromString,
+                    response_serializer=niscope__pb2.CheckAttributeViBooleanResponse.SerializeToString,
             ),
-            'SetAttributeViInt64': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetAttributeViInt64,
-                    request_deserializer=niscope__pb2.SetAttributeViInt64Request.FromString,
-                    response_serializer=niscope__pb2.SetAttributeViInt64Response.SerializeToString,
+            'ImportAttributeConfigurationBuffer': grpc.unary_unary_rpc_method_handler(
+                    servicer.ImportAttributeConfigurationBuffer,
+                    request_deserializer=niscope__pb2.ImportAttributeConfigurationBufferRequest.FromString,
+                    response_serializer=niscope__pb2.ImportAttributeConfigurationBufferResponse.SerializeToString,
             ),
-            'SetAttributeViReal64': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetAttributeViReal64,
-                    request_deserializer=niscope__pb2.SetAttributeViReal64Request.FromString,
-                    response_serializer=niscope__pb2.SetAttributeViReal64Response.SerializeToString,
+            'ExportAttributeConfigurationBuffer': grpc.unary_unary_rpc_method_handler(
+                    servicer.ExportAttributeConfigurationBuffer,
+                    request_deserializer=niscope__pb2.ExportAttributeConfigurationBufferRequest.FromString,
+                    response_serializer=niscope__pb2.ExportAttributeConfigurationBufferResponse.SerializeToString,
             ),
-            'SetAttributeViSession': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetAttributeViSession,
-                    request_deserializer=niscope__pb2.SetAttributeViSessionRequest.FromString,
-                    response_serializer=niscope__pb2.SetAttributeViSessionResponse.SerializeToString,
+            'ImportAttributeConfigurationFile': grpc.unary_unary_rpc_method_handler(
+                    servicer.ImportAttributeConfigurationFile,
+                    request_deserializer=niscope__pb2.ImportAttributeConfigurationFileRequest.FromString,
+                    response_serializer=niscope__pb2.ImportAttributeConfigurationFileResponse.SerializeToString,
             ),
-            'SetAttributeViString': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetAttributeViString,
-                    request_deserializer=niscope__pb2.SetAttributeViStringRequest.FromString,
-                    response_serializer=niscope__pb2.SetAttributeViStringResponse.SerializeToString,
+            'ExportAttributeConfigurationFile': grpc.unary_unary_rpc_method_handler(
+                    servicer.ExportAttributeConfigurationFile,
+                    request_deserializer=niscope__pb2.ExportAttributeConfigurationFileRequest.FromString,
+                    response_serializer=niscope__pb2.ExportAttributeConfigurationFileResponse.SerializeToString,
+            ),
+            'GetScalingCoefficients': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetScalingCoefficients,
+                    request_deserializer=niscope__pb2.GetScalingCoefficientsRequest.FromString,
+                    response_serializer=niscope__pb2.GetScalingCoefficientsResponse.SerializeToString,
+            ),
+            'GetNormalizationCoefficients': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetNormalizationCoefficients,
+                    request_deserializer=niscope__pb2.GetNormalizationCoefficientsRequest.FromString,
+                    response_serializer=niscope__pb2.GetNormalizationCoefficientsResponse.SerializeToString,
+            ),
+            'GetStreamEndpointHandle': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetStreamEndpointHandle,
+                    request_deserializer=niscope__pb2.GetStreamEndpointHandleRequest.FromString,
+                    response_serializer=niscope__pb2.GetStreamEndpointHandleResponse.SerializeToString,
+            ),
+            'CalFetchDate': grpc.unary_unary_rpc_method_handler(
+                    servicer.CalFetchDate,
+                    request_deserializer=niscope__pb2.CalFetchDateRequest.FromString,
+                    response_serializer=niscope__pb2.CalFetchDateResponse.SerializeToString,
+            ),
+            'CalFetchTemperature': grpc.unary_unary_rpc_method_handler(
+                    servicer.CalFetchTemperature,
+                    request_deserializer=niscope__pb2.CalFetchTemperatureRequest.FromString,
+                    response_serializer=niscope__pb2.CalFetchTemperatureResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'niscope_grpc.NiScope', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class NiScope(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def Abort(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Abort',
-            niscope__pb2.AbortRequest.SerializeToString,
-            niscope__pb2.AbortResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def AcquisitionStatus(request,
+    def Init(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/AcquisitionStatus',
-            niscope__pb2.AcquisitionStatusRequest.SerializeToString,
-            niscope__pb2.AcquisitionStatusResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Init',
+            niscope__pb2.InitRequest.SerializeToString,
+            niscope__pb2.InitResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ActualMeasWfmSize(request,
+    def InitWithOptions(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ActualMeasWfmSize',
-            niscope__pb2.ActualMeasWfmSizeRequest.SerializeToString,
-            niscope__pb2.ActualMeasWfmSizeResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/InitWithOptions',
+            niscope__pb2.InitWithOptionsRequest.SerializeToString,
+            niscope__pb2.InitWithOptionsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ActualNumWfms(request,
+    def Close(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ActualNumWfms',
-            niscope__pb2.ActualNumWfmsRequest.SerializeToString,
-            niscope__pb2.ActualNumWfmsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Close',
+            niscope__pb2.CloseRequest.SerializeToString,
+            niscope__pb2.CloseResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ActualRecordLength(request,
+    def AutoSetup(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ActualRecordLength',
-            niscope__pb2.ActualRecordLengthRequest.SerializeToString,
-            niscope__pb2.ActualRecordLengthResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/AutoSetup',
+            niscope__pb2.AutoSetupRequest.SerializeToString,
+            niscope__pb2.AutoSetupResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def AddWaveformProcessing(request,
+    def ConfigureVertical(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/AddWaveformProcessing',
-            niscope__pb2.AddWaveformProcessingRequest.SerializeToString,
-            niscope__pb2.AddWaveformProcessingResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureVertical',
+            niscope__pb2.ConfigureVerticalRequest.SerializeToString,
+            niscope__pb2.ConfigureVerticalResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def AdjustSampleClockRelativeDelay(request,
+    def ConfigureChanCharacteristics(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/AdjustSampleClockRelativeDelay',
-            niscope__pb2.AdjustSampleClockRelativeDelayRequest.SerializeToString,
-            niscope__pb2.AdjustSampleClockRelativeDelayResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureChanCharacteristics',
+            niscope__pb2.ConfigureChanCharacteristicsRequest.SerializeToString,
+            niscope__pb2.ConfigureChanCharacteristicsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def AutoSetup(request,
+    def ConfigureHorizontalTiming(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/AutoSetup',
-            niscope__pb2.AutoSetupRequest.SerializeToString,
-            niscope__pb2.AutoSetupResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureHorizontalTiming',
+            niscope__pb2.ConfigureHorizontalTimingRequest.SerializeToString,
+            niscope__pb2.ConfigureHorizontalTimingResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CableSenseSignalStart(request,
+    def ConfigureClock(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CableSenseSignalStart',
-            niscope__pb2.CableSenseSignalStartRequest.SerializeToString,
-            niscope__pb2.CableSenseSignalStartResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureClock',
+            niscope__pb2.ConfigureClockRequest.SerializeToString,
+            niscope__pb2.ConfigureClockResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CableSenseSignalStop(request,
+    def ExportSignal(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CableSenseSignalStop',
-            niscope__pb2.CableSenseSignalStopRequest.SerializeToString,
-            niscope__pb2.CableSenseSignalStopResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ExportSignal',
+            niscope__pb2.ExportSignalRequest.SerializeToString,
+            niscope__pb2.ExportSignalResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CalFetchDate(request,
+    def AdjustSampleClockRelativeDelay(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CalFetchDate',
-            niscope__pb2.CalFetchDateRequest.SerializeToString,
-            niscope__pb2.CalFetchDateResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/AdjustSampleClockRelativeDelay',
+            niscope__pb2.AdjustSampleClockRelativeDelayRequest.SerializeToString,
+            niscope__pb2.AdjustSampleClockRelativeDelayResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CalFetchTemperature(request,
+    def ConfigureTriggerEdge(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CalFetchTemperature',
-            niscope__pb2.CalFetchTemperatureRequest.SerializeToString,
-            niscope__pb2.CalFetchTemperatureResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerEdge',
+            niscope__pb2.ConfigureTriggerEdgeRequest.SerializeToString,
+            niscope__pb2.ConfigureTriggerEdgeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CalSelfCalibrate(request,
+    def ConfigureTriggerGlitch(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CalSelfCalibrate',
-            niscope__pb2.CalSelfCalibrateRequest.SerializeToString,
-            niscope__pb2.CalSelfCalibrateResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerGlitch',
+            niscope__pb2.ConfigureTriggerGlitchRequest.SerializeToString,
+            niscope__pb2.ConfigureTriggerGlitchResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CheckAttributeViBoolean(request,
+    def ConfigureTriggerHysteresis(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViBoolean',
-            niscope__pb2.CheckAttributeViBooleanRequest.SerializeToString,
-            niscope__pb2.CheckAttributeViBooleanResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerHysteresis',
+            niscope__pb2.ConfigureTriggerHysteresisRequest.SerializeToString,
+            niscope__pb2.ConfigureTriggerHysteresisResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CheckAttributeViInt32(request,
+    def ConfigureTriggerWindow(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViInt32',
-            niscope__pb2.CheckAttributeViInt32Request.SerializeToString,
-            niscope__pb2.CheckAttributeViInt32Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerWindow',
+            niscope__pb2.ConfigureTriggerWindowRequest.SerializeToString,
+            niscope__pb2.ConfigureTriggerWindowResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CheckAttributeViInt64(request,
+    def ConfigureTriggerSoftware(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViInt64',
-            niscope__pb2.CheckAttributeViInt64Request.SerializeToString,
-            niscope__pb2.CheckAttributeViInt64Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerSoftware',
+            niscope__pb2.ConfigureTriggerSoftwareRequest.SerializeToString,
+            niscope__pb2.ConfigureTriggerSoftwareResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CheckAttributeViReal64(request,
+    def SendSoftwareTriggerEdge(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViReal64',
-            niscope__pb2.CheckAttributeViReal64Request.SerializeToString,
-            niscope__pb2.CheckAttributeViReal64Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SendSoftwareTriggerEdge',
+            niscope__pb2.SendSoftwareTriggerEdgeRequest.SerializeToString,
+            niscope__pb2.SendSoftwareTriggerEdgeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CheckAttributeViSession(request,
+    def ConfigureTriggerImmediate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViSession',
-            niscope__pb2.CheckAttributeViSessionRequest.SerializeToString,
-            niscope__pb2.CheckAttributeViSessionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerImmediate',
+            niscope__pb2.ConfigureTriggerImmediateRequest.SerializeToString,
+            niscope__pb2.ConfigureTriggerImmediateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CheckAttributeViString(request,
+    def ConfigureTriggerRunt(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViString',
-            niscope__pb2.CheckAttributeViStringRequest.SerializeToString,
-            niscope__pb2.CheckAttributeViStringResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerRunt',
+            niscope__pb2.ConfigureTriggerRuntRequest.SerializeToString,
+            niscope__pb2.ConfigureTriggerRuntResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ClearWaveformMeasurementStats(request,
+    def ConfigureTriggerDigital(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ClearWaveformMeasurementStats',
-            niscope__pb2.ClearWaveformMeasurementStatsRequest.SerializeToString,
-            niscope__pb2.ClearWaveformMeasurementStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerDigital',
+            niscope__pb2.ConfigureTriggerDigitalRequest.SerializeToString,
+            niscope__pb2.ConfigureTriggerDigitalResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ClearWaveformProcessing(request,
+    def ConfigureTriggerVideo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ClearWaveformProcessing',
-            niscope__pb2.ClearWaveformProcessingRequest.SerializeToString,
-            niscope__pb2.ClearWaveformProcessingResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerVideo',
+            niscope__pb2.ConfigureTriggerVideoRequest.SerializeToString,
+            niscope__pb2.ConfigureTriggerVideoResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Close(request,
+    def ConfigureTriggerWidth(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Close',
-            niscope__pb2.CloseRequest.SerializeToString,
-            niscope__pb2.CloseResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerWidth',
+            niscope__pb2.ConfigureTriggerWidthRequest.SerializeToString,
+            niscope__pb2.ConfigureTriggerWidthResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Commit(request,
+    def ConfigureEqualizationFilterCoefficients(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Commit',
-            niscope__pb2.CommitRequest.SerializeToString,
-            niscope__pb2.CommitResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureEqualizationFilterCoefficients',
+            niscope__pb2.ConfigureEqualizationFilterCoefficientsRequest.SerializeToString,
+            niscope__pb2.ConfigureEqualizationFilterCoefficientsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureAcquisition(request,
+    def GetEqualizationFilterCoefficients(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureAcquisition',
-            niscope__pb2.ConfigureAcquisitionRequest.SerializeToString,
-            niscope__pb2.ConfigureAcquisitionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetEqualizationFilterCoefficients',
+            niscope__pb2.GetEqualizationFilterCoefficientsRequest.SerializeToString,
+            niscope__pb2.GetEqualizationFilterCoefficientsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureChanCharacteristics(request,
+    def GetFrequencyResponse(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureChanCharacteristics',
-            niscope__pb2.ConfigureChanCharacteristicsRequest.SerializeToString,
-            niscope__pb2.ConfigureChanCharacteristicsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetFrequencyResponse',
+            niscope__pb2.GetFrequencyResponseRequest.SerializeToString,
+            niscope__pb2.GetFrequencyResponseResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureClock(request,
+    def ConfigureAcquisition(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureClock',
-            niscope__pb2.ConfigureClockRequest.SerializeToString,
-            niscope__pb2.ConfigureClockResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureAcquisition',
+            niscope__pb2.ConfigureAcquisitionRequest.SerializeToString,
+            niscope__pb2.ConfigureAcquisitionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureEqualizationFilterCoefficients(request,
+    def InitiateAcquisition(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureEqualizationFilterCoefficients',
-            niscope__pb2.ConfigureEqualizationFilterCoefficientsRequest.SerializeToString,
-            niscope__pb2.ConfigureEqualizationFilterCoefficientsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/InitiateAcquisition',
+            niscope__pb2.InitiateAcquisitionRequest.SerializeToString,
+            niscope__pb2.InitiateAcquisitionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureHorizontalTiming(request,
+    def Abort(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureHorizontalTiming',
-            niscope__pb2.ConfigureHorizontalTimingRequest.SerializeToString,
-            niscope__pb2.ConfigureHorizontalTimingResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Abort',
+            niscope__pb2.AbortRequest.SerializeToString,
+            niscope__pb2.AbortResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureTriggerDigital(request,
+    def Commit(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerDigital',
-            niscope__pb2.ConfigureTriggerDigitalRequest.SerializeToString,
-            niscope__pb2.ConfigureTriggerDigitalResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Commit',
+            niscope__pb2.CommitRequest.SerializeToString,
+            niscope__pb2.CommitResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureTriggerEdge(request,
+    def Read(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerEdge',
-            niscope__pb2.ConfigureTriggerEdgeRequest.SerializeToString,
-            niscope__pb2.ConfigureTriggerEdgeResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Read',
+            niscope__pb2.ReadRequest.SerializeToString,
+            niscope__pb2.ReadResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureTriggerGlitch(request,
+    def Fetch(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerGlitch',
-            niscope__pb2.ConfigureTriggerGlitchRequest.SerializeToString,
-            niscope__pb2.ConfigureTriggerGlitchResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Fetch',
+            niscope__pb2.FetchRequest.SerializeToString,
+            niscope__pb2.FetchResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureTriggerHysteresis(request,
+    def FetchBinary8(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerHysteresis',
-            niscope__pb2.ConfigureTriggerHysteresisRequest.SerializeToString,
-            niscope__pb2.ConfigureTriggerHysteresisResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchBinary8',
+            niscope__pb2.FetchBinary8Request.SerializeToString,
+            niscope__pb2.FetchBinary8Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureTriggerImmediate(request,
+    def FetchBinary16(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerImmediate',
-            niscope__pb2.ConfigureTriggerImmediateRequest.SerializeToString,
-            niscope__pb2.ConfigureTriggerImmediateResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchBinary16',
+            niscope__pb2.FetchBinary16Request.SerializeToString,
+            niscope__pb2.FetchBinary16Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureTriggerRunt(request,
+    def FetchBinary32(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerRunt',
-            niscope__pb2.ConfigureTriggerRuntRequest.SerializeToString,
-            niscope__pb2.ConfigureTriggerRuntResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchBinary32',
+            niscope__pb2.FetchBinary32Request.SerializeToString,
+            niscope__pb2.FetchBinary32Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureTriggerSoftware(request,
+    def FetchComplex(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerSoftware',
-            niscope__pb2.ConfigureTriggerSoftwareRequest.SerializeToString,
-            niscope__pb2.ConfigureTriggerSoftwareResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchComplex',
+            niscope__pb2.FetchComplexRequest.SerializeToString,
+            niscope__pb2.FetchComplexResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureTriggerVideo(request,
+    def FetchComplexBinary16(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerVideo',
-            niscope__pb2.ConfigureTriggerVideoRequest.SerializeToString,
-            niscope__pb2.ConfigureTriggerVideoResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchComplexBinary16',
+            niscope__pb2.FetchComplexBinary16Request.SerializeToString,
+            niscope__pb2.FetchComplexBinary16Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureTriggerWidth(request,
+    def AcquisitionStatus(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerWidth',
-            niscope__pb2.ConfigureTriggerWidthRequest.SerializeToString,
-            niscope__pb2.ConfigureTriggerWidthResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/AcquisitionStatus',
+            niscope__pb2.AcquisitionStatusRequest.SerializeToString,
+            niscope__pb2.AcquisitionStatusResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureTriggerWindow(request,
+    def ActualNumWfms(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureTriggerWindow',
-            niscope__pb2.ConfigureTriggerWindowRequest.SerializeToString,
-            niscope__pb2.ConfigureTriggerWindowResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ActualNumWfms',
+            niscope__pb2.ActualNumWfmsRequest.SerializeToString,
+            niscope__pb2.ActualNumWfmsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ConfigureVertical(request,
+    def ActualMeasWfmSize(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ConfigureVertical',
-            niscope__pb2.ConfigureVerticalRequest.SerializeToString,
-            niscope__pb2.ConfigureVerticalResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ActualMeasWfmSize',
+            niscope__pb2.ActualMeasWfmSizeRequest.SerializeToString,
+            niscope__pb2.ActualMeasWfmSizeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Disable(request,
+    def ActualRecordLength(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Disable',
-            niscope__pb2.DisableRequest.SerializeToString,
-            niscope__pb2.DisableResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ActualRecordLength',
+            niscope__pb2.ActualRecordLengthRequest.SerializeToString,
+            niscope__pb2.ActualRecordLengthResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ErrorHandler(request,
+    def SampleRate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ErrorHandler',
-            niscope__pb2.ErrorHandlerRequest.SerializeToString,
-            niscope__pb2.ErrorHandlerResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SampleRate',
+            niscope__pb2.SampleRateRequest.SerializeToString,
+            niscope__pb2.SampleRateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ExportAttributeConfigurationBuffer(request,
+    def SampleMode(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ExportAttributeConfigurationBuffer',
-            niscope__pb2.ExportAttributeConfigurationBufferRequest.SerializeToString,
-            niscope__pb2.ExportAttributeConfigurationBufferResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SampleMode',
+            niscope__pb2.SampleModeRequest.SerializeToString,
+            niscope__pb2.SampleModeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ExportAttributeConfigurationFile(request,
+    def AddWaveformProcessing(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ExportAttributeConfigurationFile',
-            niscope__pb2.ExportAttributeConfigurationFileRequest.SerializeToString,
-            niscope__pb2.ExportAttributeConfigurationFileResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/AddWaveformProcessing',
+            niscope__pb2.AddWaveformProcessingRequest.SerializeToString,
+            niscope__pb2.AddWaveformProcessingResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ExportSignal(request,
+    def ClearWaveformProcessing(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ExportSignal',
-            niscope__pb2.ExportSignalRequest.SerializeToString,
-            niscope__pb2.ExportSignalResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ClearWaveformProcessing',
+            niscope__pb2.ClearWaveformProcessingRequest.SerializeToString,
+            niscope__pb2.ClearWaveformProcessingResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Fetch(request,
+    def ClearWaveformMeasurementStats(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Fetch',
-            niscope__pb2.FetchRequest.SerializeToString,
-            niscope__pb2.FetchResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ClearWaveformMeasurementStats',
+            niscope__pb2.ClearWaveformMeasurementStatsRequest.SerializeToString,
+            niscope__pb2.ClearWaveformMeasurementStatsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def FetchArrayMeasurement(request,
+    def ReadMeasurement(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchArrayMeasurement',
-            niscope__pb2.FetchArrayMeasurementRequest.SerializeToString,
-            niscope__pb2.FetchArrayMeasurementResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ReadMeasurement',
+            niscope__pb2.ReadMeasurementRequest.SerializeToString,
+            niscope__pb2.ReadMeasurementResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def FetchBinary16(request,
+    def FetchMeasurement(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchBinary16',
-            niscope__pb2.FetchBinary16Request.SerializeToString,
-            niscope__pb2.FetchBinary16Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchMeasurement',
+            niscope__pb2.FetchMeasurementRequest.SerializeToString,
+            niscope__pb2.FetchMeasurementResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def FetchBinary32(request,
+    def FetchMeasurementStats(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchBinary32',
-            niscope__pb2.FetchBinary32Request.SerializeToString,
-            niscope__pb2.FetchBinary32Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchMeasurementStats',
+            niscope__pb2.FetchMeasurementStatsRequest.SerializeToString,
+            niscope__pb2.FetchMeasurementStatsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def FetchBinary8(request,
+    def FetchArrayMeasurement(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchBinary8',
-            niscope__pb2.FetchBinary8Request.SerializeToString,
-            niscope__pb2.FetchBinary8Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchArrayMeasurement',
+            niscope__pb2.FetchArrayMeasurementRequest.SerializeToString,
+            niscope__pb2.FetchArrayMeasurementResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def FetchComplex(request,
+    def Reset(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchComplex',
-            niscope__pb2.FetchComplexRequest.SerializeToString,
-            niscope__pb2.FetchComplexResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Reset',
+            niscope__pb2.ResetRequest.SerializeToString,
+            niscope__pb2.ResetResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def FetchComplexBinary16(request,
+    def SelfTest(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchComplexBinary16',
-            niscope__pb2.FetchComplexBinary16Request.SerializeToString,
-            niscope__pb2.FetchComplexBinary16Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SelfTest',
+            niscope__pb2.SelfTestRequest.SerializeToString,
+            niscope__pb2.SelfTestResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def FetchMeasurement(request,
+    def Disable(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchMeasurement',
-            niscope__pb2.FetchMeasurementRequest.SerializeToString,
-            niscope__pb2.FetchMeasurementResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Disable',
+            niscope__pb2.DisableRequest.SerializeToString,
+            niscope__pb2.DisableResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def FetchMeasurementStats(request,
+    def ResetDevice(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/FetchMeasurementStats',
-            niscope__pb2.FetchMeasurementStatsRequest.SerializeToString,
-            niscope__pb2.FetchMeasurementStatsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ResetDevice',
+            niscope__pb2.ResetDeviceRequest.SerializeToString,
+            niscope__pb2.ResetDeviceResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetAttributeViBoolean(request,
+    def CalSelfCalibrate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViBoolean',
-            niscope__pb2.GetAttributeViBooleanRequest.SerializeToString,
-            niscope__pb2.GetAttributeViBooleanResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CalSelfCalibrate',
+            niscope__pb2.CalSelfCalibrateRequest.SerializeToString,
+            niscope__pb2.CalSelfCalibrateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetAttributeViInt32(request,
+    def RevisionQuery(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViInt32',
-            niscope__pb2.GetAttributeViInt32Request.SerializeToString,
-            niscope__pb2.GetAttributeViInt32Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/RevisionQuery',
+            niscope__pb2.RevisionQueryRequest.SerializeToString,
+            niscope__pb2.RevisionQueryResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetAttributeViInt64(request,
+    def ProbeCompensationSignalStart(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViInt64',
-            niscope__pb2.GetAttributeViInt64Request.SerializeToString,
-            niscope__pb2.GetAttributeViInt64Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ProbeCompensationSignalStart',
+            niscope__pb2.ProbeCompensationSignalStartRequest.SerializeToString,
+            niscope__pb2.ProbeCompensationSignalStartResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetAttributeViReal64(request,
+    def ProbeCompensationSignalStop(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViReal64',
-            niscope__pb2.GetAttributeViReal64Request.SerializeToString,
-            niscope__pb2.GetAttributeViReal64Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ProbeCompensationSignalStop',
+            niscope__pb2.ProbeCompensationSignalStopRequest.SerializeToString,
+            niscope__pb2.ProbeCompensationSignalStopResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetAttributeViSession(request,
+    def CableSenseSignalStart(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViSession',
-            niscope__pb2.GetAttributeViSessionRequest.SerializeToString,
-            niscope__pb2.GetAttributeViSessionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CableSenseSignalStart',
+            niscope__pb2.CableSenseSignalStartRequest.SerializeToString,
+            niscope__pb2.CableSenseSignalStartResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetAttributeViString(request,
+    def CableSenseSignalStop(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViString',
-            niscope__pb2.GetAttributeViStringRequest.SerializeToString,
-            niscope__pb2.GetAttributeViStringResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CableSenseSignalStop',
+            niscope__pb2.CableSenseSignalStopRequest.SerializeToString,
+            niscope__pb2.CableSenseSignalStopResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetChannelName(request,
             target,
             options=(),
@@ -2506,27 +2489,27 @@
         return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetChannelNameFromString',
             niscope__pb2.GetChannelNameFromStringRequest.SerializeToString,
             niscope__pb2.GetChannelNameFromStringResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetEqualizationFilterCoefficients(request,
+    def ErrorHandler(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetEqualizationFilterCoefficients',
-            niscope__pb2.GetEqualizationFilterCoefficientsRequest.SerializeToString,
-            niscope__pb2.GetEqualizationFilterCoefficientsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ErrorHandler',
+            niscope__pb2.ErrorHandlerRequest.SerializeToString,
+            niscope__pb2.ErrorHandlerResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetError(request,
             target,
             options=(),
@@ -2557,447 +2540,464 @@
         return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetErrorMessage',
             niscope__pb2.GetErrorMessageRequest.SerializeToString,
             niscope__pb2.GetErrorMessageResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetFrequencyResponse(request,
+    def GetAttributeViInt32(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetFrequencyResponse',
-            niscope__pb2.GetFrequencyResponseRequest.SerializeToString,
-            niscope__pb2.GetFrequencyResponseResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViInt32',
+            niscope__pb2.GetAttributeViInt32Request.SerializeToString,
+            niscope__pb2.GetAttributeViInt32Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetNormalizationCoefficients(request,
+    def SetAttributeViInt32(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetNormalizationCoefficients',
-            niscope__pb2.GetNormalizationCoefficientsRequest.SerializeToString,
-            niscope__pb2.GetNormalizationCoefficientsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViInt32',
+            niscope__pb2.SetAttributeViInt32Request.SerializeToString,
+            niscope__pb2.SetAttributeViInt32Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetScalingCoefficients(request,
+    def CheckAttributeViInt32(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetScalingCoefficients',
-            niscope__pb2.GetScalingCoefficientsRequest.SerializeToString,
-            niscope__pb2.GetScalingCoefficientsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViInt32',
+            niscope__pb2.CheckAttributeViInt32Request.SerializeToString,
+            niscope__pb2.CheckAttributeViInt32Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetStreamEndpointHandle(request,
+    def GetAttributeViInt64(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetStreamEndpointHandle',
-            niscope__pb2.GetStreamEndpointHandleRequest.SerializeToString,
-            niscope__pb2.GetStreamEndpointHandleResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViInt64',
+            niscope__pb2.GetAttributeViInt64Request.SerializeToString,
+            niscope__pb2.GetAttributeViInt64Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ImportAttributeConfigurationBuffer(request,
+    def SetAttributeViInt64(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ImportAttributeConfigurationBuffer',
-            niscope__pb2.ImportAttributeConfigurationBufferRequest.SerializeToString,
-            niscope__pb2.ImportAttributeConfigurationBufferResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViInt64',
+            niscope__pb2.SetAttributeViInt64Request.SerializeToString,
+            niscope__pb2.SetAttributeViInt64Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ImportAttributeConfigurationFile(request,
+    def CheckAttributeViInt64(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ImportAttributeConfigurationFile',
-            niscope__pb2.ImportAttributeConfigurationFileRequest.SerializeToString,
-            niscope__pb2.ImportAttributeConfigurationFileResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViInt64',
+            niscope__pb2.CheckAttributeViInt64Request.SerializeToString,
+            niscope__pb2.CheckAttributeViInt64Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Init(request,
+    def GetAttributeViReal64(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Init',
-            niscope__pb2.InitRequest.SerializeToString,
-            niscope__pb2.InitResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViReal64',
+            niscope__pb2.GetAttributeViReal64Request.SerializeToString,
+            niscope__pb2.GetAttributeViReal64Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def InitWithOptions(request,
+    def SetAttributeViReal64(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/InitWithOptions',
-            niscope__pb2.InitWithOptionsRequest.SerializeToString,
-            niscope__pb2.InitWithOptionsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViReal64',
+            niscope__pb2.SetAttributeViReal64Request.SerializeToString,
+            niscope__pb2.SetAttributeViReal64Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def InitiateAcquisition(request,
+    def CheckAttributeViReal64(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/InitiateAcquisition',
-            niscope__pb2.InitiateAcquisitionRequest.SerializeToString,
-            niscope__pb2.InitiateAcquisitionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViReal64',
+            niscope__pb2.CheckAttributeViReal64Request.SerializeToString,
+            niscope__pb2.CheckAttributeViReal64Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ProbeCompensationSignalStart(request,
+    def GetAttributeViString(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ProbeCompensationSignalStart',
-            niscope__pb2.ProbeCompensationSignalStartRequest.SerializeToString,
-            niscope__pb2.ProbeCompensationSignalStartResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViString',
+            niscope__pb2.GetAttributeViStringRequest.SerializeToString,
+            niscope__pb2.GetAttributeViStringResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ProbeCompensationSignalStop(request,
+    def SetAttributeViString(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ProbeCompensationSignalStop',
-            niscope__pb2.ProbeCompensationSignalStopRequest.SerializeToString,
-            niscope__pb2.ProbeCompensationSignalStopResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViString',
+            niscope__pb2.SetAttributeViStringRequest.SerializeToString,
+            niscope__pb2.SetAttributeViStringResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Read(request,
+    def CheckAttributeViString(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Read',
-            niscope__pb2.ReadRequest.SerializeToString,
-            niscope__pb2.ReadResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViString',
+            niscope__pb2.CheckAttributeViStringRequest.SerializeToString,
+            niscope__pb2.CheckAttributeViStringResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ReadMeasurement(request,
+    def GetAttributeViSession(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ReadMeasurement',
-            niscope__pb2.ReadMeasurementRequest.SerializeToString,
-            niscope__pb2.ReadMeasurementResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViSession',
+            niscope__pb2.GetAttributeViSessionRequest.SerializeToString,
+            niscope__pb2.GetAttributeViSessionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Reset(request,
+    def SetAttributeViSession(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/Reset',
-            niscope__pb2.ResetRequest.SerializeToString,
-            niscope__pb2.ResetResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViSession',
+            niscope__pb2.SetAttributeViSessionRequest.SerializeToString,
+            niscope__pb2.SetAttributeViSessionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ResetDevice(request,
+    def CheckAttributeViSession(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ResetDevice',
-            niscope__pb2.ResetDeviceRequest.SerializeToString,
-            niscope__pb2.ResetDeviceResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViSession',
+            niscope__pb2.CheckAttributeViSessionRequest.SerializeToString,
+            niscope__pb2.CheckAttributeViSessionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def RevisionQuery(request,
+    def GetAttributeViBoolean(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/RevisionQuery',
-            niscope__pb2.RevisionQueryRequest.SerializeToString,
-            niscope__pb2.RevisionQueryResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetAttributeViBoolean',
+            niscope__pb2.GetAttributeViBooleanRequest.SerializeToString,
+            niscope__pb2.GetAttributeViBooleanResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SampleMode(request,
+    def SetAttributeViBoolean(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SampleMode',
-            niscope__pb2.SampleModeRequest.SerializeToString,
-            niscope__pb2.SampleModeResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViBoolean',
+            niscope__pb2.SetAttributeViBooleanRequest.SerializeToString,
+            niscope__pb2.SetAttributeViBooleanResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SampleRate(request,
+    def CheckAttributeViBoolean(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SampleRate',
-            niscope__pb2.SampleRateRequest.SerializeToString,
-            niscope__pb2.SampleRateResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CheckAttributeViBoolean',
+            niscope__pb2.CheckAttributeViBooleanRequest.SerializeToString,
+            niscope__pb2.CheckAttributeViBooleanResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SelfTest(request,
+    def ImportAttributeConfigurationBuffer(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SelfTest',
-            niscope__pb2.SelfTestRequest.SerializeToString,
-            niscope__pb2.SelfTestResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ImportAttributeConfigurationBuffer',
+            niscope__pb2.ImportAttributeConfigurationBufferRequest.SerializeToString,
+            niscope__pb2.ImportAttributeConfigurationBufferResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SendSoftwareTriggerEdge(request,
+    def ExportAttributeConfigurationBuffer(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SendSoftwareTriggerEdge',
-            niscope__pb2.SendSoftwareTriggerEdgeRequest.SerializeToString,
-            niscope__pb2.SendSoftwareTriggerEdgeResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ExportAttributeConfigurationBuffer',
+            niscope__pb2.ExportAttributeConfigurationBufferRequest.SerializeToString,
+            niscope__pb2.ExportAttributeConfigurationBufferResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetAttributeViBoolean(request,
+    def ImportAttributeConfigurationFile(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViBoolean',
-            niscope__pb2.SetAttributeViBooleanRequest.SerializeToString,
-            niscope__pb2.SetAttributeViBooleanResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ImportAttributeConfigurationFile',
+            niscope__pb2.ImportAttributeConfigurationFileRequest.SerializeToString,
+            niscope__pb2.ImportAttributeConfigurationFileResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetAttributeViInt32(request,
+    def ExportAttributeConfigurationFile(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViInt32',
-            niscope__pb2.SetAttributeViInt32Request.SerializeToString,
-            niscope__pb2.SetAttributeViInt32Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/ExportAttributeConfigurationFile',
+            niscope__pb2.ExportAttributeConfigurationFileRequest.SerializeToString,
+            niscope__pb2.ExportAttributeConfigurationFileResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetAttributeViInt64(request,
+    def GetScalingCoefficients(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViInt64',
-            niscope__pb2.SetAttributeViInt64Request.SerializeToString,
-            niscope__pb2.SetAttributeViInt64Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetScalingCoefficients',
+            niscope__pb2.GetScalingCoefficientsRequest.SerializeToString,
+            niscope__pb2.GetScalingCoefficientsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetAttributeViReal64(request,
+    def GetNormalizationCoefficients(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViReal64',
-            niscope__pb2.SetAttributeViReal64Request.SerializeToString,
-            niscope__pb2.SetAttributeViReal64Response.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetNormalizationCoefficients',
+            niscope__pb2.GetNormalizationCoefficientsRequest.SerializeToString,
+            niscope__pb2.GetNormalizationCoefficientsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetAttributeViSession(request,
+    def GetStreamEndpointHandle(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViSession',
-            niscope__pb2.SetAttributeViSessionRequest.SerializeToString,
-            niscope__pb2.SetAttributeViSessionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/GetStreamEndpointHandle',
+            niscope__pb2.GetStreamEndpointHandleRequest.SerializeToString,
+            niscope__pb2.GetStreamEndpointHandleResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetAttributeViString(request,
+    def CalFetchDate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/SetAttributeViString',
-            niscope__pb2.SetAttributeViStringRequest.SerializeToString,
-            niscope__pb2.SetAttributeViStringResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CalFetchDate',
+            niscope__pb2.CalFetchDateRequest.SerializeToString,
+            niscope__pb2.CalFetchDateResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CalFetchTemperature(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/niscope_grpc.NiScope/CalFetchTemperature',
+            niscope__pb2.CalFetchTemperatureRequest.SerializeToString,
+            niscope__pb2.CalFetchTemperatureResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `niscope-1.4.7/niscope/session.py` & `niscope-1.4.8/niscope/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -3159,15 +3159,15 @@
         elif waveform.dtype == numpy.int8:
             wfm_info = self._fetch_binary8_into_numpy(num_samples=num_samples, waveform=waveform, timeout=timeout)
         elif waveform.dtype == numpy.int16:
             wfm_info = self._fetch_binary16_into_numpy(num_samples=num_samples, waveform=waveform, timeout=timeout)
         elif waveform.dtype == numpy.int32:
             wfm_info = self._fetch_binary32_into_numpy(num_samples=num_samples, waveform=waveform, timeout=timeout)
         else:
-            raise TypeError("Unsupported dtype. Is {0}, expected {1}, {2}, {3}, or {4}".format(waveform.dtype, numpy.float64, numpy.int8, numpy.int16, numpy.int32))
+            raise TypeError("Unsupported dtype. Is {}, expected {}, {}, {}, or {}".format(waveform.dtype, numpy.float64, numpy.int8, numpy.int16, numpy.int32))
 
         mv = memoryview(waveform)
 
         waveform_info._populate_samples_info(wfm_info, mv, num_samples)
 
         channel_names = _converters.expand_channel_string(
             self._repeated_capability,
```

### Comparing `niscope-1.4.7/niscope/session_pb2.py` & `niscope-1.4.8/niscope/session_pb2.py`

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

### Comparing `niscope-1.4.7/niscope/session_pb2_grpc.py` & `niscope-1.4.8/niscope/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.7/niscope/waveform_info.py` & `niscope-1.4.8/niscope/waveform_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             self.actual_samples = actual_samples
             self.offset = offset
             self.gain = gain
             self.reserved1 = reserved1
             self.reserved2 = reserved2
 
 
-class WaveformInfo(object):
+class WaveformInfo:
     def __init__(self, data=None, absolute_initial_x=0.0, relative_initial_x=0.0,
                  x_increment=0.0, offset=0.0, gain=0.0,
                  reserved1=0.0, reserved2=0.0):
         if data is not None:
             self.absolute_initial_x = data.absolute_initial_x
             self.relative_initial_x = data.relative_initial_x
             self.x_increment = data.x_increment
@@ -71,22 +71,22 @@
         # Additional fields filled in during fetch or fetch_into
         self.channel = None
         self.record = None
         self.samples = None
 
     def __repr__(self):
         parameter_list = [
-            'absolute_initial_x={}'.format(self.absolute_initial_x),
-            'relative_initial_x={}'.format(self.relative_initial_x),
-            'x_increment={}'.format(self.x_increment),
-            'offset={}'.format(self.offset),
-            'gain={}'.format(self.gain)
+            f'absolute_initial_x={self.absolute_initial_x}',
+            f'relative_initial_x={self.relative_initial_x}',
+            f'x_increment={self.x_increment}',
+            f'offset={self.offset}',
+            f'gain={self.gain}'
         ]
 
-        return '{0}({1})'.format(self.__class__.__name__, ', '.join(parameter_list))
+        return '{}({})'.format(self.__class__.__name__, ', '.join(parameter_list))
 
     def __str__(self):
         # different format lines
         row_format_g = '{:<20}: {:,.6g}\n'
         row_format_d = '{:<20}: {:,}\n'
         row_format_s = '{:<20}: {:}\n'
```

### Comparing `niscope-1.4.7/niscope.egg-info/PKG-INFO` & `niscope-1.4.8/niscope.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niscope
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI-SCOPE Python API
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
 
 NI-SCOPE Python API Status
 --------------------------
 
 +-------------------------------+------------------------+
 | NI-SCOPE (niscope)            |                        |
 +===============================+========================+
-| Driver Version Tested Against | 2023 Q1.1              |
+| Driver Version Tested Against | 2023 Q4                |
 +-------------------------------+------------------------+
 | PyPI Version                  | |niscopeLatestVersion| |
 +-------------------------------+------------------------+
 | Supported Python Version      | |niscopePythonVersion| |
 +-------------------------------+------------------------+
 | Documentation                 | |niscopeDocs|          |
 +-------------------------------+------------------------+
@@ -130,15 +131,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **niscope** module, you must install the NI-SCOPE runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SCOPE**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niscope~=1.4.7
+  $ python -m pip install niscope~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -153,15 +154,15 @@
     with niscope.Session("Dev1") as session:
         session.channels[0].configure_vertical(range=1.0, coupling=niscope.VerticalCoupling.AC)
         session.channels[1].configure_vertical(range=10.0, coupling=niscope.VerticalCoupling.DC)
         session.configure_horizontal_timing(min_sample_rate=50000000, min_num_pts=1000, ref_position=50.0, num_records=5, enforce_realtime=True)
         with session.initiate():
             waveforms = session.channels[0,1].fetch(num_records=5)
         for wfm in waveforms:
-            print('Channel {0}, record {1} samples acquired: {2:,}\n'.format(wfm.channel, wfm.record, len(wfm.samples)))
+            print('Channel {}, record {} samples acquired: {:,}\n'.format(wfm.channel, wfm.record, len(wfm.samples)))
 
         # Find all channel 1 records (Note channel name is always a string even if integers used in channel[])
         chan1 = [wfm for wfm in waveforms if wfm.channel == '0']
 
         # Find all record number 3
         rec3 = [wfm for wfm in waveforms if wfm.record == 3]
```

### Comparing `niscope-1.4.7/niscope.egg-info/SOURCES.txt` & `niscope-1.4.8/niscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niscope-1.4.7/setup.py` & `niscope-1.4.8/setup.py`

 * *Files 6% similar despite different names*

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
     description='NI-SCOPE Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
@@ -44,16 +43,16 @@
     packages=['niscope'],
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

