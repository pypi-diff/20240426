# Comparing `tmp/nitclk-1.4.7.tar.gz` & `tmp/nitclk-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitclk-1.4.7.tar", last modified: Fri Dec 15 19:32:20 2023, max compression
+gzip compressed data, was "nitclk-1.4.8.tar", last modified: Fri Apr 26 18:20:31 2024, max compression
```

## Comparing `nitclk-1.4.7.tar` & `nitclk-1.4.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:32:29.374612 nitclk-1.4.7/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7662 2023-12-15 19:32:29.367612 nitclk-1.4.7/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     6624 2023-12-15 19:29:49.000000 nitclk-1.4.7/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:32:29.260601 nitclk-1.4.7/nitclk/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-12-15 19:29:43.000000 nitclk-1.4.7/nitclk/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3461 2023-12-15 19:29:42.000000 nitclk-1.4.7/nitclk/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5436 2023-12-15 19:29:36.000000 nitclk-1.4.7/nitclk/_attributes.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14604 2023-12-15 19:29:42.000000 nitclk-1.4.7/nitclk/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10861 2023-12-15 19:29:37.000000 nitclk-1.4.7/nitclk/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12538 2023-12-15 19:29:38.000000 nitclk-1.4.7/nitclk/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1716 2023-12-15 19:29:38.000000 nitclk-1.4.7/nitclk/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-12-15 19:29:43.000000 nitclk-1.4.7/nitclk/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3277 2023-12-15 19:29:40.000000 nitclk-1.4.7/nitclk/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    45940 2023-12-15 19:29:39.000000 nitclk-1.4.7/nitclk/session.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:32:29.360611 nitclk-1.4.7/nitclk.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7662 2023-12-15 19:32:28.000000 nitclk-1.4.7/nitclk.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      405 2023-12-15 19:32:28.000000 nitclk-1.4.7/nitclk.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:32:28.000000 nitclk-1.4.7/nitclk.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-12-15 19:32:28.000000 nitclk-1.4.7/nitclk.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        7 2023-12-15 19:32:28.000000 nitclk-1.4.7/nitclk.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:32:28.000000 nitclk-1.4.7/nitclk.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-12-15 19:32:29.375612 nitclk-1.4.7/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1952 2023-12-15 19:29:50.000000 nitclk-1.4.7/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:20:31.510379 nitclk-1.4.8/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7713 2024-04-26 18:20:31.504378 nitclk-1.4.8/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     6624 2024-04-26 18:11:42.000000 nitclk-1.4.8/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:20:31.404377 nitclk-1.4.8/nitclk/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2024-04-26 18:11:36.000000 nitclk-1.4.8/nitclk/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3980 2024-04-26 18:11:35.000000 nitclk-1.4.8/nitclk/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5436 2024-04-26 18:11:29.000000 nitclk-1.4.8/nitclk/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14604 2024-04-26 18:11:36.000000 nitclk-1.4.8/nitclk/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10861 2024-04-26 18:11:30.000000 nitclk-1.4.8/nitclk/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12538 2024-04-26 18:11:31.000000 nitclk-1.4.8/nitclk/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1716 2024-04-26 18:11:32.000000 nitclk-1.4.8/nitclk/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      635 2024-04-26 18:11:36.000000 nitclk-1.4.8/nitclk/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3275 2024-04-26 18:11:33.000000 nitclk-1.4.8/nitclk/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    45940 2024-04-26 18:11:32.000000 nitclk-1.4.8/nitclk/session.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:20:31.497378 nitclk-1.4.8/nitclk.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7713 2024-04-26 18:20:31.000000 nitclk-1.4.8/nitclk.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      405 2024-04-26 18:20:31.000000 nitclk-1.4.8/nitclk.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:20:31.000000 nitclk-1.4.8/nitclk.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2024-04-26 18:20:31.000000 nitclk-1.4.8/nitclk.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        7 2024-04-26 18:20:31.000000 nitclk-1.4.8/nitclk.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:20:31.000000 nitclk-1.4.8/nitclk.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2024-04-26 18:20:31.511379 nitclk-1.4.8/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1978 2024-04-26 18:11:43.000000 nitclk-1.4.8/setup.py
```

### Comparing `nitclk-1.4.7/PKG-INFO` & `nitclk-1.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitclk
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI-TClk Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -17,14 +17,15 @@
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
 
 Overall Status
 --------------
