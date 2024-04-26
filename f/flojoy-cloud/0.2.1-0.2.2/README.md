# Comparing `tmp/flojoy_cloud-0.2.1.tar.gz` & `tmp/flojoy_cloud-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flojoy_cloud-0.2.1.tar", max compression
+gzip compressed data, was "flojoy_cloud-0.2.2.tar", max compression
```

## Comparing `flojoy_cloud-0.2.1.tar` & `flojoy_cloud-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-05 02:02:50.649483 flojoy_cloud-0.2.1/README.md
--rw-r--r--   0        0        0      195 2024-04-15 21:23:40.492008 flojoy_cloud-0.2.1/flojoy_cloud/__init__.py
--rw-r--r--   0        0        0    13647 2024-04-15 21:22:34.164217 flojoy_cloud-0.2.1/flojoy_cloud/client.py
--rw-r--r--   0        0        0     2562 2024-04-15 21:24:25.884752 flojoy_cloud-0.2.1/flojoy_cloud/dtypes.py
--rw-r--r--   0        0        0      792 2024-04-15 21:23:26.057490 flojoy_cloud-0.2.1/flojoy_cloud/measurement.py
--rw-r--r--   0        0        0     5961 2024-04-15 21:24:19.797797 flojoy_cloud-0.2.1/flojoy_cloud/test_sequencer.py
--rw-r--r--   0        0        0     2636 2024-04-15 21:23:10.386427 flojoy_cloud-0.2.1/flojoy_cloud/watch.py
--rw-r--r--   0        0        0      607 2024-04-15 21:24:58.825582 flojoy_cloud-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 flojoy_cloud-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-05 02:02:50.649483 flojoy_cloud-0.2.2/README.md
+-rw-r--r--   0        0        0      195 2024-04-16 16:42:27.555366 flojoy_cloud-0.2.2/flojoy_cloud/__init__.py
+-rw-r--r--   0        0        0    13647 2024-04-16 16:42:27.555642 flojoy_cloud-0.2.2/flojoy_cloud/client.py
+-rw-r--r--   0        0        0     2562 2024-04-16 16:42:27.555937 flojoy_cloud-0.2.2/flojoy_cloud/dtypes.py
+-rw-r--r--   0        0        0      792 2024-04-16 16:42:27.556102 flojoy_cloud-0.2.2/flojoy_cloud/measurement.py
+-rw-r--r--   0        0        0     5980 2024-04-26 17:56:56.111837 flojoy_cloud-0.2.2/flojoy_cloud/test_sequencer.py
+-rw-r--r--   0        0        0     2636 2024-04-16 16:42:27.556480 flojoy_cloud-0.2.2/flojoy_cloud/watch.py
+-rw-r--r--   0        0        0      607 2024-04-26 17:59:02.050915 flojoy_cloud-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 flojoy_cloud-0.2.2/PKG-INFO
```

### Comparing `flojoy_cloud-0.2.1/flojoy_cloud/client.py` & `flojoy_cloud-0.2.2/flojoy_cloud/client.py`

 * *Files identical despite different names*

### Comparing `flojoy_cloud-0.2.1/flojoy_cloud/dtypes.py` & `flojoy_cloud-0.2.2/flojoy_cloud/dtypes.py`

 * *Files identical despite different names*

### Comparing `flojoy_cloud-0.2.1/flojoy_cloud/measurement.py` & `flojoy_cloud-0.2.2/flojoy_cloud/measurement.py`

 * *Files identical despite different names*

### Comparing `flojoy_cloud-0.2.1/flojoy_cloud/test_sequencer.py` & `flojoy_cloud-0.2.2/flojoy_cloud/test_sequencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     max: ExpectedMeasurementType | None = None
 
 
 # ------ Public ------
 
 __all__ = [
     "export",
+    "is_in_range",
     "_get_most_recent_data",
     "_set_output_loc",
 ]
 
 
 def export(data: MeasurementData):
     """Export data so it can be retrieved by the test sequencer"""
```

### Comparing `flojoy_cloud-0.2.1/flojoy_cloud/watch.py` & `flojoy_cloud-0.2.2/flojoy_cloud/watch.py`

 * *Files identical despite different names*

### Comparing `flojoy_cloud-0.2.1/pyproject.toml` & `flojoy_cloud-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flojoy-cloud"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Joey Yu <joey@flojoy.io>", "Jeff Zhang <jeff@flojoy.io>"]
 readme = "README.md"
 packages = [{ include = "flojoy_cloud" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `flojoy_cloud-0.2.1/PKG-INFO` & `flojoy_cloud-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flojoy-cloud
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Joey Yu
 Author-email: joey@flojoy.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

