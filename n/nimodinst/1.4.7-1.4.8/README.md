# Comparing `tmp/nimodinst-1.4.7.tar.gz` & `tmp/nimodinst-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimodinst-1.4.7.tar", last modified: Fri Dec 15 19:32:05 2023, max compression
+gzip compressed data, was "nimodinst-1.4.8.tar", last modified: Fri Apr 26 18:19:37 2024, max compression
```

## Comparing `nimodinst-1.4.7.tar` & `nimodinst-1.4.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:32:14.283678 nimodinst-1.4.7/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8095 2023-12-15 19:32:14.275679 nimodinst-1.4.7/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7048 2023-12-15 19:29:33.000000 nimodinst-1.4.7/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:32:14.158678 nimodinst-1.4.7/nimodinst/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-12-15 19:29:27.000000 nimodinst-1.4.7/nimodinst/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2932 2023-12-15 19:29:25.000000 nimodinst-1.4.7/nimodinst/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13877 2023-12-15 19:29:26.000000 nimodinst-1.4.7/nimodinst/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4561 2023-12-15 19:29:21.000000 nimodinst-1.4.7/nimodinst/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7235 2023-12-15 19:29:21.000000 nimodinst-1.4.7/nimodinst/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1734 2023-12-15 19:29:22.000000 nimodinst-1.4.7/nimodinst/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-12-15 19:29:27.000000 nimodinst-1.4.7/nimodinst/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3310 2023-12-15 19:29:23.000000 nimodinst-1.4.7/nimodinst/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14066 2023-12-15 19:29:23.000000 nimodinst-1.4.7/nimodinst/session.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-12-15 19:32:14.267679 nimodinst-1.4.7/nimodinst.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8095 2023-12-15 19:32:13.000000 nimodinst-1.4.7/nimodinst.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      428 2023-12-15 19:32:13.000000 nimodinst-1.4.7/nimodinst.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:32:13.000000 nimodinst-1.4.7/nimodinst.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-12-15 19:32:13.000000 nimodinst-1.4.7/nimodinst.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       10 2023-12-15 19:32:13.000000 nimodinst-1.4.7/nimodinst.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-12-15 19:32:13.000000 nimodinst-1.4.7/nimodinst.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-12-15 19:32:14.284680 nimodinst-1.4.7/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1964 2023-12-15 19:29:33.000000 nimodinst-1.4.7/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:19:38.035620 nimodinst-1.4.8/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8146 2024-04-26 18:19:38.029620 nimodinst-1.4.8/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7048 2024-04-26 18:11:26.000000 nimodinst-1.4.8/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:19:37.930620 nimodinst-1.4.8/nimodinst/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2024-04-26 18:11:20.000000 nimodinst-1.4.8/nimodinst/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3451 2024-04-26 18:11:19.000000 nimodinst-1.4.8/nimodinst/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13877 2024-04-26 18:11:20.000000 nimodinst-1.4.8/nimodinst/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4561 2024-04-26 18:11:15.000000 nimodinst-1.4.8/nimodinst/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7235 2024-04-26 18:11:15.000000 nimodinst-1.4.8/nimodinst/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1734 2024-04-26 18:11:16.000000 nimodinst-1.4.8/nimodinst/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      635 2024-04-26 18:11:20.000000 nimodinst-1.4.8/nimodinst/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3308 2024-04-26 18:11:17.000000 nimodinst-1.4.8/nimodinst/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14066 2024-04-26 18:11:16.000000 nimodinst-1.4.8/nimodinst/session.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2024-04-26 18:19:38.022619 nimodinst-1.4.8/nimodinst.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8146 2024-04-26 18:19:37.000000 nimodinst-1.4.8/nimodinst.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      428 2024-04-26 18:19:37.000000 nimodinst-1.4.8/nimodinst.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:19:37.000000 nimodinst-1.4.8/nimodinst.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2024-04-26 18:19:37.000000 nimodinst-1.4.8/nimodinst.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       10 2024-04-26 18:19:37.000000 nimodinst-1.4.8/nimodinst.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2024-04-26 18:19:37.000000 nimodinst-1.4.8/nimodinst.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2024-04-26 18:19:38.036622 nimodinst-1.4.8/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1990 2024-04-26 18:11:27.000000 nimodinst-1.4.8/setup.py
```

### Comparing `nimodinst-1.4.7/PKG-INFO` & `nimodinst-1.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimodinst
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI-ModInst Python API
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
 
 NI-ModInst Python API Status
 ----------------------------
 
 +-------------------------------+--------------------------+
 | NI-ModInst (nimodinst)        |                          |
 +===============================+==========================+
