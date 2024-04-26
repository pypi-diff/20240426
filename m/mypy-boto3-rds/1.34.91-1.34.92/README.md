# Comparing `tmp/mypy_boto3_rds-1.34.91.tar.gz` & `tmp/mypy_boto3_rds-1.34.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_rds-1.34.91.tar", last modified: Thu Apr 25 01:11:55 2024, max compression
+gzip compressed data, was "mypy_boto3_rds-1.34.92.tar", last modified: Thu Apr 25 19:32:15 2024, max compression
```

## Comparing `mypy_boto3_rds-1.34.91.tar` & `mypy_boto3_rds-1.34.92.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 01:11:55.098525 mypy_boto3_rds-1.34.91/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    21964 2024-04-25 01:11:55.098525 mypy_boto3_rds-1.34.91/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20425 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 01:11:55.088525 mypy_boto3_rds-1.34.91/mypy_boto3_rds/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13119 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13119 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      903 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   164366 2024-04-25 01:11:11.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   164363 2024-04-25 01:11:08.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20349 2024-04-25 01:11:13.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20349 2024-04-25 01:11:13.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    51753 2024-04-25 01:11:12.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    51712 2024-04-25 01:11:11.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   207997 2024-04-25 01:11:22.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   207997 2024-04-25 01:11:19.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       62 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13511 2024-04-25 01:11:12.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13500 2024-04-25 01:11:12.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 01:11:55.098525 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    21964 2024-04-25 01:11:54.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      655 2024-04-25 01:11:55.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 01:11:54.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 01:11:54.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       53 2024-04-25 01:11:54.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       15 2024-04-25 01:11:54.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/top_level.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2024-04-25 01:11:55.098525 mypy_boto3_rds-1.34.91/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1946 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:15.723416 mypy_boto3_rds-1.34.92/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:31:54.000000 mypy_boto3_rds-1.34.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-04-25 19:32:15.723416 mypy_boto3_rds-1.34.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-04-25 19:31:54.000000 mypy_boto3_rds-1.34.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:15.719416 mypy_boto3_rds-1.34.92/mypy_boto3_rds/
+-rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-25 19:31:54.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-25 19:31:54.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-25 19:31:54.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   164366 2024-04-25 19:31:57.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   164363 2024-04-25 19:31:56.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20349 2024-04-25 19:31:58.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20349 2024-04-25 19:31:57.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    51753 2024-04-25 19:31:57.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51712 2024-04-25 19:31:57.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:54.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   208002 2024-04-25 19:32:02.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   208002 2024-04-25 19:32:00.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:31:54.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-04-25 19:31:57.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-04-25 19:31:57.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:15.723416 mypy_boto3_rds-1.34.92/mypy_boto3_rds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-04-25 19:32:15.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-25 19:32:15.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:15.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:15.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 19:32:15.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 19:32:15.000000 mypy_boto3_rds-1.34.92/mypy_boto3_rds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:32:15.723416 mypy_boto3_rds-1.34.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-25 19:31:54.000000 mypy_boto3_rds-1.34.92/setup.py
```

### Comparing `mypy_boto3_rds-1.34.91/LICENSE` & `mypy_boto3_rds-1.34.92/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/PKG-INFO` & `mypy_boto3_rds-1.34.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.34.91
-Summary: Type annotations for boto3.RDS 1.34.91 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.92
+Summary: Type annotations for boto3.RDS 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_rds-1.34.91/README.md` & `mypy_boto3_rds-1.34.92/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/__init__.py` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/__init__.pyi` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/__main__.py` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RDS 1.34.91\n"
-        "Version:         1.34.91\n"
+        "Type annotations for boto3.RDS 1.34.92\n"
+        "Version:         1.34.92\n"
         "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.91")
+    print("1.34.92")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/client.py` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/client.pyi` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/literals.py` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/literals.pyi` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/paginator.py` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/paginator.pyi` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/type_defs.py` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     "CreateGlobalClusterMessageRequestTypeDef",
     "CustomDBEngineVersionAMITypeDef",
     "RestoreWindowTypeDef",
     "DBClusterBacktrackTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
