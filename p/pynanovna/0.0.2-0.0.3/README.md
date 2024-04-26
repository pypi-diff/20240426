# Comparing `tmp/pynanovna-0.0.2.tar.gz` & `tmp/pynanovna-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynanovna-0.0.2.tar", last modified: Fri Apr 26 13:25:02 2024, max compression
+gzip compressed data, was "pynanovna-0.0.3.tar", last modified: Fri Apr 26 13:44:35 2024, max compression
```

## Comparing `pynanovna-0.0.2.tar` & `pynanovna-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:25:02.652293 pynanovna-0.0.2/
--rw-r--r--   0 teo        (501) staff       (20)      895 2024-04-25 07:30:24.000000 pynanovna-0.0.2/LICENCE
--rw-r--r--   0 teo        (501) staff       (20)      887 2024-04-26 13:25:02.651157 pynanovna-0.0.2/PKG-INFO
--rw-r--r--   0 teo        (501) staff       (20)      350 2024-04-25 06:12:09.000000 pynanovna-0.0.2/README.md
--rw-r--r--   0 teo        (501) staff       (20)      518 2024-04-26 13:23:53.000000 pynanovna-0.0.2/pyproject.toml
--rw-r--r--   0 teo        (501) staff       (20)       38 2024-04-26 13:25:02.652500 pynanovna-0.0.2/setup.cfg
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:25:02.630632 pynanovna-0.0.2/src/
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:25:02.638203 pynanovna-0.0.2/src/pynanovna/
--rw-r--r--   0 teo        (501) staff       (20)    16118 2024-04-25 06:18:47.000000 pynanovna-0.0.2/src/pynanovna/Calibration.py
--rw-r--r--   0 teo        (501) staff       (20)     9117 2024-04-25 06:12:43.000000 pynanovna-0.0.2/src/pynanovna/CalibrationGuide.py
--rw-r--r--   0 teo        (501) staff       (20)     4526 2024-04-25 06:16:41.000000 pynanovna-0.0.2/src/pynanovna/RFTools.py
--rw-r--r--   0 teo        (501) staff       (20)     5697 2024-04-25 06:16:34.000000 pynanovna-0.0.2/src/pynanovna/SITools.py
--rw-r--r--   0 teo        (501) staff       (20)     4626 2024-04-25 06:12:36.000000 pynanovna-0.0.2/src/pynanovna/Sweep.py
--rw-r--r--   0 teo        (501) staff       (20)    11225 2024-04-25 06:16:23.000000 pynanovna-0.0.2/src/pynanovna/SweepWorker.py
--rw-r--r--   0 teo        (501) staff       (20)       80 2024-04-26 13:14:50.000000 pynanovna-0.0.2/src/pynanovna/__init__.py
--rw-r--r--   0 teo        (501) staff       (20)      239 2024-04-25 07:21:04.000000 pynanovna-0.0.2/src/pynanovna/example.py
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:25:02.649933 pynanovna-0.0.2/src/pynanovna/hardware/
--rw-r--r--   0 teo        (501) staff       (20)      579 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/AVNA.py
--rw-r--r--   0 teo        (501) staff       (20)     5641 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/Hardware.py
--rw-r--r--   0 teo        (501) staff       (20)      541 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/JNCRadio_VNA_3G.py
--rw-r--r--   0 teo        (501) staff       (20)     4118 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA.py
--rw-r--r--   0 teo        (501) staff       (20)      270 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_F.py
--rw-r--r--   0 teo        (501) staff       (20)      273 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_F_V2.py
--rw-r--r--   0 teo        (501) staff       (20)      225 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_H.py
--rw-r--r--   0 teo        (501) staff       (20)      453 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_H4.py
--rw-r--r--   0 teo        (501) staff       (20)     9852 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_V2.py
--rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/SV4401A.py
--rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/SV6301A.py
--rw-r--r--   0 teo        (501) staff       (20)      966 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/Serial.py
--rw-r--r--   0 teo        (501) staff       (20)     3369 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/TinySA.py
--rw-r--r--   0 teo        (501) staff       (20)     6482 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/VNA.py
--rw-r--r--   0 teo        (501) staff       (20)      743 2024-04-25 05:48:01.000000 pynanovna-0.0.2/src/pynanovna/hardware/Version.py
--rw-r--r--   0 teo        (501) staff       (20)     9503 2024-04-25 07:20:10.000000 pynanovna-0.0.2/src/pynanovna/pynanovna.py
--rw-r--r--   0 teo        (501) staff       (20)     5906 2024-04-25 11:38:52.000000 pynanovna-0.0.2/src/pynanovna/vis.py
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:25:02.650636 pynanovna-0.0.2/src/pynanovna.egg-info/
--rw-r--r--   0 teo        (501) staff       (20)      887 2024-04-26 13:25:02.000000 pynanovna-0.0.2/src/pynanovna.egg-info/PKG-INFO
--rw-r--r--   0 teo        (501) staff       (20)      969 2024-04-26 13:25:02.000000 pynanovna-0.0.2/src/pynanovna.egg-info/SOURCES.txt
--rw-r--r--   0 teo        (501) staff       (20)        1 2024-04-26 13:25:02.000000 pynanovna-0.0.2/src/pynanovna.egg-info/dependency_links.txt
--rw-r--r--   0 teo        (501) staff       (20)       10 2024-04-26 13:25:02.000000 pynanovna-0.0.2/src/pynanovna.egg-info/top_level.txt
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:44:35.143474 pynanovna-0.0.3/
+-rw-r--r--   0 teo        (501) staff       (20)      895 2024-04-25 07:30:24.000000 pynanovna-0.0.3/LICENCE
+-rw-r--r--   0 teo        (501) staff       (20)     1089 2024-04-26 13:44:35.142806 pynanovna-0.0.3/PKG-INFO
+-rw-r--r--   0 teo        (501) staff       (20)      432 2024-04-26 13:34:36.000000 pynanovna-0.0.3/README.md
+-rw-r--r--   0 teo        (501) staff       (20)      637 2024-04-26 13:44:26.000000 pynanovna-0.0.3/pyproject.toml
+-rw-r--r--   0 teo        (501) staff       (20)       38 2024-04-26 13:44:35.143581 pynanovna-0.0.3/setup.cfg
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:44:35.121101 pynanovna-0.0.3/src/
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:44:35.127595 pynanovna-0.0.3/src/pynanovna/
+-rw-r--r--   0 teo        (501) staff       (20)    16118 2024-04-25 06:18:47.000000 pynanovna-0.0.3/src/pynanovna/Calibration.py
+-rw-r--r--   0 teo        (501) staff       (20)     9117 2024-04-25 06:12:43.000000 pynanovna-0.0.3/src/pynanovna/CalibrationGuide.py
+-rw-r--r--   0 teo        (501) staff       (20)     4526 2024-04-25 06:16:41.000000 pynanovna-0.0.3/src/pynanovna/RFTools.py
+-rw-r--r--   0 teo        (501) staff       (20)     5697 2024-04-25 06:16:34.000000 pynanovna-0.0.3/src/pynanovna/SITools.py
+-rw-r--r--   0 teo        (501) staff       (20)     4626 2024-04-25 06:12:36.000000 pynanovna-0.0.3/src/pynanovna/Sweep.py
+-rw-r--r--   0 teo        (501) staff       (20)    11225 2024-04-25 06:16:23.000000 pynanovna-0.0.3/src/pynanovna/SweepWorker.py
+-rw-r--r--   0 teo        (501) staff       (20)       80 2024-04-26 13:14:50.000000 pynanovna-0.0.3/src/pynanovna/__init__.py
+-rw-r--r--   0 teo        (501) staff       (20)      239 2024-04-25 07:21:04.000000 pynanovna-0.0.3/src/pynanovna/example.py
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:44:35.141655 pynanovna-0.0.3/src/pynanovna/hardware/
+-rw-r--r--   0 teo        (501) staff       (20)      579 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/AVNA.py
+-rw-r--r--   0 teo        (501) staff       (20)     5641 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/Hardware.py
+-rw-r--r--   0 teo        (501) staff       (20)      541 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/JNCRadio_VNA_3G.py
+-rw-r--r--   0 teo        (501) staff       (20)     4118 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/NanoVNA.py
+-rw-r--r--   0 teo        (501) staff       (20)      270 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/NanoVNA_F.py
+-rw-r--r--   0 teo        (501) staff       (20)      273 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/NanoVNA_F_V2.py
+-rw-r--r--   0 teo        (501) staff       (20)      225 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/NanoVNA_H.py
+-rw-r--r--   0 teo        (501) staff       (20)      453 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/NanoVNA_H4.py
+-rw-r--r--   0 teo        (501) staff       (20)     9852 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/NanoVNA_V2.py
+-rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/SV4401A.py
+-rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/SV6301A.py
+-rw-r--r--   0 teo        (501) staff       (20)      966 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/Serial.py
+-rw-r--r--   0 teo        (501) staff       (20)     3369 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/TinySA.py
+-rw-r--r--   0 teo        (501) staff       (20)     6482 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/VNA.py
+-rw-r--r--   0 teo        (501) staff       (20)      743 2024-04-25 05:48:01.000000 pynanovna-0.0.3/src/pynanovna/hardware/Version.py
+-rw-r--r--   0 teo        (501) staff       (20)     9503 2024-04-25 07:20:10.000000 pynanovna-0.0.3/src/pynanovna/pynanovna.py
+-rw-r--r--   0 teo        (501) staff       (20)     5906 2024-04-25 11:38:52.000000 pynanovna-0.0.3/src/pynanovna/vis.py
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 13:44:35.142119 pynanovna-0.0.3/src/pynanovna.egg-info/
+-rw-r--r--   0 teo        (501) staff       (20)     1089 2024-04-26 13:44:35.000000 pynanovna-0.0.3/src/pynanovna.egg-info/PKG-INFO
+-rw-r--r--   0 teo        (501) staff       (20)     1005 2024-04-26 13:44:35.000000 pynanovna-0.0.3/src/pynanovna.egg-info/SOURCES.txt
+-rw-r--r--   0 teo        (501) staff       (20)        1 2024-04-26 13:44:35.000000 pynanovna-0.0.3/src/pynanovna.egg-info/dependency_links.txt
+-rw-r--r--   0 teo        (501) staff       (20)       60 2024-04-26 13:44:35.000000 pynanovna-0.0.3/src/pynanovna.egg-info/requires.txt
+-rw-r--r--   0 teo        (501) staff       (20)       10 2024-04-26 13:44:35.000000 pynanovna-0.0.3/src/pynanovna.egg-info/top_level.txt
```

### Comparing `pynanovna-0.0.2/LICENCE` & `pynanovna-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/pyproject.toml` & `pynanovna-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 [project]
 name = "pynanovna"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
