# Comparing `tmp/mypy-boto3-oam-1.34.73.tar.gz` & `tmp/mypy_boto3_oam-1.34.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-oam-1.34.73.tar", last modified: Thu Mar 28 19:34:42 2024, max compression
+gzip compressed data, was "mypy_boto3_oam-1.34.93.tar", last modified: Fri Apr 26 19:32:23 2024, max compression
```

## Comparing `mypy-boto3-oam-1.34.73.tar` & `mypy_boto3_oam-1.34.93.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:42.712076 mypy-boto3-oam-1.34.73/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-03-28 19:34:42.712076 mypy-boto3-oam-1.34.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11525 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:42.708076 mypy-boto3-oam-1.34.73/mypy_boto3_oam/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-03-28 19:32:51.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-03-28 19:32:51.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:42.712076 mypy-boto3-oam-1.34.73/mypy_boto3_oam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-03-28 19:34:42.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-28 19:34:42.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:34:42.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:34:42.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 19:34:42.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-28 19:34:42.000000 mypy-boto3-oam-1.34.73/mypy_boto3_oam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:34:42.712076 mypy-boto3-oam-1.34.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-03-28 19:32:50.000000 mypy-boto3-oam-1.34.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:23.191547 mypy_boto3_oam-1.34.93/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-04-26 19:32:23.191547 mypy_boto3_oam-1.34.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:23.191547 mypy_boto3_oam-1.34.93/mypy_boto3_oam/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13484 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-26 19:31:59.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-26 19:31:59.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-04-26 19:31:59.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-04-26 19:31:59.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:23.191547 mypy_boto3_oam-1.34.93/mypy_boto3_oam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-04-26 19:32:23.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-26 19:32:23.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:23.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:23.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 19:32:23.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 19:32:23.000000 mypy_boto3_oam-1.34.93/mypy_boto3_oam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:32:23.191547 mypy_boto3_oam-1.34.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-26 19:31:58.000000 mypy_boto3_oam-1.34.93/setup.py
```

### Comparing `mypy-boto3-oam-1.34.73/LICENSE` & `mypy_boto3_oam-1.34.93/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-oam-1.34.73/PKG-INFO` & `mypy_boto3_oam-1.34.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-oam
-Version: 1.34.73
-Summary: Type annotations for boto3.CloudWatchObservabilityAccessManager 1.34.73 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.93
+Summary: Type annotations for boto3.CloudWatchObservabilityAccessManager 1.34.93 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-oam.svg?color=blue)](https://pypi.org/project/mypy-boto3-oam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-oam)](https://pepy.tech/project/mypy-boto3-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchObservabilityAccessManager 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
+[boto3.CloudWatchObservabilityAccessManager 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-oam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,18 +325,18 @@
 `mypy_boto3_oam.type_defs` module contains structures and shapes assembled to
 typed dictionaries and unions for additional type checking.
 
 Full list of `CloudWatchObservabilityAccessManager` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/type_defs/).
 
 ```python
-from mypy_boto3_oam.type_defs import CreateLinkInputRequestTypeDef
+from mypy_boto3_oam.type_defs import ResponseMetadataTypeDef
 
 
-def get_value() -> CreateLinkInputRequestTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-oam-1.34.73/README.md` & `mypy_boto3_oam-1.34.93/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-oam.svg?color=blue)](https://pypi.org/project/mypy-boto3-oam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-oam)](https://pepy.tech/project/mypy-boto3-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchObservabilityAccessManager 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
+[boto3.CloudWatchObservabilityAccessManager 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-oam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,18 +292,18 @@
 `mypy_boto3_oam.type_defs` module contains structures and shapes assembled to
 typed dictionaries and unions for additional type checking.
 
 Full list of `CloudWatchObservabilityAccessManager` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/type_defs/).
 
 ```python
-from mypy_boto3_oam.type_defs import CreateLinkInputRequestTypeDef
+from mypy_boto3_oam.type_defs import ResponseMetadataTypeDef
 
 
-def get_value() -> CreateLinkInputRequestTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam/__init__.py` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam/__init__.pyi` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam/__main__.py` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchObservabilityAccessManager 1.34.73\n"
-        "Version:         1.34.73\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.CloudWatchObservabilityAccessManager 1.34.93\n"
+        "Version:         1.34.93\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.73")
+    print("1.34.93")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam/client.py` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .paginator import ListAttachedLinksPaginator, ListLinksPaginator, ListSinksPaginator
 from .type_defs import (
     CreateLinkOutputTypeDef,
     CreateSinkOutputTypeDef,
     GetLinkOutputTypeDef,
     GetSinkOutputTypeDef,
     GetSinkPolicyOutputTypeDef,
+    LinkConfigurationTypeDef,
     ListAttachedLinksOutputTypeDef,
     ListLinksOutputTypeDef,
     ListSinksOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     PutSinkPolicyOutputTypeDef,
     UpdateLinkOutputTypeDef,
 )
@@ -98,14 +99,15 @@
 
     def create_link(
         self,
         *,
         LabelTemplate: str,
         ResourceTypes: Sequence[ResourceTypeType],
         SinkIdentifier: str,
+        LinkConfiguration: LinkConfigurationTypeDef = ...,
         Tags: Mapping[str, str] = ...,
     ) -> CreateLinkOutputTypeDef:
         """
         Creates a link between a source account and a sink that you have created in a
         monitoring
         account.
 
@@ -213,15 +215,15 @@
         """
         Displays the tags associated with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/client/#list_tags_for_resource)
         """
 
-    def put_sink_policy(self, *, SinkIdentifier: str, Policy: str) -> PutSinkPolicyOutputTypeDef:
+    def put_sink_policy(self, *, Policy: str, SinkIdentifier: str) -> PutSinkPolicyOutputTypeDef:
         """
         Creates or updates the resource policy that grants permissions to source
         accounts to link to the monitoring account
         sink.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Client.put_sink_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/client/#put_sink_policy)
@@ -240,15 +242,19 @@
         Removes one or more tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/client/#untag_resource)
         """
 
     def update_link(
-        self, *, Identifier: str, ResourceTypes: Sequence[ResourceTypeType]
+        self,
+        *,
+        Identifier: str,
+        ResourceTypes: Sequence[ResourceTypeType],
+        LinkConfiguration: LinkConfigurationTypeDef = ...,
     ) -> UpdateLinkOutputTypeDef:
         """
         Use this operation to change what types of data are shared from a source
         account to its linked monitoring account
         sink.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Client.update_link)