-    "ParameterOutputTypeDef",
+    "ParameterExtraOutputTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "DBClusterStatusInfoTypeDef",
     "DomainMembershipTypeDef",
     "LimitlessDatabaseTypeDef",
     "MasterUserSecretTypeDef",
     "ScalingConfigurationInfoTypeDef",
@@ -114,14 +114,15 @@
     "DBInstanceAutomatedBackupsReplicationTypeDef",
     "DBInstanceRoleTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "DBParameterGroupStatusTypeDef",
     "DBSecurityGroupMembershipTypeDef",
     "EndpointTypeDef",
     "OptionGroupMembershipTypeDef",
+    "ParameterOutputTypeDef",
     "TargetHealthTypeDef",
     "UserAuthConfigInfoTypeDef",
     "DocLinkTypeDef",
     "EC2SecurityGroupTypeDef",
     "IPRangeTypeDef",
     "DBShardGroupTypeDef",
     "DBSnapshotAttributeTypeDef",
@@ -182,15 +183,14 @@
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "ModifyIntegrationMessageRequestTypeDef",
     "ModifyTenantDatabaseMessageRequestTypeDef",
     "OptionSettingTypeDef",
     "OptionVersionTypeDef",
     "OutpostTypeDef",
-    "ParameterExtraOutputTypeDef",
     "ParameterTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "PromoteReadReplicaMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBClusterMessageRequestTypeDef",
@@ -298,20 +298,20 @@
     "ModifyDBProxyEndpointResponseTypeDef",
     "CreateDBProxyRequestRequestTypeDef",
     "ModifyDBProxyRequestRequestTypeDef",
     "DBClusterAutomatedBackupTypeDef",
     "DBClusterBacktrackMessageTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
-    "DBParameterGroupDetailsTypeDef",
-    "EngineDefaultsTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionResponseTypeDef",
     "DBEngineVersionTypeDef",
     "DBInstanceAutomatedBackupTypeDef",
+    "DBParameterGroupDetailsTypeDef",
+    "EngineDefaultsTypeDef",
     "DBProxyTargetTypeDef",
     "DBProxyTypeDef",
     "DBSecurityGroupTypeDef",
     "DescribeDBShardGroupsResponseTypeDef",
     "DBSnapshotAttributesResultTypeDef",
     "DescribeBlueGreenDeploymentsRequestRequestTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
@@ -443,23 +443,23 @@
     "CopyDBSnapshotResultTypeDef",
     "CreateDBSnapshotResultTypeDef",
     "DBSnapshotMessageTypeDef",
     "DeleteDBSnapshotResultTypeDef",
     "ModifyDBSnapshotResultTypeDef",
     "DBClusterAutomatedBackupMessageTypeDef",
     "DeleteDBClusterAutomatedBackupResultTypeDef",
-    "DescribeEngineDefaultClusterParametersResultTypeDef",
-    "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     "DBEngineVersionMessageTypeDef",
     "DBInstanceAutomatedBackupMessageTypeDef",
     "DeleteDBInstanceAutomatedBackupResultTypeDef",
     "StartDBInstanceAutomatedBackupsReplicationResultTypeDef",
     "StopDBInstanceAutomatedBackupsReplicationResultTypeDef",
+    "DescribeEngineDefaultClusterParametersResultTypeDef",
+    "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBProxyTargetsResponseTypeDef",
     "RegisterDBProxyTargetsResponseTypeDef",
     "CreateDBProxyResponseTypeDef",
     "DeleteDBProxyResponseTypeDef",
     "DescribeDBProxiesResponseTypeDef",
     "ModifyDBProxyResponseTypeDef",
     "AuthorizeDBSecurityGroupIngressResultTypeDef",
