# Comparing `tmp/mypy-boto3-codepipeline-1.34.43.tar.gz` & `tmp/mypy_boto3_codepipeline-1.34.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codepipeline-1.34.43.tar", last modified: Thu Feb 15 20:47:28 2024, max compression
+gzip compressed data, was "mypy_boto3_codepipeline-1.34.93.tar", last modified: Fri Apr 26 19:32:21 2024, max compression
```

## Comparing `mypy-boto3-codepipeline-1.34.43.tar` & `mypy_boto3_codepipeline-1.34.93.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:28.445500 mypy-boto3-codepipeline-1.34.43/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-15 20:46:47.000000 mypy-boto3-codepipeline-1.34.43/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13699 2024-02-15 20:47:28.445500 mypy-boto3-codepipeline-1.34.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-02-15 20:46:47.000000 mypy-boto3-codepipeline-1.34.43/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:28.441500 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-02-15 20:46:47.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-02-15 20:46:47.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-15 20:46:47.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32749 2024-02-15 20:46:48.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    32746 2024-02-15 20:46:47.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-02-15 20:46:48.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-02-15 20:46:48.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-02-15 20:46:48.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-02-15 20:46:48.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 20:46:47.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    43413 2024-02-15 20:46:49.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43413 2024-02-15 20:46:48.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-15 20:46:47.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:28.445500 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13699 2024-02-15 20:47:28.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-15 20:47:28.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 20:47:28.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 20:47:28.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-15 20:47:28.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-15 20:47:28.000000 mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 20:47:28.445500 mypy-boto3-codepipeline-1.34.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-02-15 20:46:47.000000 mypy-boto3-codepipeline-1.34.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:21.835533 mypy_boto3_codepipeline-1.34.93/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13699 2024-04-26 19:32:21.835533 mypy_boto3_codepipeline-1.34.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:21.835533 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33578 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    52182 2024-04-26 19:31:53.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52182 2024-04-26 19:31:53.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:21.835533 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13699 2024-04-26 19:32:21.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-26 19:32:21.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:21.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:21.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 19:32:21.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 19:32:21.000000 mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:32:21.835533 mypy_boto3_codepipeline-1.34.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-26 19:31:52.000000 mypy_boto3_codepipeline-1.34.93/setup.py
```

### Comparing `mypy-boto3-codepipeline-1.34.43/LICENSE` & `mypy_boto3_codepipeline-1.34.93/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.34.43/PKG-INFO` & `mypy_boto3_codepipeline-1.34.93/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codepipeline
-Version: 1.34.43
-Summary: Type annotations for boto3.CodePipeline 1.34.43 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.93
+Summary: Type annotations for boto3.CodePipeline 1.34.93 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-codepipeline-1.34.43/README.md` & `mypy_boto3_codepipeline-1.34.93/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/__init__.py` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/__init__.pyi` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/__main__.py` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodePipeline 1.34.43\n"
-        "Version:         1.34.43\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.CodePipeline 1.34.93\n"
+        "Version:         1.34.93\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.43")
+    print("1.34.93")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/client.py` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     ListWebhooksPaginator,
 )
 from .type_defs import (
     AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionExecutionFilterTypeDef,
-    ActionRevisionTypeDef,
-    ActionTypeDeclarationTypeDef,
+    ActionRevisionUnionTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     ActionTypeIdTypeDef,
     ActionTypeSettingsTypeDef,
     ApprovalResultTypeDef,
     ArtifactDetailsTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     CreatePipelineOutputTypeDef,
     CurrentRevisionTypeDef,
@@ -58,28 +58,30 @@
     GetThirdPartyJobDetailsOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListPipelinesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWebhooksOutputTypeDef,
-    PipelineDeclarationTypeDef,
+    PipelineDeclarationUnionTypeDef,
+    PipelineExecutionFilterTypeDef,
     PipelineVariableTypeDef,
     PollForJobsOutputTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     PutActionRevisionOutputTypeDef,
     PutApprovalResultOutputTypeDef,
     PutWebhookOutputTypeDef,
     RetryStageExecutionOutputTypeDef,
+    RollbackStageOutputTypeDef,
     SourceRevisionOverrideTypeDef,
     StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionOutputTypeDef,
     TagTypeDef,
     UpdatePipelineOutputTypeDef,
-    WebhookDefinitionTypeDef,
+    WebhookDefinitionUnionTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -120,22 +122,24 @@
     InvalidWebhookFilterPatternException: Type[BotocoreClientError]
     JobNotFoundException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotLatestPipelineExecutionException: Type[BotocoreClientError]
     OutputVariablesSizeExceededException: Type[BotocoreClientError]
     PipelineExecutionNotFoundException: Type[BotocoreClientError]
     PipelineExecutionNotStoppableException: Type[BotocoreClientError]
+    PipelineExecutionOutdatedException: Type[BotocoreClientError]
     PipelineNameInUseException: Type[BotocoreClientError]
     PipelineNotFoundException: Type[BotocoreClientError]
     PipelineVersionNotFoundException: Type[BotocoreClientError]
     RequestFailedException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     StageNotFoundException: Type[BotocoreClientError]
     StageNotRetryableException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
+    UnableToRollbackStageException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
     WebhookNotFoundException: Type[BotocoreClientError]
 
 
 class CodePipelineClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client)
@@ -207,15 +211,15 @@
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#create_custom_action_type)
         """
 
     def create_pipeline(
-        self, *, pipeline: PipelineDeclarationTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, pipeline: PipelineDeclarationUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineOutputTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#create_pipeline)
         """
@@ -381,15 +385,20 @@
         Gets a summary of all CodePipeline action types associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_action_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#list_action_types)
         """
 
     def list_pipeline_executions(
-        self, *, pipelineName: str, maxResults: int = ..., nextToken: str = ...
+        self,
+        *,
+        pipelineName: str,
+        maxResults: int = ...,
+        filter: PipelineExecutionFilterTypeDef = ...,
+        nextToken: str = ...,
     ) -> ListPipelineExecutionsOutputTypeDef:
         """
         Gets a summary of the most recent executions for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_pipeline_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#list_pipeline_executions)
         """
@@ -451,15 +460,15 @@
 
     def put_action_revision(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
-        actionRevision: ActionRevisionTypeDef,
+        actionRevision: ActionRevisionUnionTypeDef,
     ) -> PutActionRevisionOutputTypeDef:
         """
         Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_action_revision)
         """
@@ -533,15 +542,15 @@
         worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_success_result)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_third_party_job_success_result)
         """
 
     def put_webhook(
-        self, *, webhook: WebhookDefinitionTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, webhook: WebhookDefinitionUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> PutWebhookOutputTypeDef:
         """
         Defines a webhook and returns a unique webhook URL generated by CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_webhook)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_webhook)
         """
@@ -569,14 +578,24 @@
         from the
         beginning.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.retry_stage_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#retry_stage_execution)
         """
 
+    def rollback_stage(
+        self, *, pipelineName: str, stageName: str, targetPipelineExecutionId: str
+    ) -> RollbackStageOutputTypeDef:
+        """
+        Rolls back a stage execution.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.rollback_stage)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#rollback_stage)
+        """
+
     def start_pipeline_execution(
         self,
         *,
         name: str,
         variables: Sequence[PipelineVariableTypeDef] = ...,
         clientRequestToken: str = ...,
         sourceRevisions: Sequence[SourceRevisionOverrideTypeDef] = ...,
@@ -611,27 +630,27 @@
         Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#untag_resource)
         """
 
     def update_action_type(
-        self, *, actionType: ActionTypeDeclarationTypeDef
+        self, *, actionType: ActionTypeDeclarationUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an action type that was created with any supported integration model,
         where the action type is to be used by customers of the action type
         provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_action_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#update_action_type)
         """
 
     def update_pipeline(
-        self, *, pipeline: PipelineDeclarationTypeDef
+        self, *, pipeline: PipelineDeclarationUnionTypeDef
     ) -> UpdatePipelineOutputTypeDef:
         """
         Updates a specified pipeline with edits or changes to its structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#update_pipeline)
         """
```

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/client.pyi` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     ListWebhooksPaginator,
 )
 from .type_defs import (
     AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionExecutionFilterTypeDef,
-    ActionRevisionTypeDef,
-    ActionTypeDeclarationTypeDef,
+    ActionRevisionUnionTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     ActionTypeIdTypeDef,
     ActionTypeSettingsTypeDef,
     ApprovalResultTypeDef,
     ArtifactDetailsTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     CreatePipelineOutputTypeDef,
     CurrentRevisionTypeDef,
@@ -58,28 +58,30 @@
     GetThirdPartyJobDetailsOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListPipelinesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWebhooksOutputTypeDef,
-    PipelineDeclarationTypeDef,
+    PipelineDeclarationUnionTypeDef,
+    PipelineExecutionFilterTypeDef,
     PipelineVariableTypeDef,
     PollForJobsOutputTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     PutActionRevisionOutputTypeDef,
     PutApprovalResultOutputTypeDef,
     PutWebhookOutputTypeDef,
     RetryStageExecutionOutputTypeDef,
+    RollbackStageOutputTypeDef,
     SourceRevisionOverrideTypeDef,
     StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionOutputTypeDef,
     TagTypeDef,
     UpdatePipelineOutputTypeDef,
-    WebhookDefinitionTypeDef,
+    WebhookDefinitionUnionTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -118,22 +120,24 @@
     InvalidWebhookFilterPatternException: Type[BotocoreClientError]
     JobNotFoundException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotLatestPipelineExecutionException: Type[BotocoreClientError]
     OutputVariablesSizeExceededException: Type[BotocoreClientError]
     PipelineExecutionNotFoundException: Type[BotocoreClientError]
     PipelineExecutionNotStoppableException: Type[BotocoreClientError]
+    PipelineExecutionOutdatedException: Type[BotocoreClientError]
     PipelineNameInUseException: Type[BotocoreClientError]
     PipelineNotFoundException: Type[BotocoreClientError]
     PipelineVersionNotFoundException: Type[BotocoreClientError]
     RequestFailedException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     StageNotFoundException: Type[BotocoreClientError]
     StageNotRetryableException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
+    UnableToRollbackStageException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
     WebhookNotFoundException: Type[BotocoreClientError]
 
 class CodePipelineClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/)
@@ -204,15 +208,15 @@
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#create_custom_action_type)
         """
 
     def create_pipeline(
-        self, *, pipeline: PipelineDeclarationTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, pipeline: PipelineDeclarationUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineOutputTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#create_pipeline)
         """
@@ -378,15 +382,20 @@
         Gets a summary of all CodePipeline action types associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_action_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#list_action_types)
         """
 
     def list_pipeline_executions(
-        self, *, pipelineName: str, maxResults: int = ..., nextToken: str = ...
+        self,
+        *,
+        pipelineName: str,
+        maxResults: int = ...,
+        filter: PipelineExecutionFilterTypeDef = ...,
+        nextToken: str = ...,
     ) -> ListPipelineExecutionsOutputTypeDef:
         """
         Gets a summary of the most recent executions for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_pipeline_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#list_pipeline_executions)
         """
@@ -448,15 +457,15 @@
 
     def put_action_revision(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
-        actionRevision: ActionRevisionTypeDef,
+        actionRevision: ActionRevisionUnionTypeDef,
     ) -> PutActionRevisionOutputTypeDef:
         """
         Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_action_revision)
         """
@@ -530,15 +539,15 @@
         worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_success_result)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_third_party_job_success_result)
         """
 
     def put_webhook(
-        self, *, webhook: WebhookDefinitionTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, webhook: WebhookDefinitionUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> PutWebhookOutputTypeDef:
         """
         Defines a webhook and returns a unique webhook URL generated by CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_webhook)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_webhook)
         """
@@ -566,14 +575,24 @@
         from the
         beginning.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.retry_stage_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#retry_stage_execution)
         """
 