```

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam/client.pyi` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .paginator import ListAttachedLinksPaginator, ListLinksPaginator, ListSinksPaginator
 from .type_defs import (
     CreateLinkOutputTypeDef,
     CreateSinkOutputTypeDef,
     GetLinkOutputTypeDef,
     GetSinkOutputTypeDef,
     GetSinkPolicyOutputTypeDef,
+    LinkConfigurationTypeDef,
     ListAttachedLinksOutputTypeDef,
     ListLinksOutputTypeDef,
     ListSinksOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     PutSinkPolicyOutputTypeDef,
     UpdateLinkOutputTypeDef,
 )
@@ -95,14 +96,15 @@
 
     def create_link(
         self,
         *,
         LabelTemplate: str,
         ResourceTypes: Sequence[ResourceTypeType],
         SinkIdentifier: str,
+        LinkConfiguration: LinkConfigurationTypeDef = ...,
         Tags: Mapping[str, str] = ...,
     ) -> CreateLinkOutputTypeDef:
         """
         Creates a link between a source account and a sink that you have created in a
         monitoring
         account.
 
@@ -210,15 +212,15 @@
         """
         Displays the tags associated with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/client/#list_tags_for_resource)
         """
 
-    def put_sink_policy(self, *, SinkIdentifier: str, Policy: str) -> PutSinkPolicyOutputTypeDef:
+    def put_sink_policy(self, *, Policy: str, SinkIdentifier: str) -> PutSinkPolicyOutputTypeDef:
         """
         Creates or updates the resource policy that grants permissions to source
         accounts to link to the monitoring account
         sink.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Client.put_sink_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/client/#put_sink_policy)