-| Driver Version Tested Against | 2023 Q2                  |
+| Driver Version Tested Against | 2024 Q2                  |
 +-------------------------------+--------------------------+
 | PyPI Version                  | |nimodinstLatestVersion| |
 +-------------------------------+--------------------------+
 | Supported Python Version      | |nimodinstPythonVersion| |
 +-------------------------------+--------------------------+
 | Documentation                 | |nimodinstDocs|          |
 +-------------------------------+--------------------------+
@@ -126,15 +127,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nimodinst** module, you must install the NI-ModInst runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-ModInst**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nimodinst~=1.4.7
+  $ python -m pip install nimodinst~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nimodinst-1.4.7/README.rst` & `nimodinst-1.4.8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 NI-ModInst Python API Status
 ----------------------------
 
 +-------------------------------+--------------------------+
 | NI-ModInst (nimodinst)        |                          |
 +===============================+==========================+
-| Driver Version Tested Against | 2023 Q2                  |
+| Driver Version Tested Against | 2024 Q2                  |
 +-------------------------------+--------------------------+
 | PyPI Version                  | |nimodinstLatestVersion| |
 +-------------------------------+--------------------------+
 | Supported Python Version      | |nimodinstPythonVersion| |
 +-------------------------------+--------------------------+
 | Documentation                 | |nimodinstDocs|          |
 +-------------------------------+--------------------------+
@@ -98,15 +98,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nimodinst** module, you must install the NI-ModInst runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-ModInst**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nimodinst~=1.4.7
+  $ python -m pip install nimodinst~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nimodinst-1.4.7/nimodinst/__init__.py` & `nimodinst-1.4.8/nimodinst/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.7'
+__version__ = '1.4.8'
 
 from nimodinst.errors import DriverWarning  # noqa: F401
 from nimodinst.errors import Error  # noqa: F401
 from nimodinst.session import Session  # noqa: F401
 
 
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
 
@@ -50,24 +50,37 @@
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
     info['driver']['name'] = "NI-ModInst"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nimodinst'
-    info['module']['version'] = "1.4.7"
+    info['module']['version'] = "1.4.8"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nimodinst-1.4.7/nimodinst/_converters.py` & `nimodinst-1.4.8/nimodinst/_converters.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.7/nimodinst/_library.py` & `nimodinst-1.4.8/nimodinst/_library.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.7/nimodinst/_library_interpreter.py` & `nimodinst-1.4.8/nimodinst/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.7/nimodinst/_library_singleton.py` & `nimodinst-1.4.8/nimodinst/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.7/nimodinst/_visatype.py` & `nimodinst-1.4.8/nimodinst/_visatype.py`

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

### Comparing `nimodinst-1.4.7/nimodinst/errors.py` & `nimodinst-1.4.8/nimodinst/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-ModInst driver'''
 
     def __init__(self, code, description):
         assert _is_warning(code), "Should not create Warning if code is not positive."
-        super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
+        super(DriverWarning, self).__init__('Warning {} occurred.\n\n{}'.format(code, description))
 
 
 class UnsupportedConfigurationError(Error):
     '''An error due to using this module in an usupported platform.'''
 
     def __init__(self):
         super(UnsupportedConfigurationError, self).__init__('System configuration is unsupported: ' + platform.architecture()[0] + ' ' + platform.system())
```

### Comparing `nimodinst-1.4.7/nimodinst/session.py` & `nimodinst-1.4.8/nimodinst/session.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.7/nimodinst.egg-info/PKG-INFO` & `nimodinst-1.4.8/nimodinst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimodinst
-Version: 1.4.7
+Version: 1.4.8
 Summary: NI-ModInst Python API
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
 
 NI-ModInst Python API Status
 ----------------------------
 
 +-------------------------------+--------------------------+
 | NI-ModInst (nimodinst)        |                          |
 +===============================+==========================+
-| Driver Version Tested Against | 2023 Q2                  |
+| Driver Version Tested Against | 2024 Q2                  |
 +-------------------------------+--------------------------+
 | PyPI Version                  | |nimodinstLatestVersion| |
 +-------------------------------+--------------------------+
 | Supported Python Version      | |nimodinstPythonVersion| |
 +-------------------------------+--------------------------+
 | Documentation                 | |nimodinstDocs|          |
 +-------------------------------+--------------------------+
@@ -126,15 +127,15 @@
 Installation
 ------------
 
 As a prerequisite to using the **nimodinst** module, you must install the NI-ModInst runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-ModInst**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nimodinst~=1.4.7
+  $ python -m pip install nimodinst~=1.4.8
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
```

### Comparing `nimodinst-1.4.7/setup.py` & `nimodinst-1.4.8/setup.py`

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
     description='NI-ModInst Python API',
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

