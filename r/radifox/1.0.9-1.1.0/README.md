# Comparing `tmp/radifox-1.0.9.tar.gz` & `tmp/radifox-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radifox-1.0.9.tar", last modified: Tue Apr  2 01:21:35 2024, max compression
+gzip compressed data, was "radifox-1.1.0.tar", last modified: Fri Apr 26 01:37:17 2024, max compression
```

## Comparing `radifox-1.0.9.tar` & `radifox-1.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.503653 radifox-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-02 01:21:29.000000 radifox-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-04-02 01:21:35.503653 radifox-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    45907 2024-04-02 01:21:29.000000 radifox-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.503653 radifox-1.0.9/radifox/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 01:21:35.503653 radifox-1.0.9/radifox/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.499653 radifox-1.0.9/radifox/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/dicom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/lut.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    55768 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/nib_parrec_fork.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/parrec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.499653 radifox-1.0.9/radifox/conversion/parrec_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/parrec_templates/gen_info.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/parrec_templates/pixel_values.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/parrec_templates/top_header.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/parrec_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/conversion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.499653 radifox-1.0.9/radifox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16756 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/modules/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.499653 radifox-1.0.9/radifox/naming/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/naming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/naming/imagefile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.499653 radifox-1.0.9/radifox/qa/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.503653 radifox-1.0.9/radifox/qa/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/conversion.html
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/processing.html
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/project.html
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/qa/templates/subject.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.503653 radifox-1.0.9/radifox/records/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/records/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 01:21:29.000000 radifox-1.0.9/radifox/records/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:21:35.503653 radifox-1.0.9/radifox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 01:21:35.000000 radifox-1.0.9/radifox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:21:35.503653 radifox-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-02 01:21:29.000000 radifox-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:37:17.338082 radifox-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-26 01:37:13.000000 radifox-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-04-26 01:37:17.338082 radifox-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    45907 2024-04-26 01:37:13.000000 radifox-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:37:17.338082 radifox-1.1.0/radifox/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-26 01:37:17.338082 radifox-1.1.0/radifox/_static_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:37:17.334082 radifox-1.1.0/radifox/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/lut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55768 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/nib_parrec_fork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/parrec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:37:17.334082 radifox-1.1.0/radifox/conversion/parrec_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/parrec_templates/gen_info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/parrec_templates/pixel_values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/parrec_templates/top_header.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/parrec_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/conversion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:37:17.334082 radifox-1.1.0/radifox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16756 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/modules/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:37:17.334082 radifox-1.1.0/radifox/naming/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/naming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/naming/imagefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:37:17.334082 radifox-1.1.0/radifox/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/qa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/qa/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/qa/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:37:17.334082 radifox-1.1.0/radifox/qa/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    25968 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/qa/templates/conversion.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/qa/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/qa/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22900 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/qa/templates/processing.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/qa/templates/project.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/qa/templates/subject.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:37:17.338082 radifox-1.1.0/radifox/records/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/records/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-26 01:37:13.000000 radifox-1.1.0/radifox/records/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:37:17.338082 radifox-1.1.0/radifox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-04-26 01:37:17.000000 radifox-1.1.0/radifox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-26 01:37:17.000000 radifox-1.1.0/radifox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:37:17.000000 radifox-1.1.0/radifox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-26 01:37:17.000000 radifox-1.1.0/radifox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 01:37:17.000000 radifox-1.1.0/radifox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 01:37:17.000000 radifox-1.1.0/radifox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 01:37:17.338082 radifox-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-26 01:37:13.000000 radifox-1.1.0/setup.py
```

### Comparing `radifox-1.0.9/LICENSE` & `radifox-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/PKG-INFO` & `radifox-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radifox
-Version: 1.0.9
+Version: 1.1.0
 Summary: RADIFOX is the RADiological Image File Ontology eXtension, a Python package for the organization and management of medical images.
 Home-page: https://github.com/jh-mipc/radifox
 Author: Blake Dewey
 Author-email: blake.dewey@jhu.edu
 License: Apache License, 2.0
 Keywords: mri conversion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `radifox-1.0.9/README.md` & `radifox-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/_version.py` & `radifox-1.1.0/radifox/_version.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/base.py` & `radifox-1.1.0/radifox/conversion/base.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/cli.py` & `radifox-1.1.0/radifox/conversion/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,15 @@
             lut_file,
             args.verbose,
             parrec,
             True,
             None,
             json_obj.get("ManualArgs", {}),
             False,
+            False,
             0,
             manual_names,
             json_obj["InputHash"],
         )
     except ExecError:
         logging.info("Exception caught during update. Resetting to previous state.")
         for filename in ["nii", "qa", json_file.name]:
```