@@ -237,15 +239,19 @@
         Removes one or more tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/client/#untag_resource)
         """
 
     def update_link(
-        self, *, Identifier: str, ResourceTypes: Sequence[ResourceTypeType]
+        self,
+        *,
+        Identifier: str,
+        ResourceTypes: Sequence[ResourceTypeType],
+        LinkConfiguration: LinkConfigurationTypeDef = ...,
     ) -> UpdateLinkOutputTypeDef:
         """
         Use this operation to change what types of data are shared from a source
         account to its linked monitoring account
         sink.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Client.update_link)
```

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam/literals.py` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
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
@@ -129,24 +130,26 @@
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
@@ -343,14 +346,15 @@
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
```

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam/literals.pyi` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
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
@@ -129,24 +130,26 @@
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
@@ -343,14 +346,15 @@
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
```

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam/paginator.py` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam/paginator.pyi` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam/type_defs.py` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for oam service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_oam.type_defs import CreateLinkInputRequestTypeDef
+    from mypy_boto3_oam.type_defs import ResponseMetadataTypeDef
 
-    data: CreateLinkInputRequestTypeDef = ...
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ResourceTypeType
@@ -23,59 +23,53 @@
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "CreateLinkInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateSinkInputRequestTypeDef",
     "DeleteLinkInputRequestTypeDef",
     "DeleteSinkInputRequestTypeDef",
     "GetLinkInputRequestTypeDef",
     "GetSinkInputRequestTypeDef",
     "GetSinkPolicyInputRequestTypeDef",
+    "LogGroupConfigurationTypeDef",
+    "MetricConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "ListAttachedLinksInputRequestTypeDef",
     "ListAttachedLinksItemTypeDef",
     "ListLinksInputRequestTypeDef",
     "ListLinksItemTypeDef",
     "ListSinksInputRequestTypeDef",
     "ListSinksItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "PutSinkPolicyInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "UpdateLinkInputRequestTypeDef",
-    "CreateLinkOutputTypeDef",
     "CreateSinkOutputTypeDef",
-    "GetLinkOutputTypeDef",
     "GetSinkOutputTypeDef",
     "GetSinkPolicyOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "PutSinkPolicyOutputTypeDef",
-    "UpdateLinkOutputTypeDef",
+    "LinkConfigurationTypeDef",
     "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
     "ListLinksInputListLinksPaginateTypeDef",
     "ListSinksInputListSinksPaginateTypeDef",
     "ListAttachedLinksOutputTypeDef",
     "ListLinksOutputTypeDef",
     "ListSinksOutputTypeDef",
-)
-
-CreateLinkInputRequestTypeDef = TypedDict(
     "CreateLinkInputRequestTypeDef",
-    {
-        "LabelTemplate": str,
-        "ResourceTypes": Sequence[ResourceTypeType],
-        "SinkIdentifier": str,
-        "Tags": NotRequired[Mapping[str, str]],
-    },
+    "CreateLinkOutputTypeDef",
+    "GetLinkOutputTypeDef",
+    "UpdateLinkInputRequestTypeDef",
+    "UpdateLinkOutputTypeDef",
 )
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
@@ -115,14 +109,26 @@
 )
 GetSinkPolicyInputRequestTypeDef = TypedDict(
     "GetSinkPolicyInputRequestTypeDef",
     {
         "SinkIdentifier": str,
     },
 )
