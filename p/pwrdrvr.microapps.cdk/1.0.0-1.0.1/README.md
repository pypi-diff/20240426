# Comparing `tmp/pwrdrvr.microapps.cdk-1.0.0.tar.gz` & `tmp/pwrdrvr.microapps.cdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwrdrvr.microapps.cdk-1.0.0.tar", last modified: Sat Sep 30 23:12:22 2023, max compression
+gzip compressed data, was "pwrdrvr.microapps.cdk-1.0.1.tar", last modified: Fri Apr 26 04:02:44 2024, max compression
```

## Comparing `pwrdrvr.microapps.cdk-1.0.0.tar` & `pwrdrvr.microapps.cdk-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 23:12:22.632751 pwrdrvr.microapps.cdk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-09-30 23:12:05.000000 pwrdrvr.microapps.cdk-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-09-30 23:12:05.000000 pwrdrvr.microapps.cdk-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18550 2023-09-30 23:12:22.632751 pwrdrvr.microapps.cdk-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17546 2023-09-30 23:12:05.000000 pwrdrvr.microapps.cdk-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-09-30 23:12:05.000000 pwrdrvr.microapps.cdk-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-30 23:12:22.632751 pwrdrvr.microapps.cdk-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2023-09-30 23:12:05.000000 pwrdrvr.microapps.cdk-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 23:12:22.624750 pwrdrvr.microapps.cdk-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 23:12:22.624750 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 23:12:22.624750 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr/microapps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 23:12:22.628751 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr/microapps/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)   238764 2023-09-30 23:12:05.000000 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr/microapps/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 23:12:22.628751 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr/microapps/cdk/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-09-30 23:12:05.000000 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr/microapps/cdk/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2665189 2023-09-30 23:12:05.000000 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr/microapps/cdk/_jsii/microapps-cdk@1.0.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-30 23:12:05.000000 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr/microapps/cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 23:12:22.628751 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr.microapps.cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18550 2023-09-30 23:12:22.000000 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-09-30 23:12:22.000000 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr.microapps.cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-30 23:12:22.000000 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr.microapps.cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-09-30 23:12:22.000000 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr.microapps.cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-30 23:12:22.000000 pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr.microapps.cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.288272 pwrdrvr.microapps.cdk-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-04-26 04:02:44.288272 pwrdrvr.microapps.cdk-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17546 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 04:02:44.288272 pwrdrvr.microapps.cdk-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.280272 pwrdrvr.microapps.cdk-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.280272 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.280272 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.284272 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)   219448 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.284272 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2706396 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/_jsii/microapps-cdk@1.0.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:02:32.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:02:44.284272 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-04-26 04:02:44.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-26 04:02:44.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:02:44.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 04:02:44.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 04:02:44.000000 pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/top_level.txt
```

### Comparing `pwrdrvr.microapps.cdk-1.0.0/LICENSE` & `pwrdrvr.microapps.cdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pwrdrvr.microapps.cdk-1.0.0/PKG-INFO` & `pwrdrvr.microapps.cdk-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pwrdrvr.microapps.cdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: MicroApps framework, by PwrDrvr LLC, delivered as an AWS CDK construct that provides the DynamoDB, Router service, Deploy service, API Gateway, and CloudFront distribution.
 Home-page: https://github.com/pwrdrvr/microapps-core
 Author: PwrDrvr LLC<harold@pwrdrvr.com>
 License: MIT
 Project-URL: Source, https://github.com/pwrdrvr/microapps-core
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CI](https://github.com/pwrdrvr/microapps-core/actions/workflows/ci.yml/badge.svg)](https://github.com/pwrdrvr/microapps-core/actions/workflows/ci.yml) [![Merge to Main Build](https://github.com/pwrdrvr/microapps-core/actions/workflows/main-build.yml/badge.svg)](https://github.com/pwrdrvr/microapps-core/actions/workflows/main-build.yml) [![Release Packages](https://github.com/pwrdrvr/microapps-core/actions/workflows/release.yml/badge.svg)](https://github.com/pwrdrvr/microapps-core/actions/workflows/release.yml)
 
 # Overview
```

### Comparing `pwrdrvr.microapps.cdk-1.0.0/README.md` & `pwrdrvr.microapps.cdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pwrdrvr.microapps.cdk-1.0.0/setup.py` & `pwrdrvr.microapps.cdk-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pwrdrvr.microapps.cdk",
-    "version": "1.0.0",
+    "version": "1.0.1",
     "description": "MicroApps framework, by PwrDrvr LLC, delivered as an AWS CDK construct that provides the DynamoDB, Router service, Deploy service, API Gateway, and CloudFront distribution.",
     "license": "MIT",
     "url": "https://github.com/pwrdrvr/microapps-core",
     "long_description_content_type": "text/markdown",
     "author": "PwrDrvr LLC<harold@pwrdrvr.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,40 +22,37 @@
     },
     "packages": [
         "pwrdrvr.microapps.cdk",
         "pwrdrvr.microapps.cdk._jsii"
     ],
     "package_data": {
         "pwrdrvr.microapps.cdk._jsii": [
-            "microapps-cdk@1.0.0.jsii.tgz"
+            "microapps-cdk@1.0.1.jsii.tgz"
         ],
         "pwrdrvr.microapps.cdk": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.28.0, <3.0.0",
-        "aws-cdk.aws-apigatewayv2-alpha>=2.28.0.a0, <3.0.0",
-        "aws-cdk.aws-apigatewayv2-authorizers-alpha>=2.28.0.a0, <3.0.0",
-        "aws-cdk.aws-apigatewayv2-integrations-alpha>=2.28.0.a0, <3.0.0",
+        "aws-cdk-lib>=2.95.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.75.0, <2.0.0",
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
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr/microapps/cdk/__init__.py` & `pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr/microapps/cdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,14 +329,17 @@
 ### SignatureV4 Headers
 
 * `authorization`
 * `x-amz-date`
 * `x-amz-security-token`
 * `x-amz-content-sha256`
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
@@ -344,15 +347,14 @@
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
 import aws_cdk as _aws_cdk_ceddda9d
-import aws_cdk.aws_apigatewayv2_alpha as _aws_cdk_aws_apigatewayv2_alpha_050969fe
 import aws_cdk.aws_certificatemanager as _aws_cdk_aws_certificatemanager_ceddda9d
 import aws_cdk.aws_cloudfront as _aws_cdk_aws_cloudfront_ceddda9d
 import aws_cdk.aws_cloudfront_origins as _aws_cdk_aws_cloudfront_origins_ceddda9d
 import aws_cdk.aws_cloudfront.experimental as _aws_cdk_aws_cloudfront_experimental_ceddda9d
 import aws_cdk.aws_dynamodb as _aws_cdk_aws_dynamodb_ceddda9d
 import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
 import aws_cdk.aws_lambda as _aws_cdk_aws_lambda_ceddda9d
@@ -748,23 +750,14 @@
         '''(experimental) {@inheritdoc IMicroAppsSvcs}.
 
         :stability: experimental
         '''
         ...
 
     @builtins.property
-    @jsii.member(jsii_name="apigwy")
-    def apigwy(self) -> typing.Optional["IMicroAppsAPIGwy"]:
-        '''(experimental) {@inheritdoc IMicroAppsAPIGwy}.
-
-        :stability: experimental
-        '''
-        ...
-
-    @builtins.property
     @jsii.member(jsii_name="edgeToOrigin")
     def edge_to_origin(self) -> typing.Optional["IMicroAppsEdgeToOrigin"]:
         '''(experimental) {@inheritdoc IMicroAppsEdgeToOrigin}.
 
         :stability: experimental
         '''
         ...
@@ -802,95 +795,26 @@
         '''(experimental) {@inheritdoc IMicroAppsSvcs}.
 
         :stability: experimental
         '''
         return typing.cast("IMicroAppsSvcs", jsii.get(self, "svcs"))
 
     @builtins.property
-    @jsii.member(jsii_name="apigwy")
-    def apigwy(self) -> typing.Optional["IMicroAppsAPIGwy"]:
-        '''(experimental) {@inheritdoc IMicroAppsAPIGwy}.
-
-        :stability: experimental
-        '''
-        return typing.cast(typing.Optional["IMicroAppsAPIGwy"], jsii.get(self, "apigwy"))
-
-    @builtins.property
     @jsii.member(jsii_name="edgeToOrigin")
     def edge_to_origin(self) -> typing.Optional["IMicroAppsEdgeToOrigin"]:
         '''(experimental) {@inheritdoc IMicroAppsEdgeToOrigin}.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional["IMicroAppsEdgeToOrigin"], jsii.get(self, "edgeToOrigin"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IMicroApps).__jsii_proxy_class__ = lambda : _IMicroAppsProxy
 
 
-@jsii.interface(jsii_type="@pwrdrvr/microapps-cdk.IMicroAppsAPIGwy")
-class IMicroAppsAPIGwy(typing_extensions.Protocol):
-    '''(experimental) Represents a MicroApps API Gateway.
-
-    :stability: experimental
-    '''
-
-    @builtins.property
-    @jsii.member(jsii_name="httpApi")
-    def http_api(self) -> _aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi:
-        '''(experimental) API Gateway.
-
-        :stability: experimental
-        '''
-        ...
-
-    @builtins.property
-    @jsii.member(jsii_name="dnAppsOrigin")
-    def dn_apps_origin(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.IDomainName]:
-        '''(experimental) Domain Name applied to API Gateway origin.
-
-        :stability: experimental
-        '''
-        ...
-
-
-class _IMicroAppsAPIGwyProxy:
-    '''(experimental) Represents a MicroApps API Gateway.
-
-    :stability: experimental
-    '''
-
-    __jsii_type__: typing.ClassVar[str] = "@pwrdrvr/microapps-cdk.IMicroAppsAPIGwy"
-
-    @builtins.property
-    @jsii.member(jsii_name="httpApi")
-    def http_api(self) -> _aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi:
-        '''(experimental) API Gateway.
-
-        :stability: experimental
-        '''
-        return typing.cast(_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi, jsii.get(self, "httpApi"))
-
-    @builtins.property
-    @jsii.member(jsii_name="dnAppsOrigin")
-    def dn_apps_origin(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.IDomainName]:
-        '''(experimental) Domain Name applied to API Gateway origin.
-
-        :stability: experimental
-        '''
-        return typing.cast(typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.IDomainName], jsii.get(self, "dnAppsOrigin"))
-
-# Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
-typing.cast(typing.Any, IMicroAppsAPIGwy).__jsii_proxy_class__ = lambda : _IMicroAppsAPIGwyProxy
-
-
 @jsii.interface(jsii_type="@pwrdrvr/microapps-cdk.IMicroAppsCF")
 class IMicroAppsCF(typing_extensions.Protocol):
     '''(experimental) Represents a MicroApps CloudFront.
 
     :stability: experimental
     '''
 
@@ -970,15 +894,15 @@
     :stability: experimental
     '''
 
     @builtins.property
     @jsii.member(jsii_name="edgeToOriginFunction")
     def edge_to_origin_function(
         self,
-    ) -> typing.Union[_aws_cdk_aws_cloudfront_experimental_ceddda9d.EdgeFunction, _aws_cdk_aws_lambda_ceddda9d.Function]:
+    ) -> typing.Union[_aws_cdk_aws_lambda_ceddda9d.Function, _aws_cdk_aws_cloudfront_experimental_ceddda9d.EdgeFunction]:
         '''(experimental) The edge to origin function for API Gateway Request Origin Edge Lambda.
 
         The generated ``config.yml`` is included in the Lambda's code.
 
         :stability: experimental
         '''
         ...
