# Comparing `tmp/mypy-boto3-support-1.34.0.tar.gz` & `tmp/mypy_boto3_support-1.34.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-support-1.34.0.tar", last modified: Wed Dec 13 21:24:00 2023, max compression
+gzip compressed data, was "mypy_boto3_support-1.34.93.tar", last modified: Fri Apr 26 19:32:23 2024, max compression
```

## Comparing `mypy-boto3-support-1.34.0.tar` & `mypy_boto3_support-1.34.93.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:00.027400 mypy-boto3-support-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12817 2023-12-13 21:24:00.027400 mypy-boto3-support-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:00.023400 mypy-boto3-support-1.34.0/mypy_boto3_support/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14921 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8384 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16650 2023-12-13 21:20:33.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16649 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/mypy_boto3_support/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:00.027400 mypy-boto3-support-1.34.0/mypy_boto3_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12817 2023-12-13 21:23:59.000000 mypy-boto3-support-1.34.0/mypy_boto3_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-12-13 21:24:00.000000 mypy-boto3-support-1.34.0/mypy_boto3_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:59.000000 mypy-boto3-support-1.34.0/mypy_boto3_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:59.000000 mypy-boto3-support-1.34.0/mypy_boto3_support.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:59.000000 mypy-boto3-support-1.34.0/mypy_boto3_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-13 21:23:59.000000 mypy-boto3-support-1.34.0/mypy_boto3_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:24:00.027400 mypy-boto3-support-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-12-13 21:20:32.000000 mypy-boto3-support-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:23.903554 mypy_boto3_support-1.34.93/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 19:32:09.000000 mypy_boto3_support-1.34.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-04-26 19:32:23.903554 mypy_boto3_support-1.34.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-04-26 19:32:09.000000 mypy_boto3_support-1.34.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:23.903554 mypy_boto3_support-1.34.93/mypy_boto3_support/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-26 19:32:09.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-26 19:32:09.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-26 19:32:09.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14934 2024-04-26 19:32:09.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-04-26 19:32:09.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-26 19:32:10.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-26 19:32:10.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-26 19:32:10.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-26 19:32:09.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:09.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-04-26 19:32:11.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-04-26 19:32:10.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 19:32:09.000000 mypy_boto3_support-1.34.93/mypy_boto3_support/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:23.903554 mypy_boto3_support-1.34.93/mypy_boto3_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-04-26 19:32:23.000000 mypy_boto3_support-1.34.93/mypy_boto3_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-26 19:32:23.000000 mypy_boto3_support-1.34.93/mypy_boto3_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:23.000000 mypy_boto3_support-1.34.93/mypy_boto3_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:23.000000 mypy_boto3_support-1.34.93/mypy_boto3_support.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 19:32:23.000000 mypy_boto3_support-1.34.93/mypy_boto3_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 19:32:23.000000 mypy_boto3_support-1.34.93/mypy_boto3_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:32:23.903554 mypy_boto3_support-1.34.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-26 19:32:09.000000 mypy_boto3_support-1.34.93/setup.py
```

### Comparing `mypy-boto3-support-1.34.0/LICENSE` & `mypy_boto3_support-1.34.93/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-support-1.34.0/PKG-INFO` & `mypy_boto3_support-1.34.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.34.0
-Summary: Type annotations for boto3.Support 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.93
+Summary: Type annotations for boto3.Support 1.34.93 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-support"></a>
 
 # mypy-boto3-support
 
 [![PyPI - mypy-boto3-support](https://img.shields.io/pypi/v/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-support)](https://pepy.tech/project/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-support-1.34.0/README.md` & `mypy_boto3_support-1.34.93/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-support)](https://pepy.tech/project/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support/__init__.py` & `mypy_boto3_support-1.34.93/mypy_boto3_support/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,9 +21,8 @@
 """
 
 from .client import SupportClient
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 
 Client = SupportClient
 
-
 __all__ = ("Client", "DescribeCasesPaginator", "DescribeCommunicationsPaginator", "SupportClient")
```

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support/__init__.pyi` & `mypy_boto3_support-1.34.93/mypy_boto3_support/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support/__main__.py` & `mypy_boto3_support-1.34.93/mypy_boto3_support/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Support 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Support 1.34.93\n"
+        "Version:         1.34.93\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.93")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support/client.py` & `mypy_boto3_support-1.34.93/mypy_boto3_support/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 from .type_defs import (
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
-    AttachmentTypeDef,
+    AttachmentUnionTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
@@ -41,15 +41,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SupportClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -85,30 +84,30 @@
         SupportClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#exceptions)
         """
 
     def add_attachments_to_set(
-        self, *, attachments: Sequence[AttachmentTypeDef], attachmentSetId: str = ...
+        self, *, attachments: Sequence[AttachmentUnionTypeDef], attachmentSetId: str = ...
     ) -> AddAttachmentsToSetResponseTypeDef:
         """
         Adds one or more attachments to an attachment set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_attachments_to_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#add_attachments_to_set)
         """
 
     def add_communication_to_case(
         self,
         *,
         communicationBody: str,
         caseId: str = ...,
         ccEmailAddresses: Sequence[str] = ...,
-        attachmentSetId: str = ...
+        attachmentSetId: str = ...,
     ) -> AddCommunicationToCaseResponseTypeDef:
         """
         Adds additional customer communication to an Amazon Web Services Support case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_communication_to_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#add_communication_to_case)
         """
@@ -136,15 +135,15 @@
         communicationBody: str,
         serviceCode: str = ...,
         severityCode: str = ...,
         categoryCode: str = ...,
         ccEmailAddresses: Sequence[str] = ...,
         language: str = ...,
         issueType: str = ...,
-        attachmentSetId: str = ...
+        attachmentSetId: str = ...,
     ) -> CreateCaseResponseTypeDef:
         """
         Creates a case in the Amazon Web Services Support Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.create_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#create_case)
         """
@@ -164,15 +163,15 @@
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         language: str = ...,
-        includeCommunications: bool = ...
+        includeCommunications: bool = ...,
     ) -> DescribeCasesResponseTypeDef:
         """
         Returns a list of cases that you specify by passing one or more case IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_cases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_cases)
         """
