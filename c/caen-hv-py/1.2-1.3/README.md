# Comparing `tmp/caen_hv_py-1.2.tar.gz` & `tmp/caen_hv_py-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caen_hv_py-1.2.tar", last modified: Fri Apr 26 11:00:50 2024, max compression
+gzip compressed data, was "caen_hv_py-1.3.tar", last modified: Fri Apr 26 11:16:14 2024, max compression
```

## Comparing `caen_hv_py-1.2.tar` & `caen_hv_py-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 11:00:50.894190 caen_hv_py-1.2/
--rw-rw-rw-   0        0        0     2129 2024-04-26 11:00:50.893188 caen_hv_py-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1828 2024-04-26 09:31:10.000000 caen_hv_py-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 11:00:50.885182 caen_hv_py-1.2/caen_hv_py/
--rw-rw-rw-   0        0        0     4491 2024-04-26 11:00:04.000000 caen_hv_py-1.2/caen_hv_py/CAENHVController.py
--rw-rw-rw-   0        0        0      186 2024-04-26 09:31:10.000000 caen_hv_py-1.2/caen_hv_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 11:00:50.892188 caen_hv_py-1.2/caen_hv_py/hv_c_lib/
--rw-rw-rw-   0        0        0    12656 2024-04-26 09:31:10.000000 caen_hv_py-1.2/caen_hv_py/hv_c_lib/libhv_c.so
-drwxrwxrwx   0        0        0        0 2024-04-26 11:00:50.892188 caen_hv_py-1.2/caen_hv_py.egg-info/
--rw-rw-rw-   0        0        0     2129 2024-04-26 11:00:50.000000 caen_hv_py-1.2/caen_hv_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-04-26 11:00:50.000000 caen_hv_py-1.2/caen_hv_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 11:00:50.000000 caen_hv_py-1.2/caen_hv_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 11:00:50.000000 caen_hv_py-1.2/caen_hv_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 11:00:50.894190 caen_hv_py-1.2/setup.cfg
--rw-rw-rw-   0        0        0      809 2024-04-26 11:00:30.000000 caen_hv_py-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:16:14.663973 caen_hv_py-1.3/
+-rw-rw-rw-   0        0        0     2129 2024-04-26 11:16:14.663973 caen_hv_py-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1828 2024-04-26 09:31:10.000000 caen_hv_py-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 11:16:14.652963 caen_hv_py-1.3/caen_hv_py/
+-rw-rw-rw-   0        0        0     4491 2024-04-26 11:00:04.000000 caen_hv_py-1.3/caen_hv_py/CAENHVController.py
+-rw-rw-rw-   0        0        0      186 2024-04-26 09:31:10.000000 caen_hv_py-1.3/caen_hv_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:16:14.662972 caen_hv_py-1.3/caen_hv_py/hv_c_lib/
+-rw-rw-rw-   0        0        0    12656 2024-04-26 09:31:10.000000 caen_hv_py-1.3/caen_hv_py/hv_c_lib/libhv_c.so
+drwxrwxrwx   0        0        0        0 2024-04-26 11:16:14.662972 caen_hv_py-1.3/caen_hv_py.egg-info/
+-rw-rw-rw-   0        0        0     2129 2024-04-26 11:16:14.000000 caen_hv_py-1.3/caen_hv_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-04-26 11:16:14.000000 caen_hv_py-1.3/caen_hv_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 11:16:14.000000 caen_hv_py-1.3/caen_hv_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 11:16:14.000000 caen_hv_py-1.3/caen_hv_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 11:16:14.664974 caen_hv_py-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      870 2024-04-26 11:16:03.000000 caen_hv_py-1.3/setup.py
```

### Comparing `caen_hv_py-1.2/PKG-INFO` & `caen_hv_py-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caen_hv_py
-Version: 1.2
+Version: 1.3
 Summary: Python wrapper for CAEN High Voltage C library.
 Home-page: https://github.com/Dyn0402/CAEN_HV_Python
 Author: Dylan Neff
 Author-email: dneff@ucla.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `caen_hv_py-1.2/README.md` & `caen_hv_py-1.3/README.md`

 * *Files identical despite different names*

### Comparing `caen_hv_py-1.2/caen_hv_py/CAENHVController.py` & `caen_hv_py-1.3/caen_hv_py/CAENHVController.py`

 * *Files identical despite different names*

### Comparing `caen_hv_py-1.2/caen_hv_py/hv_c_lib/libhv_c.so` & `caen_hv_py-1.3/caen_hv_py/hv_c_lib/libhv_c.so`

 * *Files identical despite different names*

### Comparing `caen_hv_py-1.2/caen_hv_py.egg-info/PKG-INFO` & `caen_hv_py-1.3/caen_hv_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caen-hv-py
-Version: 1.2
+Version: 1.3
 Summary: Python wrapper for CAEN High Voltage C library.
 Home-page: https://github.com/Dyn0402/CAEN_HV_Python
 Author: Dylan Neff
 Author-email: dneff@ucla.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `caen_hv_py-1.2/setup.py` & `caen_hv_py-1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='caen_hv_py',
-    version='1.2',
+    version='1.3',
     description='Python wrapper for CAEN High Voltage C library.',
     author='Dylan Neff',
     author_email='dneff@ucla.edu',
     url='https://github.com/Dyn0402/CAEN_HV_Python',
     packages=['caen_hv_py'],
-    data_files=[('libs', ['caen_hv_py/hv_c_lib/libhv_c.so'])],
+    # data_files=[('libs', ['caen_hv_py/hv_c_lib/libhv_c.so'])],
+    package_data={'caen_hv_py': ['hv_c_lib/libhv_c.so']},
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

