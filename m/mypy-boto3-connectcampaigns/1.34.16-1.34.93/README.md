# Comparing `tmp/mypy-boto3-connectcampaigns-1.34.16.tar.gz` & `tmp/mypy_boto3_connectcampaigns-1.34.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcampaigns-1.34.16.tar", last modified: Wed Jan 10 20:32:18 2024, max compression
+gzip compressed data, was "mypy_boto3_connectcampaigns-1.34.93.tar", last modified: Fri Apr 26 19:32:22 2024, max compression
```

## Comparing `mypy-boto3-connectcampaigns-1.34.16.tar` & `mypy_boto3_connectcampaigns-1.34.93.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 20:32:18.154543 mypy-boto3-connectcampaigns-1.34.16/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-10 20:31:52.000000 mypy-boto3-connectcampaigns-1.34.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-01-10 20:32:18.154543 mypy-boto3-connectcampaigns-1.34.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-01-10 20:31:52.000000 mypy-boto3-connectcampaigns-1.34.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 20:32:18.150543 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-10 20:31:52.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-10 20:31:52.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-10 20:31:52.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-01-10 20:31:52.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16763 2024-01-10 20:31:52.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-01-10 20:31:53.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-01-10 20:31:53.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-01-10 20:31:53.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-10 20:31:53.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 20:31:52.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-01-10 20:31:53.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-01-10 20:31:53.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-10 20:31:52.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 20:32:18.150543 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-01-10 20:32:18.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-10 20:32:18.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 20:32:18.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 20:32:18.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-10 20:32:18.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-10 20:32:18.000000 mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 20:32:18.154543 mypy-boto3-connectcampaigns-1.34.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-01-10 20:31:52.000000 mypy-boto3-connectcampaigns-1.34.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:22.539540 mypy_boto3_connectcampaigns-1.34.93/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-26 19:32:22.539540 mypy_boto3_connectcampaigns-1.34.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:22.539540 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16763 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-04-26 19:31:58.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-26 19:31:58.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-26 19:31:58.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:22.539540 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-26 19:32:22.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-26 19:32:22.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:22.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:22.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 19:32:22.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-26 19:32:22.000000 mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:32:22.539540 mypy_boto3_connectcampaigns-1.34.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-26 19:31:57.000000 mypy_boto3_connectcampaigns-1.34.93/setup.py
```

### Comparing `mypy-boto3-connectcampaigns-1.34.16/LICENSE` & `mypy_boto3_connectcampaigns-1.34.93/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.34.16/PKG-INFO` & `mypy_boto3_connectcampaigns-1.34.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcampaigns
-Version: 1.34.16
-Summary: Type annotations for boto3.ConnectCampaignService 1.34.16 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.93
+Summary: Type annotations for boto3.ConnectCampaignService 1.34.93 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.34.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connectcampaigns-1.34.16/README.md` & `mypy_boto3_connectcampaigns-1.34.93/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.34.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/__init__.py` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/__init__.pyi` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/client.py` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/client.pyi` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/literals.py` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -91,14 +92,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -116,14 +118,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -136,24 +139,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -214,15 +219,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -351,14 +355,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -396,19 +401,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/literals.pyi` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -91,14 +92,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -116,14 +118,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -136,24 +139,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -214,15 +219,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -351,14 +355,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -396,19 +401,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/paginator.py` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/paginator.pyi` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/type_defs.py` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         "dialingCapacity": NotRequired[float],
     },
 )
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "enableAnswerMachineDetection": bool,
+        "awaitAnswerMachinePrompt": NotRequired[bool],
     },
 )
 InstanceIdFilterTypeDef = TypedDict(
     "InstanceIdFilterTypeDef",
     {
         "value": str,
         "operator": Literal["Eq"],
@@ -123,18 +124,18 @@
         "connectInstanceId": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
```

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns/type_defs.pyi` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         "dialingCapacity": NotRequired[float],
     },
 )
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "enableAnswerMachineDetection": bool,
+        "awaitAnswerMachinePrompt": NotRequired[bool],
     },
 )
 InstanceIdFilterTypeDef = TypedDict(
     "InstanceIdFilterTypeDef",
     {
         "value": str,
         "operator": Literal["Eq"],
@@ -123,18 +124,18 @@
         "connectInstanceId": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
```

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns.egg-info/PKG-INFO` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcampaigns
-Version: 1.34.16
-Summary: Type annotations for boto3.ConnectCampaignService 1.34.16 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.93
+Summary: Type annotations for boto3.ConnectCampaignService 1.34.93 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.34.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connectcampaigns-1.34.16/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt` & `mypy_boto3_connectcampaigns-1.34.93/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.34.16/setup.py` & `mypy_boto3_connectcampaigns-1.34.93/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcampaigns",
-    version="1.34.16",
+    version="1.34.93",
     packages=["mypy_boto3_connectcampaigns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.ConnectCampaignService 1.34.16 service generated with"
-        " mypy-boto3-builder 7.23.1"
-    ),
+    description="Type annotations for boto3.ConnectCampaignService 1.34.93 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

