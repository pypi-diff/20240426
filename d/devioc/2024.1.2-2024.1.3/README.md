# Comparing `tmp/devioc-2024.1.2.tar.gz` & `tmp/devioc-2024.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devioc-2024.1.2.tar", last modified: Wed Apr 17 15:19:54 2024, max compression
+gzip compressed data, was "devioc-2024.1.3.tar", last modified: Thu Apr 25 22:04:09 2024, max compression
```

## Comparing `devioc-2024.1.2.tar` & `devioc-2024.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-17 15:19:54.131868 devioc-2024.1.2/
--rw-rw-r--   0 michel   (70005) michel   (70005)     1066 2020-05-10 23:36:10.000000 devioc-2024.1.2/LICENSE
--rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-04-17 15:19:54.131868 devioc-2024.1.2/PKG-INFO
--rw-rw-r--   0 michel   (70005) michel   (70005)      568 2020-05-11 01:30:54.000000 devioc-2024.1.2/README.md
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-17 15:19:54.130868 devioc-2024.1.2/bin/
--rwxrwxr-x   0 michel   (70005) michel   (70005)     9465 2022-02-17 18:35:37.000000 devioc-2024.1.2/bin/devioc-startproject
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-17 15:19:54.130868 devioc-2024.1.2/devioc/
--rw-rw-r--   0 michel   (70005) michel   (70005)        0 2020-05-10 23:36:10.000000 devioc-2024.1.2/devioc/__init__.py
--rw-rw-r--   0 michel   (70005) michel   (70005)     2819 2020-05-10 23:36:10.000000 devioc-2024.1.2/devioc/log.py
--rw-rw-r--   0 michel   (70005) michel   (70005)    16849 2024-04-17 15:18:22.000000 devioc-2024.1.2/devioc/models.py
--rw-r--r--   0 michel   (70005) michel   (70005)     1366 2020-05-10 23:50:35.000000 devioc-2024.1.2/devioc/version.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-17 15:19:54.130868 devioc-2024.1.2/devioc.egg-info/
--rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-04-17 15:19:54.000000 devioc-2024.1.2/devioc.egg-info/PKG-INFO
--rw-rw-r--   0 michel   (70005) michel   (70005)      301 2024-04-17 15:19:54.000000 devioc-2024.1.2/devioc.egg-info/SOURCES.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)        1 2024-04-17 15:19:54.000000 devioc-2024.1.2/devioc.egg-info/dependency_links.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)       82 2024-04-17 15:19:54.000000 devioc-2024.1.2/devioc.egg-info/requires.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)       12 2024-04-17 15:19:54.000000 devioc-2024.1.2/devioc.egg-info/top_level.txt
--rw-r--r--   0 michel   (70005) michel   (70005)       38 2024-04-17 15:19:54.131868 devioc-2024.1.2/setup.cfg
--rw-rw-r--   0 michel   (70005) michel   (70005)     1018 2022-02-17 18:35:37.000000 devioc-2024.1.2/setup.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-17 15:19:54.130868 devioc-2024.1.2/test/
--rw-rw-r--   0 michel   (70005) michel   (70005)        0 2022-02-17 18:35:37.000000 devioc-2024.1.2/test/__init__.py
--rw-rw-r--   0 michel   (70005) michel   (70005)     4462 2024-02-16 17:57:09.000000 devioc-2024.1.2/test/test_ioc.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-25 22:04:09.141713 devioc-2024.1.3/
+-rw-rw-r--   0 michel   (70005) michel   (70005)     1066 2020-05-10 23:36:10.000000 devioc-2024.1.3/LICENSE
+-rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-04-25 22:04:09.141713 devioc-2024.1.3/PKG-INFO
+-rw-rw-r--   0 michel   (70005) michel   (70005)      568 2020-05-11 01:30:54.000000 devioc-2024.1.3/README.md
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-25 22:04:09.140713 devioc-2024.1.3/bin/
+-rwxrwxr-x   0 michel   (70005) michel   (70005)     9465 2022-02-17 18:35:37.000000 devioc-2024.1.3/bin/devioc-startproject
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-25 22:04:09.140713 devioc-2024.1.3/devioc/
+-rw-rw-r--   0 michel   (70005) michel   (70005)        0 2020-05-10 23:36:10.000000 devioc-2024.1.3/devioc/__init__.py
+-rw-rw-r--   0 michel   (70005) michel   (70005)     2819 2020-05-10 23:36:10.000000 devioc-2024.1.3/devioc/log.py
+-rw-rw-r--   0 michel   (70005) michel   (70005)    17096 2024-04-25 22:00:35.000000 devioc-2024.1.3/devioc/models.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     1366 2020-05-10 23:50:35.000000 devioc-2024.1.3/devioc/version.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-25 22:04:09.141713 devioc-2024.1.3/devioc.egg-info/
+-rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-04-25 22:04:09.000000 devioc-2024.1.3/devioc.egg-info/PKG-INFO
+-rw-rw-r--   0 michel   (70005) michel   (70005)      301 2024-04-25 22:04:09.000000 devioc-2024.1.3/devioc.egg-info/SOURCES.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)        1 2024-04-25 22:04:09.000000 devioc-2024.1.3/devioc.egg-info/dependency_links.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)       82 2024-04-25 22:04:09.000000 devioc-2024.1.3/devioc.egg-info/requires.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)       12 2024-04-25 22:04:09.000000 devioc-2024.1.3/devioc.egg-info/top_level.txt
+-rw-r--r--   0 michel   (70005) michel   (70005)       38 2024-04-25 22:04:09.141713 devioc-2024.1.3/setup.cfg
+-rw-rw-r--   0 michel   (70005) michel   (70005)     1018 2022-02-17 18:35:37.000000 devioc-2024.1.3/setup.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-25 22:04:09.141713 devioc-2024.1.3/test/
+-rw-rw-r--   0 michel   (70005) michel   (70005)        0 2022-02-17 18:35:37.000000 devioc-2024.1.3/test/__init__.py
+-rw-rw-r--   0 michel   (70005) michel   (70005)     4462 2024-02-16 17:57:09.000000 devioc-2024.1.3/test/test_ioc.py
```

### Comparing `devioc-2024.1.2/LICENSE` & `devioc-2024.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.2/PKG-INFO` & `devioc-2024.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devioc
-Version: 2024.1.2
+Version: 2024.1.3
 Summary: Simple Python based EPICS Device IOC Support
 Home-page: https://github.com/michel4j/devioc
 Author: Michel Fodje
 Author-email: michel4j@gmail.com
 License: MIT
 Keywords: epics device ioc development
 Classifier: Intended Audience :: Developers
