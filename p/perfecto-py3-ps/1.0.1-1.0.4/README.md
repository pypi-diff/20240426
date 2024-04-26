# Comparing `tmp/perfecto-py3-ps-1.0.1.tar.gz` & `tmp/perfecto_py3_ps-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfecto-py3-ps-1.0.1.tar", last modified: Wed Jan 24 19:42:06 2024, max compression
+gzip compressed data, was "perfecto_py3_ps-1.0.4.tar", last modified: Fri Apr 26 16:44:25 2024, max compression
```

## Comparing `perfecto-py3-ps-1.0.1.tar` & `perfecto_py3_ps-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-01-24 19:42:06.942660 perfecto-py3-ps-1.0.1/
--rw-r--r--   0 jack       (501) staff       (20)      510 2024-01-24 19:42:06.942446 perfecto-py3-ps-1.0.1/PKG-INFO
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-01-24 19:42:06.938020 perfecto-py3-ps-1.0.1/perfecto/
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-01-24 19:42:06.939421 perfecto-py3-ps-1.0.1/perfecto/Exceptions/
--rw-r--r--   0 jack       (501) staff       (20)       45 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/Exceptions/ReportingException.py
--rw-r--r--   0 jack       (501) staff       (20)       52 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/Exceptions/__init__.py
--rw-r--r--   0 jack       (501) staff       (20)       62 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/__init__.py
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-01-24 19:42:06.940407 perfecto-py3-ps-1.0.1/perfecto/client/
--rw-r--r--   0 jack       (501) staff       (20)     1296 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/client/PerfectoDeprecator.py
--rw-r--r--   0 jack       (501) staff       (20)     5201 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/client/PerfectoReportiumClient.py
--rw-r--r--   0 jack       (501) staff       (20)      128 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/client/__init__.py
--rw-r--r--   0 jack       (501) staff       (20)      419 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/client/constants.py
--rw-r--r--   0 jack       (501) staff       (20)      549 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/client/license.txt
--rw-r--r--   0 jack       (501) staff       (20)      549 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/license.txt
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-01-24 19:42:06.940851 perfecto-py3-ps-1.0.1/perfecto/model/
--rw-r--r--   0 jack       (501) staff       (20)      828 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/model/PerfectoExecutionContext.py
--rw-r--r--   0 jack       (501) staff       (20)       84 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/model/__init__.py
--rw-r--r--   0 jack       (501) staff       (20)      399 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/model/model.py
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-01-24 19:42:06.941403 perfecto-py3-ps-1.0.1/perfecto/test/
--rw-r--r--   0 jack       (501) staff       (20)      254 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/test/TestContext.py
--rw-r--r--   0 jack       (501) staff       (20)     1029 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/test/TestResult.py
--rw-r--r--   0 jack       (501) staff       (20)      322 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/test/TestResultFactory.py
--rw-r--r--   0 jack       (501) staff       (20)       86 2024-01-24 17:46:20.000000 perfecto-py3-ps-1.0.1/perfecto/test/__init__.py
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-01-24 19:42:06.942064 perfecto-py3-ps-1.0.1/perfecto_py3_ps.egg-info/
--rw-r--r--   0 jack       (501) staff       (20)      510 2024-01-24 19:42:06.000000 perfecto-py3-ps-1.0.1/perfecto_py3_ps.egg-info/PKG-INFO
--rw-r--r--   0 jack       (501) staff       (20)      658 2024-01-24 19:42:06.000000 perfecto-py3-ps-1.0.1/perfecto_py3_ps.egg-info/SOURCES.txt
--rw-r--r--   0 jack       (501) staff       (20)        1 2024-01-24 19:42:06.000000 perfecto-py3-ps-1.0.1/perfecto_py3_ps.egg-info/dependency_links.txt
--rw-r--r--   0 jack       (501) staff       (20)       74 2024-01-24 19:42:06.000000 perfecto-py3-ps-1.0.1/perfecto_py3_ps.egg-info/top_level.txt
--rw-r--r--   0 jack       (501) staff       (20)       38 2024-01-24 19:42:06.942710 perfecto-py3-ps-1.0.1/setup.cfg
--rw-r--r--   0 jack       (501) staff       (20)     1025 2024-01-24 18:05:36.000000 perfecto-py3-ps-1.0.1/setup.py
+drwxr-xr-x   0 agrewal    (501) staff       (20)        0 2024-04-26 16:44:24.997194 perfecto_py3_ps-1.0.4/
+-rw-r--r--   0 agrewal    (501) staff       (20)      510 2024-04-26 16:44:24.995740 perfecto_py3_ps-1.0.4/PKG-INFO
+drwxr-xr-x   0 agrewal    (501) staff       (20)        0 2024-04-26 16:44:24.947205 perfecto_py3_ps-1.0.4/perfecto/
+drwxr-xr-x   0 agrewal    (501) staff       (20)        0 2024-04-26 16:44:24.950193 perfecto_py3_ps-1.0.4/perfecto/Exceptions/
+-rw-r--r--   0 agrewal    (501) staff       (20)       45 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/Exceptions/ReportingException.py
+-rw-r--r--   0 agrewal    (501) staff       (20)       52 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/Exceptions/__init__.py
+-rw-r--r--   0 agrewal    (501) staff       (20)       62 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/__init__.py
+drwxr-xr-x   0 agrewal    (501) staff       (20)        0 2024-04-26 16:44:24.960697 perfecto_py3_ps-1.0.4/perfecto/client/
+-rw-r--r--   0 agrewal    (501) staff       (20)     1296 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/client/PerfectoDeprecator.py
+-rw-r--r--   0 agrewal    (501) staff       (20)     6100 2024-02-08 18:14:06.000000 perfecto_py3_ps-1.0.4/perfecto/client/PerfectoReportiumClient.py
+-rw-r--r--   0 agrewal    (501) staff       (20)      128 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/client/__init__.py
+-rw-r--r--   0 agrewal    (501) staff       (20)      419 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/client/constants.py
+-rw-r--r--   0 agrewal    (501) staff       (20)      549 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/client/license.txt
+-rw-r--r--   0 agrewal    (501) staff       (20)      549 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/license.txt
+drwxr-xr-x   0 agrewal    (501) staff       (20)        0 2024-04-26 16:44:24.967122 perfecto_py3_ps-1.0.4/perfecto/model/
+-rw-r--r--   0 agrewal    (501) staff       (20)      828 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/model/PerfectoExecutionContext.py
+-rw-r--r--   0 agrewal    (501) staff       (20)       84 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/model/__init__.py
+-rw-r--r--   0 agrewal    (501) staff       (20)      399 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/model/model.py
+drwxr-xr-x   0 agrewal    (501) staff       (20)        0 2024-04-26 16:44:24.974287 perfecto_py3_ps-1.0.4/perfecto/test/
+-rw-r--r--   0 agrewal    (501) staff       (20)      254 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/test/TestContext.py
+-rw-r--r--   0 agrewal    (501) staff       (20)     1029 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/test/TestResult.py
+-rw-r--r--   0 agrewal    (501) staff       (20)      322 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/test/TestResultFactory.py
+-rw-r--r--   0 agrewal    (501) staff       (20)       86 2024-01-24 22:15:33.000000 perfecto_py3_ps-1.0.4/perfecto/test/__init__.py
+drwxr-xr-x   0 agrewal    (501) staff       (20)        0 2024-04-26 16:44:24.993892 perfecto_py3_ps-1.0.4/perfecto_py3_ps.egg-info/
+-rw-r--r--   0 agrewal    (501) staff       (20)      510 2024-04-26 16:44:24.000000 perfecto_py3_ps-1.0.4/perfecto_py3_ps.egg-info/PKG-INFO
+-rw-r--r--   0 agrewal    (501) staff       (20)      658 2024-04-26 16:44:24.000000 perfecto_py3_ps-1.0.4/perfecto_py3_ps.egg-info/SOURCES.txt
+-rw-r--r--   0 agrewal    (501) staff       (20)        1 2024-04-26 16:44:24.000000 perfecto_py3_ps-1.0.4/perfecto_py3_ps.egg-info/dependency_links.txt
+-rw-r--r--   0 agrewal    (501) staff       (20)       74 2024-04-26 16:44:24.000000 perfecto_py3_ps-1.0.4/perfecto_py3_ps.egg-info/top_level.txt
+-rw-r--r--   0 agrewal    (501) staff       (20)       38 2024-04-26 16:44:24.997389 perfecto_py3_ps-1.0.4/setup.cfg
+-rw-r--r--   0 agrewal    (501) staff       (20)     1025 2024-02-08 18:20:45.000000 perfecto_py3_ps-1.0.4/setup.py
```

### Comparing `perfecto-py3-ps-1.0.1/perfecto/client/PerfectoDeprecator.py` & `perfecto_py3_ps-1.0.4/perfecto/client/PerfectoDeprecator.py`

 * *Files identical despite different names*

### Comparing `perfecto-py3-ps-1.0.1/perfecto/client/PerfectoReportiumClient.py` & `perfecto_py3_ps-1.0.4/perfecto/client/PerfectoReportiumClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,42 @@
 from .constants import *
 from .PerfectoDeprecator import deprecated
