# Comparing `tmp/botocore-a-la-carte-signer-1.34.91.tar.gz` & `tmp/botocore-a-la-carte-signer-1.34.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-signer-1.34.91.tar", last modified: Thu Apr 25 01:03:55 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-signer-1.34.92.tar", last modified: Fri Apr 26 01:01:52 2024, max compression
```

## Comparing `botocore-a-la-carte-signer-1.34.91.tar` & `botocore-a-la-carte-signer-1.34.92.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:55.619679 botocore-a-la-carte-signer-1.34.91/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-25 01:03:55.000000 botocore-a-la-carte-signer-1.34.91/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-25 01:03:55.619679 botocore-a-la-carte-signer-1.34.91/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:55.619679 botocore-a-la-carte-signer-1.34.91/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:55.619679 botocore-a-la-carte-signer-1.34.91/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:55.619679 botocore-a-la-carte-signer-1.34.91/botocore/data/signer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:55.619679 botocore-a-la-carte-signer-1.34.91/botocore/data/signer/2017-08-25/
--rw-r--r--   0 runner    (1001) docker     (127)    13726 2024-04-25 01:03:19.000000 botocore-a-la-carte-signer-1.34.91/botocore/data/signer/2017-08-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 01:03:19.000000 botocore-a-la-carte-signer-1.34.91/botocore/data/signer/2017-08-25/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-25 01:03:19.000000 botocore-a-la-carte-signer-1.34.91/botocore/data/signer/2017-08-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    71240 2024-04-25 01:03:19.000000 botocore-a-la-carte-signer-1.34.91/botocore/data/signer/2017-08-25/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-25 01:03:19.000000 botocore-a-la-carte-signer-1.34.91/botocore/data/signer/2017-08-25/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:03:55.619679 botocore-a-la-carte-signer-1.34.91/botocore_a_la_carte_signer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-25 01:03:55.000000 botocore-a-la-carte-signer-1.34.91/botocore_a_la_carte_signer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-25 01:03:55.000000 botocore-a-la-carte-signer-1.34.91/botocore_a_la_carte_signer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:03:55.000000 botocore-a-la-carte-signer-1.34.91/botocore_a_la_carte_signer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 01:03:55.000000 botocore-a-la-carte-signer-1.34.91/botocore_a_la_carte_signer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:03:55.619679 botocore-a-la-carte-signer-1.34.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-25 01:03:55.000000 botocore-a-la-carte-signer-1.34.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:01:52.069072 botocore-a-la-carte-signer-1.34.92/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-26 01:01:51.000000 botocore-a-la-carte-signer-1.34.92/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-26 01:01:52.069072 botocore-a-la-carte-signer-1.34.92/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:01:52.065072 botocore-a-la-carte-signer-1.34.92/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:01:52.065072 botocore-a-la-carte-signer-1.34.92/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:01:52.065072 botocore-a-la-carte-signer-1.34.92/botocore/data/signer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:01:52.069072 botocore-a-la-carte-signer-1.34.92/botocore/data/signer/2017-08-25/
+-rw-r--r--   0 runner    (1001) docker     (127)    13726 2024-04-26 01:01:12.000000 botocore-a-la-carte-signer-1.34.92/botocore/data/signer/2017-08-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-26 01:01:12.000000 botocore-a-la-carte-signer-1.34.92/botocore/data/signer/2017-08-25/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-26 01:01:12.000000 botocore-a-la-carte-signer-1.34.92/botocore/data/signer/2017-08-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    71240 2024-04-26 01:01:12.000000 botocore-a-la-carte-signer-1.34.92/botocore/data/signer/2017-08-25/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-26 01:01:12.000000 botocore-a-la-carte-signer-1.34.92/botocore/data/signer/2017-08-25/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:01:52.069072 botocore-a-la-carte-signer-1.34.92/botocore_a_la_carte_signer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-26 01:01:52.000000 botocore-a-la-carte-signer-1.34.92/botocore_a_la_carte_signer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-26 01:01:52.000000 botocore-a-la-carte-signer-1.34.92/botocore_a_la_carte_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:01:52.000000 botocore-a-la-carte-signer-1.34.92/botocore_a_la_carte_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 01:01:52.000000 botocore-a-la-carte-signer-1.34.92/botocore_a_la_carte_signer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 01:01:52.069072 botocore-a-la-carte-signer-1.34.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-26 01:01:51.000000 botocore-a-la-carte-signer-1.34.92/setup.py
```

### Comparing `botocore-a-la-carte-signer-1.34.91/LICENSE.txt` & `botocore-a-la-carte-signer-1.34.92/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-signer-1.34.91/PKG-INFO` & `botocore-a-la-carte-signer-1.34.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-signer
-Version: 1.34.91
+Version: 1.34.92
 Summary: signer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-signer-1.34.91/botocore/data/signer/2017-08-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-signer-1.34.92/botocore/data/signer/2017-08-25/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-signer-1.34.91/botocore/data/signer/2017-08-25/paginators-1.json` & `botocore-a-la-carte-signer-1.34.92/botocore/data/signer/2017-08-25/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-signer-1.34.91/botocore/data/signer/2017-08-25/service-2.json` & `botocore-a-la-carte-signer-1.34.92/botocore/data/signer/2017-08-25/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-signer-1.34.91/botocore/data/signer/2017-08-25/waiters-2.json` & `botocore-a-la-carte-signer-1.34.92/botocore/data/signer/2017-08-25/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-signer-1.34.91/botocore_a_la_carte_signer.egg-info/PKG-INFO` & `botocore-a-la-carte-signer-1.34.92/botocore_a_la_carte_signer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-signer
-Version: 1.34.91
+Version: 1.34.92
 Summary: signer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-signer-1.34.91/setup.py` & `botocore-a-la-carte-signer-1.34.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-signer',
-    version="1.34.91",
+    version="1.34.92",
     description='signer data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/signer/*/*.json'],
```