@@ -886,16 +886,16 @@
 DBClusterOptionGroupStatusTypeDef = TypedDict(
     "DBClusterOptionGroupStatusTypeDef",
     {
         "DBClusterOptionGroupName": NotRequired[str],
         "Status": NotRequired[str],
     },
 )
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
+ParameterExtraOutputTypeDef = TypedDict(
+    "ParameterExtraOutputTypeDef",
     {
         "ParameterName": NotRequired[str],
         "ParameterValue": NotRequired[str],
         "Description": NotRequired[str],
         "Source": NotRequired[str],
         "ApplyType": NotRequired[str],
         "DataType": NotRequired[str],
@@ -1052,14 +1052,30 @@
 OptionGroupMembershipTypeDef = TypedDict(
     "OptionGroupMembershipTypeDef",
     {
         "OptionGroupName": NotRequired[str],
         "Status": NotRequired[str],
     },
 )
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
+    {
+        "ParameterName": NotRequired[str],
+        "ParameterValue": NotRequired[str],
+        "Description": NotRequired[str],
+        "Source": NotRequired[str],
+        "ApplyType": NotRequired[str],
+        "DataType": NotRequired[str],
+        "AllowedValues": NotRequired[str],
+        "IsModifiable": NotRequired[bool],
+        "MinimumEngineVersion": NotRequired[str],
+        "ApplyMethod": NotRequired[ApplyMethodType],
+        "SupportedEngineModes": NotRequired[List[str]],
+    },
+)
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": NotRequired[TargetStateType],
         "Reason": NotRequired[TargetHealthReasonType],
         "Description": NotRequired[str],
     },
@@ -1587,30 +1603,14 @@
 )
 OutpostTypeDef = TypedDict(
     "OutpostTypeDef",
     {
         "Arn": NotRequired[str],
     },
 )
-ParameterExtraOutputTypeDef = TypedDict(
-    "ParameterExtraOutputTypeDef",
-    {
-        "ParameterName": NotRequired[str],
-        "ParameterValue": NotRequired[str],
-        "Description": NotRequired[str],
-        "Source": NotRequired[str],
-        "ApplyType": NotRequired[str],
-        "DataType": NotRequired[str],
-        "AllowedValues": NotRequired[str],
-        "IsModifiable": NotRequired[bool],
-        "MinimumEngineVersion": NotRequired[str],
-        "ApplyMethod": NotRequired[ApplyMethodType],
-        "SupportedEngineModes": NotRequired[List[str]],
-    },
-)
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterName": NotRequired[str],
         "ParameterValue": NotRequired[str],
         "Description": NotRequired[str],
         "Source": NotRequired[str],
@@ -3229,35 +3229,19 @@
         "DBClusterEndpoints": List[DBClusterEndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterExtraOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DBParameterGroupDetailsTypeDef = TypedDict(
-    "DBParameterGroupDetailsTypeDef",
-    {
-        "Parameters": List[ParameterOutputTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-EngineDefaultsTypeDef = TypedDict(
-    "EngineDefaultsTypeDef",
-    {
-        "DBParameterGroupFamily": NotRequired[str],
-        "Marker": NotRequired[str],
-        "Parameters": NotRequired[List[ParameterOutputTypeDef]],
-    },
-)
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": NotRequired[str],
         "DBClusterSnapshotAttributes": NotRequired[List[DBClusterSnapshotAttributeTypeDef]],
     },
 )
@@ -3372,14 +3356,30 @@
         "BackupTarget": NotRequired[str],
         "StorageThroughput": NotRequired[int],
         "AwsBackupRecoveryPointArn": NotRequired[str],
         "DedicatedLogVolume": NotRequired[bool],
         "MultiTenant": NotRequired[bool],
     },
 )
