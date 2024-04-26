# Comparing `tmp/RepoAuditor-0.1.0-py3-none-any.whl.zip` & `tmp/RepoAuditor-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 6299 bytes, number of entries: 10
--rw-r--r--  2.0 unx     3592 b- defN 24-Apr-12 12:40 BuildBinary.py
--rw-r--r--  2.0 unx     2572 b- defN 24-Apr-12 12:40 RepoAuditor/EntryPoint.py
--rw-r--r--  2.0 unx      876 b- defN 24-Apr-12 12:40 RepoAuditor/Math.py
--rw-r--r--  2.0 unx      639 b- defN 24-Apr-12 12:41 RepoAuditor/__init__.py
--rw-r--r--  2.0 unx     1132 b- defN 24-Apr-12 12:41 RepoAuditor-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2044 b- defN 24-Apr-12 12:41 RepoAuditor-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 12:41 RepoAuditor-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 24-Apr-12 12:41 RepoAuditor-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 24-Apr-12 12:41 RepoAuditor-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      816 b- defN 24-Apr-12 12:41 RepoAuditor-0.1.0.dist-info/RECORD
-10 files, 11846 bytes uncompressed, 4901 bytes compressed:  58.6%
+Zip file size: 8361 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     3592 b- defN 24-Apr-26 13:16 BuildBinary.py
+-rw-r--r--  2.0 unx     1912 b- defN 24-Apr-26 13:16 RepoAuditor/EntryPoint.py
+-rw-r--r--  2.0 unx     3227 b- defN 24-Apr-26 13:16 RepoAuditor/Requirement.py
+-rw-r--r--  2.0 unx      600 b- defN 24-Apr-26 13:16 RepoAuditor/__init__.py
+-rw-r--r--  2.0 unx     4511 b- defN 24-Apr-26 13:16 RepoAuditor/Impl/ParallelSequentialProcessor.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 13:16 RepoAuditor/Impl/__init__.py
+-rw-r--r--  2.0 unx     1132 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2104 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1010 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/RECORD
+12 files, 18263 bytes uncompressed, 6647 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,31 +1,37 @@
 Filename: BuildBinary.py
 Comment: 
 
 Filename: RepoAuditor/EntryPoint.py
 Comment: 
 
-Filename: RepoAuditor/Math.py
+Filename: RepoAuditor/Requirement.py
 Comment: 
 
 Filename: RepoAuditor/__init__.py
 Comment: 
 
-Filename: RepoAuditor-0.1.0.dist-info/LICENSE.txt
+Filename: RepoAuditor/Impl/ParallelSequentialProcessor.py
 Comment: 
 
-Filename: RepoAuditor-0.1.0.dist-info/METADATA
+Filename: RepoAuditor/Impl/__init__.py
 Comment: 
 
-Filename: RepoAuditor-0.1.0.dist-info/WHEEL
+Filename: RepoAuditor-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: RepoAuditor-0.1.0.dist-info/entry_points.txt
+Filename: RepoAuditor-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: RepoAuditor-0.1.0.dist-info/top_level.txt
+Filename: RepoAuditor-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: RepoAuditor-0.1.0.dist-info/RECORD
+Filename: RepoAuditor-0.1.1.dist-info/entry_points.txt
+Comment: 
+
+Filename: RepoAuditor-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: RepoAuditor-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RepoAuditor/EntryPoint.py

```diff
@@ -8,15 +8,15 @@
 
 import sys
 
 import typer
 
 from typer.core import TyperGroup  # type: ignore [import-untyped]
 
-from RepoAuditor import Math, __version__
+from RepoAuditor import __version__
 
 
 # ----------------------------------------------------------------------
 class NaturalOrderGrouper(TyperGroup):
     # pylint: disable=missing-class-docstring
     # ----------------------------------------------------------------------
     def list_commands(self, *args, **kwargs):  # pylint: disable=unused-argument
@@ -30,55 +30,18 @@
     no_args_is_help=True,
     pretty_exceptions_show_locals=False,
     pretty_exceptions_enable=False,
 )
 
 
 # ----------------------------------------------------------------------
-@app.command("Add")
-def Add(
-    x: int,
-    y: int,
-) -> None:
-    """Adds 2 values."""
-
-    sys.stdout.write(str(Math.Add(x, y)))
-
-
-# ----------------------------------------------------------------------
-@app.command("Sub")
-def Sub(
-    x: int,
-    y: int,
-) -> None:
-    """Subtracts 2 values."""
-
-    sys.stdout.write(str(Math.Sub(x, y)))
-
-
-# ----------------------------------------------------------------------
-@app.command("Mult")
-def Mult(
-    x: int,
-    y: int,
-) -> None:
-    """Multiplies 2 values."""
-
-    sys.stdout.write(str(Math.Mult(x, y)))
-
-
-# ----------------------------------------------------------------------
-@app.command("Div")
-def Div(
-    x: int,
-    y: int,
-) -> None:
-    """Divides 1 value by another."""
-
-    sys.stdout.write(str(Math.Div(x, y)))
+@app.command("Placeholder")
+def Placeholder() -> None:
+    """This is a placeholder command that should be removed once actual functionality is added."""
+    pass
 
 
 # ----------------------------------------------------------------------
 @app.command("Version")
 def Version() -> None:
     """Prints the version of the package."""
```

