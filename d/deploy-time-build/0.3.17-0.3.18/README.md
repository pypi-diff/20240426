# Comparing `tmp/deploy-time-build-0.3.17.tar.gz` & `tmp/deploy-time-build-0.3.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploy-time-build-0.3.17.tar", last modified: Mon Apr  1 07:56:59 2024, max compression
+gzip compressed data, was "deploy-time-build-0.3.18.tar", last modified: Fri Apr 26 15:01:57 2024, max compression
```

## Comparing `deploy-time-build-0.3.17.tar` & `deploy-time-build-0.3.18.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:56:59.862811 deploy-time-build-0.3.17/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-01 07:56:49.000000 deploy-time-build-0.3.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 07:56:49.000000 deploy-time-build-0.3.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-01 07:56:59.862811 deploy-time-build-0.3.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-01 07:56:49.000000 deploy-time-build-0.3.17/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-01 07:56:49.000000 deploy-time-build-0.3.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 07:56:59.862811 deploy-time-build-0.3.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-01 07:56:49.000000 deploy-time-build-0.3.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:56:59.858811 deploy-time-build-0.3.17/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:56:59.862811 deploy-time-build-0.3.17/src/deploy_time_build/
--rw-r--r--   0 runner    (1001) docker     (127)    39965 2024-04-01 07:56:49.000000 deploy-time-build-0.3.17/src/deploy_time_build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:56:59.862811 deploy-time-build-0.3.17/src/deploy_time_build/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-01 07:56:49.000000 deploy-time-build-0.3.17/src/deploy_time_build/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   316192 2024-04-01 07:56:49.000000 deploy-time-build-0.3.17/src/deploy_time_build/_jsii/deploy-time-build@0.3.17.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 07:56:49.000000 deploy-time-build-0.3.17/src/deploy_time_build/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:56:59.862811 deploy-time-build-0.3.17/src/deploy_time_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-01 07:56:59.000000 deploy-time-build-0.3.17/src/deploy_time_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-01 07:56:59.000000 deploy-time-build-0.3.17/src/deploy_time_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 07:56:59.000000 deploy-time-build-0.3.17/src/deploy_time_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 07:56:59.000000 deploy-time-build-0.3.17/src/deploy_time_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 07:56:59.000000 deploy-time-build-0.3.17/src/deploy_time_build.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:01:57.912614 deploy-time-build-0.3.18/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-26 15:01:47.000000 deploy-time-build-0.3.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 15:01:47.000000 deploy-time-build-0.3.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-26 15:01:57.912614 deploy-time-build-0.3.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-04-26 15:01:47.000000 deploy-time-build-0.3.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 15:01:47.000000 deploy-time-build-0.3.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:01:57.912614 deploy-time-build-0.3.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-26 15:01:47.000000 deploy-time-build-0.3.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:01:57.912614 deploy-time-build-0.3.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:01:57.912614 deploy-time-build-0.3.18/src/deploy_time_build/
+-rw-r--r--   0 runner    (1001) docker     (127)    62188 2024-04-26 15:01:47.000000 deploy-time-build-0.3.18/src/deploy_time_build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:01:57.912614 deploy-time-build-0.3.18/src/deploy_time_build/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-26 15:01:47.000000 deploy-time-build-0.3.18/src/deploy_time_build/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   334707 2024-04-26 15:01:47.000000 deploy-time-build-0.3.18/src/deploy_time_build/_jsii/deploy-time-build@0.3.18.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:01:47.000000 deploy-time-build-0.3.18/src/deploy_time_build/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:01:57.912614 deploy-time-build-0.3.18/src/deploy_time_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-26 15:01:57.000000 deploy-time-build-0.3.18/src/deploy_time_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-26 15:01:57.000000 deploy-time-build-0.3.18/src/deploy_time_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:01:57.000000 deploy-time-build-0.3.18/src/deploy_time_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 15:01:57.000000 deploy-time-build-0.3.18/src/deploy_time_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 15:01:57.000000 deploy-time-build-0.3.18/src/deploy_time_build.egg-info/top_level.txt
```

### Comparing `deploy-time-build-0.3.17/LICENSE` & `deploy-time-build-0.3.18/LICENSE`

 * *Files identical despite different names*

### Comparing `deploy-time-build-0.3.17/PKG-INFO` & `deploy-time-build-0.3.18/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deploy-time-build
-Version: 0.3.17
+Version: 0.3.18
 Summary: Build during CDK deployment.
 Home-page: https://github.com/tmokmss/deploy-time-build.git
 Author: tmokmss<tomookam@live.jp>
 License: MIT
 Project-URL: Source, https://github.com/tmokmss/deploy-time-build.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -22,14 +22,15 @@
 License-File: LICENSE
 
 # Deploy-time Build
 
 AWS CDK L3 construct that allows you to run a build job for specific purposes. Currently this library supports the following use cases:
 
 * Build web frontend static files
