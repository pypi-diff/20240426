# Comparing `tmp/mypy-boto3-marketplace-entitlement-1.34.0.tar.gz` & `tmp/mypy_boto3_marketplace_entitlement-1.34.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-marketplace-entitlement-1.34.0.tar", last modified: Wed Dec 13 21:23:12 2023, max compression
+gzip compressed data, was "mypy_boto3_marketplace_entitlement-1.34.93.tar", last modified: Fri Apr 26 19:32:22 2024, max compression
```

## Comparing `mypy-boto3-marketplace-entitlement-1.34.0.tar` & `mypy_boto3_marketplace_entitlement-1.34.93.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:12.815282 mypy-boto3-marketplace-entitlement-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13707 2023-12-13 21:23:12.815282 mypy-boto3-marketplace-entitlement-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12104 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:12.815282 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8529 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:12.815282 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13707 2023-12-13 21:23:12.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 21:23:12.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:12.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:12.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:12.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 21:23:12.000000 mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:12.815282 mypy-boto3-marketplace-entitlement-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-12-13 21:13:39.000000 mypy-boto3-marketplace-entitlement-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:22.867543 mypy_boto3_marketplace_entitlement-1.34.93/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-04-26 19:32:22.867543 mypy_boto3_marketplace_entitlement-1.34.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:22.867543 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:22.867543 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-04-26 19:32:22.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-26 19:32:22.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:22.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:22.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 19:32:22.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-26 19:32:22.000000 mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:32:22.867543 mypy_boto3_marketplace_entitlement-1.34.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-26 19:31:58.000000 mypy_boto3_marketplace_entitlement-1.34.93/setup.py
```

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/LICENSE` & `mypy_boto3_marketplace_entitlement-1.34.93/LICENSE`

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

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/PKG-INFO` & `mypy_boto3_marketplace_entitlement-1.34.93/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-marketplace-entitlement
-Version: 1.34.0
-Summary: Type annotations for boto3.MarketplaceEntitlementService 1.34.0 service generated with mypy-boto3-builder 7.21.0
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 marketplace-entitlement type-annotations botocore mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-marketplace-entitlement"></a>
 
 # mypy-boto3-marketplace-entitlement
 
 [![PyPI - mypy-boto3-marketplace-entitlement](https://img.shields.io/pypi/v/mypy-boto3-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-entitlement)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-entitlement)](https://pepy.tech/project/mypy-boto3-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceEntitlementService 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[boto3.MarketplaceEntitlementService 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
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
 [mypy-boto3-marketplace-entitlement docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/README.md` & `mypy_boto3_marketplace_entitlement-1.34.93/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,62 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-marketplace-entitlement
+Version: 1.34.93
+Summary: Type annotations for boto3.MarketplaceEntitlementService 1.34.93 service generated with mypy-boto3-builder 7.24.0
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 marketplace-entitlement type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
+
 <a id="mypy-boto3-marketplace-entitlement"></a>
 
 # mypy-boto3-marketplace-entitlement
 
 [![PyPI - mypy-boto3-marketplace-entitlement](https://img.shields.io/pypi/v/mypy-boto3-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-entitlement)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-entitlement)](https://pepy.tech/project/mypy-boto3-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceEntitlementService 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[boto3.MarketplaceEntitlementService 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
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
 [mypy-boto3-marketplace-entitlement docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/__init__.py` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,9 +19,8 @@
 """
 
 from .client import MarketplaceEntitlementServiceClient
 from .paginator import GetEntitlementsPaginator
 
 Client = MarketplaceEntitlementServiceClient
 
-
 __all__ = ("Client", "GetEntitlementsPaginator", "MarketplaceEntitlementServiceClient")
```

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/__init__.pyi` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/__main__.py` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceEntitlementService 1.34.0\nVersion:        "
-        " 1.34.0\nBuilder version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement//\nBoto3"
-        " docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.MarketplaceEntitlementService 1.34.93\n"
+        "Version:         1.34.93\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService\n"
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

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/client.py` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from .type_defs import GetEntitlementsResultTypeDef
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MarketplaceEntitlementServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -96,15 +95,15 @@
 
     def get_entitlements(
         self,
         *,
         ProductCode: str,
         Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetEntitlementsResultTypeDef:
         """
         GetEntitlements retrieves entitlement values for a given product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.get_entitlements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/client/#get_entitlements)
         """
```

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/client.pyi` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     def get_entitlements(
         self,
         *,
         ProductCode: str,
         Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetEntitlementsResultTypeDef:
         """
         GetEntitlements retrieves entitlement values for a given product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.get_entitlements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/client/#get_entitlements)
         """
```

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/literals.py` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GetEntitlementFilterNameType",
     "GetEntitlementsPaginatorName",
     "MarketplaceEntitlementServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 GetEntitlementFilterNameType = Literal["CUSTOMER_IDENTIFIER", "DIMENSION"]
 GetEntitlementsPaginatorName = Literal["get_entitlements"]
 MarketplaceEntitlementServiceServiceName = Literal["marketplace-entitlement"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -56,14 +54,15 @@
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
@@ -74,14 +73,15 @@
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
@@ -99,14 +99,15 @@
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
@@ -119,24 +120,26 @@
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
@@ -197,15 +200,14 @@
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
@@ -277,17 +279,19 @@
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
@@ -332,14 +336,15 @@
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
@@ -377,19 +382,21 @@
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

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/literals.pyi` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
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
@@ -72,14 +73,15 @@
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
@@ -97,14 +99,15 @@
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
@@ -117,24 +120,26 @@
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
@@ -195,15 +200,14 @@
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
@@ -275,17 +279,19 @@
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
@@ -330,14 +336,15 @@
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
@@ -375,19 +382,21 @@
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

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/paginator.py` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import GetEntitlementFilterNameType
 from .type_defs import GetEntitlementsResultTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("GetEntitlementsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -47,13 +46,13 @@
     """
 
     def paginate(
         self,
         *,
         ProductCode: str,
         Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[GetEntitlementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Paginator.GetEntitlements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/paginators/#getentitlementspaginator)
         """
```

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/paginator.pyi` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -44,13 +44,13 @@
     """
 
     def paginate(
         self,
         *,
         ProductCode: str,
         Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[GetEntitlementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Paginator.GetEntitlements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/paginators/#getentitlementspaginator)
         """
```

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/type_defs.py` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "EntitlementValueTypeDef",
     "PaginatorConfigTypeDef",
     "GetEntitlementsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EntitlementTypeDef",
     "GetEntitlementsRequestGetEntitlementsPaginateTypeDef",
@@ -64,18 +63,18 @@
         "MaxResults": NotRequired[int],
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
 EntitlementTypeDef = TypedDict(
     "EntitlementTypeDef",
     {
         "ProductCode": NotRequired[str],
         "Dimension": NotRequired[str],
@@ -92,11 +91,11 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 GetEntitlementsResultTypeDef = TypedDict(
     "GetEntitlementsResultTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement/type_defs.pyi` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -63,18 +63,18 @@
         "MaxResults": NotRequired[int],
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
 EntitlementTypeDef = TypedDict(
     "EntitlementTypeDef",
     {
         "ProductCode": NotRequired[str],
         "Dimension": NotRequired[str],
@@ -91,11 +91,11 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 GetEntitlementsResultTypeDef = TypedDict(
     "GetEntitlementsResultTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement.egg-info/PKG-INFO` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-entitlement
-Version: 1.34.0
-Summary: Type annotations for boto3.MarketplaceEntitlementService 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.93
+Summary: Type annotations for boto3.MarketplaceEntitlementService 1.34.93 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/
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
 
 <a id="mypy-boto3-marketplace-entitlement"></a>
 
 # mypy-boto3-marketplace-entitlement
 
 [![PyPI - mypy-boto3-marketplace-entitlement](https://img.shields.io/pypi/v/mypy-boto3-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-entitlement)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-entitlement)](https://pepy.tech/project/mypy-boto3-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceEntitlementService 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[boto3.MarketplaceEntitlementService 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
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
 [mypy-boto3-marketplace-entitlement docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/mypy_boto3_marketplace_entitlement.egg-info/SOURCES.txt` & `mypy_boto3_marketplace_entitlement-1.34.93/mypy_boto3_marketplace_entitlement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-entitlement-1.34.0/setup.py` & `mypy_boto3_marketplace_entitlement-1.34.93/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,52 +7,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-marketplace-entitlement",
-    version="1.34.0",
+    version="1.34.93",
     packages=["mypy_boto3_marketplace_entitlement"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.MarketplaceEntitlementService 1.34.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.MarketplaceEntitlementService 1.34.93 service generated with mypy-boto3-builder 7.24.0",
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
     keywords="boto3 marketplace-entitlement type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_marketplace_entitlement": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
-        "Documentation": (
-            "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/"
-        ),
+        "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
     ],
     zip_safe=False,
```