@@ -1012,22 +936,22 @@
 
     __jsii_type__: typing.ClassVar[str] = "@pwrdrvr/microapps-cdk.IMicroAppsEdgeToOrigin"
 
     @builtins.property
     @jsii.member(jsii_name="edgeToOriginFunction")
     def edge_to_origin_function(
         self,
-    ) -> typing.Union[_aws_cdk_aws_cloudfront_experimental_ceddda9d.EdgeFunction, _aws_cdk_aws_lambda_ceddda9d.Function]:
+    ) -> typing.Union[_aws_cdk_aws_lambda_ceddda9d.Function, _aws_cdk_aws_cloudfront_experimental_ceddda9d.EdgeFunction]:
         '''(experimental) The edge to origin function for API Gateway Request Origin Edge Lambda.
 
         The generated ``config.yml`` is included in the Lambda's code.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Union[_aws_cdk_aws_cloudfront_experimental_ceddda9d.EdgeFunction, _aws_cdk_aws_lambda_ceddda9d.Function], jsii.get(self, "edgeToOriginFunction"))
+        return typing.cast(typing.Union[_aws_cdk_aws_lambda_ceddda9d.Function, _aws_cdk_aws_cloudfront_experimental_ceddda9d.EdgeFunction], jsii.get(self, "edgeToOriginFunction"))
 
     @builtins.property
     @jsii.member(jsii_name="edgeToOriginLambdas")
     def edge_to_origin_lambdas(
         self,
     ) -> typing.List[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda]:
         '''(experimental) Configuration of the edge to origin lambda functions.
@@ -1309,15 +1233,15 @@
 
     Do not use this construct when adding MicroApps to an existing
     CloudFront, API Gateway, S3 Bucket, etc. or where access
     to all features of the AWS Resources are needed (e.g. to
     add additional Behaviors to the CloudFront distribution, set authorizors
     on API Gateway, etc.).
 
