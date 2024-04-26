# Comparing `tmp/pwrdrvr.microapps.cdk-1.0.1.tar.gz` & `tmp/pwrdrvr.microapps.cdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwrdrvr.microapps.cdk-1.0.1.tar", last modified: Fri Apr 26 04:02:44 2024, max compression
+gzip compressed data, was "pwrdrvr.microapps.cdk-1.0.2.tar", last modified: Fri Apr 26 04:18:58 2024, max compression
```

## Comparing `pwrdrvr.microapps.cdk-1.0.1.tar` & `pwrdrvr.microapps.cdk-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.288272 pwrdrvr.microapps.cdk-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-04-26 04:02:44.288272 pwrdrvr.microapps.cdk-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17546 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 04:02:44.288272 pwrdrvr.microapps.cdk-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.280272 pwrdrvr.microapps.cdk-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.280272 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.280272 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.284272 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)   219448 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.284272 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2706396 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/_jsii/microapps-cdk@1.0.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.284272 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-04-26 04:02:44.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-26 04:02:44.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:02:44.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 04:02:44.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 04:02:44.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:18:58.418984 pwrdrvr.microapps.cdk-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-26 04:18:48.000000 pwrdrvr.microapps.cdk-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 04:18:48.000000 pwrdrvr.microapps.cdk-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-04-26 04:18:58.418984 pwrdrvr.microapps.cdk-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17546 2024-04-26 04:18:48.000000 pwrdrvr.microapps.cdk-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 04:18:48.000000 pwrdrvr.microapps.cdk-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 04:18:58.418984 pwrdrvr.microapps.cdk-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-26 04:18:48.000000 pwrdrvr.microapps.cdk-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:18:58.410984 pwrdrvr.microapps.cdk-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:18:58.410984 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:18:58.410984 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr/microapps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:18:58.414984 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr/microapps/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)   219448 2024-04-26 04:18:48.000000 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr/microapps/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:18:58.414984 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr/microapps/cdk/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-26 04:18:48.000000 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr/microapps/cdk/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2706396 2024-04-26 04:18:48.000000 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr/microapps/cdk/_jsii/microapps-cdk@1.0.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:18:48.000000 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr/microapps/cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:18:58.410984 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr.microapps.cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-04-26 04:18:58.000000 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-26 04:18:58.000000 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr.microapps.cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:18:58.000000 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr.microapps.cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 04:18:58.000000 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr.microapps.cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 04:18:58.000000 pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr.microapps.cdk.egg-info/top_level.txt
```

### Comparing `pwrdrvr.microapps.cdk-1.0.1/LICENSE` & `pwrdrvr.microapps.cdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pwrdrvr.microapps.cdk-1.0.1/PKG-INFO` & `pwrdrvr.microapps.cdk-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwrdrvr.microapps.cdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: MicroApps framework, by PwrDrvr LLC, delivered as an AWS CDK construct that provides the DynamoDB, Router service, Deploy service, API Gateway, and CloudFront distribution.
 Home-page: https://github.com/pwrdrvr/microapps-core
 Author: PwrDrvr LLC<harold@pwrdrvr.com>
 License: MIT
 Project-URL: Source, https://github.com/pwrdrvr/microapps-core
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pwrdrvr.microapps.cdk-1.0.1/README.md` & `pwrdrvr.microapps.cdk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pwrdrvr.microapps.cdk-1.0.1/setup.py` & `pwrdrvr.microapps.cdk-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pwrdrvr.microapps.cdk",
-    "version": "1.0.1",
+    "version": "1.0.2",
     "description": "MicroApps framework, by PwrDrvr LLC, delivered as an AWS CDK construct that provides the DynamoDB, Router service, Deploy service, API Gateway, and CloudFront distribution.",
     "license": "MIT",
     "url": "https://github.com/pwrdrvr/microapps-core",
     "long_description_content_type": "text/markdown",
     "author": "PwrDrvr LLC<harold@pwrdrvr.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "pwrdrvr.microapps.cdk",
         "pwrdrvr.microapps.cdk._jsii"
     ],
     "package_data": {
         "pwrdrvr.microapps.cdk._jsii": [
-            "microapps-cdk@1.0.1.jsii.tgz"
+            "microapps-cdk@1.0.2.jsii.tgz"
         ],
         "pwrdrvr.microapps.cdk": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/__init__.py` & `pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr/microapps/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO` & `pwrdrvr.microapps.cdk-1.0.2/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwrdrvr.microapps.cdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: MicroApps framework, by PwrDrvr LLC, delivered as an AWS CDK construct that provides the DynamoDB, Router service, Deploy service, API Gateway, and CloudFront distribution.
 Home-page: https://github.com/pwrdrvr/microapps-core
 Author: PwrDrvr LLC<harold@pwrdrvr.com>
 License: MIT
 Project-URL: Source, https://github.com/pwrdrvr/microapps-core
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