@@ -180,15 +179,15 @@
     def describe_communications(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeCommunicationsResponseTypeDef:
         """
         Returns communications and attachments for one or more support cases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_communications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_communications)
         """
```

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support/client.pyi` & `mypy_boto3_support-1.34.93/mypy_boto3_support/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 from .type_defs import (
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
-    AttachmentTypeDef,
+    AttachmentUnionTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
@@ -81,30 +81,30 @@
         SupportClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#exceptions)
         """
 
     def add_attachments_to_set(
-        self, *, attachments: Sequence[AttachmentTypeDef], attachmentSetId: str = ...
+        self, *, attachments: Sequence[AttachmentUnionTypeDef], attachmentSetId: str = ...
     ) -> AddAttachmentsToSetResponseTypeDef:
         """
         Adds one or more attachments to an attachment set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_attachments_to_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#add_attachments_to_set)
         """
 
     def add_communication_to_case(
         self,
         *,
         communicationBody: str,
         caseId: str = ...,
         ccEmailAddresses: Sequence[str] = ...,
-        attachmentSetId: str = ...
+        attachmentSetId: str = ...,
     ) -> AddCommunicationToCaseResponseTypeDef:
         """
         Adds additional customer communication to an Amazon Web Services Support case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_communication_to_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#add_communication_to_case)
         """
@@ -132,15 +132,15 @@
         communicationBody: str,
         serviceCode: str = ...,
         severityCode: str = ...,
         categoryCode: str = ...,
         ccEmailAddresses: Sequence[str] = ...,
         language: str = ...,
         issueType: str = ...,
-        attachmentSetId: str = ...
+        attachmentSetId: str = ...,
     ) -> CreateCaseResponseTypeDef:
         """
         Creates a case in the Amazon Web Services Support Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.create_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#create_case)
         """
@@ -160,15 +160,15 @@
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         language: str = ...,
-        includeCommunications: bool = ...
+        includeCommunications: bool = ...,
     ) -> DescribeCasesResponseTypeDef:
         """
         Returns a list of cases that you specify by passing one or more case IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_cases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_cases)
         """
@@ -176,15 +176,15 @@
     def describe_communications(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeCommunicationsResponseTypeDef:
         """
         Returns communications and attachments for one or more support cases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_communications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#describe_communications)
         """
```

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support/literals.py` & `mypy_boto3_support-1.34.93/mypy_boto3_support/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeCasesPaginatorName",
     "DescribeCommunicationsPaginatorName",
     "SupportServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 DescribeCasesPaginatorName = Literal["describe_cases"]
 DescribeCommunicationsPaginatorName = Literal["describe_communications"]
 SupportServiceName = Literal["support"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -55,14 +53,15 @@
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
@@ -73,14 +72,15 @@
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
@@ -98,14 +98,15 @@
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
@@ -118,24 +119,26 @@
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
@@ -196,15 +199,14 @@
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
@@ -276,17 +278,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -331,14 +335,15 @@
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
@@ -376,19 +381,21 @@
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

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support/literals.pyi` & `mypy_boto3_support-1.34.93/mypy_boto3_support/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,15 @@
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
@@ -71,14 +72,15 @@
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
@@ -96,14 +98,15 @@
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
@@ -116,24 +119,26 @@
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
@@ -194,15 +199,14 @@
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
@@ -274,17 +278,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -329,14 +335,15 @@
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
@@ -374,19 +381,21 @@
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

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support/paginator.py` & `mypy_boto3_support-1.34.93/mypy_boto3_support/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeCasesPaginator", "DescribeCommunicationsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -57,15 +56,15 @@
         caseIdList: Sequence[str] = ...,
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         language: str = ...,
         includeCommunications: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecasespaginator)
         """
 
 
@@ -77,13 +76,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeCommunicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCommunications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecommunicationspaginator)
         """
```

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support/paginator.pyi` & `mypy_boto3_support-1.34.93/mypy_boto3_support/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         caseIdList: Sequence[str] = ...,
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         language: str = ...,
         includeCommunications: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecasespaginator)
         """
 
 class DescribeCommunicationsPaginator(Paginator):
@@ -73,13 +73,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeCommunicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCommunications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecommunicationspaginator)
         """
```

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support/type_defs.py` & `mypy_boto3_support-1.34.93/mypy_boto3_support/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
     "AttachmentDetailsTypeDef",
+    "AttachmentOutputTypeDef",
     "BlobTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -58,47 +58,48 @@
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
     "AddAttachmentsToSetResponseTypeDef",
     "AddCommunicationToCaseResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
+    "DescribeAttachmentResponseTypeDef",
     "AttachmentTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
     "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
     "RecentCaseCommunicationsTypeDef",
-    "AddAttachmentsToSetRequestRequestTypeDef",
-    "DescribeAttachmentResponseTypeDef",
+    "AttachmentUnionTypeDef",
     "DescribeServicesResponseTypeDef",
     "DescribeCreateCaseOptionsResponseTypeDef",
     "TrustedAdvisorCheckResultTypeDef",
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
+    "AddAttachmentsToSetRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
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
 AddCommunicationToCaseRequestRequestTypeDef = TypedDict(
     "AddCommunicationToCaseRequestRequestTypeDef",
     {
         "communicationBody": str,
         "caseId": NotRequired[str],
@@ -109,14 +110,21 @@
 AttachmentDetailsTypeDef = TypedDict(
     "AttachmentDetailsTypeDef",
     {
         "attachmentId": NotRequired[str],
         "fileName": NotRequired[str],
     },
 )
+AttachmentOutputTypeDef = TypedDict(
+    "AttachmentOutputTypeDef",
+    {
+        "fileName": NotRequired[str],
+        "data": NotRequired[bytes],
+    },
+)
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
         "code": NotRequired[str],
         "name": NotRequired[str],
     },
@@ -349,14 +357,21 @@
         "caseId": NotRequired[str],
         "body": NotRequired[str],
         "submittedBy": NotRequired[str],
         "timeCreated": NotRequired[str],
         "attachmentSet": NotRequired[List[AttachmentDetailsTypeDef]],
     },
 )
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "fileName": NotRequired[str],
         "data": NotRequired[BlobTypeDef],
     },
 )
