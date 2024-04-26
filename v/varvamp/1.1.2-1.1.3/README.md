# Comparing `tmp/varvamp-1.1.2.tar.gz` & `tmp/varvamp-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvamp-1.1.2.tar", last modified: Tue Apr  2 12:29:03 2024, max compression
+gzip compressed data, was "varvamp-1.1.3.tar", last modified: Fri Apr 26 09:56:00 2024, max compression
```

## Comparing `varvamp-1.1.2.tar` & `varvamp-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:29:03.807459 varvamp-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-02 12:29:03.807459 varvamp-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-02 12:28:55.000000 varvamp-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:29:03.807459 varvamp-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-02 12:28:55.000000 varvamp-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:29:03.803459 varvamp-1.1.2/varvamp/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:29:03.807459 varvamp-1.1.2/varvamp/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/blast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/consensus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/default_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/param_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/primers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/qpcr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:29:03.807459 varvamp-1.1.2/varvamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:56:00.671611 varvamp-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-26 09:56:00.671611 varvamp-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-26 09:55:49.000000 varvamp-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:56:00.671611 varvamp-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-26 09:55:49.000000 varvamp-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:56:00.667611 varvamp-1.1.3/varvamp/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:56:00.671611 varvamp-1.1.3/varvamp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/blast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/param_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/primers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/qpcr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:56:00.671611 varvamp-1.1.3/varvamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/top_level.txt
```

### Comparing `varvamp-1.1.2/PKG-INFO` & `varvamp-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 1.1.2
+Version: 1.1.3
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-1.1.2/README.md` & `varvamp-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/setup.py` & `varvamp-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/command.py` & `varvamp-1.1.3/varvamp/command.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/scripts/alignment.py` & `varvamp-1.1.3/varvamp/scripts/alignment.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/scripts/blast.py` & `varvamp-1.1.3/varvamp/scripts/blast.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
     for off_target in results:
         if off_target is None:
             continue
         off_targets.append(off_target)
         if mode == "single_tiled":
             amplicons[off_target][5] = amplicons[off_target][5] + config.BLAST_PENALTY
         elif mode == "qpcr":
-            amplicons[off_target]["penalty"][0] = amplicons[off_target]["penalty"][0] + config.BLAST_PENALTY
+            amplicons[off_target]["penalty"] = amplicons[off_target]["penalty"] + config.BLAST_PENALTY
 
     return off_targets, amplicons
 
 
 def primer_blast(data_dir, db, query_path, amplicons, max_length, n_threads, log_file, mode):
     """
     performs the blast search for the single or tiled workflow
```

### Comparing `varvamp-1.1.2/varvamp/scripts/consensus.py` & `varvamp-1.1.3/varvamp/scripts/consensus.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/scripts/default_config.py` & `varvamp-1.1.3/varvamp/scripts/default_config.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/scripts/get_config.py` & `varvamp-1.1.3/varvamp/scripts/get_config.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/scripts/logging.py` & `varvamp-1.1.3/varvamp/scripts/logging.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/scripts/param_estimation.py` & `varvamp-1.1.3/varvamp/scripts/param_estimation.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/scripts/primers.py` & `varvamp-1.1.3/varvamp/scripts/primers.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/scripts/qpcr.py` & `varvamp-1.1.3/varvamp/scripts/qpcr.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/scripts/regions.py` & `varvamp-1.1.3/varvamp/scripts/regions.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/scripts/reporting.py` & `varvamp-1.1.3/varvamp/scripts/reporting.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp/scripts/scheme.py` & `varvamp-1.1.3/varvamp/scripts/scheme.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.2/varvamp.egg-info/PKG-INFO` & `varvamp-1.1.3/varvamp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 1.1.2
+Version: 1.1.3
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-1.1.2/varvamp.egg-info/SOURCES.txt` & `varvamp-1.1.3/varvamp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