-    :see: {@link https://github.com/pwrdrvr/microapps-core/blob/main/packages/cdk/lib/MicroApps.ts | example usage in a CDK Stack }
+    :see: {@link https://github.com/pwrdrvr/microapps-core/blob/main/packages/cdk/lib/MicroApps.ts example usage in a CDK Stack }
     :stability: experimental
     :warning:
 
     This construct is not intended for production use.
     In a production stack the DynamoDB Table, API Gateway, S3 Buckets,
     etc. should be created in a "durable" stack where the IDs will not
     change and where changes to the MicroApps construct will not
@@ -1350,15 +1274,15 @@
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
         replace_host_header: typing.Optional[builtins.bool] = None,
         root_path_prefix: typing.Optional[builtins.str] = None,
         s3_policy_bypass_aro_as: typing.Optional[typing.Sequence[builtins.str]] = None,
         s3_policy_bypass_principal_ar_ns: typing.Optional[typing.Sequence[builtins.str]] = None,
         s3_strict_bucket_policy: typing.Optional[builtins.bool] = None,
         signing_mode: typing.Optional[builtins.str] = None,
-        table: typing.Optional[_aws_cdk_aws_dynamodb_ceddda9d.ITable] = None,
+        table: typing.Optional[typing.Union[_aws_cdk_aws_dynamodb_ceddda9d.ITable, _aws_cdk_aws_dynamodb_ceddda9d.ITableV2]] = None,
         table_name_for_edge_to_origin: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param app_env: (experimental) Passed to NODE_ENV of Router and Deployer Lambda functions. Default: dev
         :param add_x_forwarded_host_header: (experimental) Adds an X-Forwarded-Host-Header when calling API Gateway. Can only be trusted if ``signingMode`` is enabled, which restricts access to API Gateway to only IAM signed requests. Note: if true, creates OriginRequest Lambda @ Edge function for API Gateway Origin Default: true
@@ -1450,319 +1374,23 @@
         '''(experimental) {@inheritdoc IMicroAppsSvcs}.
 
         :stability: experimental
         '''
         return typing.cast(IMicroAppsSvcs, jsii.get(self, "svcs"))
 
     @builtins.property
-    @jsii.member(jsii_name="apigwy")
-    def apigwy(self) -> typing.Optional[IMicroAppsAPIGwy]:
-        '''(experimental) {@inheritdoc IMicroAppsAPIGwy}.
-
-        :stability: experimental
-        '''
-        return typing.cast(typing.Optional[IMicroAppsAPIGwy], jsii.get(self, "apigwy"))
-
-    @builtins.property
     @jsii.member(jsii_name="edgeToOrigin")
     def edge_to_origin(self) -> typing.Optional[IMicroAppsEdgeToOrigin]:
         '''(experimental) {@inheritdoc IMicroAppsEdgeToOrigin}.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[IMicroAppsEdgeToOrigin], jsii.get(self, "edgeToOrigin"))
 
 
-@jsii.implements(IMicroAppsAPIGwy)
-class MicroAppsAPIGwy(
-    _constructs_77d1e7e8.Construct,
-    metaclass=jsii.JSIIMeta,
-    jsii_type="@pwrdrvr/microapps-cdk.MicroAppsAPIGwy",
-):
-    '''(experimental) Create a new MicroApps API Gateway HTTP API endpoint, optionally requiring IAM authorization.
-
-    :stability: experimental
-    '''
-
-    def __init__(
-        self,
-        scope: _constructs_77d1e7e8.Construct,
-        id: builtins.str,
-        *,
-        asset_name_root: typing.Optional[builtins.str] = None,
-        asset_name_suffix: typing.Optional[builtins.str] = None,
-        cert_origin: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
-        domain_name_edge: typing.Optional[builtins.str] = None,
-        domain_name_origin: typing.Optional[builtins.str] = None,
-        r53_zone: typing.Optional[_aws_cdk_aws_route53_ceddda9d.IHostedZone] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-        require_iam_authorization: typing.Optional[builtins.bool] = None,
-        root_path_prefix: typing.Optional[builtins.str] = None,
-    ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param asset_name_root: (experimental) Optional asset name root. Default: - resource names auto assigned
-        :param asset_name_suffix: (experimental) Optional asset name suffix. Default: none
-        :param cert_origin: (experimental) Optional local region ACM certificate to use for API Gateway Note: required when using a custom domain. Default: none
-        :param domain_name_edge: (experimental) CloudFront edge domain name. Default: auto-assigned
-        :param domain_name_origin: (experimental) API Gateway origin domain name. Default: auto-assigned
-        :param r53_zone: (experimental) Route53 zone in which to create optional ``domainNameEdge`` record.
-        :param removal_policy: (experimental) RemovalPolicy override for child resources. Note: if set to DESTROY the S3 buckes will have ``autoDeleteObjects`` set to ``true`` Default: - per resource default
-        :param require_iam_authorization: (experimental) Require IAM auth on API Gateway. Default: true
-        :param root_path_prefix: (experimental) Path prefix on the root of the API Gateway Stage. Default: none
-
-        :stability: experimental
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__34bab1c0e9dae52015406b7b6cb0e2dc511c7bb54c69bd79c4bcf3e233cfe80c)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        props = MicroAppsAPIGwyProps(
-            asset_name_root=asset_name_root,
-            asset_name_suffix=asset_name_suffix,
-            cert_origin=cert_origin,
-            domain_name_edge=domain_name_edge,
-            domain_name_origin=domain_name_origin,
-            r53_zone=r53_zone,
-            removal_policy=removal_policy,
-            require_iam_authorization=require_iam_authorization,
-            root_path_prefix=root_path_prefix,
-        )
-
-        jsii.create(self.__class__, self, [scope, id, props])
-
-    @builtins.property
-    @jsii.member(jsii_name="httpApi")
-    def http_api(self) -> _aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi:
-        '''(experimental) API Gateway.
-
-        :stability: experimental
-        '''
-        return typing.cast(_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi, jsii.get(self, "httpApi"))
-
-    @builtins.property
-    @jsii.member(jsii_name="dnAppsOrigin")
-    def dn_apps_origin(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.IDomainName]:
-        '''(experimental) Domain Name applied to API Gateway origin.
-
-        :stability: experimental
-        '''
-        return typing.cast(typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.IDomainName], jsii.get(self, "dnAppsOrigin"))
-
-
-@jsii.data_type(
-    jsii_type="@pwrdrvr/microapps-cdk.MicroAppsAPIGwyProps",
-    jsii_struct_bases=[],
-    name_mapping={
-        "asset_name_root": "assetNameRoot",
-        "asset_name_suffix": "assetNameSuffix",
-        "cert_origin": "certOrigin",
-        "domain_name_edge": "domainNameEdge",
-        "domain_name_origin": "domainNameOrigin",
-        "r53_zone": "r53Zone",
-        "removal_policy": "removalPolicy",
-        "require_iam_authorization": "requireIAMAuthorization",
-        "root_path_prefix": "rootPathPrefix",
-    },
-)
-class MicroAppsAPIGwyProps:
-    def __init__(
-        self,
-        *,
-        asset_name_root: typing.Optional[builtins.str] = None,
-        asset_name_suffix: typing.Optional[builtins.str] = None,
-        cert_origin: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
-        domain_name_edge: typing.Optional[builtins.str] = None,
-        domain_name_origin: typing.Optional[builtins.str] = None,
-        r53_zone: typing.Optional[_aws_cdk_aws_route53_ceddda9d.IHostedZone] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-        require_iam_authorization: typing.Optional[builtins.bool] = None,
-        root_path_prefix: typing.Optional[builtins.str] = None,
-    ) -> None:
-        '''(experimental) Properties to initialize an instance of ``MicroAppsAPIGwy``.
-
-        :param asset_name_root: (experimental) Optional asset name root. Default: - resource names auto assigned
-        :param asset_name_suffix: (experimental) Optional asset name suffix. Default: none
-        :param cert_origin: (experimental) Optional local region ACM certificate to use for API Gateway Note: required when using a custom domain. Default: none
-        :param domain_name_edge: (experimental) CloudFront edge domain name. Default: auto-assigned
-        :param domain_name_origin: (experimental) API Gateway origin domain name. Default: auto-assigned
-        :param r53_zone: (experimental) Route53 zone in which to create optional ``domainNameEdge`` record.
-        :param removal_policy: (experimental) RemovalPolicy override for child resources. Note: if set to DESTROY the S3 buckes will have ``autoDeleteObjects`` set to ``true`` Default: - per resource default
-        :param require_iam_authorization: (experimental) Require IAM auth on API Gateway. Default: true
-        :param root_path_prefix: (experimental) Path prefix on the root of the API Gateway Stage. Default: none
-
-        :stability: experimental
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0ac58d864c4aee10362ea8caa1497daadeb0c8daba1b2f6e5094584e36ebb863)
-            check_type(argname="argument asset_name_root", value=asset_name_root, expected_type=type_hints["asset_name_root"])
-            check_type(argname="argument asset_name_suffix", value=asset_name_suffix, expected_type=type_hints["asset_name_suffix"])
-            check_type(argname="argument cert_origin", value=cert_origin, expected_type=type_hints["cert_origin"])
-            check_type(argname="argument domain_name_edge", value=domain_name_edge, expected_type=type_hints["domain_name_edge"])
-            check_type(argname="argument domain_name_origin", value=domain_name_origin, expected_type=type_hints["domain_name_origin"])
-            check_type(argname="argument r53_zone", value=r53_zone, expected_type=type_hints["r53_zone"])
-            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
-            check_type(argname="argument require_iam_authorization", value=require_iam_authorization, expected_type=type_hints["require_iam_authorization"])
-            check_type(argname="argument root_path_prefix", value=root_path_prefix, expected_type=type_hints["root_path_prefix"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if asset_name_root is not None:
-            self._values["asset_name_root"] = asset_name_root
-        if asset_name_suffix is not None:
-            self._values["asset_name_suffix"] = asset_name_suffix
-        if cert_origin is not None:
-            self._values["cert_origin"] = cert_origin
-        if domain_name_edge is not None:
-            self._values["domain_name_edge"] = domain_name_edge
-        if domain_name_origin is not None:
-            self._values["domain_name_origin"] = domain_name_origin
-        if r53_zone is not None:
-            self._values["r53_zone"] = r53_zone
-        if removal_policy is not None:
-            self._values["removal_policy"] = removal_policy
-        if require_iam_authorization is not None:
-            self._values["require_iam_authorization"] = require_iam_authorization
-        if root_path_prefix is not None:
-            self._values["root_path_prefix"] = root_path_prefix
-
-    @builtins.property
-    def asset_name_root(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Optional asset name root.
-
-        :default: - resource names auto assigned
-
-        :stability: experimental
-
-        Example::
-
-            microapps
-        '''
-        result = self._values.get("asset_name_root")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def asset_name_suffix(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Optional asset name suffix.
-
-        :default: none
-
-        :stability: experimental
-
-        Example::
-
-            -dev-pr-12
-        '''
-        result = self._values.get("asset_name_suffix")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def cert_origin(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate]:
-        '''(experimental) Optional local region ACM certificate to use for API Gateway Note: required when using a custom domain.
-
-        :default: none
-
-        :stability: experimental
-        '''
-        result = self._values.get("cert_origin")
-        return typing.cast(typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate], result)
-
-    @builtins.property
-    def domain_name_edge(self) -> typing.Optional[builtins.str]:
-        '''(experimental) CloudFront edge domain name.
-
-        :default: auto-assigned
-
-        :stability: experimental
-
-        Example::
-
-            apps.pwrdrvr.com
-        '''
-        result = self._values.get("domain_name_edge")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def domain_name_origin(self) -> typing.Optional[builtins.str]:
-        '''(experimental) API Gateway origin domain name.
-
-        :default: auto-assigned
-
-        :stability: experimental
-
-        Example::
-
-            apps-origin.pwrdrvr.com
-        '''
-        result = self._values.get("domain_name_origin")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def r53_zone(self) -> typing.Optional[_aws_cdk_aws_route53_ceddda9d.IHostedZone]:
-        '''(experimental) Route53 zone in which to create optional ``domainNameEdge`` record.
-
-        :stability: experimental
-        '''
-        result = self._values.get("r53_zone")
-        return typing.cast(typing.Optional[_aws_cdk_aws_route53_ceddda9d.IHostedZone], result)
-
-    @builtins.property
-    def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
-        '''(experimental) RemovalPolicy override for child resources.
-
-        Note: if set to DESTROY the S3 buckes will have ``autoDeleteObjects`` set to ``true``
-
-        :default: - per resource default
-
-        :stability: experimental
-        '''
-        result = self._values.get("removal_policy")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
-
-    @builtins.property
-    def require_iam_authorization(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Require IAM auth on API Gateway.
-
-        :default: true
-
-        :stability: experimental
-        '''
-        result = self._values.get("require_iam_authorization")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    @builtins.property
-    def root_path_prefix(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Path prefix on the root of the API Gateway Stage.
-
-        :default: none
-
-        :stability: experimental
-
-        Example::
-
-            dev/
-        '''
-        result = self._values.get("root_path_prefix")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "MicroAppsAPIGwyProps(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
 @jsii.implements(IMicroAppsCF)
 class MicroAppsCF(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="@pwrdrvr/microapps-cdk.MicroAppsCF",
 ):
     '''(experimental) Create a new MicroApps CloudFront Distribution.
@@ -1782,15 +1410,14 @@
         bucket_logs: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
         cert_edge: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
         create_api_path_route: typing.Optional[builtins.bool] = None,
         create_next_data_path_route: typing.Optional[builtins.bool] = None,
         domain_name_edge: typing.Optional[builtins.str] = None,
         domain_name_origin: typing.Optional[builtins.str] = None,
         edge_lambdas: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda, typing.Dict[builtins.str, typing.Any]]]] = None,
-        http_api: typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi] = None,
         origin_shield_region: typing.Optional[builtins.str] = None,
         r53_zone: typing.Optional[_aws_cdk_aws_route53_ceddda9d.IHostedZone] = None,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
         root_path_prefix: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
@@ -1802,15 +1429,14 @@
         :param bucket_logs: (experimental) S3 bucket for CloudFront logs.
         :param cert_edge: (experimental) ACM Certificate that covers ``domainNameEdge`` name.
         :param create_api_path_route: (experimental) Create an extra Behavior (Route) for /api/ that allows API routes to have a period in them. When false API routes with a period in the path will get routed to S3. When true API routes that contain /api/ in the path will get routed to API Gateway even if they have a period in the path. Default: true if httpApi is provided
         :param create_next_data_path_route: (experimental) Create an extra Behavior (Route) for /_next/data/ This route is used by Next.js to load data from the API Gateway on ``getServerSideProps`` calls. The requests can end in ``.json``, which would cause them to be routed to S3 if this route is not created. When false API routes with a period in the path will get routed to S3. When true API routes that contain /_next/data/ in the path will get routed to API Gateway even if they have a period in the path. Default: true if httpApi is provided
         :param domain_name_edge: (experimental) CloudFront Distribution domain name. Default: auto-assigned
         :param domain_name_origin: (experimental) API Gateway custom origin domain name. Default: - retrieved from httpApi, if possible
         :param edge_lambdas: (experimental) Configuration of the edge to origin lambda functions. Default: - no edge to API Gateway origin functions added
-        :param http_api: (experimental) API Gateway v2 HTTP API for apps.
         :param origin_shield_region: (experimental) Optional Origin Shield Region. This should be the region where the DynamoDB is located so the EdgeToOrigin calls have the lowest latency (~1 ms). Default: - none
         :param r53_zone: (experimental) Route53 zone in which to create optional ``domainNameEdge`` record.
         :param removal_policy: (experimental) RemovalPolicy override for child resources. Note: if set to DESTROY the S3 buckes will have ``autoDeleteObjects`` set to ``true`` Default: - per resource default
         :param root_path_prefix: (experimental) Path prefix on the root of the CloudFront distribution.
 
         :stability: experimental
         '''
@@ -1826,15 +1452,14 @@
             bucket_logs=bucket_logs,
             cert_edge=cert_edge,
             create_api_path_route=create_api_path_route,
             create_next_data_path_route=create_next_data_path_route,
             domain_name_edge=domain_name_edge,
             domain_name_origin=domain_name_origin,
             edge_lambdas=edge_lambdas,
-            http_api=http_api,
             origin_shield_region=origin_shield_region,
             r53_zone=r53_zone,
             removal_policy=removal_policy,
             root_path_prefix=root_path_prefix,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
@@ -1936,15 +1561,14 @@
         "bucket_logs": "bucketLogs",
         "cert_edge": "certEdge",
         "create_api_path_route": "createAPIPathRoute",
         "create_next_data_path_route": "createNextDataPathRoute",
         "domain_name_edge": "domainNameEdge",
         "domain_name_origin": "domainNameOrigin",
         "edge_lambdas": "edgeLambdas",
-        "http_api": "httpApi",
         "origin_shield_region": "originShieldRegion",
         "r53_zone": "r53Zone",
         "removal_policy": "removalPolicy",
         "root_path_prefix": "rootPathPrefix",
     },
 )
 class MicroAppsCFProps:
@@ -1958,15 +1582,14 @@
         bucket_logs: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
         cert_edge: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
         create_api_path_route: typing.Optional[builtins.bool] = None,
         create_next_data_path_route: typing.Optional[builtins.bool] = None,
         domain_name_edge: typing.Optional[builtins.str] = None,
         domain_name_origin: typing.Optional[builtins.str] = None,
         edge_lambdas: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda, typing.Dict[builtins.str, typing.Any]]]] = None,
