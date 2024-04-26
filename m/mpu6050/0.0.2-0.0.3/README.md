# Comparing `tmp/mpu6050-0.0.2.tar.gz` & `tmp/mpu6050-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpu6050-0.0.2.tar", last modified: Wed Apr 24 21:21:45 2024, max compression
+gzip compressed data, was "mpu6050-0.0.3.tar", last modified: Fri Apr 26 15:06:03 2024, max compression
```

## Comparing `mpu6050-0.0.2.tar` & `mpu6050-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 21:21:45.051225 mpu6050-0.0.2/
--rw-rw-rw-   0        0        0     1082 2024-03-27 20:06:00.000000 mpu6050-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     4582 2024-04-24 21:21:45.051225 mpu6050-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3839 2024-04-23 20:19:47.000000 mpu6050-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 21:21:45.019982 mpu6050-0.0.2/mpu6050/
--rw-rw-rw-   0        0        0    40489 2024-04-23 21:19:16.000000 mpu6050-0.0.2/mpu6050/MPU6050.py
--rw-rw-rw-   0        0        0    32538 2024-04-16 21:53:09.000000 mpu6050-0.0.2/mpu6050/MPUConstants.py
--rw-rw-rw-   0        0        0       22 2024-04-24 21:18:09.000000 mpu6050-0.0.2/mpu6050/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 21:21:45.051225 mpu6050-0.0.2/mpu6050.egg-info/
--rw-rw-rw-   0        0        0     4582 2024-04-24 21:21:44.000000 mpu6050-0.0.2/mpu6050.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-04-24 21:21:44.000000 mpu6050-0.0.2/mpu6050.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 21:21:44.000000 mpu6050-0.0.2/mpu6050.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-24 21:21:44.000000 mpu6050-0.0.2/mpu6050.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 21:21:44.000000 mpu6050-0.0.2/mpu6050.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 21:21:45.051225 mpu6050-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1299 2024-04-24 21:21:41.000000 mpu6050-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:06:03.268011 mpu6050-0.0.3/
+-rw-rw-rw-   0        0        0     1082 2024-03-27 20:06:00.000000 mpu6050-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2013 2024-04-26 15:06:03.268011 mpu6050-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1296 2024-04-26 15:01:36.000000 mpu6050-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 15:06:03.236769 mpu6050-0.0.3/mpu6050/
+-rw-rw-rw-   0        0        0    40497 2024-04-26 15:03:15.000000 mpu6050-0.0.3/mpu6050/MPU6050.py
+-rw-rw-rw-   0        0        0    32538 2024-04-25 07:33:56.000000 mpu6050-0.0.3/mpu6050/MPUConstants.py
+-rw-rw-rw-   0        0        0       67 2024-04-26 14:54:56.000000 mpu6050-0.0.3/mpu6050/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:06:03.268011 mpu6050-0.0.3/mpu6050.egg-info/
+-rw-rw-rw-   0        0        0     2013 2024-04-26 15:06:03.000000 mpu6050-0.0.3/mpu6050.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-26 15:06:03.000000 mpu6050-0.0.3/mpu6050.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 15:06:03.000000 mpu6050-0.0.3/mpu6050.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 15:06:03.000000 mpu6050-0.0.3/mpu6050.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 15:06:03.000000 mpu6050-0.0.3/mpu6050.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 15:06:03.268011 mpu6050-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1299 2024-04-26 15:05:09.000000 mpu6050-0.0.3/setup.py
```

### Comparing `mpu6050-0.0.2/LICENSE.txt` & `mpu6050-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpu6050-0.0.2/mpu6050/MPU6050.py` & `mpu6050-0.0.3/mpu6050/MPU6050.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 """
 
 import math
 import ctypes
 import time
 import smbus
 import csv
-from MPUConstants import MPUConstants as C
+from mpu6050.MPUConstants import MPUConstants as C
 from quat import Quaternion as Q
 from quat import XYZVector as V
 
 ### Extra Libraries (You need to install) ###
 from scipy.spatial.transform import Rotation as R
```

### Comparing `mpu6050-0.0.2/mpu6050/MPUConstants.py` & `mpu6050-0.0.3/mpu6050/MPUConstants.py`

 * *Files identical despite different names*

### Comparing `mpu6050-0.0.2/setup.py` & `mpu6050-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A Python Library for Efficient MPU6050 DMP Access.'
 LONG_DESCRIPTION = 'This library aims to simplify the use of digital motion processor (DMP) inside inertial motion unit (IMU), along with other motion data.'
 
 # Setting up
 setup(
     name="mpu6050",
     version=VERSION,
```