## RepoAuditor/__init__.py

```diff
@@ -5,10 +5,8 @@
 # |
 # ----------------------------------------------------------------------
 # pylint: disable=missing-module-docstring,invalid-name
 
 # Note that this value will be overwritten by calls to `python ../../Build.py update_version` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.1.0"
-
-from .Math import Add, Sub, Mult, Div
+__version__ = "0.1.1"
```

## Comparing `RepoAuditor-0.1.0.dist-info/LICENSE.txt` & `RepoAuditor-0.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `RepoAuditor-0.1.0.dist-info/METADATA` & `RepoAuditor-0.1.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepoAuditor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Audits repositories for best practices.
 Author-email: Scientific Software Engineering Center at Georgia Tech <sse-center@gatech.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/gt-sse-center/RepoAuditor
 Project-URL: Documentation, https://github.com/gt-sse-center/RepoAuditor
 Project-URL: Repository, https://github.com/gt-sse-center/RepoAuditor
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,16 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: dbrownell-Common
+Requires-Dist: pluggy ==1.*
 Requires-Dist: typer ~=0.9
 Provides-Extra: dev
 Requires-Dist: dbrownell-DevTools ; extra == 'dev'
 Provides-Extra: package
 Requires-Dist: build ==1.* ; extra == 'package'
 Requires-Dist: cx-Freeze ==6.* ; extra == 'package'
 Requires-Dist: twine ==4.* ; extra == 'package'
```

### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: RepoAuditor Version: 0.1.0 Summary: Audits
+Metadata-Version: 2.1 Name: RepoAuditor Version: 0.1.1 Summary: Audits
 repositories for best practices. Author-email: Scientific Software Engineering
 Center at Georgia Tech
 gatech.edu> License: MIT Project-URL: Homepage, https://github.com/gt-sse-
 center/RepoAuditor Project-URL: Documentation, https://github.com/gt-sse-
 center/RepoAuditor Project-URL: Repository, https://github.com/gt-sse-center/
 RepoAuditor Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Description-Content-Type: text/markdown License-File:
-LICENSE.txt Requires-Dist: typer ~=0.9 Provides-Extra: dev Requires-Dist:
-dbrownell-DevTools ; extra == 'dev' Provides-Extra: package Requires-Dist:
-build ==1.* ; extra == 'package' Requires-Dist: cx-Freeze ==6.* ; extra ==
-'package' Requires-Dist: twine ==4.* ; extra == 'package' # RepoAuditor Audits
+LICENSE.txt Requires-Dist: dbrownell-Common Requires-Dist: pluggy ==1.*
+Requires-Dist: typer ~=0.9 Provides-Extra: dev Requires-Dist: dbrownell-
+DevTools ; extra == 'dev' Provides-Extra: package Requires-Dist: build ==1.* ;
+extra == 'package' Requires-Dist: cx-Freeze ==6.* ; extra == 'package'
+Requires-Dist: twine ==4.* ; extra == 'package' # RepoAuditor Audits
 repositories for best practices. ### Overview TODO: Complete this section ###
 How to use RepoAuditor TODO: Complete this section ## Installation via
 Executable Download an executable for Linux, MacOS, or Windows to use the
 functionality provided by this repository without a dependency on [Python]
 (https://www.python.org). 1. Download the archive for the latest release [here]
 (https://github.com/gt-sse-center/RepoAuditor/releases/latest); the files will
 begin with `exe.` and contain the name of your operating system. 2. Decompress
```

