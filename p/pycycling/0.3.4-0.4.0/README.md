# Comparing `tmp/pycycling-0.3.4.tar.gz` & `tmp/pycycling-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycycling-0.3.4.tar", last modified: Sat Jan  6 11:04:58 2024, max compression
+gzip compressed data, was "pycycling-0.4.0.tar", last modified: Fri Apr 26 20:28:29 2024, max compression
```

## Comparing `pycycling-0.3.4.tar` & `pycycling-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 11:04:58.149412 pycycling-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-06 11:04:50.000000 pycycling-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-01-06 11:04:58.149412 pycycling-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-01-06 11:04:50.000000 pycycling-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 11:04:58.145412 pycycling-0.3.4/pycycling/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/battery_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/cycling_power_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/cycling_speed_cadence_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 11:04:58.149412 pycycling-0.3.4/pycycling/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   131072 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/data/sterzo-challenge-codes.dat
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/fitness_machine_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 11:04:58.149412 pycycling-0.3.4/pycycling/ftms_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/ftms_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/ftms_parsers/control_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/ftms_parsers/fitness_machine_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/ftms_parsers/fitness_machine_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/ftms_parsers/indoor_bike_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/ftms_parsers/training_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/heart_rate_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/rear_view_radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/sterzo.py
--rw-r--r--   0 runner    (1001) docker     (127)    20849 2024-01-06 11:04:50.000000 pycycling-0.3.4/pycycling/tacx_trainer_control.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 11:04:58.149412 pycycling-0.3.4/pycycling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-01-06 11:04:58.000000 pycycling-0.3.4/pycycling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-06 11:04:58.000000 pycycling-0.3.4/pycycling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 11:04:58.000000 pycycling-0.3.4/pycycling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-06 11:04:58.000000 pycycling-0.3.4/pycycling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-06 11:04:58.000000 pycycling-0.3.4/pycycling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 11:04:58.149412 pycycling-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-06 11:04:50.000000 pycycling-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 11:04:58.149412 pycycling-0.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 11:04:50.000000 pycycling-0.3.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-01-06 11:04:50.000000 pycycling-0.3.4/test/test_battery_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-01-06 11:04:50.000000 pycycling-0.3.4/test/test_cycling_power_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-01-06 11:04:50.000000 pycycling-0.3.4/test/test_cycling_speed_cadence_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-01-06 11:04:50.000000 pycycling-0.3.4/test/test_heart_rate_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-06 11:04:50.000000 pycycling-0.3.4/test/test_rear_view_radar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:28:29.435620 pycycling-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 20:28:25.000000 pycycling-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-26 20:28:29.431620 pycycling-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-26 20:28:25.000000 pycycling-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:28:29.427620 pycycling-0.4.0/pycycling/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/battery_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/cycling_power_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/cycling_speed_cadence_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:28:29.431620 pycycling-0.4.0/pycycling/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131072 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/data/sterzo-challenge-codes.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    16089 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/fitness_machine_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:28:29.431620 pycycling-0.4.0/pycycling/ftms_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/ftms_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/ftms_parsers/control_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/ftms_parsers/fitness_machine_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/ftms_parsers/fitness_machine_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/ftms_parsers/indoor_bike_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/ftms_parsers/training_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/heart_rate_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/rear_view_radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/rizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/sterzo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20849 2024-04-26 20:28:25.000000 pycycling-0.4.0/pycycling/tacx_trainer_control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:28:29.431620 pycycling-0.4.0/pycycling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-26 20:28:29.000000 pycycling-0.4.0/pycycling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-26 20:28:29.000000 pycycling-0.4.0/pycycling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:28:29.000000 pycycling-0.4.0/pycycling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 20:28:29.000000 pycycling-0.4.0/pycycling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 20:28:29.000000 pycycling-0.4.0/pycycling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:28:29.435620 pycycling-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-26 20:28:25.000000 pycycling-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:28:29.431620 pycycling-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:28:25.000000 pycycling-0.4.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-26 20:28:25.000000 pycycling-0.4.0/test/test_battery_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-26 20:28:25.000000 pycycling-0.4.0/test/test_cycling_power_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-26 20:28:25.000000 pycycling-0.4.0/test/test_cycling_speed_cadence_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-26 20:28:25.000000 pycycling-0.4.0/test/test_heart_rate_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-26 20:28:25.000000 pycycling-0.4.0/test/test_rear_view_radar.py
```

### Comparing `pycycling-0.3.4/LICENSE` & `pycycling-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/PKG-INFO` & `pycycling-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycycling
-Version: 0.3.4
+Version: 0.4.0
 Summary: A Python package for interacting with Bluetooth Low Energy (BLE) compatible bike trainers, power meters, radars and heart rate monitors
 Home-page: https://github.com/zacharyedwardbull/pycycling
 Author: Zachary Bull
 Author-email: zacharyedwardbull@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,32 +23,35 @@
 MacOS, and Linux. Please refer to the Bleak repository for more information about supported platforms.
 
 ## Disclaimer
 
 __I take no responsibility if the use of this package breaks your turbo trainer or stationary bike. Use at your own
 risk!__
 