-        http_api: typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi] = None,
         origin_shield_region: typing.Optional[builtins.str] = None,
         r53_zone: typing.Optional[_aws_cdk_aws_route53_ceddda9d.IHostedZone] = None,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
         root_path_prefix: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Properties to initialize an instance of ``MicroAppsCF``.
 
@@ -1977,15 +1600,14 @@
         :param bucket_logs: (experimental) S3 bucket for CloudFront logs.
         :param cert_edge: (experimental) ACM Certificate that covers ``domainNameEdge`` name.
         :param create_api_path_route: (experimental) Create an extra Behavior (Route) for /api/ that allows API routes to have a period in them. When false API routes with a period in the path will get routed to S3. When true API routes that contain /api/ in the path will get routed to API Gateway even if they have a period in the path. Default: true if httpApi is provided
         :param create_next_data_path_route: (experimental) Create an extra Behavior (Route) for /_next/data/ This route is used by Next.js to load data from the API Gateway on ``getServerSideProps`` calls. The requests can end in ``.json``, which would cause them to be routed to S3 if this route is not created. When false API routes with a period in the path will get routed to S3. When true API routes that contain /_next/data/ in the path will get routed to API Gateway even if they have a period in the path. Default: true if httpApi is provided
         :param domain_name_edge: (experimental) CloudFront Distribution domain name. Default: auto-assigned
         :param domain_name_origin: (experimental) API Gateway custom origin domain name. Default: - retrieved from httpApi, if possible
         :param edge_lambdas: (experimental) Configuration of the edge to origin lambda functions. Default: - no edge to API Gateway origin functions added