@@ -77,15 +78,15 @@
 
 NI-TClk Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-TClk (nitclk)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 2023 Q2               |
+| Driver Version Tested Against | 2024 Q2               |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nitclkLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nitclkPythonVersion| |
 +-------------------------------+-----------------------+
 | Documentation                 | |nitclkDocs|          |
 +-------------------------------+-----------------------+
@@ -126,15 +127,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nitclk** module, you must install the NI-TClk runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-TClk**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nitclk~=1.4.7
+  $ python -m pip install nitclk~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nitclk-1.4.7/README.rst` & `nitclk-1.4.8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 NI-TClk Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-TClk (nitclk)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 2023 Q2               |
+| Driver Version Tested Against | 2024 Q2               |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nitclkLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nitclkPythonVersion| |
 +-------------------------------+-----------------------+
 | Documentation                 | |nitclkDocs|          |
 +-------------------------------+-----------------------+
@@ -98,15 +98,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nitclk** module, you must install the NI-TClk runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-TClk**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nitclk~=1.4.7
+  $ python -m pip install nitclk~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nitclk-1.4.7/nitclk/__init__.py` & `nitclk-1.4.8/nitclk/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.7'
+__version__ = '1.4.8'
 
 from nitclk.errors import DriverWarning  # noqa: F401
 from nitclk.errors import Error  # noqa: F401
 from nitclk.session import SessionReference  # noqa: F401
 
 # Function imports
 from nitclk.session import configure_for_homogeneous_triggers  # noqa: F401
@@ -22,16 +22,16 @@
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
 
@@ -60,24 +60,37 @@
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
     info['driver']['name'] = "NI-TClk"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nitclk'
-    info['module']['version'] = "1.4.7"
+    info['module']['version'] = "1.4.8"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nitclk-1.4.7/nitclk/_attributes.py` & `nitclk-1.4.8/nitclk/_attributes.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.7/nitclk/_converters.py` & `nitclk-1.4.8/nitclk/_converters.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.7/nitclk/_library.py` & `nitclk-1.4.8/nitclk/_library.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.7/nitclk/_library_interpreter.py` & `nitclk-1.4.8/nitclk/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.7/nitclk/_library_singleton.py` & `nitclk-1.4.8/nitclk/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.7/nitclk/_visatype.py` & `nitclk-1.4.8/nitclk/_visatype.py`

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

### Comparing `nitclk-1.4.7/nitclk/errors.py` & `nitclk-1.4.8/nitclk/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-TClk driver'''
 
     def __init__(self, code, description):
         assert _is_warning(code), "Should not create Warning if code is not positive."
-        super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
+        super(DriverWarning, self).__init__('Warning {} occurred.\n\n{}'.format(code, description))
 
 
 class UnsupportedConfigurationError(Error):
     '''An error due to using this module in an usupported platform.'''
 
     def __init__(self):
         super(UnsupportedConfigurationError, self).__init__('System configuration is unsupported: ' + platform.architecture()[0] + ' ' + platform.system())
```

### Comparing `nitclk-1.4.7/nitclk/session.py` & `nitclk-1.4.8/nitclk/session.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.7/nitclk.egg-info/PKG-INFO` & `nitclk-1.4.8/nitclk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitclk
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI-TClk Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -17,14 +17,15 @@
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
 
 Overall Status
 --------------
@@ -77,15 +78,15 @@
 
 NI-TClk Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-TClk (nitclk)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 2023 Q2               |
+| Driver Version Tested Against | 2024 Q2               |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nitclkLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nitclkPythonVersion| |
 +-------------------------------+-----------------------+
 | Documentation                 | |nitclkDocs|          |
 +-------------------------------+-----------------------+
@@ -126,15 +127,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nitclk** module, you must install the NI-TClk runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-TClk**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nitclk~=1.4.7
+  $ python -m pip install nitclk~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nitclk-1.4.7/setup.py` & `nitclk-1.4.8/setup.py`

 * *Files 4% similar despite different names*

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
     description='NI-TClk Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
@@ -57,13 +56,14 @@
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