@@ -450,28 +465,15 @@
 RecentCaseCommunicationsTypeDef = TypedDict(
     "RecentCaseCommunicationsTypeDef",
     {
         "communications": NotRequired[List[CommunicationTypeDef]],
         "nextToken": NotRequired[str],
     },
 )
-AddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "AddAttachmentsToSetRequestRequestTypeDef",
-    {
-        "attachments": Sequence[AttachmentTypeDef],
-        "attachmentSetId": NotRequired[str],
-    },
-)
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
-    {
-        "attachment": AttachmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+AttachmentUnionTypeDef = Union[AttachmentTypeDef, AttachmentOutputTypeDef]
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -518,14 +520,21 @@
         "submittedBy": NotRequired[str],
         "timeCreated": NotRequired[str],
         "recentCommunications": NotRequired[RecentCaseCommunicationsTypeDef],
         "ccEmailAddresses": NotRequired[List[str]],
         "language": NotRequired[str],
     },
 )
+AddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "AddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachments": Sequence[AttachmentUnionTypeDef],
+        "attachmentSetId": NotRequired[str],
+    },
+)
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support/type_defs.pyi` & `mypy_boto3_support-1.34.93/mypy_boto3_support/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
     "AttachmentDetailsTypeDef",
+    "AttachmentOutputTypeDef",
     "BlobTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -57,47 +58,48 @@
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
     "AddAttachmentsToSetResponseTypeDef",
     "AddCommunicationToCaseResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
