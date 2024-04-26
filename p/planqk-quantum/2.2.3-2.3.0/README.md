# Comparing `tmp/planqk-quantum-2.2.3.tar.gz` & `tmp/planqk-quantum-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planqk-quantum-2.2.3.tar", last modified: Tue Apr 16 13:34:41 2024, max compression
+gzip compressed data, was "planqk-quantum-2.3.0.tar", last modified: Fri Apr 26 15:51:03 2024, max compression
```

## Comparing `planqk-quantum-2.2.3.tar` & `planqk-quantum-2.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:41.563366 planqk-quantum-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-16 13:34:41.563366 planqk-quantum-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:41.559366 planqk-quantum-2.2.3/planqk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:41.559366 planqk-quantum-2.2.3/planqk/dwave/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/dwave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/dwave/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:41.559366 planqk-quantum-2.2.3/planqk/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:41.559366 planqk-quantum-2.2.3/planqk/qiskit/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/client/backend_dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/client/dto_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/client/job_dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/planqk_runtime_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:41.559366 planqk-quantum-2.2.3/planqk/qiskit/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:41.559366 planqk-quantum-2.2.3/planqk/qiskit/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/aws/aws_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/aws_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:41.559366 planqk-quantum-2.2.3/planqk/qiskit/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/azure/azure_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/azure/ionq_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:41.559366 planqk-quantum-2.2.3/planqk/qiskit/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/ibm/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/ibm/ibm_provider_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/ibm/ibm_runtime_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:41.563366 planqk-quantum-2.2.3/planqk/qiskit/providers/qryd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/qryd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/qryd/pcp_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/qryd/pcz_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/qryd/qryd_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/providers/qryd/qryd_converter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/planqk/qiskit/runtime_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:34:41.563366 planqk-quantum-2.2.3/planqk_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-16 13:34:41.000000 planqk-quantum-2.2.3/planqk_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-16 13:34:41.000000 planqk-quantum-2.2.3/planqk_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:34:41.000000 planqk-quantum-2.2.3/planqk_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 13:34:41.000000 planqk-quantum-2.2.3/planqk_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 13:34:41.000000 planqk-quantum-2.2.3/planqk_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:34:41.563366 planqk-quantum-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-16 13:34:32.000000 planqk-quantum-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.949325 planqk-quantum-2.3.0/planqk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/dwave/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/dwave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/dwave/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/qiskit/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/client/backend_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/client/dto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/client/job_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/planqk_runtime_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/qiskit/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/qiskit/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/aws/aws_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/aws_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/qiskit/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/azure/azure_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/azure/ionq_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/ibm_provider_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/ibm_runtime_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/pcp_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/pcz_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/qryd_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/qryd_converter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/runtime_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/planqk_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-26 15:51:03.000000 planqk-quantum-2.3.0/planqk_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-26 15:51:03.000000 planqk-quantum-2.3.0/planqk_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:51:03.000000 planqk-quantum-2.3.0/planqk_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-26 15:51:03.000000 planqk-quantum-2.3.0/planqk_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 15:51:03.000000 planqk-quantum-2.3.0/planqk_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/setup.py
```

### Comparing `planqk-quantum-2.2.3/LICENSE` & `planqk-quantum-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/PKG-INFO` & `planqk-quantum-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 2.2.3
+Version: 2.3.0
 Summary: Python SDK for the PlanQK Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: Anaqor AG
 Author-email: info@anaqor.io
 License: apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `planqk-quantum-2.2.3/README.md` & `planqk-quantum-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/context.py` & `planqk-quantum-2.3.0/planqk/context.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/credentials.py` & `planqk-quantum-2.3.0/planqk/credentials.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/dwave/provider.py` & `planqk-quantum-2.3.0/planqk/dwave/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/exceptions.py` & `planqk-quantum-2.3.0/planqk/exceptions.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/backend.py` & `planqk-quantum-2.3.0/planqk/qiskit/backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/client/backend_dtos.py` & `planqk-quantum-2.3.0/planqk/qiskit/client/backend_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/client/client.py` & `planqk-quantum-2.3.0/planqk/qiskit/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,14 +112,19 @@
         if provider is not None:
             params["provider"] = provider.name
 
         response = cls.perform_request(requests.get, f"{base_url()}/jobs/{job_id}", params=params)
         return JobDto(**response)
 
     @classmethod
+    def get_jobs(cls) -> List[JobDto]:
+        response = cls.perform_request(requests.get, f"{base_url()}/jobs")
+        return [JobDto(**job_info) for job_info in response]
+
+    @classmethod
     def get_job_result(cls, job_id: str, provider: Optional[PROVIDER] = None) -> Dict[str, Any]:
         params = {}
         if provider is not None:
             params["provider"] = provider.name
 
         response = cls.perform_request(requests.get, f"{base_url()}/jobs/{job_id}/result", params=params)
         return response
```

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/client/job_dtos.py` & `planqk-quantum-2.3.0/planqk/qiskit/client/job_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/job.py` & `planqk-quantum-2.3.0/planqk/qiskit/job.py`

 * *Files 9% similar despite different names*

```diff
@@ -130,12 +130,19 @@
 
     def to_dict(self) -> dict:
         """
         Return a dictionary representation of the job.
         """
         return {key: value for key, value in vars(self).items() if not key.startswith('_')}
 