-I have tested it with (tested protocols in brackets):
+The package has been tested with (tested protocols in brackets):
 
 - a Tacx NEO trainer (ANT+ FE-C over BLE, CPS, CSCS)
 - a Tacx NEO 2T trainer (ANT+ FE-C over BLE, CPS, CSCS)
 - an Elite Sterzo Smart steering plate (STERZO)
 - a pair of Garmin Vector 3 power meter pedals (CPS)
 - a Garmin RVR315 rear view radar (RDR)
 - a Magene S3+ Speed/Cadence sensor (CSCS)
-- a Elite Suito-T smart trainer (CPS, CSCS, FTMS)
+- an Elite Suito-T smart trainer (CPS, CSCS, FTMS)
+- an Elite Justo smart trainer (CPS, CSCS, FTMS)
+- an Elite Rizer grade simulator (RIZER)
 
 Please let me know if you have used it with another device, and I will add it to the list.
 
 ## Supported protocols
 
 * Battery Service (BAS)
 * Cycling Power Service (CPS)
 * Cycling Speed and Cadence Service (CSCS)
 * Elite Sterzo Steering Service (STERZO)
+* Elite Rizer Steering Service (RIZER)
 * FiTness Machine Service (FTMS)
 * Heart Rate Service (HRS)
 * Rear View Radar (RDR)
 * Tacx Trainer Control (ANT+ FE-C over BLE)
 
 ## Installation
```

### Comparing `pycycling-0.3.4/README.md` & `pycycling-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,32 +8,35 @@
 MacOS, and Linux. Please refer to the Bleak repository for more information about supported platforms.
 
 ## Disclaimer
 
 __I take no responsibility if the use of this package breaks your turbo trainer or stationary bike. Use at your own
 risk!__
 
-I have tested it with (tested protocols in brackets):
+The package has been tested with (tested protocols in brackets):
 
 - a Tacx NEO trainer (ANT+ FE-C over BLE, CPS, CSCS)
 - a Tacx NEO 2T trainer (ANT+ FE-C over BLE, CPS, CSCS)
 - an Elite Sterzo Smart steering plate (STERZO)
 - a pair of Garmin Vector 3 power meter pedals (CPS)
 - a Garmin RVR315 rear view radar (RDR)
 - a Magene S3+ Speed/Cadence sensor (CSCS)
-- a Elite Suito-T smart trainer (CPS, CSCS, FTMS)
+- an Elite Suito-T smart trainer (CPS, CSCS, FTMS)
+- an Elite Justo smart trainer (CPS, CSCS, FTMS)
+- an Elite Rizer grade simulator (RIZER)
 
 Please let me know if you have used it with another device, and I will add it to the list.
 
 ## Supported protocols
 
 * Battery Service (BAS)
 * Cycling Power Service (CPS)
 * Cycling Speed and Cadence Service (CSCS)
 * Elite Sterzo Steering Service (STERZO)
+* Elite Rizer Steering Service (RIZER)
 * FiTness Machine Service (FTMS)
 * Heart Rate Service (HRS)
 * Rear View Radar (RDR)
 * Tacx Trainer Control (ANT+ FE-C over BLE)
 
 ## Installation
```

### Comparing `pycycling-0.3.4/pycycling/__init__.py` & `pycycling-0.4.0/pycycling/__init__.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/pycycling/battery_service.py` & `pycycling-0.4.0/pycycling/battery_service.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/pycycling/cycling_power_service.py` & `pycycling-0.4.0/pycycling/cycling_power_service.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/pycycling/cycling_speed_cadence_service.py` & `pycycling-0.4.0/pycycling/cycling_speed_cadence_service.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/pycycling/data/sterzo-challenge-codes.dat` & `pycycling-0.4.0/pycycling/data/sterzo-challenge-codes.dat`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/pycycling/ftms_parsers/fitness_machine_status.py` & `pycycling-0.4.0/pycycling/ftms_parsers/fitness_machine_status.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/pycycling/ftms_parsers/indoor_bike_data.py` & `pycycling-0.4.0/pycycling/ftms_parsers/indoor_bike_data.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/pycycling/ftms_parsers/training_status.py` & `pycycling-0.4.0/pycycling/ftms_parsers/training_status.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/pycycling/heart_rate_service.py` & `pycycling-0.4.0/pycycling/heart_rate_service.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/pycycling/rear_view_radar.py` & `pycycling-0.4.0/pycycling/rear_view_radar.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/pycycling/sterzo.py` & `pycycling-0.4.0/pycycling/sterzo.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         await self._activate_steering_measurements()
 
     async def _activate_steering_measurements(self):
         # importlib.resources.path is deprecated since 3.11
         if sys.version_info >= (3, 11):
             challenge_file = importlib.resources.files(pycycling.data).joinpath('sterzo-challenge-codes.dat').open('rb')
         else:  # legacy support < 3.9
-            challenge_file = importlib.resources.open_binary(pycycling.data, 'sterzo-challenge-codes.dat')
+            challenge_file = importlib.resources.open_binary(pycycling.data, 'sterzo-challenge-codes.dat') # pylint: disable=deprecated-method
 
         with challenge_file:
             challenge_file.seek(self._latest_challenge * 2, 1)
             code_1 = int.from_bytes(challenge_file.read(1), 'little')
             code_2 = int.from_bytes(challenge_file.read(1), 'little')
 
         byte_array = bytearray([0x03, 0x11, code_1, code_2])
```