+    "DescribeAttachmentResponseTypeDef",
     "AttachmentTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
     "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
     "RecentCaseCommunicationsTypeDef",
-    "AddAttachmentsToSetRequestRequestTypeDef",
-    "DescribeAttachmentResponseTypeDef",
+    "AttachmentUnionTypeDef",
     "DescribeServicesResponseTypeDef",
     "DescribeCreateCaseOptionsResponseTypeDef",
     "TrustedAdvisorCheckResultTypeDef",
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
+    "AddAttachmentsToSetRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
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
 AddCommunicationToCaseRequestRequestTypeDef = TypedDict(
     "AddCommunicationToCaseRequestRequestTypeDef",
     {
         "communicationBody": str,
         "caseId": NotRequired[str],
@@ -108,14 +110,21 @@
 AttachmentDetailsTypeDef = TypedDict(
     "AttachmentDetailsTypeDef",
     {
         "attachmentId": NotRequired[str],
         "fileName": NotRequired[str],
     },
 )
+AttachmentOutputTypeDef = TypedDict(
+    "AttachmentOutputTypeDef",
+    {
+        "fileName": NotRequired[str],
+        "data": NotRequired[bytes],
+    },
+)
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
         "code": NotRequired[str],
         "name": NotRequired[str],
     },
@@ -348,14 +357,21 @@
         "caseId": NotRequired[str],
         "body": NotRequired[str],
         "submittedBy": NotRequired[str],
         "timeCreated": NotRequired[str],
         "attachmentSet": NotRequired[List[AttachmentDetailsTypeDef]],
     },
 )
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "fileName": NotRequired[str],
         "data": NotRequired[BlobTypeDef],
     },
 )
@@ -449,28 +465,15 @@
 RecentCaseCommunicationsTypeDef = TypedDict(
     "RecentCaseCommunicationsTypeDef",
     {
         "communications": NotRequired[List[CommunicationTypeDef]],
         "nextToken": NotRequired[str],
     },
 )
-AddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "AddAttachmentsToSetRequestRequestTypeDef",
-    {
-        "attachments": Sequence[AttachmentTypeDef],
-        "attachmentSetId": NotRequired[str],
-    },
-)
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
-    {
-        "attachment": AttachmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+AttachmentUnionTypeDef = Union[AttachmentTypeDef, AttachmentOutputTypeDef]
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -517,14 +520,21 @@
         "submittedBy": NotRequired[str],
         "timeCreated": NotRequired[str],
         "recentCommunications": NotRequired[RecentCaseCommunicationsTypeDef],
         "ccEmailAddresses": NotRequired[List[str]],
         "language": NotRequired[str],
     },
 )
+AddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "AddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachments": Sequence[AttachmentUnionTypeDef],
+        "attachmentSetId": NotRequired[str],
+    },
+)
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support.egg-info/PKG-INFO` & `mypy_boto3_support-1.34.93/mypy_boto3_support.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.34.0
-Summary: Type annotations for boto3.Support 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.93
+Summary: Type annotations for boto3.Support 1.34.93 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-support"></a>
 
 # mypy-boto3-support
 
 [![PyPI - mypy-boto3-support](https://img.shields.io/pypi/v/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-support)](https://pepy.tech/project/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-support-1.34.0/mypy_boto3_support.egg-info/SOURCES.txt` & `mypy_boto3_support-1.34.93/mypy_boto3_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.34.0/setup.py` & `mypy_boto3_support-1.34.93/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-support",
-    version="1.34.0",
+    version="1.34.93",
     packages=["mypy_boto3_support"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.Support 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.Support 1.34.93 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 support type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_support": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