-        :param http_api: (experimental) API Gateway v2 HTTP API for apps.
         :param origin_shield_region: (experimental) Optional Origin Shield Region. This should be the region where the DynamoDB is located so the EdgeToOrigin calls have the lowest latency (~1 ms). Default: - none
         :param r53_zone: (experimental) Route53 zone in which to create optional ``domainNameEdge`` record.
         :param removal_policy: (experimental) RemovalPolicy override for child resources. Note: if set to DESTROY the S3 buckes will have ``autoDeleteObjects`` set to ``true`` Default: - per resource default
         :param root_path_prefix: (experimental) Path prefix on the root of the CloudFront distribution.
 
         :stability: experimental
         '''
@@ -1998,15 +1620,14 @@
             check_type(argname="argument bucket_logs", value=bucket_logs, expected_type=type_hints["bucket_logs"])
             check_type(argname="argument cert_edge", value=cert_edge, expected_type=type_hints["cert_edge"])
             check_type(argname="argument create_api_path_route", value=create_api_path_route, expected_type=type_hints["create_api_path_route"])
             check_type(argname="argument create_next_data_path_route", value=create_next_data_path_route, expected_type=type_hints["create_next_data_path_route"])
             check_type(argname="argument domain_name_edge", value=domain_name_edge, expected_type=type_hints["domain_name_edge"])
             check_type(argname="argument domain_name_origin", value=domain_name_origin, expected_type=type_hints["domain_name_origin"])
             check_type(argname="argument edge_lambdas", value=edge_lambdas, expected_type=type_hints["edge_lambdas"])
-            check_type(argname="argument http_api", value=http_api, expected_type=type_hints["http_api"])
             check_type(argname="argument origin_shield_region", value=origin_shield_region, expected_type=type_hints["origin_shield_region"])
             check_type(argname="argument r53_zone", value=r53_zone, expected_type=type_hints["r53_zone"])
             check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
             check_type(argname="argument root_path_prefix", value=root_path_prefix, expected_type=type_hints["root_path_prefix"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "bucket_apps_origin_app": bucket_apps_origin_app,
             "bucket_apps_origin_s3": bucket_apps_origin_s3,
@@ -2025,16 +1646,14 @@
             self._values["create_next_data_path_route"] = create_next_data_path_route
         if domain_name_edge is not None:
             self._values["domain_name_edge"] = domain_name_edge
         if domain_name_origin is not None:
             self._values["domain_name_origin"] = domain_name_origin
         if edge_lambdas is not None:
             self._values["edge_lambdas"] = edge_lambdas
-        if http_api is not None:
-            self._values["http_api"] = http_api
         if origin_shield_region is not None:
             self._values["origin_shield_region"] = origin_shield_region
         if r53_zone is not None:
             self._values["r53_zone"] = r53_zone
         if removal_policy is not None:
             self._values["removal_policy"] = removal_policy
         if root_path_prefix is not None:
@@ -2186,25 +1805,14 @@
 
         :stability: experimental
         '''
         result = self._values.get("edge_lambdas")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda]], result)
 
     @builtins.property
-    def http_api(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi]:
-        '''(experimental) API Gateway v2 HTTP API for apps.
-
-        :stability: experimental
-        '''
-        result = self._values.get("http_api")
-        return typing.cast(typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi], result)
-
-    @builtins.property
     def origin_shield_region(self) -> typing.Optional[builtins.str]:
         '''(experimental) Optional Origin Shield Region.
 
         This should be the region where the DynamoDB is located so the
         EdgeToOrigin calls have the lowest latency (~1 ms).
 
         :default: - none
@@ -2589,22 +2197,22 @@
 
         return typing.cast(builtins.str, jsii.sinvoke(cls, "generateEdgeToOriginConfig", [props]))
 
     @builtins.property
     @jsii.member(jsii_name="edgeToOriginFunction")
     def edge_to_origin_function(
         self,
-    ) -> typing.Union[_aws_cdk_aws_cloudfront_experimental_ceddda9d.EdgeFunction, _aws_cdk_aws_lambda_ceddda9d.Function]:
+    ) -> typing.Union[_aws_cdk_aws_lambda_ceddda9d.Function, _aws_cdk_aws_cloudfront_experimental_ceddda9d.EdgeFunction]:
         '''(experimental) The edge to origin function for API Gateway Request Origin Edge Lambda.
 
         The generated ``config.yml`` is included in the Lambda's code.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Union[_aws_cdk_aws_cloudfront_experimental_ceddda9d.EdgeFunction, _aws_cdk_aws_lambda_ceddda9d.Function], jsii.get(self, "edgeToOriginFunction"))
+        return typing.cast(typing.Union[_aws_cdk_aws_lambda_ceddda9d.Function, _aws_cdk_aws_cloudfront_experimental_ceddda9d.EdgeFunction], jsii.get(self, "edgeToOriginFunction"))
 
     @builtins.property
     @jsii.member(jsii_name="edgeToOriginLambdas")
     def edge_to_origin_lambdas(
         self,
     ) -> typing.List[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda]:
         '''(experimental) Configuration of the edge to origin lambda functions.
@@ -2959,15 +2567,15 @@
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
         replace_host_header: typing.Optional[builtins.bool] = None,
         root_path_prefix: typing.Optional[builtins.str] = None,
         s3_policy_bypass_aro_as: typing.Optional[typing.Sequence[builtins.str]] = None,
         s3_policy_bypass_principal_ar_ns: typing.Optional[typing.Sequence[builtins.str]] = None,
         s3_strict_bucket_policy: typing.Optional[builtins.bool] = None,
         signing_mode: typing.Optional[builtins.str] = None,
-        table: typing.Optional[_aws_cdk_aws_dynamodb_ceddda9d.ITable] = None,
+        table: typing.Optional[typing.Union[_aws_cdk_aws_dynamodb_ceddda9d.ITable, _aws_cdk_aws_dynamodb_ceddda9d.ITableV2]] = None,
         table_name_for_edge_to_origin: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Properties to initialize an instance of ``MicroApps``.
 
         :param app_env: (experimental) Passed to NODE_ENV of Router and Deployer Lambda functions. Default: dev
         :param add_x_forwarded_host_header: (experimental) Adds an X-Forwarded-Host-Header when calling API Gateway. Can only be trusted if ``signingMode`` is enabled, which restricts access to API Gateway to only IAM signed requests. Note: if true, creates OriginRequest Lambda @ Edge function for API Gateway Origin Default: true
         :param allowed_function_url_accounts: (experimental) Account IDs allowed for cross-account Function URL invocations. Default: []
@@ -3462,15 +3070,17 @@
 
         :stability: experimental
         '''
         result = self._values.get("signing_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def table(self) -> typing.Optional[_aws_cdk_aws_dynamodb_ceddda9d.ITable]:
+    def table(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_aws_dynamodb_ceddda9d.ITable, _aws_cdk_aws_dynamodb_ceddda9d.ITableV2]]:
         '''(experimental) Existing table for apps/versions/rules.
 
         :default: created by construct
 
         :stability: experimental
         :warning:
 
@@ -3481,15 +3091,15 @@
 
         Requirements:
 
         - Hash Key: ``PK``
         - Sort Key: ``SK``
         '''
         result = self._values.get("table")
