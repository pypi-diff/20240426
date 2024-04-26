# Comparing `tmp/caen_hv_py-1.4.tar.gz` & `tmp/caen_hv_py-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caen_hv_py-1.4.tar", last modified: Fri Apr 26 11:21:15 2024, max compression
+gzip compressed data, was "caen_hv_py-1.5.tar", last modified: Fri Apr 26 11:34:42 2024, max compression
```

## Comparing `caen_hv_py-1.4.tar` & `caen_hv_py-1.5.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 11:21:15.241642 caen_hv_py-1.4/
--rw-rw-rw-   0        0        0     2129 2024-04-26 11:21:15.241642 caen_hv_py-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1828 2024-04-26 09:31:10.000000 caen_hv_py-1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 11:21:15.231633 caen_hv_py-1.4/caen_hv_py/
--rw-rw-rw-   0        0        0     4256 2024-04-26 11:19:00.000000 caen_hv_py-1.4/caen_hv_py/CAENHVController.py
--rw-rw-rw-   0        0        0      186 2024-04-26 09:31:10.000000 caen_hv_py-1.4/caen_hv_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 11:21:15.240640 caen_hv_py-1.4/caen_hv_py/hv_c_lib/
--rw-rw-rw-   0        0        0    12656 2024-04-26 09:31:10.000000 caen_hv_py-1.4/caen_hv_py/hv_c_lib/libhv_c.so
-drwxrwxrwx   0        0        0        0 2024-04-26 11:21:15.239640 caen_hv_py-1.4/caen_hv_py.egg-info/
--rw-rw-rw-   0        0        0     2129 2024-04-26 11:21:15.000000 caen_hv_py-1.4/caen_hv_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-04-26 11:21:15.000000 caen_hv_py-1.4/caen_hv_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 11:21:15.000000 caen_hv_py-1.4/caen_hv_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 11:21:15.000000 caen_hv_py-1.4/caen_hv_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 11:21:15.241642 caen_hv_py-1.4/setup.cfg
--rw-rw-rw-   0        0        0      884 2024-04-26 11:20:52.000000 caen_hv_py-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:34:42.018392 caen_hv_py-1.5/
+-rw-rw-rw-   0        0        0     2129 2024-04-26 11:34:42.018392 caen_hv_py-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1828 2024-04-26 09:31:10.000000 caen_hv_py-1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 11:34:41.995248 caen_hv_py-1.5/caen_hv_py/
+-rw-rw-rw-   0        0        0     4297 2024-04-26 11:29:21.000000 caen_hv_py-1.5/caen_hv_py/CAENHVController.py
+-rw-rw-rw-   0        0        0      186 2024-04-26 09:31:10.000000 caen_hv_py-1.5/caen_hv_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:34:42.008382 caen_hv_py-1.5/caen_hv_py/hv_c_lib/
+-rw-rw-rw-   0        0        0    12656 2024-04-26 09:31:10.000000 caen_hv_py-1.5/caen_hv_py/hv_c_lib/libhv_c.so
+drwxrwxrwx   0        0        0        0 2024-04-26 11:34:42.017392 caen_hv_py-1.5/caen_hv_py/tests/
+-rw-rw-rw-   0        0        0      184 2024-04-26 11:20:34.000000 caen_hv_py-1.5/caen_hv_py/tests/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-04-26 11:03:59.000000 caen_hv_py-1.5/caen_hv_py/tests/power_test.py
+-rw-rw-rw-   0        0        0     1804 2024-04-26 09:31:10.000000 caen_hv_py-1.5/caen_hv_py/tests/voltage_power_test.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:34:42.007382 caen_hv_py-1.5/caen_hv_py.egg-info/
+-rw-rw-rw-   0        0        0     2129 2024-04-26 11:34:41.000000 caen_hv_py-1.5/caen_hv_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-04-26 11:34:41.000000 caen_hv_py-1.5/caen_hv_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 11:34:41.000000 caen_hv_py-1.5/caen_hv_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 11:34:41.000000 caen_hv_py-1.5/caen_hv_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 11:34:42.018392 caen_hv_py-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      832 2024-04-26 11:34:37.000000 caen_hv_py-1.5/setup.py
```

### Comparing `caen_hv_py-1.4/PKG-INFO` & `caen_hv_py-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caen_hv_py
-Version: 1.4
+Version: 1.5
 Summary: Python wrapper for CAEN High Voltage C library.
 Home-page: https://github.com/Dyn0402/CAEN_HV_Python
 Author: Dylan Neff
 Author-email: dneff@ucla.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `caen_hv_py-1.4/README.md` & `caen_hv_py-1.5/README.md`

 * *Files identical despite different names*

### Comparing `caen_hv_py-1.4/caen_hv_py/CAENHVController.py` & `caen_hv_py-1.5/caen_hv_py/CAENHVController.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 Created as CAEN_HV_Python/CAENHVController.py
 
 @author: Dylan Neff, Dylan
 """
 
 import ctypes
 import ctypes.util
+from pkg_resources import resource_filename
 
 
 class CAENHVController:
     """
     Wrapper class for the CAEN HV C library. This class loads the shared library and defines the function prototypes
     Needed to call the functions in the shared library. The class has methods that call the C functions with the proper
     parameters and return the results.
 
     Need to make a call within 15 seconds of the last, otherwise the connection will be lost and the sys_handle will be
     invalid. This is a limitation of the C library.
     """
-    def __init__(self, ip_address, username, password, library_path='/hv_c_lib/libhv_c.so'):
-        self.library_path = library_path
+    def __init__(self, ip_address, username, password):
+        self.library_path = resource_filename('caen_hv_py', 'libhv_c.so')
         self.ip_address = ip_address
         self.username = username
         self.password = password
         self.sys_handle = None
 
     def __enter__(self):
         # Load the shared library
```

### Comparing `caen_hv_py-1.4/caen_hv_py/hv_c_lib/libhv_c.so` & `caen_hv_py-1.5/caen_hv_py/hv_c_lib/libhv_c.so`

 * *Files identical despite different names*

### Comparing `caen_hv_py-1.4/caen_hv_py.egg-info/PKG-INFO` & `caen_hv_py-1.5/caen_hv_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caen-hv-py
-Version: 1.4
+Version: 1.5
 Summary: Python wrapper for CAEN High Voltage C library.
 Home-page: https://github.com/Dyn0402/CAEN_HV_Python
 Author: Dylan Neff
 Author-email: dneff@ucla.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