### Comparing `radifox-1.0.9/radifox/conversion/dicom.py` & `radifox-1.1.0/radifox/conversion/dicom.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/exec.py` & `radifox-1.1.0/radifox/conversion/exec.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/json.py` & `radifox-1.1.0/radifox/conversion/json.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/logging.py` & `radifox-1.1.0/radifox/conversion/logging.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/lut.py` & `radifox-1.1.0/radifox/conversion/lut.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/metadata.py` & `radifox-1.1.0/radifox/conversion/metadata.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/nib_parrec_fork.py` & `radifox-1.1.0/radifox/conversion/nib_parrec_fork.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/parrec.py` & `radifox-1.1.0/radifox/conversion/parrec.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/parrec_templates/gen_info.txt` & `radifox-1.1.0/radifox/conversion/parrec_templates/gen_info.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/parrec_templates/pixel_values.txt` & `radifox-1.1.0/radifox/conversion/parrec_templates/pixel_values.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/parrec_writer.py` & `radifox-1.1.0/radifox/conversion/parrec_writer.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/conversion/utils.py` & `radifox-1.1.0/radifox/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/modules/staging.py` & `radifox-1.1.0/radifox/modules/staging.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/naming/imagefile.py` & `radifox-1.1.0/radifox/naming/imagefile.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/qa/app.py` & `radifox-1.1.0/radifox/qa/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import datetime
 import itertools
 import json
 from collections import defaultdict
 from pathlib import Path
 import secrets
 
 from flask import (
@@ -40,25 +41,31 @@
         return redirect(url_for("login"))
 
 
 @app.route("/login", methods=["GET", "POST"])
 def login():
     error = None
     if request.method == "POST":
-        test_key = request.form["key"]
+        key = request.form["key"]
+        user = request.form["user"]
     else:
-        test_key = request.args.get("key")
+        key = request.args.get("key", "")
+        user = ""
 
-    if test_key is not None:
-        if test_key == SECRET_KEY:
-            session["qa_secret_key"] = test_key
-            return redirect(url_for("index"))
+    if key:
+        if key == SECRET_KEY:
+            if user:
+                session["qa_user"] = user
+                session["qa_secret_key"] = key
+                return redirect(url_for("index"))
+            else:
+                error = "Please enter a username"
         else:
             error = "Invalid Key"
-    return render_template("login.html", error=error)
+    return render_template("login.html", error=error, key=key, user=user)
 
 
 @app.route("/")
 def index():
     projects = sorted([proj.name for proj in DATA_DIR.glob("*") if proj.is_dir()])
     return render_template("index.html", projects=projects)
 
@@ -160,14 +167,18 @@
                 if any(
                     [
                         j is not None and i != j
                         for i, j in zip(image_arr, manual_json[si["SourcePath"]])
                     ]
                 ):
                     created_by = "MODIFIED"
+        elif created_by == "LOOKUP":
+            manual_name = "/".join(
+                [item if item is not None else "--" for item in si["LookupName"]]
+            )
         study_num, series_num = si["NiftiName"].split("_")[-2].split("-")
         image_obj = {
             "acq_date_time": si["AcqDateTime"],
             "series_number": series_num,
             "study_number": study_num,
             "acq_number": "%02d" % int(si["SeriesUID"].split(".")[-1]),
             "image_name": si["NiftiName"].split("_")[-1],
@@ -258,35 +269,63 @@
     prov_objs = {
         k: v
         for k, v in sorted(
             prov_objs.items(), key=lambda x: min(val["StartTime"] for val in x[1].values())
         )
     }
 
+    qa_filepath = (
+            DATA_DIR
+            / project_id
+            / subject_id
+            / session_id
+            / "_".join([subject_id, session_id, "QA.yml"])
+    )
+    qa_data = yaml.safe_load_all(qa_filepath.read_text()) if qa_filepath.exists() else []
+    qa_dict = {}
+    for entry in qa_data:
+        qa_dict[entry["file"]] = entry["status"]
+
     for module_str, provs in prov_objs.items():
         for idstr, prov_obj in provs.items():
             prov_obj["OutputQA"] = {}
             for key, val in prov_obj["Outputs"].items():
                 prov_obj["OutputQA"][key] = {}
                 if not isinstance(val, list):
                     val = [val]
                 for v in val:
                     filestr = v.split(":")[0]
+                    if not filestr.endswith(".nii.gz"):
+                        continue
+                    existing_qa = qa_dict.get(filestr, "")
                     filepath = session_dir.parent.parent / filestr
                     qa_path = (
                         filepath.parent.parent
                         / "qa"
                         / module_str.split(":")[0]
                         / (filepath.name.replace(".nii.gz", ".png"))
                     )
+                    display_name = (
+                        filestr.split("_")[2]
+                        + "_"
+                        + " / ".join(filestr.split(".")[0].split("_")[3:])
+                    )
                     prov_obj["OutputQA"][key][filestr] = (
-                        (qa_path.parent.parent.parent.name, qa_path.parent.name, qa_path.name)
+                        (
+                            qa_path.parent.parent.parent.name,
+                            qa_path.parent.name,
+                            qa_path.name,
+                            display_name,
+                            existing_qa,
+                        )
                         if qa_path.exists()
                         else None
                     )
+                if len(prov_obj["OutputQA"][key]) == 0:
+                    del prov_obj["OutputQA"][key]
 
     return render_template(
         "processing.html",
         processing_results=prov_objs,
         project_id=project_id,
         subject_id=subject_id,
         session_id=session_id,
@@ -314,14 +353,32 @@
         / "_".join([subject_id, session_id, "ManualNaming.json"])
     )
     json_obj = json.loads(filepath.read_text()) if filepath.exists() else {}
     json_obj[key] = value
     save_manual(json_obj, filepath)
 
 
+def add_qa_entry(project_id, subject_id, session_id, key, value):
+    filepath = (
+        DATA_DIR
+        / project_id
+        / subject_id
+        / session_id
+        / "_".join([subject_id, session_id, "QA.yml"])
+    )
+    yml_obj = {
+        "user": session["qa_user"],
+        "timestamp": datetime.datetime.now().isoformat(),
+        "file": key,
+        "status": value,
+    }
+    with open(filepath, "a") as f:
+        yaml.safe_dump(yml_obj, f, explicit_start=True, explicit_end=True, sort_keys=True)
+
+
 def update_manual_entry(project_id, subject_id, session_id, data):
     filepath = (
         DATA_DIR
         / project_id
         / subject_id
         / session_id
         / "_".join([subject_id, session_id, "ManualNaming.json"])
@@ -385,14 +442,40 @@
         data["session"],
         data["source"],
         False,
     )
     return jsonify(message="Image Ignored")
 
 
+@app.route("/qa/qa-pass-btn", methods=["POST"])
+def qa_pass_btn():
+    data = request.get_json()
+    add_qa_entry(
+        data["project"],
+        data["subject"],
+        data["session"],
+        data["source"],
+        'pass',
+    )
+    return jsonify(message="QA Pass")
+
+
+@app.route("/qa/qa-fail-btn", methods=["POST"])
+def qa_fail_btn():
+    data = request.get_json()
+    add_qa_entry(
+        data["project"],
+        data["subject"],
+        data["session"],
+        data["source"],
+        'fail',
+    )
+    return jsonify(message="QA Fail")
+
+
 @app.route("/change-btn", methods=["POST"])
 def change_btn():
     data = request.get_json()
     update_manual_entry(
         data["project"],
         data["subject"],
         data["session"],
```

### Comparing `radifox-1.0.9/radifox/qa/create.py` & `radifox-1.1.0/radifox/qa/create.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/qa/run.py` & `radifox-1.1.0/radifox/qa/run.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/qa/templates/conversion.html` & `radifox-1.1.0/radifox/qa/templates/conversion.html`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                     </button>
                 </div>
             </div>
             <div class="row">
                 <div class="col-5">
                     {% if item.manual_name != '' %}
                         <h4 class="{% if item.created_by == 'MODIFIED' %}negative{% else %}neutral{% endif %}">
-                            Manual: {{ item.manual_name }}
+                            {% if item.created_by == 'LOOKUP' %}Lookup{% else %}Manual{% endif %}: {{ item.manual_name }}
                         </h4>
                     {% endif %}
                 </div>
                 <div class="col-7 right-button">
                     <button type="button"
                             onclick="sendPostRequest(this)"
                             data-api="ignore"
```

#### html2text {}

```diff
@@ -6,15 +6,16 @@
 
 {% for item in conversion_images %}
 ******** ##{{{{ iitteemm..ssttuuddyy__nnuummbbeerr }}}}--{{{{ iitteemm..sseerriieess__nnuummbbeerr }}}}--{{{{ iitteemm..aaccqq__nnuummbbeerr }}}}:: {{
 {{ iitteemm..iimmaaggee__nnaammee }}}} ********
 ****** {{{{ iitteemm..ccrreeaatteedd__bbyy }}}} ******
 CORRECT NAME
 {% if item.manual_name != '' %}
-****** MMaannuuaall:: {{{{ iitteemm..mmaannuuaall__nnaammee }}}} ******
+****** {{%% iiff iitteemm..ccrreeaatteedd__bbyy ==== ''LLOOOOKKUUPP'' %%}}LLooookkuupp{{%% eellssee %%}}MMaannuuaall{{%% eennddiiff %%}}:: {{
+{{ iitteemm..mmaannuuaall__nnaammee }}}} ******
 {% endif %}
 IGNORE {% set button_index = loop.index %} {% for part in ["brain", "cspine",
 "tspine", "lspine", "orbits"] %}   {{ part | upper() }} {% endfor %}
 {% if item.image_src %}
 [{{ item.image_name }}]
 {% endif %}
```

### Comparing `radifox-1.0.9/radifox/qa/templates/index.html` & `radifox-1.1.0/radifox/qa/templates/index.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/qa/templates/login.html` & `radifox-1.1.0/radifox/qa/templates/login.html`

 * *Files 8% similar despite different names*

```diff
@@ -58,15 +58,17 @@
             <div class="modal-body">
                 {% if error %}
                     <div class="alert alert-warning" role="alert">
                         {{ error }}
                     </div>
                 {% endif %}
                 <form method="POST" action="{{ url_for('login') }}">
-                    Key: <input type="password" name="key" class="form-control">
+                    User: <input type="text" name="user" value="{{ user }}" class="form-control">
+                    <br />
+                    Key: <input type="password" name="key" value="{{ key }}" class="form-control">
                     <br>
                     <input type="submit" value="Login" class="btn btn-primary">
                 </form>
             </div>
         </div>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 _R_A_D_I_F_O_X_ _Q_A
 **** LLooggiinn RReeqquuiirreedd ****
 {% if error %}
 {{ error }}
 {% endif %}
+User: [{{ user }}          ]
 Key:[********************]
 [Login]
```

### Comparing `radifox-1.0.9/radifox/qa/templates/processing.html` & `radifox-1.1.0/radifox/qa/templates/processing.html`

 * *Files 10% similar despite different names*

```diff
@@ -43,22 +43,14 @@
         }
 
         .right-button {
             display: flex;
             justify-content: right;
             align-items: center;
         }
-
-        .negative {
-            color: red;
-        }
-
-        .neutral {
-            color: black;
-        }
     </style>
     <title>RADIFOX QA - {{ subject_id }}&nbsp;/&nbsp;{{ session_id }}</title>
 </head>
 <body>
 <nav class="navbar navbar-expand-md sticky-top navbar-dark bg-dark">
     <a class="navbar-brand" href="{{ url_for('index') }}">RADIFOX QA</a>
     <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
@@ -79,148 +71,85 @@
     </span>
   </div>
 </nav>
 <br />
 <br />
 <div class="container-fluid">
     {% for key, value in processing_results|items %}
+        {% set steploop = loop %}
         <h2 class="text-center">{{ key | upper() | replace(':', ' v') }}</h2>
         <hr /><hr />
         <br />
         {% for id, prov in value|items %}
+            {% set provloop = loop %}
             {% for output_name, qa_dict in prov.OutputQA|items %}
+                {% set outloop = loop %}
                 <div class="container-fluid">
                     <div class="row"><div class="col">
                         <h4>{{ output_name|replace('_',' ')|title() }}:</h4>
                     </div></div>
                     <div class="row"><div class="col">
                         {% for filestr, qa_img in qa_dict|items %}
-                            <div class="container-fluid outer-container" id="image{{ loop.index }}">
-                                <div class="row"><div class="col"><h5>{{ filestr }}</h5></div></div>
+                            {% set imgloop = loop %}
+                            <div class="container-fluid outer-container" id="image{{ steploop.index }}-{{ provloop.index }}-{{ outloop.index }}-{{ imgloop.index }}">
+                                <div class="row">
+                                    <div class="col-10"><h5>{{ qa_img[3] }}</h5></div>
+                                    <div class="col-2 right-button">
+                                        <button type="button"
+                                                onclick="sendPostRequest(this)"
+                                                data-api="qa-pass"
+                                                data-project="{{ project_id }}"
+                                                data-subject="{{ subject_id }}"
+                                                data-session="{{ session_id }}"
+                                                data-source_path="{{ filestr }}"
+                                                data-loop_index="{{ steploop.index }}-{{ provloop.index }}-{{ outloop.index }}-{{ imgloop.index }}"
+                                                id="qa-pass{{ steploop.index }}-{{ provloop.index }}-{{ outloop.index }}-{{ imgloop.index }}"
+                                                class="btn {% if qa_img[4] == "pass" %}btn-success{% else %}btn-dark{% endif %}">
+                                            PASS
+                                        </button>
+                                        &nbsp;
+                                        <button type="button"
+                                                onclick="sendPostRequest(this)"
+                                                data-api="qa-fail"
+                                                data-project="{{ project_id }}"
+                                                data-subject="{{ subject_id }}"
+                                                data-session="{{ session_id }}"
+                                                data-source_path="{{ filestr }}"
+                                                data-loop_index="{{ steploop.index }}-{{ provloop.index }}-{{ outloop.index }}-{{ imgloop.index }}"
+                                                id="qa-fail{{ steploop.index }}-{{ provloop.index }}-{{ outloop.index }}-{{ imgloop.index }}"
+                                                class="btn {% if qa_img[4] == "fail" %}btn-danger{% else %}btn-dark{% endif %}">
+                                            FAIL
+                                        </button>
+                                    </div>
+                                </div>
                             {% if qa_img %}
                                 <div class="row border-10 border-secondary mx-auto" style="background:#000000; width: 100%">
                                     <div class="col text-center">
                                         <img src="{{ url_for('image', project_id=project_id, subject_id=subject_id, session_id=qa_img[0], qa_dir=qa_img[1], image_name=qa_img[2]) }}"
                                              class="pop img-fluid" alt="{{ qa_img[2] }}" loading="lazy"/>
                                     </div>
                                 </div>
                             {% endif %}
                             </div>
                             <br />
                         {% endfor %}
                     </div></div>
                 </div>
             {% endfor %}
-            <div class="container-fluid" id="image{{ prov.OutputQA|length }}">
-               <br/>
-                <div class="row">
-                    <div class="col">
-                        <h5 class="text-center"><span class="font-weight-bold">ID: </span>{{ prov.Id }}</h5>
-                    </div>
-                </div>
-                <div class="row">
-                    <div class="col">
-                        <h5 class="text-left">
-                            <span class="font-weight-bold">Container:</span>
-                            <br/>
-                            {{ prov.Container.url }}
-                            <br />
-                            {{ prov.Container.hash }}
-                            <br />
-                            Built: {{ prov.Container.timestamp.strftime('%Y-%m-%d %H:%M:%S') }} by {{ prov.Container.builder }}
-                        </h5>
-                    </div>
-                    <div class="col">
-                        <h5 class="text-right">
-                            <span class="font-weight-bold">Run Info:</span>
-                            <br/>
-                            Started: {{ prov.StartTime }}
-                            <br />
-                            Duration: {{ prov.Duration }}
-                            <br />
-                            User: {{ prov.User }}
-                        </h5>
-                    </div>
-                </div>
-                <div class="row">
-                    <div class="col">
-                        <h5 class="text-left">
-                            <span class="font-weight-bold">Inputs:</span>
-                            <br/>
-                            {% for key, value in prov.Inputs|items %}
-                                {% if value is iterable and value is not string %}
-                                    {{ key }}: <br />
-                                    {% for sub in value %}
-                                        {% set val = sub.split(':') %}
-                                        &emsp; - {{ val[0] }}<br />
-                                        <span class="text-muted">&emsp;&emsp;[{{ val[1] }}:{{ val[2] }}]</span><br />
-                                    {% endfor %}
-                                {% else %}
-                                    {% set val = value.split(':') %}
-                                    {{ key }}: {{ val[0] }}<br />
-                                    <span class="text-muted">&emsp;&emsp;[{{ val[1] }}:{{ val[2] }}]</span><br />
-                                {% endif %}
-                            {% endfor %}
-                        </h5>
-                    </div>
-                </div>
-                <div class="row">
-                    <div class="col">
-                        <h5 class="text-left">
-                            <span class="font-weight-bold">Outputs:</span>
-                            <br/>
-                            {% for key, value in prov.Outputs|items %}
-                                {% if value is iterable and value is not string %}
-                                    {{ key }}: <br />
-                                    {% for sub in value %}
-                                        {% set val = sub.split(':') %}
-                                        &emsp; - {{ val[0] }}<br />
-                                        <span class="text-muted">&emsp;&emsp;[{{ val[1] }}:{{ val[2] }}]</span><br />
-                                    {% endfor %}
-                                {% else %}
-                                    {% set val = value.split(':') %}
-                                    {{ key }}: {{ val[0] }}<br />
-                                    <span class="text-muted">&emsp;&emsp;[{{ val[1] }}:{{ val[2] }}]</span><br />
-                                {% endif %}
-                            {% endfor %}
-                        </h5>
-                    </div>
-                </div>
-                <div class="row">
-                    <div class="col">
-                        <h5 class="text-left">
-                            <span class="font-weight-bold">Parameters:</span>
-                            {% if prov.Parameters is mapping %}
-                                <br/>
-                                {% for key, value in prov.Parameters|items %}
-                                    {% if value is iterable and value is not string %}
-                                        {{ key }}: <br />
-                                        {% for sub in value %}
-                                            &emsp; - {{ sub }}<br />
-                                        {% endfor %}
-                                    {% else %}
-                                        {{ key }}: {{ value }}<br />
-                                    {% endif %}
-                                {% endfor %}
-                            {% else %}
-                                None
-                            {% endif %}
-                        </h5>
-                    </div>
-                </div>
-                <div class="row">
-                        <div class="col">
-                            <h5 class="text-left">
-                                <span class="font-weight-bold">Command:</span>
-                                <br/>
-                                {{ prov.Command }}
-                            </h5>
-                        </div>
-                    </div>
-                </div>
+            <div class="container-fluid">
+                <div class="row"><div class="col text-center">
+                    <button type="button"
+                            data-toggle="modal"
+                            data-target="#prov{{ steploop.index }}{{ provloop.index }}"
+                            class="btn btn-dark">
+                        PROVENANCE
+                    </button>
+                </div></div>
+            </div>
+            <hr />
             <br />
         {% endfor %}
         <br /><br />
     {% endfor %}
 </div>
 <button id="scrollToNextContainer" class="btn btn-primary position-fixed mb-4" style="bottom: 20px; right: 5px;">Next Image</button>
 <button id="scrollToPrevContainer" class="btn btn-primary position-fixed mb-4" style="bottom: 20px; right: 125px;">Prev Image</button>
@@ -239,24 +168,147 @@
         {% elif next_subject %}
             <a href="{{ url_for('subject', project_id=project_id, subject_id=next_subject) }}">{{ next_subject }}</a>&nbsp;&nbsp;&rarr;
         {% endif %}
     </span>
 </nav>
 
 <div class="modal fade" id="imagemodal" tabindex="-1" role="dialog" aria-labelledby="myModalLabel" aria-hidden="true">
-    <div class="modal-dialog modal-dialog-centered modal-dialog-scrollable" style="max-width: 100%"
-         data-dismiss="modal">
+    <div class="modal-dialog modal-dialog-centered modal-dialog-scrollable" style="max-width: 100%" data-dismiss="modal">
         <div class="modal-content">
             <div class="modal-body">
                 <img src="" class="imagepreview" alt="full size image">
             </div>
         </div>
     </div>
 </div>
 
+{% for key, value in processing_results|items %}
+    {% set steploop = loop %}
+        {% for id, prov in value|items %}
+            {% set provloop = loop %}
+            <div class="modal fade" id="prov{{ steploop.index }}{{ provloop.index }}" tabindex="-1" role="dialog" aria-labelledby="prov{{ steploop.index }}-{{ provloop.index }}" aria-hidden="true">
+                <div class="modal-dialog modal-dialog-centered modal-dialog-scrollable" style="max-width: 90%" data-dismiss="modal">
+                    <div class="modal-content">
+                        <div class="modal-body">
+                            <div class="container-fluid" id="prov{{ steploop.index }}-{{ provloop.index }}">
+                                <br/>
+                                <div class="row">
+                                    <div class="col">
+                                        <h6 class="text-center"><span class="font-weight-bold" style="font-size: 120%">ID: </span>{{ prov.Id }}</h6>
+                                    </div>
+                                </div>
+                                <div class="row">
+                                    <div class="col">
+                                        <h6 class="text-left">
+                                            <span class="font-weight-bold" style="font-size: 120%">Container:</span>
+                                            <br/>
+                                            {{ prov.Container.url }}
+                                            <br />
+                                            {{ prov.Container.hash }}
+                                            <br />
+                                            Built: {{ prov.Container.timestamp.strftime('%Y-%m-%d %H:%M:%S') }} by {{ prov.Container.builder }}
+                                        </h6>
+                                    </div>
+                                    <div class="col">
+                                        <h6 class="text-right">
+                                            <span class="font-weight-bold" style="font-size: 120%">Run Info:</span>
+                                            <br/>
+                                            Started: {{ prov.StartTime }}
+                                            <br />
+                                            Duration: {{ prov.Duration }}
+                                            <br />
+                                            User: {{ prov.User }}
+                                        </h6>
+                                    </div>
+                                </div>
+                                <div class="row">
+                                    <div class="col">
+                                        <h6 class="text-left">
+                                            <span class="font-weight-bold" style="font-size: 120%">Inputs:</span>
+                                            <br/>
+                                            {% for key, value in prov.Inputs|items %}
+                                                {% if value is iterable and value is not string %}
+                                                    {{ key }}: <br />
+                                                    {% for sub in value %}
+                                                        {% set val = sub.split(':') %}
+                                                        &emsp; - {{ val[0] }}<br />
+                                                        <span class="text-muted">&emsp;&emsp;[{{ val[1] }}:{{ val[2] }}]</span><br />
+                                                    {% endfor %}
+                                                {% else %}
+                                                    {% set val = value.split(':') %}
+                                                    {{ key }}: <br />
+                                                    &emsp; - {{ val[0] }}<br />
+                                                    <span class="text-muted">&emsp;&emsp;[{{ val[1] }}:{{ val[2] }}]</span><br />
+                                                {% endif %}
+                                            {% endfor %}
+                                        </h6>
+                                    </div>
+                                </div>
+                                <div class="row">
+                                    <div class="col">
+                                        <h6 class="text-left">
+                                            <span class="font-weight-bold" style="font-size: 120%">Outputs:</span>
+                                            <br/>
+                                            {% for key, value in prov.Outputs|items %}
+                                                {% if value is iterable and value is not string %}
+                                                    {{ key }}: <br />
+                                                    {% for sub in value %}
+                                                        {% set val = sub.split(':') %}
+                                                        &emsp; - {{ val[0] }}<br />
+                                                        <span class="text-muted">&emsp;&emsp;[{{ val[1] }}:{{ val[2] }}]</span><br />
+                                                    {% endfor %}
+                                                {% else %}
+                                                    {% set val = value.split(':') %}
+                                                    {{ key }}: <br />
+                                                    &emsp; - {{ val[0] }}<br />
+                                                    <span class="text-muted">&emsp;&emsp;[{{ val[1] }}:{{ val[2] }}]</span><br />
+                                                {% endif %}
+                                            {% endfor %}
+                                        </h6>
+                                    </div>
+                                </div>
+                                <div class="row">
+                                    <div class="col">
+                                        <h6 class="text-left">
+                                            <span class="font-weight-bold" style="font-size: 120%">Parameters:</span>
+                                            {% if prov.Parameters is mapping %}
+                                                <br/>
+                                                {% for key, value in prov.Parameters|items %}
+                                                    {% if value is iterable and value is not string %}
+                                                        {{ key }}: <br />
+                                                        {% for sub in value %}
+                                                            &emsp; - {{ sub }}<br />
+                                                        {% endfor %}
+                                                    {% else %}
+                                                        {{ key }}: {{ value }}<br />
+                                                    {% endif %}
+                                                {% endfor %}
+                                            {% else %}
+                                                None
+                                            {% endif %}
+                                        </h6>
+                                    </div>
+                                </div>
+                                <div class="row">
+                                    <div class="col">
+                                        <h6 class="text-left">
+                                            <span class="font-weight-bold" style="font-size: 120%">Command:</span>
+                                            <br/>
+                                            {{ prov.Command }}
+                                        </h6>
+                                    </div>
+                                </div>
+                            </div>
+                        </div>
+                    </div>
+                </div>
+            </div>
+        {% endfor %}
+{% endfor %}
+
 <!-- Optional JavaScript -->
 <!-- jQuery first, then Popper.js, then Bootstrap JS -->
 <script src="https://code.jquery.com/jquery-3.3.1.min.js"
         integrity="sha384-tsQFqpEReu7ZLhBV2VZlAu7zcOV+rXbYlF2cqB8txI/8aZajjp4Bqd+V6D5IgvKT"
         crossorigin="anonymous"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js"
         integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1"
@@ -341,92 +393,53 @@
             }, 200); // 200ms animation duration
         }
     });
     // Update the button status on page load and when scrolling
     $(window).on('load scroll', updateButtonStatus);
 
     function sendPostRequest(btn) {
-        const btn_types = ['ignore', 'change-brain', 'change-cspine', 'change-tspine', 'change-lspine', 'change-orbits'];
         // Retrieve data from the custom data-* attributes of the button
         const api = btn.getAttribute('data-api');
         const loop_idx = btn.getAttribute('data-loop_index');
         const data = {
             project: btn.getAttribute('data-project'),
             subject: btn.getAttribute('data-subject'),
             session: btn.getAttribute('data-session'),
             source: btn.getAttribute('data-source_path'),
-            body_part: btn.getAttribute('data-body_part'),
-            original_name: btn.getAttribute('data-name')
         };
-        const api_str = (api === 'change') ? `${api}-${data['body_part']}` : api;
-
         // Define the URL to which the POST request will be sent
         const url = window.location.protocol + "//" + window.location.hostname + (window.location.port ? ':' + window.location.port : '') + `/qa/${api}-btn`;
 
         // Use the jQuery $.ajax() function to send the POST request
         $.ajax({
             url: url,
             type: 'POST',
             dataType: 'json',
             contentType: 'application/json',
             data: JSON.stringify(data),
             success: function (json) {
                 // Handle a successful response
-                btn_types.forEach(curstr => {
-                    let curr_btn = document.getElementById(`${curstr}${loop_idx}`);
-                    curr_btn.classList.remove("btn-success");
-                    curr_btn.classList.add("btn-dark");
-                });
-                const button = document.getElementById(`${api_str}${loop_idx}`);
+                const fail_btn = document.getElementById(`qa-fail${loop_idx}`);
+                fail_btn.classList.remove("btn-danger");
+                fail_btn.classList.add("btn-dark");
+
+                const pass_btn = document.getElementById(`qa-pass${loop_idx}`);
+                pass_btn.classList.remove("btn-success");
+                pass_btn.classList.add("btn-dark");
+
+                const button = document.getElementById(`${api}${loop_idx}`);
                 button.classList.remove("btn-dark");
-                button.classList.add("btn-success");
+                if (api === 'qa-pass') {
+                    button.classList.add("btn-success");
+                } else {
+                    button.classList.add("btn-danger");
+                }
             },
             error: function (xhr, status, error) {
                 // Handle any errors
                 console.error("Error:", error);
             }
         });
     }
-
-    $(function () {
-        $('#exampleModal').on('show.bs.modal', function (event) {
-            const button = $(event.relatedTarget) // Button that triggered the modal
-            const name = button.data('name') // Extract info from data-* attributes
-            const project = button.data('project')
-            const subject = button.data('subject')
-            const session = button.data('session')
-            const source_path = button.data('source_path')
-            const name_array = name.split('-')
-            // If necessary, you could initiate an AJAX request here (and then do the updating in a callback).
-            // Update the modal's content. We'll use jQuery here, but you could use a data binding library or other methods instead.
-            const modal = $(this)
-            modal.find('.modal-title').text('Correct Naming -- ' + subject + ' / ' + session)
-            modal.find('.modal-body #original-name').val(name)
-            modal.find('.modal-body #project-id').val(project)
-            modal.find('.modal-body #subject-id').val(subject)
-            modal.find('.modal-body #session-id').val(session)
-            modal.find('.modal-body #source-path').val(source_path)
-            modal.find('.modal-body #body-part').val(name_array[0])
-            modal.find('.modal-body #modality').val(name_array[1])
-            modal.find('.modal-body #technique').val(name_array[2])
-            modal.find('.modal-body #acq-dim').val(name_array[3])
-            modal.find('.modal-body #orient').val(name_array[4])
-            modal.find('.modal-body #ex-contrast').val(name_array[5])
-        });
-    });
-    $(function () {
-        $('#note-form-submit').click(function (e) {
-            e.preventDefault();
-            $.post(window.location.protocol + "//" + window.location.hostname + (window.location.port ? ':' + window.location.port : '') + `/qa/manual-entry`, $('#note-form').serialize())
-            $('#exampleModal').modal('hide');
-        });
-    });
-    $(function () {
-        $('#ignore-button-submit').click(function (e) {
-            e.preventDefault();
-            $.post(window.location.protocol + "//" + window.location.hostname + (window.location.port ? ':' + window.location.port : '') + `/qa/ignore-entry`, $('#note-form').serialize())
-            $('#exampleModal').modal('hide');
-        });
-    });
 </script>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,67 +1,74 @@
 _R_A_D_I_F_O_X_ _Q_A
     * _C_o_n_v_e_r_s_i_o_n
     * _P_r_o_c_e_s_s_i_n_g
 _{_{_ _p_r_o_j_e_c_t___i_d_ _|_ _u_p_p_e_r_(_)_ _}_} /  _{_{_ _s_u_b_j_e_c_t___i_d_ _}_} / {{ session_id }}
 
 
-{% for key, value in processing_results|items %}
+{% for key, value in processing_results|items %} {% set steploop = loop %}
 ********** {{{{ kkeeyy || uuppppeerr(()) || rreeppllaaccee((''::'',, '' vv'')) }}}} **********
 ===============================================================================
 ===============================================================================
 
-{% for id, prov in value|items %} {% for output_name, qa_dict in
-prov.OutputQA|items %}
+{% for id, prov in value|items %} {% set provloop = loop %} {% for output_name,
+qa_dict in prov.OutputQA|items %} {% set outloop = loop %}
 ****** {{{{ oouuttppuutt__nnaammee||rreeppllaaccee((''__'',,'' ''))||ttiittllee(()) }}}}:: ******
-{% for filestr, qa_img in qa_dict|items %}
-**** {{{{ ffiilleessttrr }}}} ****
+{% for filestr, qa_img in qa_dict|items %} {% set imgloop = loop %}
+**** {{{{ qqaa__iimmgg[[33]] }}}} ****
+}btn-success{% else %}btn-dark{% endif %}"> PASS  
+}btn-danger{% else %}btn-dark{% endif %}"> FAIL
 {% if qa_img %}
 [{{ qa_img[2] }}]
 {% endif %}
 
 {% endfor %}
 {% endfor %}
+PROVENANCE
+===============================================================================
+
+{% endfor %}
+
+{% endfor %}
+Next Image Prev Image {% if prev_session %} ←  _{_{_ _p_r_e_v___s_e_s_s_i_o_n_ _}_} {% elif
+prev_subject %} ←  _{_{_ _p_r_e_v___s_u_b_j_e_c_t_ _}_} {% endif %} {% if next_session %} _{
+_{_ _n_e_x_t___s_e_s_s_i_o_n_ _}_}  → {% elif next_subject %} _{_{_ _n_e_x_t___s_u_b_j_e_c_t_ _}_}  → {% endif %}
+[full size image]
+{% for key, value in processing_results|items %} {% set steploop = loop %} {%
+for id, prov in value|items %} {% set provloop = loop %}
 
-**** IIDD:: {{{{ pprroovv..IIdd }}}} ****
-**** CCoonnttaaiinneerr::
+** IIDD:: {{{{ pprroovv..IIdd }}}} **
+** CCoonnttaaiinneerr::
 {{{{ pprroovv..CCoonnttaaiinneerr..uurrll }}}}
 {{{{ pprroovv..CCoonnttaaiinneerr..hhaasshh }}}}
 BBuuiilltt:: {{{{ pprroovv..CCoonnttaaiinneerr..ttiimmeessttaammpp..ssttrrffttiimmee((''%%YY--%%mm--%%dd %%HH::%%MM::%%SS'')) }}}} bbyy {{
-{{ pprroovv..CCoonnttaaiinneerr..bbuuiillddeerr }}}} ****
-**** RRuunn IInnffoo::
+{{ pprroovv..CCoonnttaaiinneerr..bbuuiillddeerr }}}} **
+** RRuunn IInnffoo::
 SSttaarrtteedd:: {{{{ pprroovv..SSttaarrttTTiimmee }}}}
 DDuurraattiioonn:: {{{{ pprroovv..DDuurraattiioonn }}}}
-UUsseerr:: {{{{ pprroovv..UUsseerr }}}} ****
-**** IInnppuuttss::
+UUsseerr:: {{{{ pprroovv..UUsseerr }}}} **
+** IInnppuuttss::
 {{%% ffoorr kkeeyy,, vvaalluuee iinn pprroovv..IInnppuuttss||iitteemmss %%}} {{%% iiff vvaalluuee iiss iitteerraabbllee aanndd vvaalluuee iiss
 nnoott ssttrriinngg %%}} {{{{ kkeeyy }}}}::
 {{%% ffoorr ssuubb iinn vvaalluuee %%}} {{%% sseett vvaall == ssuubb..sspplliitt((''::'')) %%}} ?  -- {{{{ vvaall[[00]] }}}}
 ? ? [[{{{{ vvaall[[11]] }}}}::{{{{ vvaall[[22]] }}}}]]
-{{%% eennddffoorr %%}} {{%% eellssee %%}} {{%% sseett vvaall == vvaalluuee..sspplliitt((''::'')) %%}} {{{{ kkeeyy }}}}:: {{{{ vvaall[[00]]
-}}}}
+{{%% eennddffoorr %%}} {{%% eellssee %%}} {{%% sseett vvaall == vvaalluuee..sspplliitt((''::'')) %%}} {{{{ kkeeyy }}}}::
+?  -- {{{{ vvaall[[00]] }}}}
 ? ? [[{{{{ vvaall[[11]] }}}}::{{{{ vvaall[[22]] }}}}]]
-{{%% eennddiiff %%}} {{%% eennddffoorr %%}} ****
-**** OOuuttppuuttss::
+{{%% eennddiiff %%}} {{%% eennddffoorr %%}} **
+** OOuuttppuuttss::
 {{%% ffoorr kkeeyy,, vvaalluuee iinn pprroovv..OOuuttppuuttss||iitteemmss %%}} {{%% iiff vvaalluuee iiss iitteerraabbllee aanndd vvaalluuee iiss
 nnoott ssttrriinngg %%}} {{{{ kkeeyy }}}}::
 {{%% ffoorr ssuubb iinn vvaalluuee %%}} {{%% sseett vvaall == ssuubb..sspplliitt((''::'')) %%}} ?  -- {{{{ vvaall[[00]] }}}}
 ? ? [[{{{{ vvaall[[11]] }}}}::{{{{ vvaall[[22]] }}}}]]
-{{%% eennddffoorr %%}} {{%% eellssee %%}} {{%% sseett vvaall == vvaalluuee..sspplliitt((''::'')) %%}} {{{{ kkeeyy }}}}:: {{{{ vvaall[[00]]
-}}}}
+{{%% eennddffoorr %%}} {{%% eellssee %%}} {{%% sseett vvaall == vvaalluuee..sspplliitt((''::'')) %%}} {{{{ kkeeyy }}}}::
+?  -- {{{{ vvaall[[00]] }}}}
 ? ? [[{{{{ vvaall[[11]] }}}}::{{{{ vvaall[[22]] }}}}]]
-{{%% eennddiiff %%}} {{%% eennddffoorr %%}} ****
-**** PPaarraammeetteerrss:: {{%% iiff pprroovv..PPaarraammeetteerrss iiss mmaappppiinngg %%}}
+{{%% eennddiiff %%}} {{%% eennddffoorr %%}} **
+** PPaarraammeetteerrss:: {{%% iiff pprroovv..PPaarraammeetteerrss iiss mmaappppiinngg %%}}
 {{%% ffoorr kkeeyy,, vvaalluuee iinn pprroovv..PPaarraammeetteerrss||iitteemmss %%}} {{%% iiff vvaalluuee iiss iitteerraabbllee aanndd vvaalluuee
 iiss nnoott ssttrriinngg %%}} {{{{ kkeeyy }}}}::
 {{%% ffoorr ssuubb iinn vvaalluuee %%}} ?  -- {{{{ ssuubb }}}}
 {{%% eennddffoorr %%}} {{%% eellssee %%}} {{{{ kkeeyy }}}}:: {{{{ vvaalluuee }}}}
-{{%% eennddiiff %%}} {{%% eennddffoorr %%}} {{%% eellssee %%}} NNoonnee {{%% eennddiiff %%}} ****
-**** CCoommmmaanndd::
-{{{{ pprroovv..CCoommmmaanndd }}}} ****
-
-{% endfor %}
-
-{% endfor %}
-Next Image Prev Image {% if prev_session %} ←  _{_{_ _p_r_e_v___s_e_s_s_i_o_n_ _}_} {% elif
-prev_subject %} ←  _{_{_ _p_r_e_v___s_u_b_j_e_c_t_ _}_} {% endif %} {% if next_session %} _{
-_{_ _n_e_x_t___s_e_s_s_i_o_n_ _}_}  → {% elif next_subject %} _{_{_ _n_e_x_t___s_u_b_j_e_c_t_ _}_}  → {% endif %}
-[full size image]
+{{%% eennddiiff %%}} {{%% eennddffoorr %%}} {{%% eellssee %%}} NNoonnee {{%% eennddiiff %%}} **
+** CCoommmmaanndd::
+{{{{ pprroovv..CCoommmmaanndd }}}} **
+{% endfor %} {% endfor %}
```

### Comparing `radifox-1.0.9/radifox/qa/templates/project.html` & `radifox-1.1.0/radifox/qa/templates/project.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/qa/templates/subject.html` & `radifox-1.1.0/radifox/qa/templates/subject.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox/records/processing.py` & `radifox-1.1.0/radifox/records/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         try:
             logging.info(f"Beginning processing using: {self.name} v{self.version}.")
             logging.info(f"Command: {self.cli_call}")
             self.outputs = self.run(**self.parsed_args)
             if not self.check_outputs():
                 logging.error(f"Processing failed. No outputs reported.")
                 return
-            logging.info(f"Generating QA imagees.")
+            logging.info(f"Generating QA images.")
             self.generate_qa_images()
             logging.info(f"Generating provenance records.")
             self.generate_prov()
             logging.info(f"Processing complete.")
         except Exception as e:
             logging.error(f"An error occurred during processing: {e}.", exc_info=True)
             raise
```

### Comparing `radifox-1.0.9/radifox/records/utils.py` & `radifox-1.1.0/radifox/records/utils.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/radifox.egg-info/PKG-INFO` & `radifox-1.1.0/radifox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radifox
-Version: 1.0.9
+Version: 1.1.0
 Summary: RADIFOX is the RADiological Image File Ontology eXtension, a Python package for the organization and management of medical images.
 Home-page: https://github.com/jh-mipc/radifox
 Author: Blake Dewey
 Author-email: blake.dewey@jhu.edu
 License: Apache License, 2.0
 Keywords: mri conversion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `radifox-1.0.9/radifox.egg-info/SOURCES.txt` & `radifox-1.1.0/radifox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.0.9/setup.py` & `radifox-1.1.0/setup.py`

 * *Files identical despite different names*

