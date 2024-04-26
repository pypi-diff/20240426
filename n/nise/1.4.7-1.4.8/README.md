# Comparing `tmp/nise-1.4.7.tar.gz` & `tmp/nise-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nise-1.4.7.tar", last modified: Fri Dec 15 19:31:49 2023, max compression
+gzip compressed data, was "nise-1.4.8.tar", last modified: Fri Apr 26 18:18:43 2024, max compression
```

## Comparing `nise-1.4.7.tar` & `nise-1.4.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:58.507579 nise-1.4.7/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7901 2023-12-15 19:31:58.499576 nise-1.4.7/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     6855 2023-12-15 19:29:17.000000 nise-1.4.7/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:58.386575 nise-1.4.7/nise/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-12-15 19:29:11.000000 nise-1.4.7/nise/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2976 2023-12-15 19:29:09.000000 nise-1.4.7/nise/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13867 2023-12-15 19:29:10.000000 nise-1.4.7/nise/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8599 2023-12-15 19:29:04.000000 nise-1.4.7/nise/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10784 2023-12-15 19:29:05.000000 nise-1.4.7/nise/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1701 2023-12-15 19:29:06.000000 nise-1.4.7/nise/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-12-15 19:29:11.000000 nise-1.4.7/nise/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1160 2023-12-15 19:29:04.000000 nise-1.4.7/nise/enums.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3725 2023-12-15 19:29:07.000000 nise-1.4.7/nise/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    36136 2023-12-15 19:29:06.000000 nise-1.4.7/nise/session.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:31:58.491578 nise-1.4.7/nise.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7901 2023-12-15 19:31:58.000000 nise-1.4.7/nise.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      367 2023-12-15 19:31:58.000000 nise-1.4.7/nise.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:31:58.000000 nise-1.4.7/nise.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-12-15 19:31:58.000000 nise-1.4.7/nise.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        5 2023-12-15 19:31:58.000000 nise-1.4.7/nise.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:31:58.000000 nise-1.4.7/nise.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-12-15 19:31:58.508577 nise-1.4.7/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1958 2023-12-15 19:29:18.000000 nise-1.4.7/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:18:44.086327 nise-1.4.8/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7952 2024-04-26 18:18:44.080326 nise-1.4.8/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     6855 2024-04-26 18:11:11.000000 nise-1.4.8/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:18:43.982323 nise-1.4.8/nise/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2024-04-26 18:11:04.000000 nise-1.4.8/nise/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3495 2024-04-26 18:11:03.000000 nise-1.4.8/nise/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13867 2024-04-26 18:11:04.000000 nise-1.4.8/nise/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8599 2024-04-26 18:10:58.000000 nise-1.4.8/nise/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10784 2024-04-26 18:10:59.000000 nise-1.4.8/nise/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1701 2024-04-26 18:11:00.000000 nise-1.4.8/nise/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      635 2024-04-26 18:11:05.000000 nise-1.4.8/nise/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1160 2024-04-26 18:10:57.000000 nise-1.4.8/nise/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3721 2024-04-26 18:11:01.000000 nise-1.4.8/nise/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    36136 2024-04-26 18:11:00.000000 nise-1.4.8/nise/session.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:18:44.073325 nise-1.4.8/nise.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7952 2024-04-26 18:18:43.000000 nise-1.4.8/nise.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      367 2024-04-26 18:18:43.000000 nise-1.4.8/nise.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:18:43.000000 nise-1.4.8/nise.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2024-04-26 18:18:43.000000 nise-1.4.8/nise.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        5 2024-04-26 18:18:43.000000 nise-1.4.8/nise.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:18:43.000000 nise-1.4.8/nise.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2024-04-26 18:18:44.087325 nise-1.4.8/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1984 2024-04-26 18:11:12.000000 nise-1.4.8/setup.py
```

### Comparing `nise-1.4.7/PKG-INFO` & `nise-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nise
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI Switch Executive Python API
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
@@ -126,15 +127,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nise** module, you must install the NI Switch Executive runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI Switch Executive**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nise~=1.4.7
+  $ python -m pip install nise~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nise-1.4.7/README.rst` & `nise-1.4.8/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nise** module, you must install the NI Switch Executive runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI Switch Executive**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nise~=1.4.7
+  $ python -m pip install nise~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nise-1.4.7/nise/__init__.py` & `nise-1.4.8/nise/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.7'
+__version__ = '1.4.8'
 
 from nise.enums import *  # noqa: F403,F401,H303
 from nise.errors import DriverWarning  # noqa: F401
 from nise.errors import Error  # noqa: F401
 from nise.session import Session  # noqa: F401
 
 
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
 
@@ -51,24 +51,37 @@
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
     info['driver']['name'] = "NI Switch Executive"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nise'
-    info['module']['version'] = "1.4.7"
+    info['module']['version'] = "1.4.8"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nise-1.4.7/nise/_converters.py` & `nise-1.4.8/nise/_converters.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.7/nise/_library.py` & `nise-1.4.8/nise/_library.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.7/nise/_library_interpreter.py` & `nise-1.4.8/nise/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.7/nise/_library_singleton.py` & `nise-1.4.8/nise/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.7/nise/_visatype.py` & `nise-1.4.8/nise/_visatype.py`

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

### Comparing `nise-1.4.7/nise/enums.py` & `nise-1.4.8/nise/enums.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.7/nise/errors.py` & `nise-1.4.8/nise/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI Switch Executive driver'''
 
     def __init__(self, code, description):
         assert _is_warning(code), "Should not create Warning if code is not positive."
-        super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
+        super(DriverWarning, self).__init__('Warning {} occurred.\n\n{}'.format(code, description))
 
 
 class UnsupportedConfigurationError(Error):
     '''An error due to using this module in an usupported platform.'''
 
     def __init__(self):
         super(UnsupportedConfigurationError, self).__init__('System configuration is unsupported: ' + platform.architecture()[0] + ' ' + platform.system())
@@ -71,15 +71,15 @@
         super(DriverTooNewError, self).__init__('The NI Switch Executive runtime returned an unexpected value. This can occur if it is too new for the nise Python module. Upgrade the nise Python module.')
 
 
 class InvalidRepeatedCapabilityError(Error):
     '''An error due to an invalid character in a repeated capability'''
 
     def __init__(self, invalid_character, invalid_string):
-        super(InvalidRepeatedCapabilityError, self).__init__('An invalid character ({0}) was found in repeated capability string ({1})'.format(invalid_character, invalid_string))
+        super(InvalidRepeatedCapabilityError, self).__init__('An invalid character ({}) was found in repeated capability string ({})'.format(invalid_character, invalid_string))
 
 
 def handle_error(library_interpreter, code, ignore_warnings, is_error_handling):
     '''handle_error
 
     Helper function for handling errors returned by nise.Library.
     It calls back into the LibraryInterpreter to get the corresponding error
```

### Comparing `nise-1.4.7/nise/session.py` & `nise-1.4.8/nise/session.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.7/nise.egg-info/PKG-INFO` & `nise-1.4.8/nise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nise
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI Switch Executive Python API
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
@@ -126,15 +127,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nise** module, you must install the NI Switch Executive runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI Switch Executive**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nise~=1.4.7
+  $ python -m pip install nise~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nise-1.4.7/setup.py` & `nise-1.4.8/setup.py`

 * *Files 9% similar despite different names*

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
     description='NI Switch Executive Python API',
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