+* Build a container image
 * Build Seekable OCI (SOCI) indices for container images
 
 ## Usage
 
 Install from npm:
 
 ```sh
@@ -142,14 +143,44 @@
           // Set a fixed string as a asset hash to prevent deploying changes.
           // This can be useful for an environment you use to develop locally.
           assetHash: 'frontend_asset',
         },
       ],
 ```
 
+### Build a container image
+
+You can build a container image at deploy time by the following code:
+
+```python
+import { ContainerImageBuild } from 'deploy-time-build;
+
+const image = new ContainerImageBuild(this, 'Build', {
+    directory: 'example-image',
+    buildArgs: { DUMMY_FILE_SIZE_MB: '15' },
+    tag: 'my-image-tag',
+});
+new DockerImageFunction(this, 'Function', {
+    code: image.toLambdaDockerImageCode(),
+});
+const armImage = new ContainerImageBuild(this, 'BuildArm', {
+    directory: 'example-image',
+    platform: Platform.LINUX_ARM64,
+    repository: image.repository,
+    zstdCompression: true,
+});
+new FargateTaskDefinition(this, 'TaskDefinition', {
+    runtimePlatform: { cpuArchitecture: CpuArchitecture.ARM64 }
+}).addContainer('main', {
+    image: armImage.toEcsDockerImageCode(),
+});
+```
+
+The third argument (props) are the super set of DockerImageAsset's properties. You can additionally set `tag` and `repository`.
+
 ### Build SOCI index for a container image
 
 [Seekable OCI (SOCI)](https://aws.amazon.com/about-aws/whats-new/2022/09/introducing-seekable-oci-lazy-loading-container-images/) is a way to help start tasks faster for Amazon ECS tasks on Fargate 1.4.0. You can build and push a SOCI index using the `SociIndexBuild` construct.
 
 ![soci-architecture](imgs/soci-architecture.png)
 
 The following code is an example to use the construct:
```

### Comparing `deploy-time-build-0.3.17/README.md` & `deploy-time-build-0.3.18/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Deploy-time Build
 
 AWS CDK L3 construct that allows you to run a build job for specific purposes. Currently this library supports the following use cases:
 
 * Build web frontend static files
+* Build a container image
 * Build Seekable OCI (SOCI) indices for container images
 
 ## Usage
 
 Install from npm:
 
 ```sh
@@ -119,14 +120,44 @@
           // Set a fixed string as a asset hash to prevent deploying changes.
           // This can be useful for an environment you use to develop locally.
           assetHash: 'frontend_asset',
         },
       ],
 ```
 
+### Build a container image
+
+You can build a container image at deploy time by the following code:
+
+```python
+import { ContainerImageBuild } from 'deploy-time-build;
+
+const image = new ContainerImageBuild(this, 'Build', {
+    directory: 'example-image',
+    buildArgs: { DUMMY_FILE_SIZE_MB: '15' },
+    tag: 'my-image-tag',
+});
+new DockerImageFunction(this, 'Function', {
+    code: image.toLambdaDockerImageCode(),
+});
+const armImage = new ContainerImageBuild(this, 'BuildArm', {
+    directory: 'example-image',
+    platform: Platform.LINUX_ARM64,
+    repository: image.repository,
+    zstdCompression: true,
+});
+new FargateTaskDefinition(this, 'TaskDefinition', {
+    runtimePlatform: { cpuArchitecture: CpuArchitecture.ARM64 }
+}).addContainer('main', {
+    image: armImage.toEcsDockerImageCode(),
+});
+```
+
+The third argument (props) are the super set of DockerImageAsset's properties. You can additionally set `tag` and `repository`.
+
 ### Build SOCI index for a container image
 
 [Seekable OCI (SOCI)](https://aws.amazon.com/about-aws/whats-new/2022/09/introducing-seekable-oci-lazy-loading-container-images/) is a way to help start tasks faster for Amazon ECS tasks on Fargate 1.4.0. You can build and push a SOCI index using the `SociIndexBuild` construct.
 
 ![soci-architecture](imgs/soci-architecture.png)
 
 The following code is an example to use the construct:
```

### Comparing `deploy-time-build-0.3.17/setup.py` & `deploy-time-build-0.3.18/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "deploy-time-build",
-    "version": "0.3.17",
+    "version": "0.3.18",
     "description": "Build during CDK deployment.",
     "license": "MIT",
     "url": "https://github.com/tmokmss/deploy-time-build.git",
     "long_description_content_type": "text/markdown",
     "author": "tmokmss<tomookam@live.jp>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "deploy_time_build",
         "deploy_time_build._jsii"
     ],
     "package_data": {
         "deploy_time_build._jsii": [
-            "deploy-time-build@0.3.17.jsii.tgz"
+            "deploy-time-build@0.3.18.jsii.tgz"
         ],
         "deploy_time_build": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `deploy-time-build-0.3.17/src/deploy_time_build/__init__.py` & `deploy-time-build-0.3.18/src/deploy_time_build/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 '''
 # Deploy-time Build
 
 AWS CDK L3 construct that allows you to run a build job for specific purposes. Currently this library supports the following use cases:
 
 * Build web frontend static files
+* Build a container image
 * Build Seekable OCI (SOCI) indices for container images
 
 ## Usage
 
 Install from npm:
 
 ```sh
@@ -120,14 +121,44 @@
           // Set a fixed string as a asset hash to prevent deploying changes.
           // This can be useful for an environment you use to develop locally.
           assetHash: 'frontend_asset',
         },
       ],
 ```
 
+### Build a container image
+
+You can build a container image at deploy time by the following code:
+
+```python
+import { ContainerImageBuild } from 'deploy-time-build;
+
+const image = new ContainerImageBuild(this, 'Build', {
+    directory: 'example-image',
+    buildArgs: { DUMMY_FILE_SIZE_MB: '15' },
+    tag: 'my-image-tag',
+});
+new DockerImageFunction(this, 'Function', {
+    code: image.toLambdaDockerImageCode(),
+});
+const armImage = new ContainerImageBuild(this, 'BuildArm', {
+    directory: 'example-image',
+    platform: Platform.LINUX_ARM64,
+    repository: image.repository,
+    zstdCompression: true,
+});
+new FargateTaskDefinition(this, 'TaskDefinition', {
+    runtimePlatform: { cpuArchitecture: CpuArchitecture.ARM64 }
+}).addContainer('main', {
+    image: armImage.toEcsDockerImageCode(),
+});
+```
+
+The third argument (props) are the super set of DockerImageAsset's properties. You can additionally set `tag` and `repository`.
+
 ### Build SOCI index for a container image
 
 [Seekable OCI (SOCI)](https://aws.amazon.com/about-aws/whats-new/2022/09/introducing-seekable-oci-lazy-loading-container-images/) is a way to help start tasks faster for Amazon ECS tasks on Fargate 1.4.0. You can build and push a SOCI index using the `SociIndexBuild` construct.
 
 ![soci-architecture](imgs/soci-architecture.png)
 
 The following code is an example to use the construct:
@@ -176,15 +207,17 @@
 
 from ._jsii import *
 
 import aws_cdk as _aws_cdk_ceddda9d
 import aws_cdk.aws_cloudfront as _aws_cdk_aws_cloudfront_ceddda9d
 import aws_cdk.aws_ecr as _aws_cdk_aws_ecr_ceddda9d
 import aws_cdk.aws_ecr_assets as _aws_cdk_aws_ecr_assets_ceddda9d
+import aws_cdk.aws_ecs as _aws_cdk_aws_ecs_ceddda9d
 import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
+import aws_cdk.aws_lambda as _aws_cdk_aws_lambda_ceddda9d
 import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
 import aws_cdk.aws_s3_assets as _aws_cdk_aws_s3_assets_ceddda9d
 import constructs as _constructs_77d1e7e8
 
 
 @jsii.data_type(
     jsii_type="deploy-time-build.AssetConfig",
@@ -400,14 +433,369 @@
     def __repr__(self) -> str:
         return "AssetConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.implements(_aws_cdk_aws_iam_ceddda9d.IGrantable)
+class ContainerImageBuild(
+    _constructs_77d1e7e8.Construct,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="deploy-time-build.ContainerImageBuild",
+):
+    '''Build a container image and push it to an ECR repository on deploy-time.'''
+
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        repository: typing.Optional[_aws_cdk_aws_ecr_ceddda9d.IRepository] = None,
+        tag: typing.Optional[builtins.str] = None,
+        zstd_compression: typing.Optional[builtins.bool] = None,
+        directory: builtins.str,
+        build_args: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        file: typing.Optional[builtins.str] = None,
+        invalidation: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetInvalidationOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        network_mode: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.NetworkMode] = None,
+        platform: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.Platform] = None,
+        target: typing.Optional[builtins.str] = None,
+        extra_hash: typing.Optional[builtins.str] = None,
+        exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
+        follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
+        ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
+    ) -> None:
+        '''
+        :param scope: -
+        :param id: -
+        :param repository: The ECR repository to push the image. Default: create a new ECR repository
+        :param tag: The tag when to push the image. Default: use assetHash as tag
+        :param zstd_compression: Use zstd for compressing a container image. Default: false
+        :param directory: The directory where the Dockerfile is stored. Any directory inside with a name that matches the CDK output folder (cdk.out by default) will be excluded from the asset
+        :param build_args: Build args to pass to the ``docker build`` command. Since Docker build arguments are resolved before deployment, keys and values cannot refer to unresolved tokens (such as ``lambda.functionArn`` or ``queue.queueUrl``). Default: - no build args are passed
+        :param file: Path to the Dockerfile (relative to the directory). Default: 'Dockerfile'
+        :param invalidation: Options to control which parameters are used to invalidate the asset hash. Default: - hash all parameters
+        :param network_mode: Networking mode for the RUN commands during build. Support docker API 1.25+. Default: - no networking mode specified (the default networking mode ``NetworkMode.DEFAULT`` will be used)
+        :param platform: Platform to build for. *Requires Docker Buildx*. Default: - no platform specified (the current machine architecture will be used)
+        :param target: Docker target to build to. Default: - no target
+        :param extra_hash: Extra information to encode into the fingerprint (e.g. build instructions and other inputs). Default: - hash is only based on source content
+        :param exclude: File paths matching the patterns will be excluded. See ``ignoreMode`` to set the matching behavior. Has no effect on Assets bundled using the ``bundling`` property. Default: - nothing is excluded
+        :param follow_symlinks: A strategy for how to handle symlinks. Default: SymlinkFollowMode.NEVER
+        :param ignore_mode: The ignore behavior to use for ``exclude`` patterns. Default: IgnoreMode.GLOB
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c8d9ec5e24290134189760e6d1b810fb7ee3324a2867dc530f78668f65c292d3)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = ContainerImageBuildProps(
+            repository=repository,
+            tag=tag,
+            zstd_compression=zstd_compression,
+            directory=directory,
+            build_args=build_args,
+            file=file,
+            invalidation=invalidation,
+            network_mode=network_mode,
+            platform=platform,
+            target=target,
+            extra_hash=extra_hash,
+            exclude=exclude,
+            follow_symlinks=follow_symlinks,
+            ignore_mode=ignore_mode,
+        )
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+    @jsii.member(jsii_name="toEcsDockerImageCode")
+    def to_ecs_docker_image_code(self) -> _aws_cdk_aws_ecs_ceddda9d.EcrImage:
+        '''Get the instance of {@link ContainerImage} for an ECS task definition.'''
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.EcrImage, jsii.invoke(self, "toEcsDockerImageCode", []))
+
+    @jsii.member(jsii_name="toLambdaDockerImageCode")
+    def to_lambda_docker_image_code(
+        self,
+    ) -> _aws_cdk_aws_lambda_ceddda9d.DockerImageCode:
+        '''Get the instance of {@link DockerImageCode} for a Lambda function image.'''
+        return typing.cast(_aws_cdk_aws_lambda_ceddda9d.DockerImageCode, jsii.invoke(self, "toLambdaDockerImageCode", []))
+
+    @builtins.property
+    @jsii.member(jsii_name="grantPrincipal")
+    def grant_principal(self) -> _aws_cdk_aws_iam_ceddda9d.IPrincipal:
+        '''The principal to grant permissions to.'''
+        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IPrincipal, jsii.get(self, "grantPrincipal"))
+
+    @builtins.property
+    @jsii.member(jsii_name="imageTag")
+    def image_tag(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "imageTag"))
+
+    @builtins.property
+    @jsii.member(jsii_name="repository")
+    def repository(self) -> _aws_cdk_aws_ecr_ceddda9d.IRepository:
+        return typing.cast(_aws_cdk_aws_ecr_ceddda9d.IRepository, jsii.get(self, "repository"))
+
+
+@jsii.data_type(
+    jsii_type="deploy-time-build.ContainerImageBuildProps",
+    jsii_struct_bases=[_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetProps],
+    name_mapping={
+        "exclude": "exclude",
+        "follow_symlinks": "followSymlinks",
+        "ignore_mode": "ignoreMode",
+        "extra_hash": "extraHash",
+        "build_args": "buildArgs",
+        "file": "file",
+        "invalidation": "invalidation",
+        "network_mode": "networkMode",
+        "platform": "platform",
+        "target": "target",
+        "directory": "directory",
+        "repository": "repository",
+        "tag": "tag",
+        "zstd_compression": "zstdCompression",
+    },
+)
+class ContainerImageBuildProps(_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetProps):
+    def __init__(
+        self,
+        *,
+        exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
+        follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
+        ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
+        extra_hash: typing.Optional[builtins.str] = None,
+        build_args: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        file: typing.Optional[builtins.str] = None,
+        invalidation: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetInvalidationOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        network_mode: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.NetworkMode] = None,
+        platform: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.Platform] = None,
+        target: typing.Optional[builtins.str] = None,
+        directory: builtins.str,
+        repository: typing.Optional[_aws_cdk_aws_ecr_ceddda9d.IRepository] = None,
+        tag: typing.Optional[builtins.str] = None,
+        zstd_compression: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''
+        :param exclude: File paths matching the patterns will be excluded. See ``ignoreMode`` to set the matching behavior. Has no effect on Assets bundled using the ``bundling`` property. Default: - nothing is excluded
+        :param follow_symlinks: A strategy for how to handle symlinks. Default: SymlinkFollowMode.NEVER
+        :param ignore_mode: The ignore behavior to use for ``exclude`` patterns. Default: IgnoreMode.GLOB
+        :param extra_hash: Extra information to encode into the fingerprint (e.g. build instructions and other inputs). Default: - hash is only based on source content
+        :param build_args: Build args to pass to the ``docker build`` command. Since Docker build arguments are resolved before deployment, keys and values cannot refer to unresolved tokens (such as ``lambda.functionArn`` or ``queue.queueUrl``). Default: - no build args are passed
+        :param file: Path to the Dockerfile (relative to the directory). Default: 'Dockerfile'
+        :param invalidation: Options to control which parameters are used to invalidate the asset hash. Default: - hash all parameters
+        :param network_mode: Networking mode for the RUN commands during build. Support docker API 1.25+. Default: - no networking mode specified (the default networking mode ``NetworkMode.DEFAULT`` will be used)
+        :param platform: Platform to build for. *Requires Docker Buildx*. Default: - no platform specified (the current machine architecture will be used)
+        :param target: Docker target to build to. Default: - no target
+        :param directory: The directory where the Dockerfile is stored. Any directory inside with a name that matches the CDK output folder (cdk.out by default) will be excluded from the asset
+        :param repository: The ECR repository to push the image. Default: create a new ECR repository
+        :param tag: The tag when to push the image. Default: use assetHash as tag
+        :param zstd_compression: Use zstd for compressing a container image. Default: false
+        '''
+        if isinstance(invalidation, dict):
+            invalidation = _aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetInvalidationOptions(**invalidation)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__04b8bd65bfca7b137073a2a9bdedee6b10ff714618c0018ffcc6ba5061c7bddc)
+            check_type(argname="argument exclude", value=exclude, expected_type=type_hints["exclude"])
+            check_type(argname="argument follow_symlinks", value=follow_symlinks, expected_type=type_hints["follow_symlinks"])
+            check_type(argname="argument ignore_mode", value=ignore_mode, expected_type=type_hints["ignore_mode"])
+            check_type(argname="argument extra_hash", value=extra_hash, expected_type=type_hints["extra_hash"])
+            check_type(argname="argument build_args", value=build_args, expected_type=type_hints["build_args"])
+            check_type(argname="argument file", value=file, expected_type=type_hints["file"])
+            check_type(argname="argument invalidation", value=invalidation, expected_type=type_hints["invalidation"])
+            check_type(argname="argument network_mode", value=network_mode, expected_type=type_hints["network_mode"])
+            check_type(argname="argument platform", value=platform, expected_type=type_hints["platform"])
+            check_type(argname="argument target", value=target, expected_type=type_hints["target"])
+            check_type(argname="argument directory", value=directory, expected_type=type_hints["directory"])
+            check_type(argname="argument repository", value=repository, expected_type=type_hints["repository"])
+            check_type(argname="argument tag", value=tag, expected_type=type_hints["tag"])
+            check_type(argname="argument zstd_compression", value=zstd_compression, expected_type=type_hints["zstd_compression"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "directory": directory,
+        }
+        if exclude is not None:
+            self._values["exclude"] = exclude
+        if follow_symlinks is not None:
+            self._values["follow_symlinks"] = follow_symlinks
+        if ignore_mode is not None:
+            self._values["ignore_mode"] = ignore_mode
+        if extra_hash is not None:
+            self._values["extra_hash"] = extra_hash
+        if build_args is not None:
+            self._values["build_args"] = build_args
+        if file is not None:
+            self._values["file"] = file
+        if invalidation is not None:
+            self._values["invalidation"] = invalidation
+        if network_mode is not None:
+            self._values["network_mode"] = network_mode
+        if platform is not None:
+            self._values["platform"] = platform
+        if target is not None:
+            self._values["target"] = target
+        if repository is not None:
+            self._values["repository"] = repository
+        if tag is not None:
+            self._values["tag"] = tag
+        if zstd_compression is not None:
+            self._values["zstd_compression"] = zstd_compression
+
+    @builtins.property
+    def exclude(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''File paths matching the patterns will be excluded.
+
+        See ``ignoreMode`` to set the matching behavior.
+        Has no effect on Assets bundled using the ``bundling`` property.
+
+        :default: - nothing is excluded
+        '''
+        result = self._values.get("exclude")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
+    def follow_symlinks(self) -> typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode]:
+        '''A strategy for how to handle symlinks.
+
+        :default: SymlinkFollowMode.NEVER
+        '''
+        result = self._values.get("follow_symlinks")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode], result)
+
+    @builtins.property
+    def ignore_mode(self) -> typing.Optional[_aws_cdk_ceddda9d.IgnoreMode]:
+        '''The ignore behavior to use for ``exclude`` patterns.
+
+        :default: IgnoreMode.GLOB
+        '''
+        result = self._values.get("ignore_mode")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.IgnoreMode], result)
+
+    @builtins.property
+    def extra_hash(self) -> typing.Optional[builtins.str]:
+        '''Extra information to encode into the fingerprint (e.g. build instructions and other inputs).
+
+        :default: - hash is only based on source content
+        '''
+        result = self._values.get("extra_hash")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def build_args(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        '''Build args to pass to the ``docker build`` command.
+
+        Since Docker build arguments are resolved before deployment, keys and
+        values cannot refer to unresolved tokens (such as ``lambda.functionArn`` or
+        ``queue.queueUrl``).
+
+        :default: - no build args are passed
+        '''
+        result = self._values.get("build_args")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    @builtins.property
+    def file(self) -> typing.Optional[builtins.str]:
+        '''Path to the Dockerfile (relative to the directory).
+
+        :default: 'Dockerfile'
+        '''
+        result = self._values.get("file")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def invalidation(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetInvalidationOptions]:
+        '''Options to control which parameters are used to invalidate the asset hash.
+
+        :default: - hash all parameters
+        '''
+        result = self._values.get("invalidation")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetInvalidationOptions], result)
+
+    @builtins.property
+    def network_mode(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.NetworkMode]:
+        '''Networking mode for the RUN commands during build.
+
+        Support docker API 1.25+.
+
+        :default: - no networking mode specified (the default networking mode ``NetworkMode.DEFAULT`` will be used)
+        '''
+        result = self._values.get("network_mode")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.NetworkMode], result)
+
+    @builtins.property
+    def platform(self) -> typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.Platform]:
+        '''Platform to build for.
+
+        *Requires Docker Buildx*.
+
+        :default: - no platform specified (the current machine architecture will be used)
+        '''
+        result = self._values.get("platform")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.Platform], result)
+
+    @builtins.property
+    def target(self) -> typing.Optional[builtins.str]:
+        '''Docker target to build to.
+
+        :default: - no target
+        '''
+        result = self._values.get("target")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def directory(self) -> builtins.str:
+        '''The directory where the Dockerfile is stored.
+
+        Any directory inside with a name that matches the CDK output folder (cdk.out by default) will be excluded from the asset
+        '''
+        result = self._values.get("directory")
+        assert result is not None, "Required property 'directory' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def repository(self) -> typing.Optional[_aws_cdk_aws_ecr_ceddda9d.IRepository]:
+        '''The ECR repository to push the image.
+
+        :default: create a new ECR repository
+        '''
+        result = self._values.get("repository")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecr_ceddda9d.IRepository], result)
+
+    @builtins.property
+    def tag(self) -> typing.Optional[builtins.str]:
+        '''The tag when to push the image.
+
+        :default: use assetHash as tag
+        '''
+        result = self._values.get("tag")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def zstd_compression(self) -> typing.Optional[builtins.bool]:
+        '''Use zstd for compressing a container image.
+
+        :default: false
+        '''
+        result = self._values.get("zstd_compression")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "ContainerImageBuildProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.implements(_aws_cdk_aws_iam_ceddda9d.IGrantable)
 class NodejsBuild(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="deploy-time-build.NodejsBuild",
 ):
     '''Build Node.js app and optionally publish the artifact to an S3 bucket.'''
 
@@ -738,14 +1126,16 @@
         return "SociIndexBuildProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
     "AssetConfig",
+    "ContainerImageBuild",
+    "ContainerImageBuildProps",
     "NodejsBuild",
     "NodejsBuildProps",
     "SociIndexBuild",
     "SociIndexBuildProps",
 ]
 
 publication.publish()
@@ -762,14 +1152,56 @@
     path: builtins.str,
     commands: typing.Optional[typing.Sequence[builtins.str]] = None,
     extract_path: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__c8d9ec5e24290134189760e6d1b810fb7ee3324a2867dc530f78668f65c292d3(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    repository: typing.Optional[_aws_cdk_aws_ecr_ceddda9d.IRepository] = None,
+    tag: typing.Optional[builtins.str] = None,
+    zstd_compression: typing.Optional[builtins.bool] = None,
+    directory: builtins.str,
+    build_args: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    file: typing.Optional[builtins.str] = None,
+    invalidation: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetInvalidationOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    network_mode: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.NetworkMode] = None,
+    platform: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.Platform] = None,
+    target: typing.Optional[builtins.str] = None,
+    extra_hash: typing.Optional[builtins.str] = None,
+    exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
+    follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
+    ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__04b8bd65bfca7b137073a2a9bdedee6b10ff714618c0018ffcc6ba5061c7bddc(
+    *,
+    exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
+    follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
+    ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
+    extra_hash: typing.Optional[builtins.str] = None,
+    build_args: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    file: typing.Optional[builtins.str] = None,
+    invalidation: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetInvalidationOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    network_mode: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.NetworkMode] = None,
+    platform: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.Platform] = None,
+    target: typing.Optional[builtins.str] = None,
+    directory: builtins.str,
+    repository: typing.Optional[_aws_cdk_aws_ecr_ceddda9d.IRepository] = None,
+    tag: typing.Optional[builtins.str] = None,
+    zstd_compression: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__3c71280e3aba0c9512a180cd9b287eb9fa61158e0b247676de51e6b48a0b58d3(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     assets: typing.Sequence[typing.Union[AssetConfig, typing.Dict[builtins.str, typing.Any]]],
     destination_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
     output_source_directory: builtins.str,
```

