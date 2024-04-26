# Comparing `tmp/caen_hv_py-1.0.tar.gz` & `tmp/caen_hv_py-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caen_hv_py-1.0.tar", last modified: Fri Apr 26 09:32:32 2024, max compression
+gzip compressed data, was "caen_hv_py-1.1.tar", last modified: Fri Apr 26 09:58:49 2024, max compression
```

## Comparing `caen_hv_py-1.0.tar` & `caen_hv_py-1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 09:32:32.864531 caen_hv_py-1.0/
--rw-rw-rw-   0        0        0     2129 2024-04-26 09:32:32.863530 caen_hv_py-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1828 2024-04-26 09:31:10.000000 caen_hv_py-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 09:32:32.852521 caen_hv_py-1.0/caen_hv_py/
-drwxrwxrwx   0        0        0        0 2024-04-26 09:32:32.862529 caen_hv_py-1.0/caen_hv_py/hv_c_lib/
--rw-rw-rw-   0        0        0    12656 2024-04-26 09:31:10.000000 caen_hv_py-1.0/caen_hv_py/hv_c_lib/libhv_c.so
-drwxrwxrwx   0        0        0        0 2024-04-26 09:32:32.862529 caen_hv_py-1.0/caen_hv_py.egg-info/
--rw-rw-rw-   0        0        0     2129 2024-04-26 09:32:32.000000 caen_hv_py-1.0/caen_hv_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-04-26 09:32:32.000000 caen_hv_py-1.0/caen_hv_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 09:32:32.000000 caen_hv_py-1.0/caen_hv_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 09:32:32.000000 caen_hv_py-1.0/caen_hv_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 09:32:32.864531 caen_hv_py-1.0/setup.cfg
--rw-rw-rw-   0        0        0      815 2024-04-26 09:32:24.000000 caen_hv_py-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:58:49.070232 caen_hv_py-1.1/
+-rw-rw-rw-   0        0        0     2129 2024-04-26 09:58:49.070232 caen_hv_py-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1828 2024-04-26 09:31:10.000000 caen_hv_py-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 09:58:49.055217 caen_hv_py-1.1/caen_hv_py/
+-rw-rw-rw-   0        0        0     4235 2024-04-26 09:31:10.000000 caen_hv_py-1.1/caen_hv_py/CAENHVController.py
+-rw-rw-rw-   0        0        0      186 2024-04-26 09:31:10.000000 caen_hv_py-1.1/caen_hv_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:58:49.069230 caen_hv_py-1.1/caen_hv_py/hv_c_lib/
+-rw-rw-rw-   0        0        0    12656 2024-04-26 09:31:10.000000 caen_hv_py-1.1/caen_hv_py/hv_c_lib/libhv_c.so
+drwxrwxrwx   0        0        0        0 2024-04-26 09:58:49.068229 caen_hv_py-1.1/caen_hv_py.egg-info/
+-rw-rw-rw-   0        0        0     2129 2024-04-26 09:58:49.000000 caen_hv_py-1.1/caen_hv_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-04-26 09:58:49.000000 caen_hv_py-1.1/caen_hv_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 09:58:49.000000 caen_hv_py-1.1/caen_hv_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 09:58:49.000000 caen_hv_py-1.1/caen_hv_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 09:58:49.070232 caen_hv_py-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      809 2024-04-26 09:58:36.000000 caen_hv_py-1.1/setup.py
```

### Comparing `caen_hv_py-1.0/PKG-INFO` & `caen_hv_py-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caen_hv_py
-Version: 1.0
+Version: 1.1
 Summary: Python wrapper for CAEN High Voltage C library.
 Home-page: https://github.com/Dyn0402/CAEN_HV_Python
 Author: Dylan Neff
 Author-email: dneff@ucla.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `caen_hv_py-1.0/README.md` & `caen_hv_py-1.1/README.md`

 * *Files identical despite different names*

### Comparing `caen_hv_py-1.0/caen_hv_py/hv_c_lib/libhv_c.so` & `caen_hv_py-1.1/caen_hv_py/hv_c_lib/libhv_c.so`

 * *Files identical despite different names*

### Comparing `caen_hv_py-1.0/caen_hv_py.egg-info/PKG-INFO` & `caen_hv_py-1.1/caen_hv_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caen-hv-py
-Version: 1.0
+Version: 1.1
 Summary: Python wrapper for CAEN High Voltage C library.
 Home-page: https://github.com/Dyn0402/CAEN_HV_Python
 Author: Dylan Neff
 Author-email: dneff@ucla.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `caen_hv_py-1.0/setup.py` & `caen_hv_py-1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='caen_hv_py',
-    version='1.0',
+    version='1.1',
     description='Python wrapper for CAEN High Voltage C library.',
     author='Dylan Neff',
     author_email='dneff@ucla.edu',
     url='https://github.com/Dyn0402/CAEN_HV_Python',
-    # packages=['CAEN_HV_Python'],
+    packages=['caen_hv_py'],
     data_files=[('libs', ['caen_hv_py/hv_c_lib/libhv_c.so'])],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