+    def backend(self) -> Backend:
+        """Return the backend where this job was executed."""
+        if self._backend is None:
+            from planqk.qiskit import PlanqkBackend
+            self._backend = PlanqkBackend(self._job_details.backend_id)
+        return self._backend
+
     def queue_position(self):
         """
         Return the position of the job in the server queue.
         """
         return None
```

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/options.py` & `planqk-quantum-2.3.0/planqk/qiskit/options.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/planqk_runtime_job.py` & `planqk-quantum-2.3.0/planqk/qiskit/planqk_runtime_job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/provider.py` & `planqk-quantum-2.3.0/planqk/qiskit/provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from typing import List
 
 from qiskit.providers import ProviderV1 as Provider, QiskitBackendNotFoundError
 
 from planqk.credentials import DefaultCredentialsProvider
 from planqk.exceptions import PlanqkClientError
 from planqk.qiskit import PlanqkJob
 from planqk.qiskit.backend import PlanqkBackend
@@ -120,7 +121,18 @@
             backend (PlanqkBackend): the backend that run the job.
             job_id (str): the job id.
 
         Returns:
             Job: the job from the backend with the given id.
         """
         return PlanqkJob(backend=backend, job_id=job_id)
+
+    def jobs(self) -> List[PlanqkJob]:
+        """
+        Returns all jobs of the user or organization.
+
+        Returns:
+            List[PlanqkJob]: a list of active jobs.
+        """
+        print("Getting your jobs from PlanQK, this may take a few seconds...")
+        job_dtos = _PlanqkClient.get_jobs()
+        return [PlanqkJob(backend=None, job_id=job_dto.id, job_details=job_dto) for job_dto in job_dtos]
```

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/providers/aws/aws_backend.py` & `planqk-quantum-2.3.0/planqk/qiskit/providers/aws/aws_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/providers/aws_converters.py` & `planqk-quantum-2.3.0/planqk/qiskit/providers/aws_converters.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/providers/azure/azure_backend.py` & `planqk-quantum-2.3.0/planqk/qiskit/providers/azure/azure_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/providers/ibm/ibm_backend.py` & `planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/ibm_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/providers/ibm/ibm_provider_backend.py` & `planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/ibm_provider_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/providers/qryd/pcp_gate.py` & `planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/pcp_gate.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/providers/qryd/pcz_gate.py` & `planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/pcz_gate.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/providers/qryd/qryd_backend.py` & `planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/qryd_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/providers/qryd/qryd_converter_utils.py` & `planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/qryd_converter_utils.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk/qiskit/runtime_provider.py` & `planqk-quantum-2.3.0/planqk/qiskit/runtime_provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/planqk_quantum.egg-info/PKG-INFO` & `planqk-quantum-2.3.0/planqk_quantum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 2.2.3
+Version: 2.3.0
 Summary: Python SDK for the PlanQK Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: Anaqor AG
 Author-email: info@anaqor.io
 License: apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `planqk-quantum-2.2.3/planqk_quantum.egg-info/SOURCES.txt` & `planqk-quantum-2.3.0/planqk_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.3/setup.py` & `planqk-quantum-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setup(
     name='planqk-quantum',
-    version="2.2.3",
+    version="2.3.0",
     author='Anaqor AG',
     author_email='info@anaqor.io',
     url='https://github.com/planqk/planqk-quantum',
     description='Python SDK for the PlanQK Platform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['planqk', 'planqk.*']),
```