-  { name="Teo Bergkvist", email="bergkvist.teo@protonmail.com" },
+  { name = "Teo Bergkvist", email = "bergkvist.teo@protonmail.com" },
 ]
 description = "A package to use a NanoVNA"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
+dependencies = [
+    "matplotlib >= 3.6.2",
+    "numpy >= 1.26.4",
+    "pyserial >= 3.5",
+    "scipy >= 1.13.0"
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/PICC-Group/pynanovna"
-Issues = "https://github.com/PICC-Group/pynanovna/issues"
+Issues = "https://github.com/PICC-Group/pynanovna/issues"
```

### Comparing `pynanovna-0.0.2/src/pynanovna/Calibration.py` & `pynanovna-0.0.3/src/pynanovna/Calibration.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/CalibrationGuide.py` & `pynanovna-0.0.3/src/pynanovna/CalibrationGuide.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/RFTools.py` & `pynanovna-0.0.3/src/pynanovna/RFTools.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/SITools.py` & `pynanovna-0.0.3/src/pynanovna/SITools.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/Sweep.py` & `pynanovna-0.0.3/src/pynanovna/Sweep.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/SweepWorker.py` & `pynanovna-0.0.3/src/pynanovna/SweepWorker.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/hardware/AVNA.py` & `pynanovna-0.0.3/src/pynanovna/hardware/AVNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/hardware/Hardware.py` & `pynanovna-0.0.3/src/pynanovna/hardware/Hardware.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/hardware/JNCRadio_VNA_3G.py` & `pynanovna-0.0.3/src/pynanovna/hardware/JNCRadio_VNA_3G.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA.py` & `pynanovna-0.0.3/src/pynanovna/hardware/NanoVNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/hardware/NanoVNA_V2.py` & `pynanovna-0.0.3/src/pynanovna/hardware/NanoVNA_V2.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/hardware/SV4401A.py` & `pynanovna-0.0.3/src/pynanovna/hardware/SV4401A.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/hardware/SV6301A.py` & `pynanovna-0.0.3/src/pynanovna/hardware/SV6301A.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/hardware/Serial.py` & `pynanovna-0.0.3/src/pynanovna/hardware/Serial.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/hardware/TinySA.py` & `pynanovna-0.0.3/src/pynanovna/hardware/TinySA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/hardware/VNA.py` & `pynanovna-0.0.3/src/pynanovna/hardware/VNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/hardware/Version.py` & `pynanovna-0.0.3/src/pynanovna/hardware/Version.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/pynanovna.py` & `pynanovna-0.0.3/src/pynanovna/pynanovna.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna/vis.py` & `pynanovna-0.0.3/src/pynanovna/vis.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.2/src/pynanovna.egg-info/SOURCES.txt` & `pynanovna-0.0.3/src/pynanovna.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/pynanovna/__init__.py
 src/pynanovna/example.py
 src/pynanovna/pynanovna.py
 src/pynanovna/vis.py
 src/pynanovna.egg-info/PKG-INFO
 src/pynanovna.egg-info/SOURCES.txt
 src/pynanovna.egg-info/dependency_links.txt
+src/pynanovna.egg-info/requires.txt
 src/pynanovna.egg-info/top_level.txt
 src/pynanovna/hardware/AVNA.py
 src/pynanovna/hardware/Hardware.py
 src/pynanovna/hardware/JNCRadio_VNA_3G.py
 src/pynanovna/hardware/NanoVNA.py
 src/pynanovna/hardware/NanoVNA_F.py
 src/pynanovna/hardware/NanoVNA_F_V2.py
```