-        return typing.cast(typing.Optional[_aws_cdk_aws_dynamodb_ceddda9d.ITable], result)
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_aws_dynamodb_ceddda9d.ITable, _aws_cdk_aws_dynamodb_ceddda9d.ITableV2]], result)
 
     @builtins.property
     def table_name_for_edge_to_origin(self) -> typing.Optional[builtins.str]:
         '''(experimental) Pre-set table name for apps/versions/rules.
 
         This is required when using v2 routing
 
@@ -3809,15 +3419,14 @@
         bucket_apps: _aws_cdk_aws_s3_ceddda9d.IBucket,
         bucket_apps_oai: _aws_cdk_aws_cloudfront_ceddda9d.OriginAccessIdentity,
         bucket_apps_staging: _aws_cdk_aws_s3_ceddda9d.IBucket,
         asset_name_root: typing.Optional[builtins.str] = None,
         asset_name_suffix: typing.Optional[builtins.str] = None,
         deployer_timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         edge_to_origin_role_arn: typing.Optional[typing.Sequence[builtins.str]] = None,
-        http_api: typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi] = None,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
         require_iam_authorization: typing.Optional[builtins.bool] = None,
         root_path_prefix: typing.Optional[builtins.str] = None,
         s3_policy_bypass_aro_as: typing.Optional[typing.Sequence[builtins.str]] = None,
         s3_policy_bypass_principal_ar_ns: typing.Optional[typing.Sequence[builtins.str]] = None,
         s3_strict_bucket_policy: typing.Optional[builtins.bool] = None,
         table: typing.Optional[_aws_cdk_aws_dynamodb_ceddda9d.ITable] = None,
@@ -3829,15 +3438,14 @@
         :param bucket_apps: (experimental) S3 bucket for deployed applications.
         :param bucket_apps_oai: (experimental) CloudFront Origin Access Identity for the deployed applications bucket.
         :param bucket_apps_staging: (experimental) S3 bucket for staged applications (prior to deploy).
         :param asset_name_root: (experimental) Optional asset name root. Default: - resource names auto assigned
         :param asset_name_suffix: (experimental) Optional asset name suffix. Default: none
         :param deployer_timeout: (experimental) Deployer timeout. For larger applications this needs to be set up to 2-5 minutes for the S3 copy Default: 2 minutes
         :param edge_to_origin_role_arn: (experimental) ARN of the IAM Role for the Edge to Origin Lambda Function.
-        :param http_api: (experimental) API Gateway v2 HTTP for Router and app.
         :param removal_policy: (experimental) RemovalPolicy override for child resources. Note: if set to DESTROY the S3 buckes will have ``autoDeleteObjects`` set to ``true`` Default: - per resource default
         :param require_iam_authorization: (experimental) Require IAM auth on API Gateway and Lambda Function URLs. Default: true
         :param root_path_prefix: (experimental) Path prefix on the root of the deployment. Default: none
         :param s3_policy_bypass_aro_as: (experimental) Applies when using s3StrictBucketPolicy = true. AROAs of the IAM Role to exclude from the DENY rules on the S3 Bucket Policy. This allows sessions that assume the IAM Role to be excluded from the DENY rules on the S3 Bucket Policy. Typically any admin roles / users that need to view or manage the S3 Bucket would be added to this list. Roles / users that are used directly, not assumed, can be added to ``s3PolicyBypassRoleNames`` instead. Note: This AROA must be specified to prevent this policy from locking out non-root sessions that have assumed the admin role. The notPrincipals will only match the role name exactly and will not match any session that has assumed the role since notPrincipals does not allow wildcard matches and does not do wildcard matches implicitly either. The AROA must be used because there are only 3 Principal variables available: https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_variables.html#principaltable aws:username, aws:userid, aws:PrincipalTag For an assumed role, aws:username is blank, aws:userid is: [unique id AKA AROA for Role]:[session name] Table of unique ID prefixes such as AROA: https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_identifiers.html#identifiers-prefixes The name of the role is simply not available for an assumed role and, if it was, a complicated comparison would be requierd to prevent exclusion of applying the Deny Rule to roles from other accounts. To get the AROA with the AWS CLI: aws iam get-role --role-name ROLE-NAME aws iam get-user --user-name USER-NAME
         :param s3_policy_bypass_principal_ar_ns: (experimental) Applies when using s3StrictBucketPolicy = true. IAM Role or IAM User names to exclude from the DENY rules on the S3 Bucket Policy. Roles that are Assumed must instead have their AROA added to ``s3PolicyBypassAROAs``. Typically any admin roles / users that need to view or manage the S3 Bucket would be added to this list.
         :param s3_strict_bucket_policy: (experimental) Use a strict S3 Bucket Policy that prevents applications from reading/writing/modifying/deleting files in the S3 Bucket outside of the path that is specific to their app/version. This setting should be used when applications are less than fully trusted. Default: false
         :param table: (experimental) Existing table for apps/versions/rules. Default: created by construct
@@ -3853,15 +3461,14 @@
             bucket_apps=bucket_apps,
             bucket_apps_oai=bucket_apps_oai,
             bucket_apps_staging=bucket_apps_staging,
             asset_name_root=asset_name_root,
             asset_name_suffix=asset_name_suffix,
             deployer_timeout=deployer_timeout,
             edge_to_origin_role_arn=edge_to_origin_role_arn,
-            http_api=http_api,
             removal_policy=removal_policy,
             require_iam_authorization=require_iam_authorization,
             root_path_prefix=root_path_prefix,
             s3_policy_bypass_aro_as=s3_policy_bypass_aro_as,
             s3_policy_bypass_principal_ar_ns=s3_policy_bypass_principal_ar_ns,
             s3_strict_bucket_policy=s3_strict_bucket_policy,
             table=table,
@@ -3905,15 +3512,14 @@
         "bucket_apps": "bucketApps",
         "bucket_apps_oai": "bucketAppsOAI",
         "bucket_apps_staging": "bucketAppsStaging",
         "asset_name_root": "assetNameRoot",
         "asset_name_suffix": "assetNameSuffix",
         "deployer_timeout": "deployerTimeout",
         "edge_to_origin_role_arn": "edgeToOriginRoleARN",
-        "http_api": "httpApi",
         "removal_policy": "removalPolicy",
         "require_iam_authorization": "requireIAMAuthorization",
         "root_path_prefix": "rootPathPrefix",
         "s3_policy_bypass_aro_as": "s3PolicyBypassAROAs",
         "s3_policy_bypass_principal_ar_ns": "s3PolicyBypassPrincipalARNs",
         "s3_strict_bucket_policy": "s3StrictBucketPolicy",
         "table": "table",
@@ -3927,15 +3533,14 @@
         bucket_apps: _aws_cdk_aws_s3_ceddda9d.IBucket,
         bucket_apps_oai: _aws_cdk_aws_cloudfront_ceddda9d.OriginAccessIdentity,
         bucket_apps_staging: _aws_cdk_aws_s3_ceddda9d.IBucket,
         asset_name_root: typing.Optional[builtins.str] = None,
         asset_name_suffix: typing.Optional[builtins.str] = None,
         deployer_timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         edge_to_origin_role_arn: typing.Optional[typing.Sequence[builtins.str]] = None,
-        http_api: typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi] = None,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
         require_iam_authorization: typing.Optional[builtins.bool] = None,
         root_path_prefix: typing.Optional[builtins.str] = None,
         s3_policy_bypass_aro_as: typing.Optional[typing.Sequence[builtins.str]] = None,
         s3_policy_bypass_principal_ar_ns: typing.Optional[typing.Sequence[builtins.str]] = None,
         s3_strict_bucket_policy: typing.Optional[builtins.bool] = None,
         table: typing.Optional[_aws_cdk_aws_dynamodb_ceddda9d.ITable] = None,
@@ -3946,15 +3551,14 @@
         :param bucket_apps: (experimental) S3 bucket for deployed applications.
         :param bucket_apps_oai: (experimental) CloudFront Origin Access Identity for the deployed applications bucket.
         :param bucket_apps_staging: (experimental) S3 bucket for staged applications (prior to deploy).
         :param asset_name_root: (experimental) Optional asset name root. Default: - resource names auto assigned
         :param asset_name_suffix: (experimental) Optional asset name suffix. Default: none
         :param deployer_timeout: (experimental) Deployer timeout. For larger applications this needs to be set up to 2-5 minutes for the S3 copy Default: 2 minutes
         :param edge_to_origin_role_arn: (experimental) ARN of the IAM Role for the Edge to Origin Lambda Function.
-        :param http_api: (experimental) API Gateway v2 HTTP for Router and app.
         :param removal_policy: (experimental) RemovalPolicy override for child resources. Note: if set to DESTROY the S3 buckes will have ``autoDeleteObjects`` set to ``true`` Default: - per resource default
         :param require_iam_authorization: (experimental) Require IAM auth on API Gateway and Lambda Function URLs. Default: true
         :param root_path_prefix: (experimental) Path prefix on the root of the deployment. Default: none
         :param s3_policy_bypass_aro_as: (experimental) Applies when using s3StrictBucketPolicy = true. AROAs of the IAM Role to exclude from the DENY rules on the S3 Bucket Policy. This allows sessions that assume the IAM Role to be excluded from the DENY rules on the S3 Bucket Policy. Typically any admin roles / users that need to view or manage the S3 Bucket would be added to this list. Roles / users that are used directly, not assumed, can be added to ``s3PolicyBypassRoleNames`` instead. Note: This AROA must be specified to prevent this policy from locking out non-root sessions that have assumed the admin role. The notPrincipals will only match the role name exactly and will not match any session that has assumed the role since notPrincipals does not allow wildcard matches and does not do wildcard matches implicitly either. The AROA must be used because there are only 3 Principal variables available: https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_variables.html#principaltable aws:username, aws:userid, aws:PrincipalTag For an assumed role, aws:username is blank, aws:userid is: [unique id AKA AROA for Role]:[session name] Table of unique ID prefixes such as AROA: https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_identifiers.html#identifiers-prefixes The name of the role is simply not available for an assumed role and, if it was, a complicated comparison would be requierd to prevent exclusion of applying the Deny Rule to roles from other accounts. To get the AROA with the AWS CLI: aws iam get-role --role-name ROLE-NAME aws iam get-user --user-name USER-NAME
         :param s3_policy_bypass_principal_ar_ns: (experimental) Applies when using s3StrictBucketPolicy = true. IAM Role or IAM User names to exclude from the DENY rules on the S3 Bucket Policy. Roles that are Assumed must instead have their AROA added to ``s3PolicyBypassAROAs``. Typically any admin roles / users that need to view or manage the S3 Bucket would be added to this list.
         :param s3_strict_bucket_policy: (experimental) Use a strict S3 Bucket Policy that prevents applications from reading/writing/modifying/deleting files in the S3 Bucket outside of the path that is specific to their app/version. This setting should be used when applications are less than fully trusted. Default: false
         :param table: (experimental) Existing table for apps/versions/rules. Default: created by construct
@@ -3967,15 +3571,14 @@
             check_type(argname="argument bucket_apps", value=bucket_apps, expected_type=type_hints["bucket_apps"])
             check_type(argname="argument bucket_apps_oai", value=bucket_apps_oai, expected_type=type_hints["bucket_apps_oai"])
             check_type(argname="argument bucket_apps_staging", value=bucket_apps_staging, expected_type=type_hints["bucket_apps_staging"])
             check_type(argname="argument asset_name_root", value=asset_name_root, expected_type=type_hints["asset_name_root"])
             check_type(argname="argument asset_name_suffix", value=asset_name_suffix, expected_type=type_hints["asset_name_suffix"])
             check_type(argname="argument deployer_timeout", value=deployer_timeout, expected_type=type_hints["deployer_timeout"])
             check_type(argname="argument edge_to_origin_role_arn", value=edge_to_origin_role_arn, expected_type=type_hints["edge_to_origin_role_arn"])
-            check_type(argname="argument http_api", value=http_api, expected_type=type_hints["http_api"])
             check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
             check_type(argname="argument require_iam_authorization", value=require_iam_authorization, expected_type=type_hints["require_iam_authorization"])
             check_type(argname="argument root_path_prefix", value=root_path_prefix, expected_type=type_hints["root_path_prefix"])
             check_type(argname="argument s3_policy_bypass_aro_as", value=s3_policy_bypass_aro_as, expected_type=type_hints["s3_policy_bypass_aro_as"])
             check_type(argname="argument s3_policy_bypass_principal_ar_ns", value=s3_policy_bypass_principal_ar_ns, expected_type=type_hints["s3_policy_bypass_principal_ar_ns"])
             check_type(argname="argument s3_strict_bucket_policy", value=s3_strict_bucket_policy, expected_type=type_hints["s3_strict_bucket_policy"])
             check_type(argname="argument table", value=table, expected_type=type_hints["table"])
@@ -3989,16 +3592,14 @@
             self._values["asset_name_root"] = asset_name_root
         if asset_name_suffix is not None:
             self._values["asset_name_suffix"] = asset_name_suffix
         if deployer_timeout is not None:
             self._values["deployer_timeout"] = deployer_timeout
         if edge_to_origin_role_arn is not None:
             self._values["edge_to_origin_role_arn"] = edge_to_origin_role_arn
-        if http_api is not None:
-            self._values["http_api"] = http_api
         if removal_policy is not None:
             self._values["removal_policy"] = removal_policy
         if require_iam_authorization is not None:
             self._values["require_iam_authorization"] = require_iam_authorization
         if root_path_prefix is not None:
             self._values["root_path_prefix"] = root_path_prefix
         if s3_policy_bypass_aro_as is not None:
@@ -4099,25 +3700,14 @@
 
         :stability: experimental
         '''
         result = self._values.get("edge_to_origin_role_arn")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
