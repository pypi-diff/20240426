# Comparing `tmp/silmused-0.0.8.tar.gz` & `tmp/silmused-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silmused-0.0.8.tar", last modified: Sun Jan  7 11:53:41 2024, max compression
+gzip compressed data, was "silmused-0.0.9.tar", last modified: Sun Jan  7 11:56:09 2024, max compression
```

## Comparing `silmused-0.0.8.tar` & `silmused-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:53:41.860445 silmused-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-01-07 11:53:25.000000 silmused-0.0.8/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-07 11:53:41.860445 silmused-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-07 11:53:25.000000 silmused-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 11:53:41.860445 silmused-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-07 11:53:25.000000 silmused-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:53:41.860445 silmused-0.0.8/silmused/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/ExecuteLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/Runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/TitleLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:53:41.860445 silmused-0.0.8/silmused/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/tests/ConstraintTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/tests/DataTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/tests/FunctionTest.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/tests/IndexTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/tests/ProcedureTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/tests/StructureTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/tests/TestDefinition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/tests/TriggerTest.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/tests/ViewTest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-07 11:53:25.000000 silmused-0.0.8/silmused/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:53:41.860445 silmused-0.0.8/silmused.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-07 11:53:41.000000 silmused-0.0.8/silmused.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-07 11:53:41.000000 silmused-0.0.8/silmused.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 11:53:41.000000 silmused-0.0.8/silmused.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-07 11:53:41.000000 silmused-0.0.8/silmused.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-07 11:53:41.000000 silmused-0.0.8/silmused.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:56:09.624387 silmused-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-01-07 11:55:54.000000 silmused-0.0.9/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-07 11:56:09.624387 silmused-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-07 11:55:54.000000 silmused-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 11:56:09.624387 silmused-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-07 11:55:54.000000 silmused-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:56:09.620387 silmused-0.0.9/silmused/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/ExecuteLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/Runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/TitleLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:56:09.624387 silmused-0.0.9/silmused/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/ConstraintTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/DataTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/FunctionTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/IndexTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/ProcedureTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/StructureTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/TestDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/TriggerTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/ViewTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-07 11:55:54.000000 silmused-0.0.9/silmused/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:56:09.620387 silmused-0.0.9/silmused.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-07 11:56:09.000000 silmused-0.0.9/silmused.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-07 11:56:09.000000 silmused-0.0.9/silmused.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 11:56:09.000000 silmused-0.0.9/silmused.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-07 11:56:09.000000 silmused-0.0.9/silmused.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-07 11:56:09.000000 silmused-0.0.9/silmused.egg-info/top_level.txt
```

### Comparing `silmused-0.0.8/LICENCE.txt` & `silmused-0.0.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused/ExecuteLayer.py` & `silmused-0.0.9/silmused/ExecuteLayer.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused/Runner.py` & `silmused-0.0.9/silmused/Runner.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused/__init__.py` & `silmused-0.0.9/silmused/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .tests.StructureTest import StructureTest
 from .tests.ConstraintTest import ConstraintTest
 from .tests.FunctionTest import FunctionTest
 from .tests.IndexTest import IndexTest
 from .tests.ProcedureTest import ProcedureTest
 from .tests.TriggerTest import TriggerTest
 from .tests.ViewTest import ViewTest
-import Runner
+import silmused.Runner
 
 __all__ = [
     'ExecuteLayer',
     'TitleLayer',
     'DataTest',
     'StructureTest',
     'ConstraintTest',
```

### Comparing `silmused-0.0.8/silmused/tests/ConstraintTest.py` & `silmused-0.0.9/silmused/tests/ConstraintTest.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused/tests/DataTest.py` & `silmused-0.0.9/silmused/tests/DataTest.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused/tests/FunctionTest.py` & `silmused-0.0.9/silmused/tests/FunctionTest.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused/tests/IndexTest.py` & `silmused-0.0.9/silmused/tests/IndexTest.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused/tests/ProcedureTest.py` & `silmused-0.0.9/silmused/tests/ProcedureTest.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused/tests/StructureTest.py` & `silmused-0.0.9/silmused/tests/StructureTest.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused/tests/TestDefinition.py` & `silmused-0.0.9/silmused/tests/TestDefinition.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused/tests/TriggerTest.py` & `silmused-0.0.9/silmused/tests/TriggerTest.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused/tests/ViewTest.py` & `silmused-0.0.9/silmused/tests/ViewTest.py`

 * *Files identical despite different names*

### Comparing `silmused-0.0.8/silmused.egg-info/SOURCES.txt` & `silmused-0.0.9/silmused.egg-info/SOURCES.txt`

 * *Files identical despite different names*

