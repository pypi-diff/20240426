# Comparing `tmp/cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0.tar.gz` & `tmp/cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0.tar", last modified: Tue Oct 31 11:48:52 2023, max compression
+gzip compressed data, was "cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1.tar", last modified: Fri Apr 26 15:33:14 2024, max compression
```

## Comparing `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0.tar` & `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 11:48:52.345500 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-31 11:48:33.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-31 11:48:33.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2023-10-31 11:48:52.341500 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2023-10-31 11:48:33.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-31 11:48:33.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 11:48:52.345500 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-10-31 11:48:33.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 11:48:52.341500 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 11:48:52.341500 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 11:48:52.341500 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel/cdk_rds_sanitized_snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)    21293 2023-10-31 11:48:33.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel/cdk_rds_sanitized_snapshots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 11:48:52.341500 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel/cdk_rds_sanitized_snapshots/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-10-31 11:48:33.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel/cdk_rds_sanitized_snapshots/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74512 2023-10-31 11:48:33.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel/cdk_rds_sanitized_snapshots/_jsii/cdk-rds-sanitized-snapshots@0.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 11:48:33.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel/cdk_rds_sanitized_snapshots/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 11:48:52.341500 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2023-10-31 11:48:52.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-10-31 11:48:52.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 11:48:52.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-31 11:48:52.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-31 11:48:52.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:33:14.920055 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-26 15:33:04.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 15:33:04.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-26 15:33:14.920055 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-26 15:33:04.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 15:33:04.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:33:14.920055 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-26 15:33:04.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:33:14.920055 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:33:14.920055 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:33:14.920055 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel/cdk_rds_sanitized_snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-04-26 15:33:04.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel/cdk_rds_sanitized_snapshots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:33:14.920055 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel/cdk_rds_sanitized_snapshots/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-26 15:33:04.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel/cdk_rds_sanitized_snapshots/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74630 2024-04-26 15:33:04.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel/cdk_rds_sanitized_snapshots/_jsii/cdk-rds-sanitized-snapshots@0.1.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:33:04.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel/cdk_rds_sanitized_snapshots/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:33:14.920055 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-26 15:33:14.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-26 15:33:14.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:33:14.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 15:33:14.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 15:33:14.000000 cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/top_level.txt
```

### Comparing `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/LICENSE` & `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/PKG-INFO` & `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: cloudsnorkel.cdk-rds-sanitized-snapshots
-Version: 0.1.0
+Version: 0.1.1
 Summary: CDK construct to periodically take snapshots of RDS databases, sanitize them, and share with selected accounts.
 Home-page: https://github.com/CloudSnorkel/cdk-rds-sanitized-snapshots.git
 Author: Amir Szekely<amir@cloudsnorkel.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/CloudSnorkel/cdk-rds-sanitized-snapshots.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CDK Construct for RDS Sanitized Snapshots
 
 [![NPM](https://img.shields.io/npm/v/@cloudsnorkel/cdk-rds-sanitized-snapshots?label=npm&logo=npm)](https://www.npmjs.com/package/@cloudsnorkel/cdk-rds-sanitized-snapshots)
 [![PyPI](https://img.shields.io/pypi/v/cloudsnorkel.cdk-rds-sanitized-snapshots?label=pypi&logo=pypi)](https://pypi.org/project/cloudsnorkel.cdk-rds-sanitized-snapshots)
```

### Comparing `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/README.md` & `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/setup.py` & `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudsnorkel.cdk-rds-sanitized-snapshots",
-    "version": "0.1.0",
+    "version": "0.1.1",
     "description": "CDK construct to periodically take snapshots of RDS databases, sanitize them, and share with selected accounts.",
     "license": "Apache-2.0",
     "url": "https://github.com/CloudSnorkel/cdk-rds-sanitized-snapshots.git",
     "long_description_content_type": "text/markdown",
     "author": "Amir Szekely<amir@cloudsnorkel.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,34 +22,33 @@
     },
     "packages": [
         "cloudsnorkel.cdk_rds_sanitized_snapshots",
         "cloudsnorkel.cdk_rds_sanitized_snapshots._jsii"
     ],
     "package_data": {
         "cloudsnorkel.cdk_rds_sanitized_snapshots._jsii": [
-            "cdk-rds-sanitized-snapshots@0.1.0.jsii.tgz"
+            "cdk-rds-sanitized-snapshots@0.1.1.jsii.tgz"
         ],
         "cloudsnorkel.cdk_rds_sanitized_snapshots": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.85.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.91.0, <2.0.0",
+        "jsii>=1.97.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved"
```

### Comparing `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel/cdk_rds_sanitized_snapshots/__init__.py` & `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel/cdk_rds_sanitized_snapshots/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,17 @@
 
 ## Testing
 
 ```
 npm run bundle && npm run integ:default:deploy
 ```
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/PKG-INFO` & `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: cloudsnorkel.cdk-rds-sanitized-snapshots
-Version: 0.1.0
+Version: 0.1.1
 Summary: CDK construct to periodically take snapshots of RDS databases, sanitize them, and share with selected accounts.
 Home-page: https://github.com/CloudSnorkel/cdk-rds-sanitized-snapshots.git
 Author: Amir Szekely<amir@cloudsnorkel.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/CloudSnorkel/cdk-rds-sanitized-snapshots.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CDK Construct for RDS Sanitized Snapshots
 
 [![NPM](https://img.shields.io/npm/v/@cloudsnorkel/cdk-rds-sanitized-snapshots?label=npm&logo=npm)](https://www.npmjs.com/package/@cloudsnorkel/cdk-rds-sanitized-snapshots)
 [![PyPI](https://img.shields.io/pypi/v/cloudsnorkel.cdk-rds-sanitized-snapshots?label=pypi&logo=pypi)](https://pypi.org/project/cloudsnorkel.cdk-rds-sanitized-snapshots)
```

### Comparing `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.0/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/SOURCES.txt` & `cloudsnorkel.cdk-rds-sanitized-snapshots-0.1.1/src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/SOURCES.txt
 src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/dependency_links.txt
 src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/requires.txt
 src/cloudsnorkel.cdk_rds_sanitized_snapshots.egg-info/top_level.txt
 src/cloudsnorkel/cdk_rds_sanitized_snapshots/__init__.py
 src/cloudsnorkel/cdk_rds_sanitized_snapshots/py.typed
 src/cloudsnorkel/cdk_rds_sanitized_snapshots/_jsii/__init__.py
-src/cloudsnorkel/cdk_rds_sanitized_snapshots/_jsii/cdk-rds-sanitized-snapshots@0.1.0.jsii.tgz
+src/cloudsnorkel/cdk_rds_sanitized_snapshots/_jsii/cdk-rds-sanitized-snapshots@0.1.1.jsii.tgz
```