### Comparing `deploy-time-build-0.3.17/src/deploy_time_build.egg-info/PKG-INFO` & `deploy-time-build-0.3.18/src/deploy_time_build.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deploy-time-build
-Version: 0.3.17
+Version: 0.3.18
 Summary: Build during CDK deployment.
 Home-page: https://github.com/tmokmss/deploy-time-build.git
 Author: tmokmss<tomookam@live.jp>
 License: MIT
 Project-URL: Source, https://github.com/tmokmss/deploy-time-build.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -22,14 +22,15 @@
 License-File: LICENSE
 
 # Deploy-time Build
 
 AWS CDK L3 construct that allows you to run a build job for specific purposes. Currently this library supports the following use cases:
 
 * Build web frontend static files
+* Build a container image
 * Build Seekable OCI (SOCI) indices for container images
 
 ## Usage
 
 Install from npm:
 
 ```sh
@@ -142,14 +143,44 @@
           // Set a fixed string as a asset hash to prevent deploying changes.
           // This can be useful for an environment you use to develop locally.
           assetHash: 'frontend_asset',
         },
       ],
 ```
 
+### Build a container image
+
+You can build a container image at deploy time by the following code:
+
+```python
+import { ContainerImageBuild } from 'deploy-time-build;
+
+const image = new ContainerImageBuild(this, 'Build', {
+    directory: 'example-image',
+    buildArgs: { DUMMY_FILE_SIZE_MB: '15' },
+    tag: 'my-image-tag',
+});
+new DockerImageFunction(this, 'Function', {
+    code: image.toLambdaDockerImageCode(),
+});
+const armImage = new ContainerImageBuild(this, 'BuildArm', {
+    directory: 'example-image',
+    platform: Platform.LINUX_ARM64,
+    repository: image.repository,
+    zstdCompression: true,
+});
+new FargateTaskDefinition(this, 'TaskDefinition', {
+    runtimePlatform: { cpuArchitecture: CpuArchitecture.ARM64 }
+}).addContainer('main', {
+    image: armImage.toEcsDockerImageCode(),
+});
+```
+
+The third argument (props) are the super set of DockerImageAsset's properties. You can additionally set `tag` and `repository`.
+
 ### Build SOCI index for a container image
 
 [Seekable OCI (SOCI)](https://aws.amazon.com/about-aws/whats-new/2022/09/introducing-seekable-oci-lazy-loading-container-images/) is a way to help start tasks faster for Amazon ECS tasks on Fargate 1.4.0. You can build and push a SOCI index using the `SociIndexBuild` construct.
 
 ![soci-architecture](imgs/soci-architecture.png)
 
 The following code is an example to use the construct:
```

