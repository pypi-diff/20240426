# Comparing `tmp/daxa-0.0.2.tar.gz` & `tmp/daxa-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daxa-0.0.2.tar", last modified: Thu Apr 25 20:54:06 2024, max compression
+gzip compressed data, was "daxa-0.0.3.tar", last modified: Thu Apr 25 22:00:35 2024, max compression
```

## Comparing `daxa-0.0.2.tar` & `daxa-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:54:06.754969 daxa-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-25 20:54:03.000000 daxa-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-25 20:54:03.000000 daxa-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-25 20:54:06.754969 daxa-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-25 20:54:03.000000 daxa-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:54:06.750969 daxa-0.0.2/daxa/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:54:06.754969 daxa-0.0.2/daxa/files/
--rw-r--r--   0 runner    (1001) docker     (127)    19204 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/files/browse_extract.pl
--rw-r--r--   0 runner    (1001) docker     (127)   128218 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/files/daxa-high-resolution-color-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   147370 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/files/daxa-high-resolution-logo-black-on-transparent-background.png
--rw-r--r--   0 runner    (1001) docker     (127)   108001 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/files/daxa-high-resolution-logo-black-on-white-background.png
--rw-r--r--   0 runner    (1001) docker     (127)   558372 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/files/erass_de_dr1_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)    35542 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/files/erosita_calpv_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21704 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/files/sas_errors.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15345 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/files/sas_warnings.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-25 20:54:03.000000 daxa-0.0.2/daxa/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:54:06.754969 daxa-0.0.2/daxa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-25 20:54:06.000000 daxa-0.0.2/daxa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-25 20:54:06.000000 daxa-0.0.2/daxa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:54:06.000000 daxa-0.0.2/daxa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 20:54:06.000000 daxa-0.0.2/daxa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 20:54:06.000000 daxa-0.0.2/daxa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 20:54:06.754969 daxa-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-25 20:54:04.000000 daxa-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:00:35.882563 daxa-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-25 22:00:32.000000 daxa-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-25 22:00:32.000000 daxa-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-25 22:00:35.882563 daxa-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-25 22:00:32.000000 daxa-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:00:35.878563 daxa-0.0.3/daxa/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:00:35.882563 daxa-0.0.3/daxa/files/
+-rw-r--r--   0 runner    (1001) docker     (127)    19204 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/files/browse_extract.pl
+-rw-r--r--   0 runner    (1001) docker     (127)   128218 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/files/daxa-high-resolution-color-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   147370 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/files/daxa-high-resolution-logo-black-on-transparent-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)   108001 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/files/daxa-high-resolution-logo-black-on-white-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)   558372 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/files/erass_de_dr1_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    35542 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/files/erosita_calpv_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21704 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/files/sas_errors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15345 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/files/sas_warnings.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-25 22:00:32.000000 daxa-0.0.3/daxa/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:00:35.882563 daxa-0.0.3/daxa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-25 22:00:35.000000 daxa-0.0.3/daxa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-25 22:00:35.000000 daxa-0.0.3/daxa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 22:00:35.000000 daxa-0.0.3/daxa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-25 22:00:35.000000 daxa-0.0.3/daxa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 22:00:35.000000 daxa-0.0.3/daxa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 22:00:35.882563 daxa-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-25 22:00:34.000000 daxa-0.0.3/setup.py
```

### Comparing `daxa-0.0.2/LICENSE` & `daxa-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/PKG-INFO` & `daxa-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: daxa
-Version: 0.0.2
+Version: 0.0.3
 Summary: Democratising Astronomy X-ray Archives (DAXA) is an easy-to-use Python module which enables the simple processing and reduction of archives of X-ray telescope observations.
 Home-page: https://github.com/DavidT3/DAXA
 Author: David J Turner
 Author-email: turne540@msu.edu
 License: BSD 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy==1.23.4
-Requires-Dist: astroquery==0.4.6
-Requires-Dist: pandas==1.5.1
-Requires-Dist: astropy==5.1.1
+Requires-Dist: numpy==1.24.4
+Requires-Dist: astroquery==0.4.7
+Requires-Dist: pandas==2.0.3
+Requires-Dist: astropy==5.2.2
 Requires-Dist: packaging==21.3
-Requires-Dist: tqdm==4.64.1
+Requires-Dist: tqdm==4.66.2
 Requires-Dist: exceptiongroup==1.0.4
-Requires-Dist: scipy==1.1.0
+Requires-Dist: scipy==1.10.1
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: unlzw3==0.2.2
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/DavidT3/DAXA/master/daxa/files/daxa-high-resolution-logo-black-on-white-background.png" width="500">
 </p>