-    def http_api(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi]:
-        '''(experimental) API Gateway v2 HTTP for Router and app.
-
-        :stability: experimental
-        '''
-        result = self._values.get("http_api")
-        return typing.cast(typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi], result)
-
-    @builtins.property
     def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
         '''(experimental) RemovalPolicy override for child resources.
 
         Note: if set to DESTROY the S3 buckes will have ``autoDeleteObjects`` set to ``true``
 
         :default: - per resource default
 
@@ -4423,24 +4013,21 @@
 
 
 __all__ = [
     "AddRoutesOptions",
     "CreateAPIOriginPolicyOptions",
     "GenerateEdgeToOriginConfigOptions",
     "IMicroApps",
-    "IMicroAppsAPIGwy",
     "IMicroAppsCF",
     "IMicroAppsChildDeployer",
     "IMicroAppsEdgeToOrigin",
     "IMicroAppsS3",
     "IMicroAppsSvcs",
     "IMicroAppsTable",
     "MicroApps",
-    "MicroAppsAPIGwy",
-    "MicroAppsAPIGwyProps",
     "MicroAppsCF",
     "MicroAppsCFProps",
     "MicroAppsChildDeployer",
     "MicroAppsChildDeployerProps",
     "MicroAppsEdgeToOrigin",
     "MicroAppsEdgeToOriginProps",
     "MicroAppsProps",
@@ -4513,52 +4100,20 @@
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
     replace_host_header: typing.Optional[builtins.bool] = None,
     root_path_prefix: typing.Optional[builtins.str] = None,
     s3_policy_bypass_aro_as: typing.Optional[typing.Sequence[builtins.str]] = None,
     s3_policy_bypass_principal_ar_ns: typing.Optional[typing.Sequence[builtins.str]] = None,
     s3_strict_bucket_policy: typing.Optional[builtins.bool] = None,
     signing_mode: typing.Optional[builtins.str] = None,
-    table: typing.Optional[_aws_cdk_aws_dynamodb_ceddda9d.ITable] = None,
+    table: typing.Optional[typing.Union[_aws_cdk_aws_dynamodb_ceddda9d.ITable, _aws_cdk_aws_dynamodb_ceddda9d.ITableV2]] = None,
     table_name_for_edge_to_origin: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__34bab1c0e9dae52015406b7b6cb0e2dc511c7bb54c69bd79c4bcf3e233cfe80c(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    asset_name_root: typing.Optional[builtins.str] = None,
-    asset_name_suffix: typing.Optional[builtins.str] = None,
-    cert_origin: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
-    domain_name_edge: typing.Optional[builtins.str] = None,
-    domain_name_origin: typing.Optional[builtins.str] = None,
-    r53_zone: typing.Optional[_aws_cdk_aws_route53_ceddda9d.IHostedZone] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    require_iam_authorization: typing.Optional[builtins.bool] = None,
-    root_path_prefix: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0ac58d864c4aee10362ea8caa1497daadeb0c8daba1b2f6e5094584e36ebb863(
-    *,
-    asset_name_root: typing.Optional[builtins.str] = None,
-    asset_name_suffix: typing.Optional[builtins.str] = None,
-    cert_origin: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
-    domain_name_edge: typing.Optional[builtins.str] = None,
-    domain_name_origin: typing.Optional[builtins.str] = None,
-    r53_zone: typing.Optional[_aws_cdk_aws_route53_ceddda9d.IHostedZone] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    require_iam_authorization: typing.Optional[builtins.bool] = None,
-    root_path_prefix: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
 def _typecheckingstub__08cfd52ef695aa191ba9b6b6d048fcba758e19b43da791b1e65d1f4dd5c47eb6(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     bucket_apps_origin_app: _aws_cdk_aws_cloudfront_origins_ceddda9d.S3Origin,
     bucket_apps_origin_s3: _aws_cdk_aws_cloudfront_origins_ceddda9d.S3Origin,
     asset_name_root: typing.Optional[builtins.str] = None,
@@ -4566,15 +4121,14 @@
     bucket_logs: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
     cert_edge: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
     create_api_path_route: typing.Optional[builtins.bool] = None,
     create_next_data_path_route: typing.Optional[builtins.bool] = None,
     domain_name_edge: typing.Optional[builtins.str] = None,
     domain_name_origin: typing.Optional[builtins.str] = None,
     edge_lambdas: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda, typing.Dict[builtins.str, typing.Any]]]] = None,
-    http_api: typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi] = None,
     origin_shield_region: typing.Optional[builtins.str] = None,
     r53_zone: typing.Optional[_aws_cdk_aws_route53_ceddda9d.IHostedZone] = None,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
     root_path_prefix: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -4611,15 +4165,14 @@
     bucket_logs: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
     cert_edge: typing.Optional[_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate] = None,
     create_api_path_route: typing.Optional[builtins.bool] = None,
     create_next_data_path_route: typing.Optional[builtins.bool] = None,
     domain_name_edge: typing.Optional[builtins.str] = None,
     domain_name_origin: typing.Optional[builtins.str] = None,
     edge_lambdas: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudfront_ceddda9d.EdgeLambda, typing.Dict[builtins.str, typing.Any]]]] = None,
-    http_api: typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi] = None,
     origin_shield_region: typing.Optional[builtins.str] = None,
     r53_zone: typing.Optional[_aws_cdk_aws_route53_ceddda9d.IHostedZone] = None,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
     root_path_prefix: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -4713,15 +4266,15 @@
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
     replace_host_header: typing.Optional[builtins.bool] = None,
     root_path_prefix: typing.Optional[builtins.str] = None,
     s3_policy_bypass_aro_as: typing.Optional[typing.Sequence[builtins.str]] = None,
     s3_policy_bypass_principal_ar_ns: typing.Optional[typing.Sequence[builtins.str]] = None,
     s3_strict_bucket_policy: typing.Optional[builtins.bool] = None,
     signing_mode: typing.Optional[builtins.str] = None,
-    table: typing.Optional[_aws_cdk_aws_dynamodb_ceddda9d.ITable] = None,
+    table: typing.Optional[typing.Union[_aws_cdk_aws_dynamodb_ceddda9d.ITable, _aws_cdk_aws_dynamodb_ceddda9d.ITableV2]] = None,
     table_name_for_edge_to_origin: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__3516e5e32d6ea085c89294517fb9d0d4ff6f76e8cc7ccdd09625d599d54d757a(
     scope: _constructs_77d1e7e8.Construct,
@@ -4759,15 +4312,14 @@
     bucket_apps: _aws_cdk_aws_s3_ceddda9d.IBucket,
     bucket_apps_oai: _aws_cdk_aws_cloudfront_ceddda9d.OriginAccessIdentity,
     bucket_apps_staging: _aws_cdk_aws_s3_ceddda9d.IBucket,
     asset_name_root: typing.Optional[builtins.str] = None,
     asset_name_suffix: typing.Optional[builtins.str] = None,
     deployer_timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     edge_to_origin_role_arn: typing.Optional[typing.Sequence[builtins.str]] = None,
-    http_api: typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi] = None,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
     require_iam_authorization: typing.Optional[builtins.bool] = None,
     root_path_prefix: typing.Optional[builtins.str] = None,
     s3_policy_bypass_aro_as: typing.Optional[typing.Sequence[builtins.str]] = None,
     s3_policy_bypass_principal_ar_ns: typing.Optional[typing.Sequence[builtins.str]] = None,
     s3_strict_bucket_policy: typing.Optional[builtins.bool] = None,
     table: typing.Optional[_aws_cdk_aws_dynamodb_ceddda9d.ITable] = None,
@@ -4781,15 +4333,14 @@
     bucket_apps: _aws_cdk_aws_s3_ceddda9d.IBucket,
     bucket_apps_oai: _aws_cdk_aws_cloudfront_ceddda9d.OriginAccessIdentity,
     bucket_apps_staging: _aws_cdk_aws_s3_ceddda9d.IBucket,
     asset_name_root: typing.Optional[builtins.str] = None,
     asset_name_suffix: typing.Optional[builtins.str] = None,
     deployer_timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     edge_to_origin_role_arn: typing.Optional[typing.Sequence[builtins.str]] = None,
-    http_api: typing.Optional[_aws_cdk_aws_apigatewayv2_alpha_050969fe.HttpApi] = None,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
     require_iam_authorization: typing.Optional[builtins.bool] = None,
     root_path_prefix: typing.Optional[builtins.str] = None,
     s3_policy_bypass_aro_as: typing.Optional[typing.Sequence[builtins.str]] = None,
     s3_policy_bypass_principal_ar_ns: typing.Optional[typing.Sequence[builtins.str]] = None,
     s3_strict_bucket_policy: typing.Optional[builtins.bool] = None,
     table: typing.Optional[_aws_cdk_aws_dynamodb_ceddda9d.ITable] = None,
```

### Comparing `pwrdrvr.microapps.cdk-1.0.0/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO` & `pwrdrvr.microapps.cdk-1.0.1/src/pwrdrvr.microapps.cdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pwrdrvr.microapps.cdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: MicroApps framework, by PwrDrvr LLC, delivered as an AWS CDK construct that provides the DynamoDB, Router service, Deploy service, API Gateway, and CloudFront distribution.
 Home-page: https://github.com/pwrdrvr/microapps-core
 Author: PwrDrvr LLC<harold@pwrdrvr.com>
 License: MIT
 Project-URL: Source, https://github.com/pwrdrvr/microapps-core
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CI](https://github.com/pwrdrvr/microapps-core/actions/workflows/ci.yml/badge.svg)](https://github.com/pwrdrvr/microapps-core/actions/workflows/ci.yml) [![Merge to Main Build](https://github.com/pwrdrvr/microapps-core/actions/workflows/main-build.yml/badge.svg)](https://github.com/pwrdrvr/microapps-core/actions/workflows/main-build.yml) [![Release Packages](https://github.com/pwrdrvr/microapps-core/actions/workflows/release.yml/badge.svg)](https://github.com/pwrdrvr/microapps-core/actions/workflows/release.yml)
 
 # Overview
```