+DBParameterGroupDetailsTypeDef = TypedDict(
+    "DBParameterGroupDetailsTypeDef",
+    {
+        "Parameters": List[ParameterOutputTypeDef],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+EngineDefaultsTypeDef = TypedDict(
+    "EngineDefaultsTypeDef",
+    {
+        "DBParameterGroupFamily": NotRequired[str],
+        "Marker": NotRequired[str],
+        "Parameters": NotRequired[List[ParameterOutputTypeDef]],
+    },
+)
 DBProxyTargetTypeDef = TypedDict(
     "DBProxyTargetTypeDef",
     {
         "TargetArn": NotRequired[str],
         "Endpoint": NotRequired[str],
         "TrackedClusterId": NotRequired[str],
         "RdsResourceId": NotRequired[str],
@@ -4858,28 +4858,14 @@
 DeleteDBClusterAutomatedBackupResultTypeDef = TypedDict(
     "DeleteDBClusterAutomatedBackupResultTypeDef",
     {
         "DBClusterAutomatedBackup": DBClusterAutomatedBackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
-    "DescribeEngineDefaultClusterParametersResultTypeDef",
-    {
-        "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeEngineDefaultParametersResultTypeDef = TypedDict(
-    "DescribeEngineDefaultParametersResultTypeDef",
-    {
-        "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeDBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4923,14 +4909,28 @@
 StopDBInstanceAutomatedBackupsReplicationResultTypeDef = TypedDict(
     "StopDBInstanceAutomatedBackupsReplicationResultTypeDef",
     {
         "DBInstanceAutomatedBackup": DBInstanceAutomatedBackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
+    "DescribeEngineDefaultClusterParametersResultTypeDef",
+    {
+        "EngineDefaults": EngineDefaultsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeEngineDefaultParametersResultTypeDef = TypedDict(
+    "DescribeEngineDefaultParametersResultTypeDef",
+    {
+        "EngineDefaults": EngineDefaultsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeDBProxyTargetsResponseTypeDef = TypedDict(
     "DescribeDBProxyTargetsResponseTypeDef",
     {
         "Targets": List[DBProxyTargetTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/type_defs.pyi` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     "CreateGlobalClusterMessageRequestTypeDef",
     "CustomDBEngineVersionAMITypeDef",
     "RestoreWindowTypeDef",
     "DBClusterBacktrackTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
-    "ParameterOutputTypeDef",
+    "ParameterExtraOutputTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "DBClusterStatusInfoTypeDef",
     "DomainMembershipTypeDef",
     "LimitlessDatabaseTypeDef",
     "MasterUserSecretTypeDef",
     "ScalingConfigurationInfoTypeDef",
@@ -114,14 +114,15 @@
     "DBInstanceAutomatedBackupsReplicationTypeDef",
     "DBInstanceRoleTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "DBParameterGroupStatusTypeDef",
     "DBSecurityGroupMembershipTypeDef",
     "EndpointTypeDef",
     "OptionGroupMembershipTypeDef",
+    "ParameterOutputTypeDef",
     "TargetHealthTypeDef",
     "UserAuthConfigInfoTypeDef",
     "DocLinkTypeDef",
     "EC2SecurityGroupTypeDef",
     "IPRangeTypeDef",
     "DBShardGroupTypeDef",
     "DBSnapshotAttributeTypeDef",
@@ -182,15 +183,14 @@
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "ModifyIntegrationMessageRequestTypeDef",
     "ModifyTenantDatabaseMessageRequestTypeDef",
     "OptionSettingTypeDef",
     "OptionVersionTypeDef",
     "OutpostTypeDef",
-    "ParameterExtraOutputTypeDef",
     "ParameterTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "PromoteReadReplicaMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBClusterMessageRequestTypeDef",
@@ -298,20 +298,20 @@
     "ModifyDBProxyEndpointResponseTypeDef",
     "CreateDBProxyRequestRequestTypeDef",
     "ModifyDBProxyRequestRequestTypeDef",
     "DBClusterAutomatedBackupTypeDef",
     "DBClusterBacktrackMessageTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
-    "DBParameterGroupDetailsTypeDef",
-    "EngineDefaultsTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionResponseTypeDef",
     "DBEngineVersionTypeDef",
     "DBInstanceAutomatedBackupTypeDef",
+    "DBParameterGroupDetailsTypeDef",
+    "EngineDefaultsTypeDef",
     "DBProxyTargetTypeDef",
     "DBProxyTypeDef",
     "DBSecurityGroupTypeDef",
     "DescribeDBShardGroupsResponseTypeDef",
     "DBSnapshotAttributesResultTypeDef",
     "DescribeBlueGreenDeploymentsRequestRequestTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
@@ -443,23 +443,23 @@
     "CopyDBSnapshotResultTypeDef",
     "CreateDBSnapshotResultTypeDef",
     "DBSnapshotMessageTypeDef",
     "DeleteDBSnapshotResultTypeDef",
     "ModifyDBSnapshotResultTypeDef",
     "DBClusterAutomatedBackupMessageTypeDef",
     "DeleteDBClusterAutomatedBackupResultTypeDef",
-    "DescribeEngineDefaultClusterParametersResultTypeDef",
-    "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     "DBEngineVersionMessageTypeDef",
     "DBInstanceAutomatedBackupMessageTypeDef",
     "DeleteDBInstanceAutomatedBackupResultTypeDef",
     "StartDBInstanceAutomatedBackupsReplicationResultTypeDef",
     "StopDBInstanceAutomatedBackupsReplicationResultTypeDef",
+    "DescribeEngineDefaultClusterParametersResultTypeDef",
+    "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBProxyTargetsResponseTypeDef",
     "RegisterDBProxyTargetsResponseTypeDef",
     "CreateDBProxyResponseTypeDef",
     "DeleteDBProxyResponseTypeDef",
     "DescribeDBProxiesResponseTypeDef",
     "ModifyDBProxyResponseTypeDef",
     "AuthorizeDBSecurityGroupIngressResultTypeDef",
@@ -886,16 +886,16 @@
 DBClusterOptionGroupStatusTypeDef = TypedDict(
     "DBClusterOptionGroupStatusTypeDef",
     {
         "DBClusterOptionGroupName": NotRequired[str],
         "Status": NotRequired[str],
     },
 )
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
+ParameterExtraOutputTypeDef = TypedDict(
+    "ParameterExtraOutputTypeDef",
     {
         "ParameterName": NotRequired[str],
         "ParameterValue": NotRequired[str],
         "Description": NotRequired[str],
         "Source": NotRequired[str],
         "ApplyType": NotRequired[str],
         "DataType": NotRequired[str],
@@ -1052,14 +1052,30 @@
 OptionGroupMembershipTypeDef = TypedDict(
     "OptionGroupMembershipTypeDef",
     {
         "OptionGroupName": NotRequired[str],
         "Status": NotRequired[str],
     },
 )
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
+    {
+        "ParameterName": NotRequired[str],
+        "ParameterValue": NotRequired[str],
+        "Description": NotRequired[str],
+        "Source": NotRequired[str],
+        "ApplyType": NotRequired[str],
+        "DataType": NotRequired[str],
+        "AllowedValues": NotRequired[str],
+        "IsModifiable": NotRequired[bool],
+        "MinimumEngineVersion": NotRequired[str],
+        "ApplyMethod": NotRequired[ApplyMethodType],
+        "SupportedEngineModes": NotRequired[List[str]],
+    },
+)
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": NotRequired[TargetStateType],
         "Reason": NotRequired[TargetHealthReasonType],
         "Description": NotRequired[str],
     },
@@ -1587,30 +1603,14 @@
 )
 OutpostTypeDef = TypedDict(
     "OutpostTypeDef",
     {
         "Arn": NotRequired[str],
     },
 )
-ParameterExtraOutputTypeDef = TypedDict(
-    "ParameterExtraOutputTypeDef",
-    {
-        "ParameterName": NotRequired[str],
-        "ParameterValue": NotRequired[str],
-        "Description": NotRequired[str],
-        "Source": NotRequired[str],
-        "ApplyType": NotRequired[str],
-        "DataType": NotRequired[str],
-        "AllowedValues": NotRequired[str],
-        "IsModifiable": NotRequired[bool],
-        "MinimumEngineVersion": NotRequired[str],
-        "ApplyMethod": NotRequired[ApplyMethodType],
-        "SupportedEngineModes": NotRequired[List[str]],
-    },
-)
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterName": NotRequired[str],
         "ParameterValue": NotRequired[str],
         "Description": NotRequired[str],
         "Source": NotRequired[str],
@@ -3229,35 +3229,19 @@
         "DBClusterEndpoints": List[DBClusterEndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterExtraOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DBParameterGroupDetailsTypeDef = TypedDict(
-    "DBParameterGroupDetailsTypeDef",
-    {
-        "Parameters": List[ParameterOutputTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-EngineDefaultsTypeDef = TypedDict(
-    "EngineDefaultsTypeDef",
-    {
-        "DBParameterGroupFamily": NotRequired[str],
-        "Marker": NotRequired[str],
-        "Parameters": NotRequired[List[ParameterOutputTypeDef]],
-    },
-)
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": NotRequired[str],
         "DBClusterSnapshotAttributes": NotRequired[List[DBClusterSnapshotAttributeTypeDef]],
     },
 )
@@ -3372,14 +3356,30 @@
         "BackupTarget": NotRequired[str],
         "StorageThroughput": NotRequired[int],
         "AwsBackupRecoveryPointArn": NotRequired[str],
         "DedicatedLogVolume": NotRequired[bool],
         "MultiTenant": NotRequired[bool],
     },
 )
+DBParameterGroupDetailsTypeDef = TypedDict(
+    "DBParameterGroupDetailsTypeDef",
+    {
+        "Parameters": List[ParameterOutputTypeDef],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+EngineDefaultsTypeDef = TypedDict(
+    "EngineDefaultsTypeDef",
+    {
+        "DBParameterGroupFamily": NotRequired[str],
+        "Marker": NotRequired[str],
+        "Parameters": NotRequired[List[ParameterOutputTypeDef]],
+    },
+)
 DBProxyTargetTypeDef = TypedDict(
     "DBProxyTargetTypeDef",
     {
         "TargetArn": NotRequired[str],
         "Endpoint": NotRequired[str],
         "TrackedClusterId": NotRequired[str],
         "RdsResourceId": NotRequired[str],
@@ -4858,28 +4858,14 @@
 DeleteDBClusterAutomatedBackupResultTypeDef = TypedDict(
     "DeleteDBClusterAutomatedBackupResultTypeDef",
     {
         "DBClusterAutomatedBackup": DBClusterAutomatedBackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
-    "DescribeEngineDefaultClusterParametersResultTypeDef",
-    {
-        "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeEngineDefaultParametersResultTypeDef = TypedDict(
-    "DescribeEngineDefaultParametersResultTypeDef",
-    {
-        "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeDBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4923,14 +4909,28 @@
 StopDBInstanceAutomatedBackupsReplicationResultTypeDef = TypedDict(
     "StopDBInstanceAutomatedBackupsReplicationResultTypeDef",
     {
         "DBInstanceAutomatedBackup": DBInstanceAutomatedBackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
+    "DescribeEngineDefaultClusterParametersResultTypeDef",
+    {
+        "EngineDefaults": EngineDefaultsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeEngineDefaultParametersResultTypeDef = TypedDict(
+    "DescribeEngineDefaultParametersResultTypeDef",
+    {
+        "EngineDefaults": EngineDefaultsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeDBProxyTargetsResponseTypeDef = TypedDict(
     "DescribeDBProxyTargetsResponseTypeDef",
     {
         "Targets": List[DBProxyTargetTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/waiter.py` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds/waiter.pyi` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/PKG-INFO` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.34.91
-Summary: Type annotations for boto3.RDS 1.34.91 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.92
+Summary: Type annotations for boto3.RDS 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/SOURCES.txt` & `mypy_boto3_rds-1.34.92/mypy_boto3_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.91/setup.py` & `mypy_boto3_rds-1.34.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rds",
-    version="1.34.91",
+    version="1.34.92",
     packages=["mypy_boto3_rds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.RDS 1.34.91 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.RDS 1.34.92 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