+LogGroupConfigurationTypeDef = TypedDict(
+    "LogGroupConfigurationTypeDef",
+    {
+        "Filter": str,
+    },
+)
+MetricConfigurationTypeDef = TypedDict(
+    "MetricConfigurationTypeDef",
+    {
+        "Filter": str,
+    },
+)
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
         "PageSize": NotRequired[int],
         "StartingToken": NotRequired[str],
     },
@@ -180,16 +186,16 @@
     {
         "ResourceArn": str,
     },
 )
 PutSinkPolicyInputRequestTypeDef = TypedDict(
     "PutSinkPolicyInputRequestTypeDef",
     {
-        "SinkIdentifier": str,
         "Policy": str,
+        "SinkIdentifier": str,
     },
 )
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
@@ -198,103 +204,64 @@
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
-UpdateLinkInputRequestTypeDef = TypedDict(
-    "UpdateLinkInputRequestTypeDef",
-    {
-        "Identifier": str,
-        "ResourceTypes": Sequence[ResourceTypeType],
-    },
-)
-CreateLinkOutputTypeDef = TypedDict(
-    "CreateLinkOutputTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateSinkOutputTypeDef = TypedDict(
     "CreateSinkOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetLinkOutputTypeDef = TypedDict(
-    "GetLinkOutputTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 GetSinkOutputTypeDef = TypedDict(
     "GetSinkOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetSinkPolicyOutputTypeDef = TypedDict(
     "GetSinkPolicyOutputTypeDef",
     {
+        "Policy": str,
         "SinkArn": str,
         "SinkId": str,
-        "Policy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutSinkPolicyOutputTypeDef = TypedDict(
     "PutSinkPolicyOutputTypeDef",
     {
+        "Policy": str,
         "SinkArn": str,
         "SinkId": str,
-        "Policy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateLinkOutputTypeDef = TypedDict(
-    "UpdateLinkOutputTypeDef",
+LinkConfigurationTypeDef = TypedDict(
+    "LinkConfigurationTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LogGroupConfiguration": NotRequired[LogGroupConfigurationTypeDef],
+        "MetricConfiguration": NotRequired[MetricConfigurationTypeDef],
     },
 )
 ListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
     "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
     {
         "SinkIdentifier": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -312,27 +279,87 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListAttachedLinksOutputTypeDef = TypedDict(
     "ListAttachedLinksOutputTypeDef",
     {
         "Items": List[ListAttachedLinksItemTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListLinksOutputTypeDef = TypedDict(
     "ListLinksOutputTypeDef",
     {
         "Items": List[ListLinksItemTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSinksOutputTypeDef = TypedDict(
     "ListSinksOutputTypeDef",
     {
         "Items": List[ListSinksItemTypeDef],
-        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+CreateLinkInputRequestTypeDef = TypedDict(
+    "CreateLinkInputRequestTypeDef",
+    {
+        "LabelTemplate": str,
+        "ResourceTypes": Sequence[ResourceTypeType],
+        "SinkIdentifier": str,
+        "LinkConfiguration": NotRequired[LinkConfigurationTypeDef],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+CreateLinkOutputTypeDef = TypedDict(
+    "CreateLinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "LinkConfiguration": LinkConfigurationTypeDef,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetLinkOutputTypeDef = TypedDict(
+    "GetLinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "LinkConfiguration": LinkConfigurationTypeDef,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateLinkInputRequestTypeDef = TypedDict(
+    "UpdateLinkInputRequestTypeDef",
+    {
+        "Identifier": str,
+        "ResourceTypes": Sequence[ResourceTypeType],
+        "LinkConfiguration": NotRequired[LinkConfigurationTypeDef],
+    },
+)
+UpdateLinkOutputTypeDef = TypedDict(
+    "UpdateLinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "LinkConfiguration": LinkConfigurationTypeDef,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam/type_defs.pyi` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for oam service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_oam.type_defs import CreateLinkInputRequestTypeDef
+    from mypy_boto3_oam.type_defs import ResponseMetadataTypeDef
 
-    data: CreateLinkInputRequestTypeDef = ...
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ResourceTypeType
@@ -23,59 +23,53 @@
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "CreateLinkInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateSinkInputRequestTypeDef",
     "DeleteLinkInputRequestTypeDef",
     "DeleteSinkInputRequestTypeDef",
     "GetLinkInputRequestTypeDef",
     "GetSinkInputRequestTypeDef",
     "GetSinkPolicyInputRequestTypeDef",
+    "LogGroupConfigurationTypeDef",
+    "MetricConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "ListAttachedLinksInputRequestTypeDef",
     "ListAttachedLinksItemTypeDef",
     "ListLinksInputRequestTypeDef",
     "ListLinksItemTypeDef",
     "ListSinksInputRequestTypeDef",
     "ListSinksItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "PutSinkPolicyInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "UpdateLinkInputRequestTypeDef",
-    "CreateLinkOutputTypeDef",
     "CreateSinkOutputTypeDef",
-    "GetLinkOutputTypeDef",
     "GetSinkOutputTypeDef",
     "GetSinkPolicyOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "PutSinkPolicyOutputTypeDef",
-    "UpdateLinkOutputTypeDef",
+    "LinkConfigurationTypeDef",
     "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
     "ListLinksInputListLinksPaginateTypeDef",
     "ListSinksInputListSinksPaginateTypeDef",
     "ListAttachedLinksOutputTypeDef",
     "ListLinksOutputTypeDef",
     "ListSinksOutputTypeDef",
-)
-
-CreateLinkInputRequestTypeDef = TypedDict(
     "CreateLinkInputRequestTypeDef",
-    {
-        "LabelTemplate": str,
-        "ResourceTypes": Sequence[ResourceTypeType],
-        "SinkIdentifier": str,
-        "Tags": NotRequired[Mapping[str, str]],
-    },
+    "CreateLinkOutputTypeDef",
+    "GetLinkOutputTypeDef",
+    "UpdateLinkInputRequestTypeDef",
+    "UpdateLinkOutputTypeDef",
 )
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
@@ -115,14 +109,26 @@
 )
 GetSinkPolicyInputRequestTypeDef = TypedDict(
     "GetSinkPolicyInputRequestTypeDef",
     {
         "SinkIdentifier": str,
     },
 )
+LogGroupConfigurationTypeDef = TypedDict(
+    "LogGroupConfigurationTypeDef",
+    {
+        "Filter": str,
+    },
+)
+MetricConfigurationTypeDef = TypedDict(
+    "MetricConfigurationTypeDef",
+    {
+        "Filter": str,
+    },
+)
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
         "PageSize": NotRequired[int],
         "StartingToken": NotRequired[str],
     },
@@ -180,16 +186,16 @@
     {
         "ResourceArn": str,
     },
 )
 PutSinkPolicyInputRequestTypeDef = TypedDict(
     "PutSinkPolicyInputRequestTypeDef",
     {
-        "SinkIdentifier": str,
         "Policy": str,
+        "SinkIdentifier": str,
     },
 )
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
@@ -198,103 +204,64 @@
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
-UpdateLinkInputRequestTypeDef = TypedDict(
-    "UpdateLinkInputRequestTypeDef",
-    {
-        "Identifier": str,
-        "ResourceTypes": Sequence[ResourceTypeType],
-    },
-)
-CreateLinkOutputTypeDef = TypedDict(
-    "CreateLinkOutputTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateSinkOutputTypeDef = TypedDict(
     "CreateSinkOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetLinkOutputTypeDef = TypedDict(
-    "GetLinkOutputTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 GetSinkOutputTypeDef = TypedDict(
     "GetSinkOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetSinkPolicyOutputTypeDef = TypedDict(
     "GetSinkPolicyOutputTypeDef",
     {
+        "Policy": str,
         "SinkArn": str,
         "SinkId": str,
-        "Policy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutSinkPolicyOutputTypeDef = TypedDict(
     "PutSinkPolicyOutputTypeDef",
     {
+        "Policy": str,
         "SinkArn": str,
         "SinkId": str,
-        "Policy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateLinkOutputTypeDef = TypedDict(
-    "UpdateLinkOutputTypeDef",
+LinkConfigurationTypeDef = TypedDict(
+    "LinkConfigurationTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LogGroupConfiguration": NotRequired[LogGroupConfigurationTypeDef],
+        "MetricConfiguration": NotRequired[MetricConfigurationTypeDef],
     },
 )
 ListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
     "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
     {
         "SinkIdentifier": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -312,27 +279,87 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListAttachedLinksOutputTypeDef = TypedDict(
     "ListAttachedLinksOutputTypeDef",
     {
         "Items": List[ListAttachedLinksItemTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListLinksOutputTypeDef = TypedDict(
     "ListLinksOutputTypeDef",
     {
         "Items": List[ListLinksItemTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSinksOutputTypeDef = TypedDict(
     "ListSinksOutputTypeDef",
     {
         "Items": List[ListSinksItemTypeDef],
-        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+CreateLinkInputRequestTypeDef = TypedDict(
+    "CreateLinkInputRequestTypeDef",
+    {
+        "LabelTemplate": str,
+        "ResourceTypes": Sequence[ResourceTypeType],
+        "SinkIdentifier": str,
+        "LinkConfiguration": NotRequired[LinkConfigurationTypeDef],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+CreateLinkOutputTypeDef = TypedDict(
+    "CreateLinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "LinkConfiguration": LinkConfigurationTypeDef,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetLinkOutputTypeDef = TypedDict(
+    "GetLinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "LinkConfiguration": LinkConfigurationTypeDef,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateLinkInputRequestTypeDef = TypedDict(
+    "UpdateLinkInputRequestTypeDef",
+    {
+        "Identifier": str,
+        "ResourceTypes": Sequence[ResourceTypeType],
+        "LinkConfiguration": NotRequired[LinkConfigurationTypeDef],
+    },
+)
+UpdateLinkOutputTypeDef = TypedDict(
+    "UpdateLinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "LinkConfiguration": LinkConfigurationTypeDef,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam.egg-info/PKG-INFO` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-oam
-Version: 1.34.73
-Summary: Type annotations for boto3.CloudWatchObservabilityAccessManager 1.34.73 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.93
+Summary: Type annotations for boto3.CloudWatchObservabilityAccessManager 1.34.93 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-oam.svg?color=blue)](https://pypi.org/project/mypy-boto3-oam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-oam)](https://pepy.tech/project/mypy-boto3-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchObservabilityAccessManager 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
+[boto3.CloudWatchObservabilityAccessManager 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-oam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,18 +325,18 @@
 `mypy_boto3_oam.type_defs` module contains structures and shapes assembled to
 typed dictionaries and unions for additional type checking.
 
 Full list of `CloudWatchObservabilityAccessManager` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_oam/type_defs/).
 
 ```python
-from mypy_boto3_oam.type_defs import CreateLinkInputRequestTypeDef
+from mypy_boto3_oam.type_defs import ResponseMetadataTypeDef
 
 
-def get_value() -> CreateLinkInputRequestTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-oam-1.34.73/mypy_boto3_oam.egg-info/SOURCES.txt` & `mypy_boto3_oam-1.34.93/mypy_boto3_oam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-oam-1.34.73/setup.py` & `mypy_boto3_oam-1.34.93/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-oam",
-    version="1.34.73",
+    version="1.34.93",
     packages=["mypy_boto3_oam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CloudWatchObservabilityAccessManager 1.34.73 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.CloudWatchObservabilityAccessManager 1.34.93 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

