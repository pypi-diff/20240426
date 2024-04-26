# Comparing `tmp/pynanovna-0.0.1.tar.gz` & `tmp/pynanovna-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynanovna-0.0.1.tar", last modified: Thu Apr 25 08:06:12 2024, max compression
+gzip compressed data, was "pynanovna-0.0.2.tar", last modified: Fri Apr 26 13:25:02 2024, max compression
```

## Comparing `pynanovna-0.0.1.tar` & `pynanovna-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-25 08:06:12.389672 pynanovna-0.0.1/
--rw-r--r--   0 teo        (501) staff       (20)      895 2024-04-25 07:30:24.000000 pynanovna-0.0.1/LICENCE
--rw-r--r--   0 teo        (501) staff       (20)      887 2024-04-25 08:06:12.389016 pynanovna-0.0.1/PKG-INFO
--rw-r--r--   0 teo        (501) staff       (20)      350 2024-04-25 06:12:09.000000 pynanovna-0.0.1/README.md
--rw-r--r--   0 teo        (501) staff       (20)      518 2024-04-25 08:06:04.000000 pynanovna-0.0.1/pyproject.toml
--rw-r--r--   0 teo        (501) staff       (20)       38 2024-04-25 08:06:12.389773 pynanovna-0.0.1/setup.cfg
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-25 08:06:12.366331 pynanovna-0.0.1/src/
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-25 08:06:12.374617 pynanovna-0.0.1/src/pynanovna/
--rw-r--r--   0 teo        (501) staff       (20)    16118 2024-04-25 06:18:47.000000 pynanovna-0.0.1/src/pynanovna/Calibration.py
--rw-r--r--   0 teo        (501) staff       (20)     9117 2024-04-25 06:12:43.000000 pynanovna-0.0.1/src/pynanovna/CalibrationGuide.py
--rw-r--r--   0 teo        (501) staff       (20)     4526 2024-04-25 06:16:41.000000 pynanovna-0.0.1/src/pynanovna/RFTools.py
--rw-r--r--   0 teo        (501) staff       (20)     5697 2024-04-25 06:16:34.000000 pynanovna-0.0.1/src/pynanovna/SITools.py
--rw-r--r--   0 teo        (501) staff       (20)     4626 2024-04-25 06:12:36.000000 pynanovna-0.0.1/src/pynanovna/Sweep.py
--rw-r--r--   0 teo        (501) staff       (20)    11225 2024-04-25 06:16:23.000000 pynanovna-0.0.1/src/pynanovna/SweepWorker.py
--rw-r--r--   0 teo        (501) staff       (20)       55 2024-04-25 07:54:12.000000 pynanovna-0.0.1/src/pynanovna/__init__.py
--rw-r--r--   0 teo        (501) staff       (20)      239 2024-04-25 07:21:04.000000 pynanovna-0.0.1/src/pynanovna/example.py
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-25 08:06:12.387644 pynanovna-0.0.1/src/pynanovna/hardware/
--rw-r--r--   0 teo        (501) staff       (20)      579 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/AVNA.py
--rw-r--r--   0 teo        (501) staff       (20)     5641 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/Hardware.py
--rw-r--r--   0 teo        (501) staff       (20)      541 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/JNCRadio_VNA_3G.py
--rw-r--r--   0 teo        (501) staff       (20)     4118 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/NanoVNA.py
--rw-r--r--   0 teo        (501) staff       (20)      270 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/NanoVNA_F.py
--rw-r--r--   0 teo        (501) staff       (20)      273 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/NanoVNA_F_V2.py
--rw-r--r--   0 teo        (501) staff       (20)      225 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/NanoVNA_H.py
--rw-r--r--   0 teo        (501) staff       (20)      453 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/NanoVNA_H4.py
--rw-r--r--   0 teo        (501) staff       (20)     9852 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/NanoVNA_V2.py
--rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/SV4401A.py
--rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/SV6301A.py
--rw-r--r--   0 teo        (501) staff       (20)      966 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/Serial.py
--rw-r--r--   0 teo        (501) staff       (20)     3369 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/TinySA.py
--rw-r--r--   0 teo        (501) staff       (20)     6482 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/VNA.py
--rw-r--r--   0 teo        (501) staff       (20)      743 2024-04-25 05:48:01.000000 pynanovna-0.0.1/src/pynanovna/hardware/Version.py
--rw-r--r--   0 teo        (501) staff       (20)     9503 2024-04-25 07:20:10.000000 pynanovna-0.0.1/src/pynanovna/pynanovna.py
--rw-r--r--   0 teo        (501) staff       (20)     2533 2024-04-25 06:35:23.000000 pynanovna-0.0.1/src/pynanovna/vis.py
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-25 08:06:12.388324 pynanovna-0.0.1/src/pynanovna.egg-info/
--rw-r--r--   0 teo        (501) staff       (20)      887 2024-04-25 08:06:12.000000 pynanovna-0.0.1/src/pynanovna.egg-info/PKG-INFO
--rw-r--r--   0 teo        (501) staff       (20)      969 2024-04-25 08:06:12.000000 pynanovna-0.0.1/src/pynanovna.egg-info/SOURCES.txt
--rw-r--r--   0 teo        (501) staff       (20)        1 2024-04-25 08:06:12.000000 pynanovna-0.0.1/src/pynanovna.egg-info/dependency_links.txt
--rw-r--r--   0 teo        (501) staff       (20)       10 2024-04-25 08:06:12.000000 pynanovna-0.0.1/src/pynanovna.egg-info/top_level.txt
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:25:02.652293 pynanovna-0.0.2/
+-rw-r--r--   0 teo        (501) staff       (20)      895 2024-04-25 07:30:24.000000 pynanovna-0.0.2/LICENCE
+-rw-r--r--   0 teo        (501) staff       (20)      887 2024-04-26 13:25:02.651157 pynanovna-0.0.2/PKG-INFO
+-rw-r--r--   0 teo        (501) staff       (20)      350 2024-04-25 06:12:09.000000 pynanovna-0.0.2/README.md
+-rw-r--r--   0 teo        (501) staff       (20)      518 2024-04-26 13:23:53.000000 pynanovna-0.0.2/pyproject.toml
+-rw-r--r--   0 teo        (501) staff       (20)       38 2024-04-26 13:25:02.652500 pynanovna-0.0.2/setup.cfg
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:25:02.630632 pynanovna-0.0.2/src/
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:25:02.638203 pynanovna-0.0.2/src/pynanovna/
+-rw-r--r--   0 teo        (501) staff       (20)    16118 2024-04-25 06:18:47.000000 pynanovna-0.0.2/src/pynanovna/Calibration.py
+-rw-r--r--   0 teo        (501) staff       (20)     9117 2024-04-25 06:12:43.000000 pynanovna-0.0.2/src/pynanovna/CalibrationGuide.py
+-rw-r--r--   0 teo        (501) staff       (20)     4526 2024-04-25 06:16:41.000000 pynanovna-0.0.2/src/pynanovna/RFTools.py
+-rw-r--r--   0 teo        (501) staff       (20)     5697 2024-04-25 06:16:34.000000 pynanovna-0.0.2/src/pynanovna/SITools.py
+-rw-r--r--   0 teo        (501) staff       (20)     4626 2024-04-25 06:12:36.000000 pynanovna-0.0.2/src/pynanovna/Sweep.py
+-rw-r--r--   0 teo        (501) staff       (20)    11225 2024-04-25 06:16:23.000000 pynanovna-0.0.2/src/pynanovna/SweepWorker.py
+-rw-r--r--   0 teo        (501) staff       (20)       80 2024-04-26 13:14:50.000000 pynanovna-0.0.2/src/pynanovna/__init__.py
+-rw-r--r--   0 teo        (501) staff       (20)      239 2024-04-25 07:21:04.000000 pynanovna-0.0.2/src/pynanovna/example.py
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:25:02.649933 pynanovna-0.0.2/src/pynanovna/hardware/
+-rw-r--r--   0 teo        (501) staff       (20)      579 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/AVNA.py
+-rw-r--r--   0 teo        (501) staff       (20)     5641 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/Hardware.py
+-rw-r--r--   0 teo        (501) staff       (20)      541 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/JNCRadio_VNA_3G.py
+-rw-r--r--   0 teo        (501) staff       (20)     4118 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA.py
+-rw-r--r--   0 teo        (501) staff       (20)      270 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_F.py
+-rw-r--r--   0 teo        (501) staff       (20)      273 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_F_V2.py
+-rw-r--r--   0 teo        (501) staff       (20)      225 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_H.py
+-rw-r--r--   0 teo        (501) staff       (20)      453 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_H4.py
+-rw-r--r--   0 teo        (501) staff       (20)     9852 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_V2.py
+-rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/SV4401A.py
+-rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/SV6301A.py
+-rw-r--r--   0 teo        (501) staff       (20)      966 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/Serial.py
+-rw-r--r--   0 teo        (501) staff       (20)     3369 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/TinySA.py
+-rw-r--r--   0 teo        (501) staff       (20)     6482 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/VNA.py
+-rw-r--r--   0 teo        (501) staff       (20)      743 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/Version.py
+-rw-r--r--   0 teo        (501) staff       (20)     9503 2024-04-25 07:20:10.000000 pynanovna-0.0.2/src/pynanovna/pynanovna.py
+-rw-r--r--   0 teo        (501) staff       (20)     5906 2024-04-25 11:38:52.000000 pynanovna-0.0.2/src/pynanovna/vis.py
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:25:02.650636 pynanovna-0.0.2/src/pynanovna.egg-info/
+-rw-r--r--   0 teo        (501) staff       (20)      887 2024-04-26 13:25:02.000000 pynanovna-0.0.2/src/pynanovna.egg-info/PKG-INFO
+-rw-r--r--   0 teo        (501) staff       (20)      969 2024-04-26 13:25:02.000000 pynanovna-0.0.2/src/pynanovna.egg-info/SOURCES.txt
+-rw-r--r--   0 teo        (501) staff       (20)        1 2024-04-26 13:25:02.000000 pynanovna-0.0.2/src/pynanovna.egg-info/dependency_links.txt
+-rw-r--r--   0 teo        (501) staff       (20)       10 2024-04-26 13:25:02.000000 pynanovna-0.0.2/src/pynanovna.egg-info/top_level.txt
```

### Comparing `pynanovna-0.0.1/LICENCE` & `pynanovna-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/PKG-INFO` & `pynanovna-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynanovna
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to use a NanoVNA
 Author-email: Teo Bergkvist <bergkvist.teo@protonmail.com>
 Project-URL: Homepage, https://github.com/PICC-Group/pynanovna
 Project-URL: Issues, https://github.com/PICC-Group/pynanovna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pynanovna-0.0.1/pyproject.toml` & `pynanovna-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pynanovna"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Teo Bergkvist", email="bergkvist.teo@protonmail.com" },
 ]
 description = "A package to use a NanoVNA"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pynanovna-0.0.1/src/pynanovna/Calibration.py` & `pynanovna-0.0.2/src/pynanovna/Calibration.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/CalibrationGuide.py` & `pynanovna-0.0.2/src/pynanovna/CalibrationGuide.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/RFTools.py` & `pynanovna-0.0.2/src/pynanovna/RFTools.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/SITools.py` & `pynanovna-0.0.2/src/pynanovna/SITools.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/Sweep.py` & `pynanovna-0.0.2/src/pynanovna/Sweep.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/SweepWorker.py` & `pynanovna-0.0.2/src/pynanovna/SweepWorker.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/hardware/AVNA.py` & `pynanovna-0.0.2/src/pynanovna/hardware/AVNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/hardware/Hardware.py` & `pynanovna-0.0.2/src/pynanovna/hardware/Hardware.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/hardware/JNCRadio_VNA_3G.py` & `pynanovna-0.0.2/src/pynanovna/hardware/JNCRadio_VNA_3G.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/hardware/NanoVNA.py` & `pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/hardware/NanoVNA_V2.py` & `pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_V2.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/hardware/SV4401A.py` & `pynanovna-0.0.2/src/pynanovna/hardware/SV4401A.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/hardware/SV6301A.py` & `pynanovna-0.0.2/src/pynanovna/hardware/SV6301A.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/hardware/Serial.py` & `pynanovna-0.0.2/src/pynanovna/hardware/Serial.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/hardware/TinySA.py` & `pynanovna-0.0.2/src/pynanovna/hardware/TinySA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/hardware/VNA.py` & `pynanovna-0.0.2/src/pynanovna/hardware/VNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/hardware/Version.py` & `pynanovna-0.0.2/src/pynanovna/hardware/Version.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna/pynanovna.py` & `pynanovna-0.0.2/src/pynanovna/pynanovna.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.1/src/pynanovna.egg-info/PKG-INFO` & `pynanovna-0.0.2/src/pynanovna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynanovna
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to use a NanoVNA
 Author-email: Teo Bergkvist <bergkvist.teo@protonmail.com>
 Project-URL: Homepage, https://github.com/PICC-Group/pynanovna
 Project-URL: Issues, https://github.com/PICC-Group/pynanovna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pynanovna-0.0.1/src/pynanovna.egg-info/SOURCES.txt` & `pynanovna-0.0.2/src/pynanovna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

