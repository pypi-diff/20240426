# Comparing `tmp/caen_hv_py-1.3.tar.gz` & `tmp/caen_hv_py-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caen_hv_py-1.3.tar", last modified: Fri Apr 26 11:16:14 2024, max compression
+gzip compressed data, was "caen_hv_py-1.4.tar", last modified: Fri Apr 26 11:21:15 2024, max compression
```

## Comparing `caen_hv_py-1.3.tar` & `caen_hv_py-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 11:16:14.663973 caen_hv_py-1.3/
--rw-rw-rw-   0        0        0     2129 2024-04-26 11:16:14.663973 caen_hv_py-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1828 2024-04-26 09:31:10.000000 caen_hv_py-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 11:16:14.652963 caen_hv_py-1.3/caen_hv_py/
--rw-rw-rw-   0        0        0     4491 2024-04-26 11:00:04.000000 caen_hv_py-1.3/caen_hv_py/CAENHVController.py
--rw-rw-rw-   0        0        0      186 2024-04-26 09:31:10.000000 caen_hv_py-1.3/caen_hv_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 11:16:14.662972 caen_hv_py-1.3/caen_hv_py/hv_c_lib/
--rw-rw-rw-   0        0        0    12656 2024-04-26 09:31:10.000000 caen_hv_py-1.3/caen_hv_py/hv_c_lib/libhv_c.so
-drwxrwxrwx   0        0        0        0 2024-04-26 11:16:14.662972 caen_hv_py-1.3/caen_hv_py.egg-info/
--rw-rw-rw-   0        0        0     2129 2024-04-26 11:16:14.000000 caen_hv_py-1.3/caen_hv_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-04-26 11:16:14.000000 caen_hv_py-1.3/caen_hv_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 11:16:14.000000 caen_hv_py-1.3/caen_hv_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 11:16:14.000000 caen_hv_py-1.3/caen_hv_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 11:16:14.664974 caen_hv_py-1.3/setup.cfg
--rw-rw-rw-   0        0        0      870 2024-04-26 11:16:03.000000 caen_hv_py-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:21:15.241642 caen_hv_py-1.4/
+-rw-rw-rw-   0        0        0     2129 2024-04-26 11:21:15.241642 caen_hv_py-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1828 2024-04-26 09:31:10.000000 caen_hv_py-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 11:21:15.231633 caen_hv_py-1.4/caen_hv_py/
+-rw-rw-rw-   0        0        0     4256 2024-04-26 11:19:00.000000 caen_hv_py-1.4/caen_hv_py/CAENHVController.py
+-rw-rw-rw-   0        0        0      186 2024-04-26 09:31:10.000000 caen_hv_py-1.4/caen_hv_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:21:15.240640 caen_hv_py-1.4/caen_hv_py/hv_c_lib/
+-rw-rw-rw-   0        0        0    12656 2024-04-26 09:31:10.000000 caen_hv_py-1.4/caen_hv_py/hv_c_lib/libhv_c.so
+drwxrwxrwx   0        0        0        0 2024-04-26 11:21:15.239640 caen_hv_py-1.4/caen_hv_py.egg-info/
+-rw-rw-rw-   0        0        0     2129 2024-04-26 11:21:15.000000 caen_hv_py-1.4/caen_hv_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-04-26 11:21:15.000000 caen_hv_py-1.4/caen_hv_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 11:21:15.000000 caen_hv_py-1.4/caen_hv_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 11:21:15.000000 caen_hv_py-1.4/caen_hv_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 11:21:15.241642 caen_hv_py-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      884 2024-04-26 11:20:52.000000 caen_hv_py-1.4/setup.py
```

### Comparing `caen_hv_py-1.3/PKG-INFO` & `caen_hv_py-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caen_hv_py
-Version: 1.3
+Version: 1.4
 Summary: Python wrapper for CAEN High Voltage C library.
 Home-page: https://github.com/Dyn0402/CAEN_HV_Python
 Author: Dylan Neff
 Author-email: dneff@ucla.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `caen_hv_py-1.3/README.md` & `caen_hv_py-1.4/README.md`

 * *Files identical despite different names*

### Comparing `caen_hv_py-1.3/caen_hv_py/CAENHVController.py` & `caen_hv_py-1.4/caen_hv_py/CAENHVController.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,27 +17,23 @@
     Wrapper class for the CAEN HV C library. This class loads the shared library and defines the function prototypes
     Needed to call the functions in the shared library. The class has methods that call the C functions with the proper
     parameters and return the results.
 
     Need to make a call within 15 seconds of the last, otherwise the connection will be lost and the sys_handle will be
     invalid. This is a limitation of the C library.
     """
-    def __init__(self, ip_address, username, password, library_path=None):
+    def __init__(self, ip_address, username, password, library_path='/hv_c_lib/libhv_c.so'):
         self.library_path = library_path
         self.ip_address = ip_address
         self.username = username
         self.password = password
         self.sys_handle = None
 
     def __enter__(self):
         # Load the shared library
-        if self.library_path is None:
-            self.library_path = ctypes.util.find_library('libhv_c.so')
-        if self.library_path is None:
-            raise FileNotFoundError('Library path not provided and not found in standard locations.')
         self.library = ctypes.CDLL(self.library_path)
         self.sys_handle = self.log_in()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.sys_handle is not None:
             self.log_out()
```

### Comparing `caen_hv_py-1.3/caen_hv_py/hv_c_lib/libhv_c.so` & `caen_hv_py-1.4/caen_hv_py/hv_c_lib/libhv_c.so`

 * *Files identical despite different names*

### Comparing `caen_hv_py-1.3/caen_hv_py.egg-info/PKG-INFO` & `caen_hv_py-1.4/caen_hv_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caen-hv-py
-Version: 1.3
+Version: 1.4
 Summary: Python wrapper for CAEN High Voltage C library.
 Home-page: https://github.com/Dyn0402/CAEN_HV_Python
 Author: Dylan Neff
 Author-email: dneff@ucla.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `caen_hv_py-1.3/setup.py` & `caen_hv_py-1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='caen_hv_py',
-    version='1.3',
+    version='1.4',
     description='Python wrapper for CAEN High Voltage C library.',
     author='Dylan Neff',
     author_email='dneff@ucla.edu',
     url='https://github.com/Dyn0402/CAEN_HV_Python',
     packages=['caen_hv_py'],
     # data_files=[('libs', ['caen_hv_py/hv_c_lib/libhv_c.so'])],
-    package_data={'caen_hv_py': ['hv_c_lib/libhv_c.so']},
+    package_data={'caen_hv_py': ['hv_c_lib/libhv_c.so', 'tests/*.py']},
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