-
+import json
 
 class PerfectoReportiumClient:
     """
     Perfecto Reporting client
     """
     def __init__(self, perfecto_execution_context):
         """
         initialize a new reporting client
         :param perfecto_execution_context:
         """
         self.perfecto_execution_context = perfecto_execution_context
         self.webdriver = perfecto_execution_context.webdriver
         self.started = False
+        if isinstance(self.webdriver, list):
+            driverCount = 0
+            externalIdAliases = []
+            for driver in self.webdriver:
+                driverCount = driverCount + 1
+                externalIDs = {
+                    'externalId':driver.desired_capabilities['executionId'],
+                    'alias':"perfectoRemote" + str(driverCount)
+                }
+                externalIdAliases.append(externalIDs)
+            finalData = json.dumps(externalIdAliases)
+            params = {}
+            params['externalIdAliases'] = finalData
+            self.started = True
+            try:
+                self.execute_script('mobile:execution:multiple',params)
+            except Exception as e: 
+                pass
+        
 
     def test_start(self, name, context):
         """
         inform reporting system about new test execution
         :param name: test name
         :param context: a context instance contains array of string tags
         :return: ---
@@ -155,8 +174,11 @@
     def execute_script(self, script, params):
         """
         Using WebDriver instance in order to execute command against reporting system
         :param script: string representation of the command to be executed
         :param params: commands parameters
         :return: command's return value
         """
-        return self.webdriver.execute_script(script, params)
+        if isinstance(self.webdriver, list):
+            return self.webdriver[0].execute_script(script, params)
+        else:
+            return self.webdriver.execute_script(script, params)
```

### Comparing `perfecto-py3-ps-1.0.1/perfecto/client/license.txt` & `perfecto_py3_ps-1.0.4/perfecto/client/license.txt`

 * *Files identical despite different names*

### Comparing `perfecto-py3-ps-1.0.1/perfecto/license.txt` & `perfecto_py3_ps-1.0.4/perfecto/license.txt`

 * *Files identical despite different names*

### Comparing `perfecto-py3-ps-1.0.1/perfecto/model/PerfectoExecutionContext.py` & `perfecto_py3_ps-1.0.4/perfecto/model/PerfectoExecutionContext.py`

 * *Files identical despite different names*

### Comparing `perfecto-py3-ps-1.0.1/perfecto/test/TestResult.py` & `perfecto_py3_ps-1.0.4/perfecto/test/TestResult.py`

 * *Files identical despite different names*

### Comparing `perfecto-py3-ps-1.0.1/perfecto_py3_ps.egg-info/SOURCES.txt` & `perfecto_py3_ps-1.0.4/perfecto_py3_ps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perfecto-py3-ps-1.0.1/setup.py` & `perfecto_py3_ps-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup
-release_version = '1.0.1'
+release_version = '1.0.4'
 
 setup(
     name='perfecto-py3-ps',
     packages=['perfecto','perfecto/client', 'perfecto/Exceptions', 'perfecto/model', 'perfecto/test'],  # this must be the same as the name above
     package_data = {'': ['*.txt']},
 	version=release_version,
     License='OSI Approved :: Apache Software License Classifier',
```