+    def rollback_stage(
+        self, *, pipelineName: str, stageName: str, targetPipelineExecutionId: str
+    ) -> RollbackStageOutputTypeDef:
+        """
+        Rolls back a stage execution.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.rollback_stage)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#rollback_stage)
+        """
+
     def start_pipeline_execution(
         self,
         *,
         name: str,
         variables: Sequence[PipelineVariableTypeDef] = ...,
         clientRequestToken: str = ...,
         sourceRevisions: Sequence[SourceRevisionOverrideTypeDef] = ...,
@@ -608,27 +627,27 @@
         Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#untag_resource)
         """
 
     def update_action_type(
-        self, *, actionType: ActionTypeDeclarationTypeDef
+        self, *, actionType: ActionTypeDeclarationUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an action type that was created with any supported integration model,
         where the action type is to be used by customers of the action type
         provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_action_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#update_action_type)
         """
 
     def update_pipeline(
-        self, *, pipeline: PipelineDeclarationTypeDef
+        self, *, pipeline: PipelineDeclarationUnionTypeDef
     ) -> UpdatePipelineOutputTypeDef:
         """
         Updates a specified pipeline with edits or changes to its structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#update_pipeline)
         """
```

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/literals.py` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,29 @@
     "ActionOwnerType",
     "ApprovalStatusType",
     "ArtifactLocationTypeType",
     "ArtifactStoreTypeType",
     "BlockerTypeType",
     "EncryptionKeyTypeType",
     "ExecutionModeType",
+    "ExecutionTypeType",
     "ExecutorTypeType",
     "FailureTypeType",
     "GitPullRequestEventTypeType",
     "JobStatusType",
     "ListActionExecutionsPaginatorName",
     "ListActionTypesPaginatorName",
     "ListPipelineExecutionsPaginatorName",
     "ListPipelinesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "ListWebhooksPaginatorName",
     "PipelineExecutionStatusType",
     "PipelineTriggerProviderTypeType",
     "PipelineTypeType",
+    "ResultType",
     "SourceRevisionTypeType",
     "StageExecutionStatusType",
     "StageRetryModeType",
     "StageTransitionTypeType",
     "StartTimeRangeType",
     "TriggerTypeType",
     "WebhookAuthenticationTypeType",
@@ -63,14 +65,15 @@
 ActionOwnerType = Literal["AWS", "Custom", "ThirdParty"]
 ApprovalStatusType = Literal["Approved", "Rejected"]
 ArtifactLocationTypeType = Literal["S3"]
 ArtifactStoreTypeType = Literal["S3"]
 BlockerTypeType = Literal["Schedule"]
 EncryptionKeyTypeType = Literal["KMS"]
 ExecutionModeType = Literal["PARALLEL", "QUEUED", "SUPERSEDED"]
+ExecutionTypeType = Literal["ROLLBACK", "STANDARD"]
 ExecutorTypeType = Literal["JobWorker", "Lambda"]
 FailureTypeType = Literal[
     "ConfigurationError",
     "JobFailed",
     "PermissionError",
     "RevisionOutOfSync",
     "RevisionUnavailable",
@@ -87,24 +90,27 @@
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 ListWebhooksPaginatorName = Literal["list_webhooks"]
 PipelineExecutionStatusType = Literal[
     "Cancelled", "Failed", "InProgress", "Stopped", "Stopping", "Succeeded", "Superseded"
 ]
 PipelineTriggerProviderTypeType = Literal["CodeStarSourceConnection"]
 PipelineTypeType = Literal["V1", "V2"]
+ResultType = Literal["ROLLBACK"]
 SourceRevisionTypeType = Literal["COMMIT_ID", "IMAGE_DIGEST", "S3_OBJECT_VERSION_ID"]
 StageExecutionStatusType = Literal[
     "Cancelled", "Failed", "InProgress", "Stopped", "Stopping", "Succeeded"
 ]
 StageRetryModeType = Literal["ALL_ACTIONS", "FAILED_ACTIONS"]
 StageTransitionTypeType = Literal["Inbound", "Outbound"]
 StartTimeRangeType = Literal["All", "Latest"]
 TriggerTypeType = Literal[
+    "AutomatedRollback",
     "CloudWatchEvent",
     "CreatePipeline",
+    "ManualRollback",
     "PollForSourceChanges",
     "PutActionRevision",
     "StartPipelineExecution",
     "Webhook",
     "WebhookV2",
 ]
 WebhookAuthenticationTypeType = Literal["GITHUB_HMAC", "IP", "UNAUTHENTICATED"]
@@ -150,14 +156,15 @@
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
@@ -175,14 +182,15 @@
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
@@ -195,24 +203,26 @@
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
@@ -273,15 +283,14 @@
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
@@ -410,14 +419,15 @@
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
@@ -461,14 +471,15 @@
     "sts",
     "supplychain",
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

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/literals.pyi` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,29 @@
     "ActionOwnerType",
     "ApprovalStatusType",
     "ArtifactLocationTypeType",
     "ArtifactStoreTypeType",
     "BlockerTypeType",
     "EncryptionKeyTypeType",
     "ExecutionModeType",
+    "ExecutionTypeType",
     "ExecutorTypeType",
     "FailureTypeType",
     "GitPullRequestEventTypeType",
     "JobStatusType",
     "ListActionExecutionsPaginatorName",
     "ListActionTypesPaginatorName",
     "ListPipelineExecutionsPaginatorName",
     "ListPipelinesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "ListWebhooksPaginatorName",
     "PipelineExecutionStatusType",
     "PipelineTriggerProviderTypeType",
     "PipelineTypeType",
+    "ResultType",
     "SourceRevisionTypeType",
     "StageExecutionStatusType",
     "StageRetryModeType",
     "StageTransitionTypeType",
     "StartTimeRangeType",
     "TriggerTypeType",
     "WebhookAuthenticationTypeType",
@@ -63,14 +65,15 @@
 ActionOwnerType = Literal["AWS", "Custom", "ThirdParty"]
 ApprovalStatusType = Literal["Approved", "Rejected"]
 ArtifactLocationTypeType = Literal["S3"]
 ArtifactStoreTypeType = Literal["S3"]
 BlockerTypeType = Literal["Schedule"]
 EncryptionKeyTypeType = Literal["KMS"]
 ExecutionModeType = Literal["PARALLEL", "QUEUED", "SUPERSEDED"]
+ExecutionTypeType = Literal["ROLLBACK", "STANDARD"]
 ExecutorTypeType = Literal["JobWorker", "Lambda"]
 FailureTypeType = Literal[
     "ConfigurationError",
     "JobFailed",
     "PermissionError",
     "RevisionOutOfSync",
     "RevisionUnavailable",
@@ -87,24 +90,27 @@
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 ListWebhooksPaginatorName = Literal["list_webhooks"]
 PipelineExecutionStatusType = Literal[
     "Cancelled", "Failed", "InProgress", "Stopped", "Stopping", "Succeeded", "Superseded"
 ]
 PipelineTriggerProviderTypeType = Literal["CodeStarSourceConnection"]
 PipelineTypeType = Literal["V1", "V2"]
+ResultType = Literal["ROLLBACK"]
 SourceRevisionTypeType = Literal["COMMIT_ID", "IMAGE_DIGEST", "S3_OBJECT_VERSION_ID"]
 StageExecutionStatusType = Literal[
     "Cancelled", "Failed", "InProgress", "Stopped", "Stopping", "Succeeded"
 ]
 StageRetryModeType = Literal["ALL_ACTIONS", "FAILED_ACTIONS"]
 StageTransitionTypeType = Literal["Inbound", "Outbound"]
 StartTimeRangeType = Literal["All", "Latest"]
 TriggerTypeType = Literal[
+    "AutomatedRollback",
     "CloudWatchEvent",
     "CreatePipeline",
+    "ManualRollback",
     "PollForSourceChanges",
     "PutActionRevision",
     "StartPipelineExecution",
     "Webhook",
     "WebhookV2",
 ]
 WebhookAuthenticationTypeType = Literal["GITHUB_HMAC", "IP", "UNAUTHENTICATED"]
@@ -150,14 +156,15 @@
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
@@ -175,14 +182,15 @@
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
@@ -195,24 +203,26 @@
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
@@ -273,15 +283,14 @@
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
@@ -410,14 +419,15 @@
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
@@ -461,14 +471,15 @@
     "sts",
     "supplychain",
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

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/paginator.py` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     ListActionExecutionsOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListPipelinesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWebhooksOutputTypeDef,
     PaginatorConfigTypeDef,
+    PipelineExecutionFilterTypeDef,
 )
 
 __all__ = (
     "ListActionExecutionsPaginator",
     "ListActionTypesPaginator",
     "ListPipelineExecutionsPaginator",
     "ListPipelinesPaginator",
@@ -106,15 +107,19 @@
 class ListPipelineExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
     """
 
     def paginate(
-        self, *, pipelineName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        pipelineName: str,
+        filter: PipelineExecutionFilterTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPipelineExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
         """
```

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/paginator.pyi` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     ListActionExecutionsOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListPipelinesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWebhooksOutputTypeDef,
     PaginatorConfigTypeDef,
+    PipelineExecutionFilterTypeDef,
 )
 
 __all__ = (
     "ListActionExecutionsPaginator",
     "ListActionTypesPaginator",
     "ListPipelineExecutionsPaginator",
     "ListPipelinesPaginator",
@@ -102,15 +103,19 @@
 class ListPipelineExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
     """
 
     def paginate(
-        self, *, pipelineName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        pipelineName: str,
+        filter: PipelineExecutionFilterTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPipelineExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
         """
 
 class ListPipelinesPaginator(Paginator):
```

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/type_defs.py` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from .literals import (
     ActionCategoryType,
     ActionConfigurationPropertyTypeType,
     ActionExecutionStatusType,
     ActionOwnerType,
     ApprovalStatusType,
     ExecutionModeType,
+    ExecutionTypeType,
     ExecutorTypeType,
     FailureTypeType,
     GitPullRequestEventTypeType,
     JobStatusType,
     PipelineExecutionStatusType,
     PipelineTypeType,
     SourceRevisionTypeType,
@@ -60,156 +61,184 @@
     "ActionConfigurationTypeDef",
     "ActionContextTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "LatestInPipelineExecutionFilterTypeDef",
     "ErrorDetailsTypeDef",
-    "ActionRevisionTypeDef",
+    "ActionRevisionOutputTypeDef",
+    "TimestampTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
     "ActionTypeIdentifierTypeDef",
-    "ActionTypePermissionsTypeDef",
+    "ActionTypePermissionsOutputTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
+    "ActionTypePermissionsTypeDef",
     "ActionTypeSettingsTypeDef",
     "ArtifactDetailsTypeDef",
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
     "EncryptionKeyTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
-    "TimestampTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
-    "JobWorkerExecutorConfigurationTypeDef",
+    "JobWorkerExecutorConfigurationOutputTypeDef",
     "LambdaExecutorConfigurationTypeDef",
+    "JobWorkerExecutorConfigurationTypeDef",
+    "FailureConditionsTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
     "PipelineMetadataTypeDef",
     "GetPipelineStateInputRequestTypeDef",
     "GetThirdPartyJobDetailsInputRequestTypeDef",
+    "GitBranchFilterCriteriaOutputTypeDef",
     "GitBranchFilterCriteriaTypeDef",
+    "GitFilePathFilterCriteriaOutputTypeDef",
     "GitFilePathFilterCriteriaTypeDef",
+    "GitTagFilterCriteriaOutputTypeDef",
     "GitTagFilterCriteriaTypeDef",
     "PaginatorConfigTypeDef",
     "ListActionTypesInputRequestTypeDef",
-    "ListPipelineExecutionsInputRequestTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListWebhooksInputRequestTypeDef",
     "StageContextTypeDef",
     "PipelineVariableDeclarationTypeDef",
+    "SucceededInStageFilterTypeDef",
+    "PipelineRollbackMetadataTypeDef",
     "SourceRevisionTypeDef",
     "StopExecutionTriggerTypeDef",
     "ResolvedPipelineVariableTypeDef",
     "PipelineVariableTypeDef",
     "ThirdPartyJobTypeDef",
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
     "RetryStageExecutionInputRequestTypeDef",
+    "RollbackStageInputRequestTypeDef",
     "SourceRevisionOverrideTypeDef",
     "StageExecutionTypeDef",
     "TransitionStateTypeDef",
     "StopPipelineExecutionInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "WebhookAuthConfigurationTypeDef",
     "WebhookFilterRuleTypeDef",
     "AcknowledgeJobOutputTypeDef",
     "AcknowledgeThirdPartyJobOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "PutActionRevisionOutputTypeDef",
     "PutApprovalResultOutputTypeDef",
     "RetryStageExecutionOutputTypeDef",
+    "RollbackStageOutputTypeDef",
     "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
+    "ActionDeclarationOutputTypeDef",
     "ActionDeclarationTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ActionExecutionTypeDef",
-    "PutActionRevisionInputRequestTypeDef",
+    "ActionRevisionTypeDef",
+    "CurrentRevisionTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
-    "CurrentRevisionTypeDef",
+    "ExecutorConfigurationOutputTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
+    "GitPullRequestFilterOutputTypeDef",
     "GitPullRequestFilterTypeDef",
+    "GitPushFilterOutputTypeDef",
     "GitPushFilterTypeDef",
     "ListActionTypesInputListActionTypesPaginateTypeDef",
-    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
+    "PipelineExecutionFilterTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PipelineExecutionTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
     "StartPipelineExecutionInputRequestTypeDef",
+    "WebhookDefinitionExtraOutputTypeDef",
+    "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
+    "StageDeclarationOutputTypeDef",
     "StageDeclarationTypeDef",
     "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionStateTypeDef",
+    "ActionRevisionUnionTypeDef",
+    "PutActionRevisionInputRequestTypeDef",
+    "PutJobSuccessResultInputRequestTypeDef",
+    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "CreateCustomActionTypeOutputTypeDef",
     "ListActionTypesOutputTypeDef",
     "ActionExecutionInputTypeDef",
     "ActionExecutionOutputTypeDef",
     "ArtifactTypeDef",
-    "PutJobSuccessResultInputRequestTypeDef",
-    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
+    "ActionTypeExecutorOutputTypeDef",
     "ActionTypeExecutorTypeDef",
+    "GitConfigurationOutputTypeDef",
     "GitConfigurationTypeDef",
+    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    "ListPipelineExecutionsInputRequestTypeDef",
     "ListPipelineExecutionsOutputTypeDef",
     "GetPipelineExecutionOutputTypeDef",
     "ListWebhookItemTypeDef",
     "PutWebhookInputRequestTypeDef",
+    "WebhookDefinitionUnionTypeDef",
     "StageStateTypeDef",
     "ActionExecutionDetailTypeDef",
     "JobDataTypeDef",
     "ThirdPartyJobDataTypeDef",
+    "ActionTypeDeclarationOutputTypeDef",
     "ActionTypeDeclarationTypeDef",
+    "PipelineTriggerDeclarationOutputTypeDef",
     "PipelineTriggerDeclarationTypeDef",
     "ListWebhooksOutputTypeDef",
     "PutWebhookOutputTypeDef",
     "GetPipelineStateOutputTypeDef",
     "ListActionExecutionsOutputTypeDef",
     "JobDetailsTypeDef",
     "JobTypeDef",
     "ThirdPartyJobDetailsTypeDef",
     "GetActionTypeOutputTypeDef",
+    "ActionTypeDeclarationUnionTypeDef",
     "UpdateActionTypeInputRequestTypeDef",
+    "PipelineDeclarationOutputTypeDef",
     "PipelineDeclarationTypeDef",
     "GetJobDetailsOutputTypeDef",
     "PollForJobsOutputTypeDef",
     "GetThirdPartyJobDetailsOutputTypeDef",
-    "CreatePipelineInputRequestTypeDef",
     "CreatePipelineOutputTypeDef",
     "GetPipelineOutputTypeDef",
-    "UpdatePipelineInputRequestTypeDef",
     "UpdatePipelineOutputTypeDef",
+    "CreatePipelineInputRequestTypeDef",
+    "PipelineDeclarationUnionTypeDef",
+    "UpdatePipelineInputRequestTypeDef",
 )
 
 AWSSessionCredentialsTypeDef = TypedDict(
     "AWSSessionCredentialsTypeDef",
     {
         "accessKeyId": str,
         "secretAccessKey": str,
@@ -223,18 +252,18 @@
         "nonce": str,
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
 AcknowledgeThirdPartyJobInputRequestTypeDef = TypedDict(
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
@@ -297,22 +326,23 @@
 ErrorDetailsTypeDef = TypedDict(
     "ErrorDetailsTypeDef",
     {
         "code": NotRequired[str],
         "message": NotRequired[str],
     },
 )
-ActionRevisionTypeDef = TypedDict(
-    "ActionRevisionTypeDef",
+ActionRevisionOutputTypeDef = TypedDict(
+    "ActionRevisionOutputTypeDef",
     {
         "revisionId": str,
         "revisionChangeId": str,
         "created": datetime,
     },
 )
+TimestampTypeDef = Union[datetime, str]
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
@@ -321,16 +351,16 @@
     {
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
     },
 )
-ActionTypePermissionsTypeDef = TypedDict(
-    "ActionTypePermissionsTypeDef",
+ActionTypePermissionsOutputTypeDef = TypedDict(
+    "ActionTypePermissionsOutputTypeDef",
     {
         "allowedAccounts": List[str],
     },
 )
 ActionTypePropertyTypeDef = TypedDict(
     "ActionTypePropertyTypeDef",
     {
@@ -347,14 +377,20 @@
     {
         "configurationUrl": NotRequired[str],
         "entityUrlTemplate": NotRequired[str],
         "executionUrlTemplate": NotRequired[str],
         "revisionUrlTemplate": NotRequired[str],
     },
 )
+ActionTypePermissionsTypeDef = TypedDict(
+    "ActionTypePermissionsTypeDef",
+    {
+        "allowedAccounts": Sequence[str],
+    },
+)
 ActionTypeSettingsTypeDef = TypedDict(
     "ActionTypeSettingsTypeDef",
     {
         "thirdPartyConfigurationUrl": NotRequired[str],
         "entityUrlTemplate": NotRequired[str],
         "executionUrlTemplate": NotRequired[str],
         "revisionUrlTemplate": NotRequired[str],
@@ -416,15 +452,14 @@
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
-TimestampTypeDef = Union[datetime, str]
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -475,27 +510,40 @@
 ExecutionTriggerTypeDef = TypedDict(
     "ExecutionTriggerTypeDef",
     {
         "triggerType": NotRequired[TriggerTypeType],
         "triggerDetail": NotRequired[str],
     },
 )
-JobWorkerExecutorConfigurationTypeDef = TypedDict(
-    "JobWorkerExecutorConfigurationTypeDef",
+JobWorkerExecutorConfigurationOutputTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationOutputTypeDef",
     {
         "pollingAccounts": NotRequired[List[str]],
         "pollingServicePrincipals": NotRequired[List[str]],
     },
 )
 LambdaExecutorConfigurationTypeDef = TypedDict(
     "LambdaExecutorConfigurationTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
+JobWorkerExecutorConfigurationTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationTypeDef",
+    {
+        "pollingAccounts": NotRequired[Sequence[str]],
+        "pollingServicePrincipals": NotRequired[Sequence[str]],
+    },
+)
+FailureConditionsTypeDef = TypedDict(
+    "FailureConditionsTypeDef",
+    {
+        "result": NotRequired[Literal["ROLLBACK"]],
+    },
+)
 FailureDetailsTypeDef = TypedDict(
     "FailureDetailsTypeDef",
     {
         "type": FailureTypeType,
         "message": str,
         "externalExecutionId": NotRequired[str],
     },
@@ -547,28 +595,49 @@
 GetThirdPartyJobDetailsInputRequestTypeDef = TypedDict(
     "GetThirdPartyJobDetailsInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
+GitBranchFilterCriteriaOutputTypeDef = TypedDict(
+    "GitBranchFilterCriteriaOutputTypeDef",
+    {
+        "includes": NotRequired[List[str]],
+        "excludes": NotRequired[List[str]],
+    },
+)
 GitBranchFilterCriteriaTypeDef = TypedDict(
     "GitBranchFilterCriteriaTypeDef",
     {
         "includes": NotRequired[Sequence[str]],
         "excludes": NotRequired[Sequence[str]],
     },
 )
+GitFilePathFilterCriteriaOutputTypeDef = TypedDict(
+    "GitFilePathFilterCriteriaOutputTypeDef",
+    {
+        "includes": NotRequired[List[str]],
+        "excludes": NotRequired[List[str]],
+    },
+)
 GitFilePathFilterCriteriaTypeDef = TypedDict(
     "GitFilePathFilterCriteriaTypeDef",
     {
         "includes": NotRequired[Sequence[str]],
         "excludes": NotRequired[Sequence[str]],
     },
 )
+GitTagFilterCriteriaOutputTypeDef = TypedDict(
+    "GitTagFilterCriteriaOutputTypeDef",
+    {
+        "includes": NotRequired[List[str]],
+        "excludes": NotRequired[List[str]],
+    },
+)
 GitTagFilterCriteriaTypeDef = TypedDict(
     "GitTagFilterCriteriaTypeDef",
     {
         "includes": NotRequired[Sequence[str]],
         "excludes": NotRequired[Sequence[str]],
     },
 )
@@ -584,22 +653,14 @@
     "ListActionTypesInputRequestTypeDef",
     {
         "actionOwnerFilter": NotRequired[ActionOwnerType],
         "nextToken": NotRequired[str],
         "regionFilter": NotRequired[str],
     },
 )
-ListPipelineExecutionsInputRequestTypeDef = TypedDict(
-    "ListPipelineExecutionsInputRequestTypeDef",
-    {
-        "pipelineName": str,
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-    },
-)
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
     },
 )
@@ -639,14 +700,26 @@
     "PipelineVariableDeclarationTypeDef",
     {
         "name": str,
         "defaultValue": NotRequired[str],
         "description": NotRequired[str],
     },
 )
+SucceededInStageFilterTypeDef = TypedDict(
+    "SucceededInStageFilterTypeDef",
+    {
+        "stageName": NotRequired[str],
+    },
+)
+PipelineRollbackMetadataTypeDef = TypedDict(
+    "PipelineRollbackMetadataTypeDef",
+    {
+        "rollbackTargetPipelineExecutionId": NotRequired[str],
+    },
+)
 SourceRevisionTypeDef = TypedDict(
     "SourceRevisionTypeDef",
     {
         "actionName": str,
         "revisionId": NotRequired[str],
         "revisionSummary": NotRequired[str],
         "revisionUrl": NotRequired[str],
@@ -690,27 +763,36 @@
     {
         "pipelineName": str,
         "stageName": str,
         "pipelineExecutionId": str,
         "retryMode": StageRetryModeType,
     },
 )
+RollbackStageInputRequestTypeDef = TypedDict(
+    "RollbackStageInputRequestTypeDef",
+    {
+        "pipelineName": str,
+        "stageName": str,
+        "targetPipelineExecutionId": str,
+    },
+)
 SourceRevisionOverrideTypeDef = TypedDict(
     "SourceRevisionOverrideTypeDef",
     {
         "actionName": str,
         "revisionType": SourceRevisionTypeType,
         "revisionValue": str,
     },
 )
 StageExecutionTypeDef = TypedDict(
     "StageExecutionTypeDef",
     {
         "pipelineExecutionId": str,
         "status": StageExecutionStatusType,
+        "type": NotRequired[ExecutionTypeType],
     },
 )
 TransitionStateTypeDef = TypedDict(
     "TransitionStateTypeDef",
     {
         "enabled": NotRequired[bool],
         "lastChangedBy": NotRequired[str],
@@ -786,14 +868,21 @@
 RetryStageExecutionOutputTypeDef = TypedDict(
     "RetryStageExecutionOutputTypeDef",
     {
         "pipelineExecutionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RollbackStageOutputTypeDef = TypedDict(
+    "RollbackStageOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 StartPipelineExecutionOutputTypeDef = TypedDict(
     "StartPipelineExecutionOutputTypeDef",
     {
         "pipelineExecutionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -815,14 +904,29 @@
 PollForThirdPartyJobsInputRequestTypeDef = TypedDict(
     "PollForThirdPartyJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
         "maxBatchSize": NotRequired[int],
     },
 )
+ActionDeclarationOutputTypeDef = TypedDict(
+    "ActionDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "actionTypeId": ActionTypeIdTypeDef,
+        "runOrder": NotRequired[int],
+        "configuration": NotRequired[Dict[str, str]],
+        "outputArtifacts": NotRequired[List[OutputArtifactTypeDef]],
+        "inputArtifacts": NotRequired[List[InputArtifactTypeDef]],
+        "roleArn": NotRequired[str],
+        "region": NotRequired[str],
+        "namespace": NotRequired[str],
+        "timeoutInMinutes": NotRequired[int],
+    },
+)
 ActionDeclarationTypeDef = TypedDict(
     "ActionDeclarationTypeDef",
     {
         "name": str,
         "actionTypeId": ActionTypeIdTypeDef,
         "runOrder": NotRequired[int],
         "configuration": NotRequired[Mapping[str, str]],
@@ -861,21 +965,29 @@
         "lastUpdatedBy": NotRequired[str],
         "externalExecutionId": NotRequired[str],
         "externalExecutionUrl": NotRequired[str],
         "percentComplete": NotRequired[int],
         "errorDetails": NotRequired[ErrorDetailsTypeDef],
     },
 )
-PutActionRevisionInputRequestTypeDef = TypedDict(
-    "PutActionRevisionInputRequestTypeDef",
+ActionRevisionTypeDef = TypedDict(
+    "ActionRevisionTypeDef",
     {
-        "pipelineName": str,
-        "stageName": str,
-        "actionName": str,
-        "actionRevision": ActionRevisionTypeDef,
+        "revisionId": str,
+        "revisionChangeId": str,
+        "created": TimestampTypeDef,
+    },
+)
+CurrentRevisionTypeDef = TypedDict(
+    "CurrentRevisionTypeDef",
+    {
+        "revision": str,
+        "changeIdentifier": str,
+        "created": NotRequired[TimestampTypeDef],
+        "revisionSummary": NotRequired[str],
     },
 )
 ActionTypeTypeDef = TypedDict(
     "ActionTypeTypeDef",
     {
         "id": ActionTypeIdTypeDef,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
@@ -940,21 +1052,19 @@
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
-CurrentRevisionTypeDef = TypedDict(
-    "CurrentRevisionTypeDef",
+ExecutorConfigurationOutputTypeDef = TypedDict(
+    "ExecutorConfigurationOutputTypeDef",
     {
-        "revision": str,
-        "changeIdentifier": str,
-        "created": NotRequired[TimestampTypeDef],
-        "revisionSummary": NotRequired[str],
+        "lambdaExecutorConfiguration": NotRequired[LambdaExecutorConfigurationTypeDef],
+        "jobWorkerExecutorConfiguration": NotRequired[JobWorkerExecutorConfigurationOutputTypeDef],
     },
 )
 ExecutorConfigurationTypeDef = TypedDict(
     "ExecutorConfigurationTypeDef",
     {
         "lambdaExecutorConfiguration": NotRequired[LambdaExecutorConfigurationTypeDef],
         "jobWorkerExecutorConfiguration": NotRequired[JobWorkerExecutorConfigurationTypeDef],
@@ -971,22 +1081,38 @@
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
         "failureDetails": FailureDetailsTypeDef,
     },
 )
+GitPullRequestFilterOutputTypeDef = TypedDict(
+    "GitPullRequestFilterOutputTypeDef",
+    {
+        "events": NotRequired[List[GitPullRequestEventTypeType]],
+        "branches": NotRequired[GitBranchFilterCriteriaOutputTypeDef],
+        "filePaths": NotRequired[GitFilePathFilterCriteriaOutputTypeDef],
+    },
+)
 GitPullRequestFilterTypeDef = TypedDict(
     "GitPullRequestFilterTypeDef",
     {
         "events": NotRequired[Sequence[GitPullRequestEventTypeType]],
         "branches": NotRequired[GitBranchFilterCriteriaTypeDef],
         "filePaths": NotRequired[GitFilePathFilterCriteriaTypeDef],
     },
 )
+GitPushFilterOutputTypeDef = TypedDict(
+    "GitPushFilterOutputTypeDef",
+    {
+        "tags": NotRequired[GitTagFilterCriteriaOutputTypeDef],
+        "branches": NotRequired[GitBranchFilterCriteriaOutputTypeDef],
+        "filePaths": NotRequired[GitFilePathFilterCriteriaOutputTypeDef],
+    },
+)
 GitPushFilterTypeDef = TypedDict(
     "GitPushFilterTypeDef",
     {
         "tags": NotRequired[GitTagFilterCriteriaTypeDef],
         "branches": NotRequired[GitBranchFilterCriteriaTypeDef],
         "filePaths": NotRequired[GitFilePathFilterCriteriaTypeDef],
     },
@@ -995,21 +1121,14 @@
     "ListActionTypesInputListActionTypesPaginateTypeDef",
     {
         "actionOwnerFilter": NotRequired[ActionOwnerType],
         "regionFilter": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "pipelineName": str,
-        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
-    },
-)
 ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
@@ -1039,39 +1158,50 @@
         "pipelineName": NotRequired[str],
         "stage": NotRequired[StageContextTypeDef],
         "action": NotRequired[ActionContextTypeDef],
         "pipelineArn": NotRequired[str],
         "pipelineExecutionId": NotRequired[str],
     },
 )
+PipelineExecutionFilterTypeDef = TypedDict(
+    "PipelineExecutionFilterTypeDef",
+    {
+        "succeededInStage": NotRequired[SucceededInStageFilterTypeDef],
+    },
+)
 PipelineExecutionSummaryTypeDef = TypedDict(
     "PipelineExecutionSummaryTypeDef",
     {
         "pipelineExecutionId": NotRequired[str],
         "status": NotRequired[PipelineExecutionStatusType],
+        "statusSummary": NotRequired[str],
         "startTime": NotRequired[datetime],
         "lastUpdateTime": NotRequired[datetime],
         "sourceRevisions": NotRequired[List[SourceRevisionTypeDef]],
         "trigger": NotRequired[ExecutionTriggerTypeDef],
         "stopTrigger": NotRequired[StopExecutionTriggerTypeDef],
         "executionMode": NotRequired[ExecutionModeType],
+        "executionType": NotRequired[ExecutionTypeType],
+        "rollbackMetadata": NotRequired[PipelineRollbackMetadataTypeDef],
     },
 )
 PipelineExecutionTypeDef = TypedDict(
     "PipelineExecutionTypeDef",
     {
         "pipelineName": NotRequired[str],
         "pipelineVersion": NotRequired[int],
         "pipelineExecutionId": NotRequired[str],
         "status": NotRequired[PipelineExecutionStatusType],
         "statusSummary": NotRequired[str],
         "artifactRevisions": NotRequired[List[ArtifactRevisionTypeDef]],
         "variables": NotRequired[List[ResolvedPipelineVariableTypeDef]],
         "trigger": NotRequired[ExecutionTriggerTypeDef],
         "executionMode": NotRequired[ExecutionModeType],
+        "executionType": NotRequired[ExecutionTypeType],
+        "rollbackMetadata": NotRequired[PipelineRollbackMetadataTypeDef],
     },
 )
 PollForThirdPartyJobsOutputTypeDef = TypedDict(
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1082,31 +1212,63 @@
     {
         "name": str,
         "variables": NotRequired[Sequence[PipelineVariableTypeDef]],
         "clientRequestToken": NotRequired[str],
         "sourceRevisions": NotRequired[Sequence[SourceRevisionOverrideTypeDef]],
     },
 )
+WebhookDefinitionExtraOutputTypeDef = TypedDict(
+    "WebhookDefinitionExtraOutputTypeDef",
+    {
+        "name": str,
+        "targetPipeline": str,
+        "targetAction": str,
+        "filters": List[WebhookFilterRuleTypeDef],
+        "authentication": WebhookAuthenticationTypeType,
+        "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
+    },
+)
+WebhookDefinitionOutputTypeDef = TypedDict(
+    "WebhookDefinitionOutputTypeDef",
+    {
+        "name": str,
+        "targetPipeline": str,
+        "targetAction": str,
+        "filters": List[WebhookFilterRuleTypeDef],
+        "authentication": WebhookAuthenticationTypeType,
+        "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
+    },
+)
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
         "targetPipeline": str,
         "targetAction": str,
-        "filters": List[WebhookFilterRuleTypeDef],
+        "filters": Sequence[WebhookFilterRuleTypeDef],
         "authentication": WebhookAuthenticationTypeType,
         "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
+StageDeclarationOutputTypeDef = TypedDict(
+    "StageDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "actions": List[ActionDeclarationOutputTypeDef],
+        "blockers": NotRequired[List[BlockerDeclarationTypeDef]],
+        "onFailure": NotRequired[FailureConditionsTypeDef],
+    },
+)
 StageDeclarationTypeDef = TypedDict(
     "StageDeclarationTypeDef",
     {
         "name": str,
         "actions": Sequence[ActionDeclarationTypeDef],
         "blockers": NotRequired[Sequence[BlockerDeclarationTypeDef]],
+        "onFailure": NotRequired[FailureConditionsTypeDef],
     },
 )
 ListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
     "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     {
         "pipelineName": str,
         "filter": NotRequired[ActionExecutionFilterTypeDef],
@@ -1122,20 +1284,50 @@
         "nextToken": NotRequired[str],
     },
 )
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": NotRequired[str],
-        "currentRevision": NotRequired[ActionRevisionTypeDef],
+        "currentRevision": NotRequired[ActionRevisionOutputTypeDef],
         "latestExecution": NotRequired[ActionExecutionTypeDef],
         "entityUrl": NotRequired[str],
         "revisionUrl": NotRequired[str],
     },
 )
+ActionRevisionUnionTypeDef = Union[ActionRevisionTypeDef, ActionRevisionOutputTypeDef]
+PutActionRevisionInputRequestTypeDef = TypedDict(
+    "PutActionRevisionInputRequestTypeDef",
+    {
+        "pipelineName": str,
+        "stageName": str,
+        "actionName": str,
+        "actionRevision": ActionRevisionTypeDef,
+    },
+)
+PutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "PutJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+        "currentRevision": NotRequired[CurrentRevisionTypeDef],
+        "continuationToken": NotRequired[str],
+        "executionDetails": NotRequired[ExecutionDetailsTypeDef],
+        "outputVariables": NotRequired[Mapping[str, str]],
+    },
+)
+PutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+        "clientToken": str,
+        "currentRevision": NotRequired[CurrentRevisionTypeDef],
+        "continuationToken": NotRequired[str],
+        "executionDetails": NotRequired[ExecutionDetailsTypeDef],
+    },
+)
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1172,51 +1364,65 @@
     "ArtifactTypeDef",
     {
         "name": NotRequired[str],
         "revision": NotRequired[str],
         "location": NotRequired[ArtifactLocationTypeDef],
     },
 )
-PutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "PutJobSuccessResultInputRequestTypeDef",
-    {
-        "jobId": str,
-        "currentRevision": NotRequired[CurrentRevisionTypeDef],
-        "continuationToken": NotRequired[str],
-        "executionDetails": NotRequired[ExecutionDetailsTypeDef],
-        "outputVariables": NotRequired[Mapping[str, str]],
-    },
-)
-PutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
+ActionTypeExecutorOutputTypeDef = TypedDict(
+    "ActionTypeExecutorOutputTypeDef",
     {
-        "jobId": str,
-        "clientToken": str,
-        "currentRevision": NotRequired[CurrentRevisionTypeDef],
-        "continuationToken": NotRequired[str],
-        "executionDetails": NotRequired[ExecutionDetailsTypeDef],
+        "configuration": ExecutorConfigurationOutputTypeDef,
+        "type": ExecutorTypeType,
+        "policyStatementsTemplate": NotRequired[str],
+        "jobTimeout": NotRequired[int],
     },
 )
 ActionTypeExecutorTypeDef = TypedDict(
     "ActionTypeExecutorTypeDef",
     {
         "configuration": ExecutorConfigurationTypeDef,
         "type": ExecutorTypeType,
         "policyStatementsTemplate": NotRequired[str],
         "jobTimeout": NotRequired[int],
     },
 )
+GitConfigurationOutputTypeDef = TypedDict(
+    "GitConfigurationOutputTypeDef",
+    {
+        "sourceActionName": str,
+        "push": NotRequired[List[GitPushFilterOutputTypeDef]],
+        "pullRequest": NotRequired[List[GitPullRequestFilterOutputTypeDef]],
+    },
+)
 GitConfigurationTypeDef = TypedDict(
     "GitConfigurationTypeDef",
     {
         "sourceActionName": str,
         "push": NotRequired[Sequence[GitPushFilterTypeDef]],
         "pullRequest": NotRequired[Sequence[GitPullRequestFilterTypeDef]],
     },
 )
+ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+        "filter": NotRequired[PipelineExecutionFilterTypeDef],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+ListPipelineExecutionsInputRequestTypeDef = TypedDict(
+    "ListPipelineExecutionsInputRequestTypeDef",
+    {
+        "pipelineName": str,
+        "maxResults": NotRequired[int],
+        "filter": NotRequired[PipelineExecutionFilterTypeDef],
+        "nextToken": NotRequired[str],
+    },
+)
 ListPipelineExecutionsOutputTypeDef = TypedDict(
     "ListPipelineExecutionsOutputTypeDef",
     {
         "pipelineExecutionSummaries": List[PipelineExecutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1227,15 +1433,15 @@
         "pipelineExecution": PipelineExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListWebhookItemTypeDef = TypedDict(
     "ListWebhookItemTypeDef",
     {
-        "definition": WebhookDefinitionTypeDef,
+        "definition": WebhookDefinitionOutputTypeDef,
         "url": str,
         "errorMessage": NotRequired[str],
         "errorCode": NotRequired[str],
         "lastTriggered": NotRequired[datetime],
         "arn": NotRequired[str],
         "tags": NotRequired[List[TagTypeDef]],
     },
@@ -1243,14 +1449,15 @@
 PutWebhookInputRequestTypeDef = TypedDict(
     "PutWebhookInputRequestTypeDef",
     {
         "webhook": WebhookDefinitionTypeDef,
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+WebhookDefinitionUnionTypeDef = Union[WebhookDefinitionTypeDef, WebhookDefinitionExtraOutputTypeDef]
 StageStateTypeDef = TypedDict(
     "StageStateTypeDef",
     {
         "stageName": NotRequired[str],
         "inboundExecution": NotRequired[StageExecutionTypeDef],
         "inboundExecutions": NotRequired[List[StageExecutionTypeDef]],
         "inboundTransitionState": NotRequired[TransitionStateTypeDef],
@@ -1296,40 +1503,60 @@
         "inputArtifacts": NotRequired[List[ArtifactTypeDef]],
         "outputArtifacts": NotRequired[List[ArtifactTypeDef]],
         "artifactCredentials": NotRequired[AWSSessionCredentialsTypeDef],
         "continuationToken": NotRequired[str],
         "encryptionKey": NotRequired[EncryptionKeyTypeDef],
     },
 )
+ActionTypeDeclarationOutputTypeDef = TypedDict(
+    "ActionTypeDeclarationOutputTypeDef",
+    {
+        "executor": ActionTypeExecutorOutputTypeDef,
+        "id": ActionTypeIdentifierTypeDef,
+        "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
+        "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
+        "description": NotRequired[str],
+        "permissions": NotRequired[ActionTypePermissionsOutputTypeDef],
+        "properties": NotRequired[List[ActionTypePropertyTypeDef]],
+        "urls": NotRequired[ActionTypeUrlsTypeDef],
+    },
+)
 ActionTypeDeclarationTypeDef = TypedDict(
     "ActionTypeDeclarationTypeDef",
     {
         "executor": ActionTypeExecutorTypeDef,
         "id": ActionTypeIdentifierTypeDef,
         "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "description": NotRequired[str],
         "permissions": NotRequired[ActionTypePermissionsTypeDef],
-        "properties": NotRequired[List[ActionTypePropertyTypeDef]],
+        "properties": NotRequired[Sequence[ActionTypePropertyTypeDef]],
         "urls": NotRequired[ActionTypeUrlsTypeDef],
     },
 )
+PipelineTriggerDeclarationOutputTypeDef = TypedDict(
+    "PipelineTriggerDeclarationOutputTypeDef",
+    {
+        "providerType": Literal["CodeStarSourceConnection"],
+        "gitConfiguration": GitConfigurationOutputTypeDef,
+    },
+)
 PipelineTriggerDeclarationTypeDef = TypedDict(
     "PipelineTriggerDeclarationTypeDef",
     {
         "providerType": Literal["CodeStarSourceConnection"],
         "gitConfiguration": GitConfigurationTypeDef,
     },
 )
 ListWebhooksOutputTypeDef = TypedDict(
     "ListWebhooksOutputTypeDef",
     {
         "webhooks": List[ListWebhookItemTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PutWebhookOutputTypeDef = TypedDict(
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1378,24 +1605,42 @@
         "data": NotRequired[ThirdPartyJobDataTypeDef],
         "nonce": NotRequired[str],
     },
 )
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
-        "actionType": ActionTypeDeclarationTypeDef,
+        "actionType": ActionTypeDeclarationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ActionTypeDeclarationUnionTypeDef = Union[
+    ActionTypeDeclarationTypeDef, ActionTypeDeclarationOutputTypeDef
+]
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
+PipelineDeclarationOutputTypeDef = TypedDict(
+    "PipelineDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "stages": List[StageDeclarationOutputTypeDef],
+        "artifactStore": NotRequired[ArtifactStoreTypeDef],
+        "artifactStores": NotRequired[Dict[str, ArtifactStoreTypeDef]],
+        "version": NotRequired[int],
+        "executionMode": NotRequired[ExecutionModeType],
+        "pipelineType": NotRequired[PipelineTypeType],
+        "variables": NotRequired[List[PipelineVariableDeclarationTypeDef]],
+        "triggers": NotRequired[List[PipelineTriggerDeclarationOutputTypeDef]],
+    },
+)
 PipelineDeclarationTypeDef = TypedDict(
     "PipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
         "artifactStore": NotRequired[ArtifactStoreTypeDef],
@@ -1424,43 +1669,46 @@
 GetThirdPartyJobDetailsOutputTypeDef = TypedDict(
     "GetThirdPartyJobDetailsOutputTypeDef",
     {
         "jobDetails": ThirdPartyJobDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreatePipelineInputRequestTypeDef = TypedDict(
-    "CreatePipelineInputRequestTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 CreatePipelineOutputTypeDef = TypedDict(
     "CreatePipelineOutputTypeDef",
     {
-        "pipeline": PipelineDeclarationTypeDef,
+        "pipeline": PipelineDeclarationOutputTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetPipelineOutputTypeDef = TypedDict(
     "GetPipelineOutputTypeDef",
     {
-        "pipeline": PipelineDeclarationTypeDef,
+        "pipeline": PipelineDeclarationOutputTypeDef,
         "metadata": PipelineMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdatePipelineInputRequestTypeDef = TypedDict(
-    "UpdatePipelineInputRequestTypeDef",
+UpdatePipelineOutputTypeDef = TypedDict(
+    "UpdatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreatePipelineInputRequestTypeDef = TypedDict(
+    "CreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
+        "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-UpdatePipelineOutputTypeDef = TypedDict(
-    "UpdatePipelineOutputTypeDef",
+PipelineDeclarationUnionTypeDef = Union[
+    PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef
+]
+UpdatePipelineInputRequestTypeDef = TypedDict(
+    "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline/type_defs.pyi` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from .literals import (
     ActionCategoryType,
     ActionConfigurationPropertyTypeType,
     ActionExecutionStatusType,
     ActionOwnerType,
     ApprovalStatusType,
     ExecutionModeType,
+    ExecutionTypeType,
     ExecutorTypeType,
     FailureTypeType,
     GitPullRequestEventTypeType,
     JobStatusType,
     PipelineExecutionStatusType,
     PipelineTypeType,
     SourceRevisionTypeType,
@@ -60,156 +61,184 @@
     "ActionConfigurationTypeDef",
     "ActionContextTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "LatestInPipelineExecutionFilterTypeDef",
     "ErrorDetailsTypeDef",
-    "ActionRevisionTypeDef",
+    "ActionRevisionOutputTypeDef",
+    "TimestampTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
     "ActionTypeIdentifierTypeDef",
-    "ActionTypePermissionsTypeDef",
+    "ActionTypePermissionsOutputTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
+    "ActionTypePermissionsTypeDef",
     "ActionTypeSettingsTypeDef",
     "ArtifactDetailsTypeDef",
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
     "EncryptionKeyTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
-    "TimestampTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
-    "JobWorkerExecutorConfigurationTypeDef",
+    "JobWorkerExecutorConfigurationOutputTypeDef",
     "LambdaExecutorConfigurationTypeDef",
+    "JobWorkerExecutorConfigurationTypeDef",
+    "FailureConditionsTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
     "PipelineMetadataTypeDef",
     "GetPipelineStateInputRequestTypeDef",
     "GetThirdPartyJobDetailsInputRequestTypeDef",
+    "GitBranchFilterCriteriaOutputTypeDef",
     "GitBranchFilterCriteriaTypeDef",
+    "GitFilePathFilterCriteriaOutputTypeDef",
     "GitFilePathFilterCriteriaTypeDef",
+    "GitTagFilterCriteriaOutputTypeDef",
     "GitTagFilterCriteriaTypeDef",
     "PaginatorConfigTypeDef",
     "ListActionTypesInputRequestTypeDef",
-    "ListPipelineExecutionsInputRequestTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListWebhooksInputRequestTypeDef",
     "StageContextTypeDef",
     "PipelineVariableDeclarationTypeDef",
+    "SucceededInStageFilterTypeDef",
+    "PipelineRollbackMetadataTypeDef",
     "SourceRevisionTypeDef",
     "StopExecutionTriggerTypeDef",
     "ResolvedPipelineVariableTypeDef",
     "PipelineVariableTypeDef",
     "ThirdPartyJobTypeDef",
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
     "RetryStageExecutionInputRequestTypeDef",
+    "RollbackStageInputRequestTypeDef",
     "SourceRevisionOverrideTypeDef",
     "StageExecutionTypeDef",
     "TransitionStateTypeDef",
     "StopPipelineExecutionInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "WebhookAuthConfigurationTypeDef",
     "WebhookFilterRuleTypeDef",
     "AcknowledgeJobOutputTypeDef",
     "AcknowledgeThirdPartyJobOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "PutActionRevisionOutputTypeDef",
     "PutApprovalResultOutputTypeDef",
     "RetryStageExecutionOutputTypeDef",
+    "RollbackStageOutputTypeDef",
     "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
+    "ActionDeclarationOutputTypeDef",
     "ActionDeclarationTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ActionExecutionTypeDef",
-    "PutActionRevisionInputRequestTypeDef",
+    "ActionRevisionTypeDef",
+    "CurrentRevisionTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
-    "CurrentRevisionTypeDef",
+    "ExecutorConfigurationOutputTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
+    "GitPullRequestFilterOutputTypeDef",
     "GitPullRequestFilterTypeDef",
+    "GitPushFilterOutputTypeDef",
     "GitPushFilterTypeDef",
     "ListActionTypesInputListActionTypesPaginateTypeDef",
-    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
+    "PipelineExecutionFilterTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PipelineExecutionTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
     "StartPipelineExecutionInputRequestTypeDef",
+    "WebhookDefinitionExtraOutputTypeDef",
+    "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
+    "StageDeclarationOutputTypeDef",
     "StageDeclarationTypeDef",
     "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionStateTypeDef",
+    "ActionRevisionUnionTypeDef",
+    "PutActionRevisionInputRequestTypeDef",
+    "PutJobSuccessResultInputRequestTypeDef",
+    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "CreateCustomActionTypeOutputTypeDef",
     "ListActionTypesOutputTypeDef",
     "ActionExecutionInputTypeDef",
     "ActionExecutionOutputTypeDef",
     "ArtifactTypeDef",
-    "PutJobSuccessResultInputRequestTypeDef",
-    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
+    "ActionTypeExecutorOutputTypeDef",
     "ActionTypeExecutorTypeDef",
+    "GitConfigurationOutputTypeDef",
     "GitConfigurationTypeDef",
+    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    "ListPipelineExecutionsInputRequestTypeDef",
     "ListPipelineExecutionsOutputTypeDef",
     "GetPipelineExecutionOutputTypeDef",
     "ListWebhookItemTypeDef",
     "PutWebhookInputRequestTypeDef",
+    "WebhookDefinitionUnionTypeDef",
     "StageStateTypeDef",
     "ActionExecutionDetailTypeDef",
     "JobDataTypeDef",
     "ThirdPartyJobDataTypeDef",
+    "ActionTypeDeclarationOutputTypeDef",
     "ActionTypeDeclarationTypeDef",
+    "PipelineTriggerDeclarationOutputTypeDef",
     "PipelineTriggerDeclarationTypeDef",
     "ListWebhooksOutputTypeDef",
     "PutWebhookOutputTypeDef",
     "GetPipelineStateOutputTypeDef",
     "ListActionExecutionsOutputTypeDef",
     "JobDetailsTypeDef",
     "JobTypeDef",
     "ThirdPartyJobDetailsTypeDef",
     "GetActionTypeOutputTypeDef",
+    "ActionTypeDeclarationUnionTypeDef",
     "UpdateActionTypeInputRequestTypeDef",
+    "PipelineDeclarationOutputTypeDef",
     "PipelineDeclarationTypeDef",
     "GetJobDetailsOutputTypeDef",
     "PollForJobsOutputTypeDef",
     "GetThirdPartyJobDetailsOutputTypeDef",
-    "CreatePipelineInputRequestTypeDef",
     "CreatePipelineOutputTypeDef",
     "GetPipelineOutputTypeDef",
-    "UpdatePipelineInputRequestTypeDef",
     "UpdatePipelineOutputTypeDef",
+    "CreatePipelineInputRequestTypeDef",
+    "PipelineDeclarationUnionTypeDef",
+    "UpdatePipelineInputRequestTypeDef",
 )
 
 AWSSessionCredentialsTypeDef = TypedDict(
     "AWSSessionCredentialsTypeDef",
     {
         "accessKeyId": str,
         "secretAccessKey": str,
@@ -223,18 +252,18 @@
         "nonce": str,
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
 AcknowledgeThirdPartyJobInputRequestTypeDef = TypedDict(
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
@@ -297,22 +326,23 @@
 ErrorDetailsTypeDef = TypedDict(
     "ErrorDetailsTypeDef",
     {
         "code": NotRequired[str],
         "message": NotRequired[str],
     },
 )
-ActionRevisionTypeDef = TypedDict(
-    "ActionRevisionTypeDef",
+ActionRevisionOutputTypeDef = TypedDict(
+    "ActionRevisionOutputTypeDef",
     {
         "revisionId": str,
         "revisionChangeId": str,
         "created": datetime,
     },
 )
+TimestampTypeDef = Union[datetime, str]
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
@@ -321,16 +351,16 @@
     {
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
     },
 )
-ActionTypePermissionsTypeDef = TypedDict(
-    "ActionTypePermissionsTypeDef",
+ActionTypePermissionsOutputTypeDef = TypedDict(
+    "ActionTypePermissionsOutputTypeDef",
     {
         "allowedAccounts": List[str],
     },
 )
 ActionTypePropertyTypeDef = TypedDict(
     "ActionTypePropertyTypeDef",
     {
@@ -347,14 +377,20 @@
     {
         "configurationUrl": NotRequired[str],
         "entityUrlTemplate": NotRequired[str],
         "executionUrlTemplate": NotRequired[str],
         "revisionUrlTemplate": NotRequired[str],
     },
 )
+ActionTypePermissionsTypeDef = TypedDict(
+    "ActionTypePermissionsTypeDef",
+    {
+        "allowedAccounts": Sequence[str],
+    },
+)
 ActionTypeSettingsTypeDef = TypedDict(
     "ActionTypeSettingsTypeDef",
     {
         "thirdPartyConfigurationUrl": NotRequired[str],
         "entityUrlTemplate": NotRequired[str],
         "executionUrlTemplate": NotRequired[str],
         "revisionUrlTemplate": NotRequired[str],
@@ -416,15 +452,14 @@
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
-TimestampTypeDef = Union[datetime, str]
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -475,27 +510,40 @@
 ExecutionTriggerTypeDef = TypedDict(
     "ExecutionTriggerTypeDef",
     {
         "triggerType": NotRequired[TriggerTypeType],
         "triggerDetail": NotRequired[str],
     },
 )
-JobWorkerExecutorConfigurationTypeDef = TypedDict(
-    "JobWorkerExecutorConfigurationTypeDef",
+JobWorkerExecutorConfigurationOutputTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationOutputTypeDef",
     {
         "pollingAccounts": NotRequired[List[str]],
         "pollingServicePrincipals": NotRequired[List[str]],
     },
 )
 LambdaExecutorConfigurationTypeDef = TypedDict(
     "LambdaExecutorConfigurationTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
+JobWorkerExecutorConfigurationTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationTypeDef",
+    {
+        "pollingAccounts": NotRequired[Sequence[str]],
+        "pollingServicePrincipals": NotRequired[Sequence[str]],
+    },
+)
+FailureConditionsTypeDef = TypedDict(
+    "FailureConditionsTypeDef",
+    {
+        "result": NotRequired[Literal["ROLLBACK"]],
+    },
+)
 FailureDetailsTypeDef = TypedDict(
     "FailureDetailsTypeDef",
     {
         "type": FailureTypeType,
         "message": str,
         "externalExecutionId": NotRequired[str],
     },
@@ -547,28 +595,49 @@
 GetThirdPartyJobDetailsInputRequestTypeDef = TypedDict(
     "GetThirdPartyJobDetailsInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
+GitBranchFilterCriteriaOutputTypeDef = TypedDict(
+    "GitBranchFilterCriteriaOutputTypeDef",
+    {
+        "includes": NotRequired[List[str]],
+        "excludes": NotRequired[List[str]],
+    },
+)
 GitBranchFilterCriteriaTypeDef = TypedDict(
     "GitBranchFilterCriteriaTypeDef",
     {
         "includes": NotRequired[Sequence[str]],
         "excludes": NotRequired[Sequence[str]],
     },
 )
+GitFilePathFilterCriteriaOutputTypeDef = TypedDict(
+    "GitFilePathFilterCriteriaOutputTypeDef",
+    {
+        "includes": NotRequired[List[str]],
+        "excludes": NotRequired[List[str]],
+    },
+)
 GitFilePathFilterCriteriaTypeDef = TypedDict(
     "GitFilePathFilterCriteriaTypeDef",
     {
         "includes": NotRequired[Sequence[str]],
         "excludes": NotRequired[Sequence[str]],
     },
 )
+GitTagFilterCriteriaOutputTypeDef = TypedDict(
+    "GitTagFilterCriteriaOutputTypeDef",
+    {
+        "includes": NotRequired[List[str]],
+        "excludes": NotRequired[List[str]],
+    },
+)
 GitTagFilterCriteriaTypeDef = TypedDict(
     "GitTagFilterCriteriaTypeDef",
     {
         "includes": NotRequired[Sequence[str]],
         "excludes": NotRequired[Sequence[str]],
     },
 )
@@ -584,22 +653,14 @@
     "ListActionTypesInputRequestTypeDef",
     {
         "actionOwnerFilter": NotRequired[ActionOwnerType],
         "nextToken": NotRequired[str],
         "regionFilter": NotRequired[str],
     },
 )
-ListPipelineExecutionsInputRequestTypeDef = TypedDict(
-    "ListPipelineExecutionsInputRequestTypeDef",
-    {
-        "pipelineName": str,
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-    },
-)
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
     },
 )
@@ -639,14 +700,26 @@
     "PipelineVariableDeclarationTypeDef",
     {
         "name": str,
         "defaultValue": NotRequired[str],
         "description": NotRequired[str],
     },
 )
+SucceededInStageFilterTypeDef = TypedDict(
+    "SucceededInStageFilterTypeDef",
+    {
+        "stageName": NotRequired[str],
+    },
+)
+PipelineRollbackMetadataTypeDef = TypedDict(
+    "PipelineRollbackMetadataTypeDef",
+    {
+        "rollbackTargetPipelineExecutionId": NotRequired[str],
+    },
+)
 SourceRevisionTypeDef = TypedDict(
     "SourceRevisionTypeDef",
     {
         "actionName": str,
         "revisionId": NotRequired[str],
         "revisionSummary": NotRequired[str],
         "revisionUrl": NotRequired[str],
@@ -690,27 +763,36 @@
     {
         "pipelineName": str,
         "stageName": str,
         "pipelineExecutionId": str,
         "retryMode": StageRetryModeType,
     },
 )
+RollbackStageInputRequestTypeDef = TypedDict(
+    "RollbackStageInputRequestTypeDef",
+    {
+        "pipelineName": str,
+        "stageName": str,
+        "targetPipelineExecutionId": str,
+    },
+)
 SourceRevisionOverrideTypeDef = TypedDict(
     "SourceRevisionOverrideTypeDef",
     {
         "actionName": str,
         "revisionType": SourceRevisionTypeType,
         "revisionValue": str,
     },
 )
 StageExecutionTypeDef = TypedDict(
     "StageExecutionTypeDef",
     {
         "pipelineExecutionId": str,
         "status": StageExecutionStatusType,
+        "type": NotRequired[ExecutionTypeType],
     },
 )
 TransitionStateTypeDef = TypedDict(
     "TransitionStateTypeDef",
     {
         "enabled": NotRequired[bool],
         "lastChangedBy": NotRequired[str],
@@ -786,14 +868,21 @@
 RetryStageExecutionOutputTypeDef = TypedDict(
     "RetryStageExecutionOutputTypeDef",
     {
         "pipelineExecutionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RollbackStageOutputTypeDef = TypedDict(
+    "RollbackStageOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 StartPipelineExecutionOutputTypeDef = TypedDict(
     "StartPipelineExecutionOutputTypeDef",
     {
         "pipelineExecutionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -815,14 +904,29 @@
 PollForThirdPartyJobsInputRequestTypeDef = TypedDict(
     "PollForThirdPartyJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
         "maxBatchSize": NotRequired[int],
     },
 )
+ActionDeclarationOutputTypeDef = TypedDict(
+    "ActionDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "actionTypeId": ActionTypeIdTypeDef,
+        "runOrder": NotRequired[int],
+        "configuration": NotRequired[Dict[str, str]],
+        "outputArtifacts": NotRequired[List[OutputArtifactTypeDef]],
+        "inputArtifacts": NotRequired[List[InputArtifactTypeDef]],
+        "roleArn": NotRequired[str],
+        "region": NotRequired[str],
+        "namespace": NotRequired[str],
+        "timeoutInMinutes": NotRequired[int],
+    },
+)
 ActionDeclarationTypeDef = TypedDict(
     "ActionDeclarationTypeDef",
     {
         "name": str,
         "actionTypeId": ActionTypeIdTypeDef,
         "runOrder": NotRequired[int],
         "configuration": NotRequired[Mapping[str, str]],
@@ -861,21 +965,29 @@
         "lastUpdatedBy": NotRequired[str],
         "externalExecutionId": NotRequired[str],
         "externalExecutionUrl": NotRequired[str],
         "percentComplete": NotRequired[int],
         "errorDetails": NotRequired[ErrorDetailsTypeDef],
     },
 )
-PutActionRevisionInputRequestTypeDef = TypedDict(
-    "PutActionRevisionInputRequestTypeDef",
+ActionRevisionTypeDef = TypedDict(
+    "ActionRevisionTypeDef",
     {
-        "pipelineName": str,
-        "stageName": str,
-        "actionName": str,
-        "actionRevision": ActionRevisionTypeDef,
+        "revisionId": str,
+        "revisionChangeId": str,
+        "created": TimestampTypeDef,
+    },
+)
+CurrentRevisionTypeDef = TypedDict(
+    "CurrentRevisionTypeDef",
+    {
+        "revision": str,
+        "changeIdentifier": str,
+        "created": NotRequired[TimestampTypeDef],
+        "revisionSummary": NotRequired[str],
     },
 )
 ActionTypeTypeDef = TypedDict(
     "ActionTypeTypeDef",
     {
         "id": ActionTypeIdTypeDef,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
@@ -940,21 +1052,19 @@
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
-CurrentRevisionTypeDef = TypedDict(
-    "CurrentRevisionTypeDef",
+ExecutorConfigurationOutputTypeDef = TypedDict(
+    "ExecutorConfigurationOutputTypeDef",
     {
-        "revision": str,
-        "changeIdentifier": str,
-        "created": NotRequired[TimestampTypeDef],
-        "revisionSummary": NotRequired[str],
+        "lambdaExecutorConfiguration": NotRequired[LambdaExecutorConfigurationTypeDef],
+        "jobWorkerExecutorConfiguration": NotRequired[JobWorkerExecutorConfigurationOutputTypeDef],
     },
 )
 ExecutorConfigurationTypeDef = TypedDict(
     "ExecutorConfigurationTypeDef",
     {
         "lambdaExecutorConfiguration": NotRequired[LambdaExecutorConfigurationTypeDef],
         "jobWorkerExecutorConfiguration": NotRequired[JobWorkerExecutorConfigurationTypeDef],
@@ -971,22 +1081,38 @@
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
         "failureDetails": FailureDetailsTypeDef,
     },
 )
+GitPullRequestFilterOutputTypeDef = TypedDict(
+    "GitPullRequestFilterOutputTypeDef",
+    {
+        "events": NotRequired[List[GitPullRequestEventTypeType]],
+        "branches": NotRequired[GitBranchFilterCriteriaOutputTypeDef],
+        "filePaths": NotRequired[GitFilePathFilterCriteriaOutputTypeDef],
+    },
+)
 GitPullRequestFilterTypeDef = TypedDict(
     "GitPullRequestFilterTypeDef",
     {
         "events": NotRequired[Sequence[GitPullRequestEventTypeType]],
         "branches": NotRequired[GitBranchFilterCriteriaTypeDef],
         "filePaths": NotRequired[GitFilePathFilterCriteriaTypeDef],
     },
 )
+GitPushFilterOutputTypeDef = TypedDict(
+    "GitPushFilterOutputTypeDef",
+    {
+        "tags": NotRequired[GitTagFilterCriteriaOutputTypeDef],
+        "branches": NotRequired[GitBranchFilterCriteriaOutputTypeDef],
+        "filePaths": NotRequired[GitFilePathFilterCriteriaOutputTypeDef],
+    },
+)
 GitPushFilterTypeDef = TypedDict(
     "GitPushFilterTypeDef",
     {
         "tags": NotRequired[GitTagFilterCriteriaTypeDef],
         "branches": NotRequired[GitBranchFilterCriteriaTypeDef],
         "filePaths": NotRequired[GitFilePathFilterCriteriaTypeDef],
     },
@@ -995,21 +1121,14 @@
     "ListActionTypesInputListActionTypesPaginateTypeDef",
     {
         "actionOwnerFilter": NotRequired[ActionOwnerType],
         "regionFilter": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "pipelineName": str,
-        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
-    },
-)
 ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
@@ -1039,39 +1158,50 @@
         "pipelineName": NotRequired[str],
         "stage": NotRequired[StageContextTypeDef],
         "action": NotRequired[ActionContextTypeDef],
         "pipelineArn": NotRequired[str],
         "pipelineExecutionId": NotRequired[str],
     },
 )
+PipelineExecutionFilterTypeDef = TypedDict(
+    "PipelineExecutionFilterTypeDef",
+    {
+        "succeededInStage": NotRequired[SucceededInStageFilterTypeDef],
+    },
+)
 PipelineExecutionSummaryTypeDef = TypedDict(
     "PipelineExecutionSummaryTypeDef",
     {
         "pipelineExecutionId": NotRequired[str],
         "status": NotRequired[PipelineExecutionStatusType],
+        "statusSummary": NotRequired[str],
         "startTime": NotRequired[datetime],
         "lastUpdateTime": NotRequired[datetime],
         "sourceRevisions": NotRequired[List[SourceRevisionTypeDef]],
         "trigger": NotRequired[ExecutionTriggerTypeDef],
         "stopTrigger": NotRequired[StopExecutionTriggerTypeDef],
         "executionMode": NotRequired[ExecutionModeType],
+        "executionType": NotRequired[ExecutionTypeType],
+        "rollbackMetadata": NotRequired[PipelineRollbackMetadataTypeDef],
     },
 )
 PipelineExecutionTypeDef = TypedDict(
     "PipelineExecutionTypeDef",
     {
         "pipelineName": NotRequired[str],
         "pipelineVersion": NotRequired[int],
         "pipelineExecutionId": NotRequired[str],
         "status": NotRequired[PipelineExecutionStatusType],
         "statusSummary": NotRequired[str],
         "artifactRevisions": NotRequired[List[ArtifactRevisionTypeDef]],
         "variables": NotRequired[List[ResolvedPipelineVariableTypeDef]],
         "trigger": NotRequired[ExecutionTriggerTypeDef],
         "executionMode": NotRequired[ExecutionModeType],
+        "executionType": NotRequired[ExecutionTypeType],
+        "rollbackMetadata": NotRequired[PipelineRollbackMetadataTypeDef],
     },
 )
 PollForThirdPartyJobsOutputTypeDef = TypedDict(
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1082,31 +1212,63 @@
     {
         "name": str,
         "variables": NotRequired[Sequence[PipelineVariableTypeDef]],
         "clientRequestToken": NotRequired[str],
         "sourceRevisions": NotRequired[Sequence[SourceRevisionOverrideTypeDef]],
     },
 )
+WebhookDefinitionExtraOutputTypeDef = TypedDict(
+    "WebhookDefinitionExtraOutputTypeDef",
+    {
+        "name": str,
+        "targetPipeline": str,
+        "targetAction": str,
+        "filters": List[WebhookFilterRuleTypeDef],
+        "authentication": WebhookAuthenticationTypeType,
+        "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
+    },
+)
+WebhookDefinitionOutputTypeDef = TypedDict(
+    "WebhookDefinitionOutputTypeDef",
+    {
+        "name": str,
+        "targetPipeline": str,
+        "targetAction": str,
+        "filters": List[WebhookFilterRuleTypeDef],
+        "authentication": WebhookAuthenticationTypeType,
+        "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
+    },
+)
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
         "targetPipeline": str,
         "targetAction": str,
-        "filters": List[WebhookFilterRuleTypeDef],
+        "filters": Sequence[WebhookFilterRuleTypeDef],
         "authentication": WebhookAuthenticationTypeType,
         "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
+StageDeclarationOutputTypeDef = TypedDict(
+    "StageDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "actions": List[ActionDeclarationOutputTypeDef],
+        "blockers": NotRequired[List[BlockerDeclarationTypeDef]],
+        "onFailure": NotRequired[FailureConditionsTypeDef],
+    },
+)
 StageDeclarationTypeDef = TypedDict(
     "StageDeclarationTypeDef",
     {
         "name": str,
         "actions": Sequence[ActionDeclarationTypeDef],
         "blockers": NotRequired[Sequence[BlockerDeclarationTypeDef]],
+        "onFailure": NotRequired[FailureConditionsTypeDef],
     },
 )
 ListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
     "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     {
         "pipelineName": str,
         "filter": NotRequired[ActionExecutionFilterTypeDef],
@@ -1122,20 +1284,50 @@
         "nextToken": NotRequired[str],
     },
 )
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": NotRequired[str],
-        "currentRevision": NotRequired[ActionRevisionTypeDef],
+        "currentRevision": NotRequired[ActionRevisionOutputTypeDef],
         "latestExecution": NotRequired[ActionExecutionTypeDef],
         "entityUrl": NotRequired[str],
         "revisionUrl": NotRequired[str],
     },
 )
+ActionRevisionUnionTypeDef = Union[ActionRevisionTypeDef, ActionRevisionOutputTypeDef]
+PutActionRevisionInputRequestTypeDef = TypedDict(
+    "PutActionRevisionInputRequestTypeDef",
+    {
+        "pipelineName": str,
+        "stageName": str,
+        "actionName": str,
+        "actionRevision": ActionRevisionTypeDef,
+    },
+)
+PutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "PutJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+        "currentRevision": NotRequired[CurrentRevisionTypeDef],
+        "continuationToken": NotRequired[str],
+        "executionDetails": NotRequired[ExecutionDetailsTypeDef],
+        "outputVariables": NotRequired[Mapping[str, str]],
+    },
+)
+PutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+        "clientToken": str,
+        "currentRevision": NotRequired[CurrentRevisionTypeDef],
+        "continuationToken": NotRequired[str],
+        "executionDetails": NotRequired[ExecutionDetailsTypeDef],
+    },
+)
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1172,51 +1364,65 @@
     "ArtifactTypeDef",
     {
         "name": NotRequired[str],
         "revision": NotRequired[str],
         "location": NotRequired[ArtifactLocationTypeDef],
     },
 )
-PutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "PutJobSuccessResultInputRequestTypeDef",
-    {
-        "jobId": str,
-        "currentRevision": NotRequired[CurrentRevisionTypeDef],
-        "continuationToken": NotRequired[str],
-        "executionDetails": NotRequired[ExecutionDetailsTypeDef],
-        "outputVariables": NotRequired[Mapping[str, str]],
-    },
-)
-PutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
+ActionTypeExecutorOutputTypeDef = TypedDict(
+    "ActionTypeExecutorOutputTypeDef",
     {
-        "jobId": str,
-        "clientToken": str,
-        "currentRevision": NotRequired[CurrentRevisionTypeDef],
-        "continuationToken": NotRequired[str],
-        "executionDetails": NotRequired[ExecutionDetailsTypeDef],
+        "configuration": ExecutorConfigurationOutputTypeDef,
+        "type": ExecutorTypeType,
+        "policyStatementsTemplate": NotRequired[str],
+        "jobTimeout": NotRequired[int],
     },
 )
 ActionTypeExecutorTypeDef = TypedDict(
     "ActionTypeExecutorTypeDef",
     {
         "configuration": ExecutorConfigurationTypeDef,
         "type": ExecutorTypeType,
         "policyStatementsTemplate": NotRequired[str],
         "jobTimeout": NotRequired[int],
     },
 )
+GitConfigurationOutputTypeDef = TypedDict(
+    "GitConfigurationOutputTypeDef",
+    {
+        "sourceActionName": str,
+        "push": NotRequired[List[GitPushFilterOutputTypeDef]],
+        "pullRequest": NotRequired[List[GitPullRequestFilterOutputTypeDef]],
+    },
+)
 GitConfigurationTypeDef = TypedDict(
     "GitConfigurationTypeDef",
     {
         "sourceActionName": str,
         "push": NotRequired[Sequence[GitPushFilterTypeDef]],
         "pullRequest": NotRequired[Sequence[GitPullRequestFilterTypeDef]],
     },
 )
+ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+        "filter": NotRequired[PipelineExecutionFilterTypeDef],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+ListPipelineExecutionsInputRequestTypeDef = TypedDict(
+    "ListPipelineExecutionsInputRequestTypeDef",
+    {
+        "pipelineName": str,
+        "maxResults": NotRequired[int],
+        "filter": NotRequired[PipelineExecutionFilterTypeDef],
+        "nextToken": NotRequired[str],
+    },
+)
 ListPipelineExecutionsOutputTypeDef = TypedDict(
     "ListPipelineExecutionsOutputTypeDef",
     {
         "pipelineExecutionSummaries": List[PipelineExecutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1227,15 +1433,15 @@
         "pipelineExecution": PipelineExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListWebhookItemTypeDef = TypedDict(
     "ListWebhookItemTypeDef",
     {
-        "definition": WebhookDefinitionTypeDef,
+        "definition": WebhookDefinitionOutputTypeDef,
         "url": str,
         "errorMessage": NotRequired[str],
         "errorCode": NotRequired[str],
         "lastTriggered": NotRequired[datetime],
         "arn": NotRequired[str],
         "tags": NotRequired[List[TagTypeDef]],
     },
@@ -1243,14 +1449,15 @@
 PutWebhookInputRequestTypeDef = TypedDict(
     "PutWebhookInputRequestTypeDef",
     {
         "webhook": WebhookDefinitionTypeDef,
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+WebhookDefinitionUnionTypeDef = Union[WebhookDefinitionTypeDef, WebhookDefinitionExtraOutputTypeDef]
 StageStateTypeDef = TypedDict(
     "StageStateTypeDef",
     {
         "stageName": NotRequired[str],
         "inboundExecution": NotRequired[StageExecutionTypeDef],
         "inboundExecutions": NotRequired[List[StageExecutionTypeDef]],
         "inboundTransitionState": NotRequired[TransitionStateTypeDef],
@@ -1296,40 +1503,60 @@
         "inputArtifacts": NotRequired[List[ArtifactTypeDef]],
         "outputArtifacts": NotRequired[List[ArtifactTypeDef]],
         "artifactCredentials": NotRequired[AWSSessionCredentialsTypeDef],
         "continuationToken": NotRequired[str],
         "encryptionKey": NotRequired[EncryptionKeyTypeDef],
     },
 )
+ActionTypeDeclarationOutputTypeDef = TypedDict(
+    "ActionTypeDeclarationOutputTypeDef",
+    {
+        "executor": ActionTypeExecutorOutputTypeDef,
+        "id": ActionTypeIdentifierTypeDef,
+        "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
+        "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
+        "description": NotRequired[str],
+        "permissions": NotRequired[ActionTypePermissionsOutputTypeDef],
+        "properties": NotRequired[List[ActionTypePropertyTypeDef]],
+        "urls": NotRequired[ActionTypeUrlsTypeDef],
+    },
+)
 ActionTypeDeclarationTypeDef = TypedDict(
     "ActionTypeDeclarationTypeDef",
     {
         "executor": ActionTypeExecutorTypeDef,
         "id": ActionTypeIdentifierTypeDef,
         "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "description": NotRequired[str],
         "permissions": NotRequired[ActionTypePermissionsTypeDef],
-        "properties": NotRequired[List[ActionTypePropertyTypeDef]],
+        "properties": NotRequired[Sequence[ActionTypePropertyTypeDef]],
         "urls": NotRequired[ActionTypeUrlsTypeDef],
     },
 )
+PipelineTriggerDeclarationOutputTypeDef = TypedDict(
+    "PipelineTriggerDeclarationOutputTypeDef",
+    {
+        "providerType": Literal["CodeStarSourceConnection"],
+        "gitConfiguration": GitConfigurationOutputTypeDef,
+    },
+)
 PipelineTriggerDeclarationTypeDef = TypedDict(
     "PipelineTriggerDeclarationTypeDef",
     {
         "providerType": Literal["CodeStarSourceConnection"],
         "gitConfiguration": GitConfigurationTypeDef,
     },
 )
 ListWebhooksOutputTypeDef = TypedDict(
     "ListWebhooksOutputTypeDef",
     {
         "webhooks": List[ListWebhookItemTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PutWebhookOutputTypeDef = TypedDict(
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1378,24 +1605,42 @@
         "data": NotRequired[ThirdPartyJobDataTypeDef],
         "nonce": NotRequired[str],
     },
 )
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
-        "actionType": ActionTypeDeclarationTypeDef,
+        "actionType": ActionTypeDeclarationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ActionTypeDeclarationUnionTypeDef = Union[
+    ActionTypeDeclarationTypeDef, ActionTypeDeclarationOutputTypeDef
+]
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
+PipelineDeclarationOutputTypeDef = TypedDict(
+    "PipelineDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "stages": List[StageDeclarationOutputTypeDef],
+        "artifactStore": NotRequired[ArtifactStoreTypeDef],
+        "artifactStores": NotRequired[Dict[str, ArtifactStoreTypeDef]],
+        "version": NotRequired[int],
+        "executionMode": NotRequired[ExecutionModeType],
+        "pipelineType": NotRequired[PipelineTypeType],
+        "variables": NotRequired[List[PipelineVariableDeclarationTypeDef]],
+        "triggers": NotRequired[List[PipelineTriggerDeclarationOutputTypeDef]],
+    },
+)
 PipelineDeclarationTypeDef = TypedDict(
     "PipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
         "artifactStore": NotRequired[ArtifactStoreTypeDef],
@@ -1424,43 +1669,46 @@
 GetThirdPartyJobDetailsOutputTypeDef = TypedDict(
     "GetThirdPartyJobDetailsOutputTypeDef",
     {
         "jobDetails": ThirdPartyJobDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreatePipelineInputRequestTypeDef = TypedDict(
-    "CreatePipelineInputRequestTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 CreatePipelineOutputTypeDef = TypedDict(
     "CreatePipelineOutputTypeDef",
     {
-        "pipeline": PipelineDeclarationTypeDef,
+        "pipeline": PipelineDeclarationOutputTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetPipelineOutputTypeDef = TypedDict(
     "GetPipelineOutputTypeDef",
     {
-        "pipeline": PipelineDeclarationTypeDef,
+        "pipeline": PipelineDeclarationOutputTypeDef,
         "metadata": PipelineMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdatePipelineInputRequestTypeDef = TypedDict(
-    "UpdatePipelineInputRequestTypeDef",
+UpdatePipelineOutputTypeDef = TypedDict(
+    "UpdatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreatePipelineInputRequestTypeDef = TypedDict(
+    "CreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
+        "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-UpdatePipelineOutputTypeDef = TypedDict(
-    "UpdatePipelineOutputTypeDef",
+PipelineDeclarationUnionTypeDef = Union[
+    PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef
+]
+UpdatePipelineInputRequestTypeDef = TypedDict(
+    "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline.egg-info/PKG-INFO` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codepipeline
-Version: 1.34.43
-Summary: Type annotations for boto3.CodePipeline 1.34.43 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.93
+Summary: Type annotations for boto3.CodePipeline 1.34.93 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-codepipeline-1.34.43/mypy_boto3_codepipeline.egg-info/SOURCES.txt` & `mypy_boto3_codepipeline-1.34.93/mypy_boto3_codepipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.34.43/setup.py` & `mypy_boto3_codepipeline-1.34.93/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codepipeline",
-    version="1.34.43",
+    version="1.34.93",
     packages=["mypy_boto3_codepipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CodePipeline 1.34.43 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.CodePipeline 1.34.93 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