### Comparing `pycycling-0.3.4/pycycling/tacx_trainer_control.py` & `pycycling-0.4.0/pycycling/tacx_trainer_control.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/pycycling.egg-info/PKG-INFO` & `pycycling-0.4.0/pycycling.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycycling
-Version: 0.3.4
+Version: 0.4.0
 Summary: A Python package for interacting with Bluetooth Low Energy (BLE) compatible bike trainers, power meters, radars and heart rate monitors
 Home-page: https://github.com/zacharyedwardbull/pycycling
 Author: Zachary Bull
 Author-email: zacharyedwardbull@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,32 +23,35 @@
 MacOS, and Linux. Please refer to the Bleak repository for more information about supported platforms.
 
 ## Disclaimer
 
 __I take no responsibility if the use of this package breaks your turbo trainer or stationary bike. Use at your own
 risk!__
 
-I have tested it with (tested protocols in brackets):
+The package has been tested with (tested protocols in brackets):
 
 - a Tacx NEO trainer (ANT+ FE-C over BLE, CPS, CSCS)
 - a Tacx NEO 2T trainer (ANT+ FE-C over BLE, CPS, CSCS)
 - an Elite Sterzo Smart steering plate (STERZO)
 - a pair of Garmin Vector 3 power meter pedals (CPS)
 - a Garmin RVR315 rear view radar (RDR)
 - a Magene S3+ Speed/Cadence sensor (CSCS)
-- a Elite Suito-T smart trainer (CPS, CSCS, FTMS)
+- an Elite Suito-T smart trainer (CPS, CSCS, FTMS)
+- an Elite Justo smart trainer (CPS, CSCS, FTMS)
+- an Elite Rizer grade simulator (RIZER)
 
 Please let me know if you have used it with another device, and I will add it to the list.
 
 ## Supported protocols
 
 * Battery Service (BAS)
 * Cycling Power Service (CPS)
 * Cycling Speed and Cadence Service (CSCS)
 * Elite Sterzo Steering Service (STERZO)
+* Elite Rizer Steering Service (RIZER)
 * FiTness Machine Service (FTMS)
 * Heart Rate Service (HRS)
 * Rear View Radar (RDR)
 * Tacx Trainer Control (ANT+ FE-C over BLE)
 
 ## Installation
```

### Comparing `pycycling-0.3.4/pycycling.egg-info/SOURCES.txt` & `pycycling-0.4.0/pycycling.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pycycling/__init__.py
 pycycling/battery_service.py
 pycycling/cycling_power_service.py
 pycycling/cycling_speed_cadence_service.py
 pycycling/fitness_machine_service.py
 pycycling/heart_rate_service.py
 pycycling/rear_view_radar.py
+pycycling/rizer.py
 pycycling/sterzo.py
 pycycling/tacx_trainer_control.py
 pycycling.egg-info/PKG-INFO
 pycycling.egg-info/SOURCES.txt
 pycycling.egg-info/dependency_links.txt
 pycycling.egg-info/requires.txt
 pycycling.egg-info/top_level.txt
```

### Comparing `pycycling-0.3.4/setup.py` & `pycycling-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pycycling",
-    version="0.3.4",
+    version="0.4.0",
     author="Zachary Bull",
     author_email="zacharyedwardbull@gmail.com",
     description=(
         "A Python package for interacting with Bluetooth Low Energy (BLE) compatible bike trainers, power meters, "
         "radars and heart rate monitors"
     ),
     long_description=long_description,
```

### Comparing `pycycling-0.3.4/test/test_cycling_power_service.py` & `pycycling-0.4.0/test/test_cycling_power_service.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/test/test_cycling_speed_cadence_service.py` & `pycycling-0.4.0/test/test_cycling_speed_cadence_service.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/test/test_heart_rate_service.py` & `pycycling-0.4.0/test/test_heart_rate_service.py`

 * *Files identical despite different names*

### Comparing `pycycling-0.3.4/test/test_rear_view_radar.py` & `pycycling-0.4.0/test/test_rear_view_radar.py`

 * *Files identical despite different names*

