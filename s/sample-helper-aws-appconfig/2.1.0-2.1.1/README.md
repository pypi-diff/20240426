# Comparing `tmp/sample_helper_aws_appconfig-2.1.0.tar.gz` & `tmp/sample_helper_aws_appconfig-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sample_helper_aws_appconfig-2.1.0.tar", max compression
+gzip compressed data, was "sample_helper_aws_appconfig-2.1.1.tar", max compression
```

## Comparing `sample_helper_aws_appconfig-2.1.0.tar` & `sample_helper_aws_appconfig-2.1.1.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0    10142 2020-08-14 14:42:33.760774 sample_helper_aws_appconfig-2.1.0/LICENSE
--rw-r--r--   0        0        0     5016 2021-11-19 17:00:15.203523 sample_helper_aws_appconfig-2.1.0/README.md
--rw-r--r--   0        0        0       60 2020-10-16 11:36:42.609119 sample_helper_aws_appconfig-2.1.0/appconfig_helper/__init__.py
--rw-r--r--   0        0        0     7171 2023-11-03 13:24:58.138982 sample_helper_aws_appconfig-2.1.0/appconfig_helper/appconfig_helper.py
--rw-r--r--   0        0        0       18 2022-04-04 11:16:35.698496 sample_helper_aws_appconfig-2.1.0/appconfig_helper/version.py
--rw-r--r--   0        0        0     1206 2023-11-03 13:25:00.905333 sample_helper_aws_appconfig-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6193 1970-01-01 00:00:00.000000 sample_helper_aws_appconfig-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2020-08-14 14:42:33.760774 sample_helper_aws_appconfig-2.1.1/LICENSE
+-rw-r--r--   0        0        0       82 2022-07-28 13:45:04.134403 sample_helper_aws_appconfig-2.1.1/NOTICE
+-rw-r--r--   0        0        0     5016 2021-11-19 17:00:15.203523 sample_helper_aws_appconfig-2.1.1/README.md
+-rw-r--r--   0        0        0       60 2020-10-16 11:36:42.609119 sample_helper_aws_appconfig-2.1.1/appconfig_helper/__init__.py
+-rw-r--r--   0        0        0     7170 2024-04-26 10:34:44.868754 sample_helper_aws_appconfig-2.1.1/appconfig_helper/appconfig_helper.py
+-rw-r--r--   0        0        0        1 2024-04-26 10:30:54.879241 sample_helper_aws_appconfig-2.1.1/appconfig_helper/py.typed
+-rw-r--r--   0        0        0       18 2022-04-04 11:16:35.698496 sample_helper_aws_appconfig-2.1.1/appconfig_helper/version.py
+-rw-r--r--   0        0        0     1206 2024-04-26 10:47:08.628520 sample_helper_aws_appconfig-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6193 1970-01-01 00:00:00.000000 sample_helper_aws_appconfig-2.1.1/PKG-INFO
```

### Comparing `sample_helper_aws_appconfig-2.1.0/LICENSE` & `sample_helper_aws_appconfig-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sample_helper_aws_appconfig-2.1.0/README.md` & `sample_helper_aws_appconfig-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sample_helper_aws_appconfig-2.1.0/appconfig_helper/appconfig_helper.py` & `sample_helper_aws_appconfig-2.1.1/appconfig_helper/appconfig_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 AppConfig Helper class
 """
 
-
 import json
 import time
 from typing import Any, Dict, Optional, Union
 
 import boto3
 import botocore
```

### Comparing `sample_helper_aws_appconfig-2.1.0/pyproject.toml` & `sample_helper_aws_appconfig-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sample-helper-aws-appconfig"
-version = "2.1.0"
+version = "2.1.1"
 description = "Sample helper library for AWS AppConfig"
 authors = ["Amazon Web Services"]
 maintainers = ["James Seward <sewardjm@amazon.co.uk>"]
 license = "OSI Approved (Apache-2.0)"
 readme = "README.md"
 repository = "https://github.com/aws-samples/sample-python-helper-aws-appconfig"
 keywords = ["aws", "appconfig"]
```

### Comparing `sample_helper_aws_appconfig-2.1.0/PKG-INFO` & `sample_helper_aws_appconfig-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample-helper-aws-appconfig
-Version: 2.1.0
+Version: 2.1.1
 Summary: Sample helper library for AWS AppConfig
 Home-page: https://github.com/aws-samples/sample-python-helper-aws-appconfig
 License: OSI Approved (Apache-2.0)
 Keywords: aws,appconfig
 Author: Amazon Web Services
 Maintainer: James Seward
 Maintainer-email: sewardjm@amazon.co.uk
```