```

### Comparing `daxa-0.0.2/README.md` & `daxa-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa/config.py` & `daxa-0.0.3/daxa/config.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa/exceptions.py` & `daxa-0.0.3/daxa/exceptions.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa/files/browse_extract.pl` & `daxa-0.0.3/daxa/files/browse_extract.pl`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa/files/daxa-high-resolution-color-logo.png` & `daxa-0.0.3/daxa/files/daxa-high-resolution-color-logo.png`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa/files/daxa-high-resolution-logo-black-on-transparent-background.png` & `daxa-0.0.3/daxa/files/daxa-high-resolution-logo-black-on-transparent-background.png`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa/files/daxa-high-resolution-logo-black-on-white-background.png` & `daxa-0.0.3/daxa/files/daxa-high-resolution-logo-black-on-white-background.png`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa/files/erass_de_dr1_info.csv` & `daxa-0.0.3/daxa/files/erass_de_dr1_info.csv`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa/files/erosita_calpv_info.csv` & `daxa-0.0.3/daxa/files/erosita_calpv_info.csv`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa/files/sas_errors.csv` & `daxa-0.0.3/daxa/files/sas_errors.csv`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa/files/sas_warnings.csv` & `daxa-0.0.3/daxa/files/sas_warnings.csv`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa/misc.py` & `daxa-0.0.3/daxa/misc.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/daxa.egg-info/PKG-INFO` & `daxa-0.0.3/daxa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: daxa
-Version: 0.0.2
+Version: 0.0.3
 Summary: Democratising Astronomy X-ray Archives (DAXA) is an easy-to-use Python module which enables the simple processing and reduction of archives of X-ray telescope observations.
 Home-page: https://github.com/DavidT3/DAXA
 Author: David J Turner
 Author-email: turne540@msu.edu
 License: BSD 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy==1.23.4
-Requires-Dist: astroquery==0.4.6
-Requires-Dist: pandas==1.5.1
-Requires-Dist: astropy==5.1.1
+Requires-Dist: numpy==1.24.4
+Requires-Dist: astroquery==0.4.7
+Requires-Dist: pandas==2.0.3
+Requires-Dist: astropy==5.2.2
 Requires-Dist: packaging==21.3
-Requires-Dist: tqdm==4.64.1
+Requires-Dist: tqdm==4.66.2
 Requires-Dist: exceptiongroup==1.0.4
-Requires-Dist: scipy==1.1.0
+Requires-Dist: scipy==1.10.1
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: unlzw3==0.2.2
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/DavidT3/DAXA/master/daxa/files/daxa-high-resolution-logo-black-on-white-background.png" width="500">
 </p>
```

### Comparing `daxa-0.0.2/daxa.egg-info/SOURCES.txt` & `daxa-0.0.3/daxa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daxa-0.0.2/setup.py` & `daxa-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #  This code is a part of the Democratising Archival X-ray Astronomy (DAXA) module.
-#  Last modified by David J Turner (turne540@msu.edu) 25/04/2024, 16:01. Copyright (c) The Contributors
+#  Last modified by David J Turner (turne540@msu.edu) 25/04/2024, 17:54. Copyright (c) The Contributors
 
 from os import path
 
 from setuptools import setup
 
 # Uses the README as the long description
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='daxa',
-    version='v0.0.2',
+    version='v0.0.3',
     packages=['daxa'],
     url='https://github.com/DavidT3/DAXA',
     license='BSD 3',
     author='David J Turner',
     author_email='turne540@msu.edu',
     description='Democratising Astronomy X-ray Archives (DAXA) is an easy-to-use Python module which enables '
                 'the simple processing and reduction of archives of X-ray telescope observations.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     setup_requires=[],
-    install_requires=["numpy==1.23.4", "astroquery==0.4.6", "pandas==1.5.1", "astropy==5.1.1", "packaging==21.3",
-                      "tqdm==4.64.1", "exceptiongroup==1.0.4", "scipy==1.1.0", "tabulate==0.9.0", "unlzw3==0.2.2"],
+    install_requires=["numpy==1.24.4", "astroquery==0.4.7", "pandas==2.0.3", "astropy==5.2.2", "packaging==21.3",
+                      "tqdm==4.66.2", "exceptiongroup==1.0.4", "scipy==1.10.1", "tabulate==0.9.0", "unlzw3==0.2.2"],
     include_package_data=True,
     python_requires='>=3.8'
 )
```