```

### Comparing `devioc-2024.1.2/README.md` & `devioc-2024.1.3/README.md`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.2/bin/devioc-startproject` & `devioc-2024.1.3/bin/devioc-startproject`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.2/devioc/log.py` & `devioc-2024.1.3/devioc/log.py`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.2/devioc/models.py` & `devioc-2024.1.3/devioc/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from __future__ import annotations
-
 import multiprocessing
 import os
 import platform
 import shutil
 import subprocess
 import sys
 import time
 from collections.abc import Iterable
 from enum import EnumMeta
 from pathlib import Path
-from typing import Tuple
+from typing import Tuple, Union
 
 import gepics
 
 from . import log
 
 ENUM_KEYS = [
     'ZR', 'ON', 'TW', 'TH', 'FR', 'FV', 'SX', 'SV',
@@ -83,14 +81,20 @@
         Delete a database record field
 
         :param key: field name
         """
         if key in self.instance_fields:
             del self.instance_fields[key]
 
+    def get(self, *args, **kwargs):
+        ...
+
+    def put(self, *args, **kwargs):
+        ...
+
 
 class Enum(Record):
     """
     Enum record type
 
     :param name: Record name (str)
     :keyword choices: list/tuple of strings corresponding to the choice names, values will be 0-index integers.
@@ -202,32 +206,34 @@
         )
         super(Toggle, self).__init__(name, **kwargs)
 
 
 class String(Record):
     """
     String record. Uses standard string record, or character array depending on length
-
-    :param name: Record name (str)
-    :keyword max_length:
-        maximum number of characters expected. Char Array records will be used for fields bigger than 40 characters, in
-        which case the NELM and FTVL field will be set.
-    :keyword default:  default value, empty string by default
-    :keyword *: Extra keyword arguments
     """
 
     record = 'stringout'
     fields = {
         'VAL': '{default}'
     }
 
-    def __init__(self, name, **kwargs):
+    def __init__(self, name, max_length: Union[int, str] = 20, default: str = " ", **kwargs):
+        """
+        :param name: Record name (str)
+        :param max_length:
+            maximum number of characters expected. Char Array records will be used for fields bigger than 40 characters, in
+            which case the NELM and FTVL field will be set.
+        :param default:  default value, empty string by default
+        :param *: Extra keyword arguments
+
+        """
         kwargs.update(
-            max_length=kwargs.get("max_length", 20),
-            default=kwargs.get("default", " ")
+            max_length=max_length,
+            default=default
         )
         super(String, self).__init__(name, **kwargs)
         if self.options['max_length'] > 40:
             self.options['record'] = 'waveform'
             self.add_field('NELM', self.options['max_length'])
             self.add_field('FTVL', 'CHAR')
             self.del_field('VAL')
@@ -253,17 +259,17 @@
         'VAL': '{default}',
         'EGU': '{units}',
     }
 
     def __init__(
             self,
             name,
-            max_val: int | str = 0.,
-            min_val: int | str = 0.,
-            default: int | str = 0.,
+            max_val: Union[int, str] = 0.,
+            min_val: Union[int, str] = 0.,
+            default: Union[int, str] = 0.,
             units: str = '',
             **kwargs
     ):
         kwargs.update(
             max_val=max_val,
             min_val=min_val,
             default=default,
@@ -295,18 +301,18 @@
         'EGU': '{units}',
         'VAL': '{default}'
     }
 
     def __init__(
             self,
             name,
-            max_val: float | str = 0.,
-            min_val: float | str = 0.,
-            default: float | str = 0.,
-            prec: int | str = 4,
+            max_val: Union[float, str] = 0.,
+            min_val: Union[float, str] = 0.,
+            default: Union[float, str] = 0.,
+            prec: Union[float, str] = 4,
             units: str = '',
             **kwargs
     ):
         kwargs.update(
             max_val=max_val,
             min_val=min_val,
             default=default,
@@ -334,16 +340,16 @@
         'SCAN': '{scan}',
         'PREC': '{prec}',
     }
 
     def __init__(
             self,
             name: str,
-            scan: int | str = 0,
-            prec: int | str = 0,
+            scan: Union[int,  str] = 0,
+            prec: Union[int,  str] = 0,
             calc: str = '',
             **kwargs
     ):
         kwargs.update(
             scan=scan,
             prec=prec,
             calc=calc
@@ -354,30 +360,32 @@
             if key.lower() in self.options:
                 self.add_field(key, self.options[key.lower()])
 
 
 class CalcOut(Calc):
     """
     CalcOutput Record
-
-    :param name: Record name
-    :keyword out: OUT Output specification
-    :keyword oopt: OOPT Output Execute field
-    :keyword dopt: DOPT Output Data field
-    :keyword *: Extra keyword arguments, supports Calc kwargs also.
     """
 
     record = 'calcout'
     fields = {
         'OOPT': '{oopt}',
         'DOPT': '{dopt}',
         'OUT': '{out}',
     }
 
-    def __init__(self, name, out: str = "", oopt: int | str = 0, dopt: int | str = 0, **kwargs):
+    def __init__(self, name, out: str = "", oopt: Union[int,  str] = 0, dopt: Union[int, str] = 0, **kwargs):
+        """
+        :param name: Record name
+        :param out: OUT Output specification
+        :param oopt: OOPT Output Execute field
+        :param dopt: DOPT Output Data field
+        :param *: Extra keyword arguments, supports Calc kwargs also.
+
+        """
         kwargs.update(out=out, oopt=oopt, dopt=dopt)
         super(CalcOut, self).__init__(name, **kwargs)
 
 
 class Array(Record):
     """
     Array Record.
@@ -389,15 +397,15 @@
     """
     record = 'waveform'
     fields = {
         'NELM': '{length}',
         'FTVL': '{type}',
     }
 
-    def __init__(self, name, type: str | type = int, length: int | str = 256, **kwargs):
+    def __init__(self, name, type: Union[str, type] = int, length: Union[int, str] = 256, **kwargs):
         kwargs.update(type=type, length=length)
         super(Array, self).__init__(name, **kwargs)
         element_type = self.options['type']
         self.options['type'] = {
             str: 'STRING',
             int: 'LONG',
             float: 'FLOAT',
```

### Comparing `devioc-2024.1.2/devioc/version.py` & `devioc-2024.1.3/devioc/version.py`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.2/devioc.egg-info/PKG-INFO` & `devioc-2024.1.3/devioc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devioc
-Version: 2024.1.2
+Version: 2024.1.3
 Summary: Simple Python based EPICS Device IOC Support
 Home-page: https://github.com/michel4j/devioc
 Author: Michel Fodje
 Author-email: michel4j@gmail.com
 License: MIT
 Keywords: epics device ioc development
 Classifier: Intended Audience :: Developers
```

### Comparing `devioc-2024.1.2/setup.py` & `devioc-2024.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.2/test/test_ioc.py` & `devioc-2024.1.3/test/test_ioc.py`

 * *Files identical despite different names*

