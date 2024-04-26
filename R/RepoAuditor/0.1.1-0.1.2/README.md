# Comparing `tmp/RepoAuditor-0.1.1-py3-none-any.whl.zip` & `tmp/RepoAuditor-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,16 @@
-Zip file size: 8361 bytes, number of entries: 12
--rw-r--r--  2.0 unx     3592 b- defN 24-Apr-26 13:16 BuildBinary.py
--rw-r--r--  2.0 unx     1912 b- defN 24-Apr-26 13:16 RepoAuditor/EntryPoint.py
--rw-r--r--  2.0 unx     3227 b- defN 24-Apr-26 13:16 RepoAuditor/Requirement.py
--rw-r--r--  2.0 unx      600 b- defN 24-Apr-26 13:16 RepoAuditor/__init__.py
--rw-r--r--  2.0 unx     4511 b- defN 24-Apr-26 13:16 RepoAuditor/Impl/ParallelSequentialProcessor.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 13:16 RepoAuditor/Impl/__init__.py
--rw-r--r--  2.0 unx     1132 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2104 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1010 b- defN 24-Apr-26 13:16 RepoAuditor-0.1.1.dist-info/RECORD
-12 files, 18263 bytes uncompressed, 6647 bytes compressed:  63.6%
+Zip file size: 11139 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     3592 b- defN 24-Apr-26 15:07 BuildBinary.py
+-rw-r--r--  2.0 unx     1912 b- defN 24-Apr-26 15:07 RepoAuditor/EntryPoint.py
+-rw-r--r--  2.0 unx     6199 b- defN 24-Apr-26 15:07 RepoAuditor/Module.py
+-rw-r--r--  2.0 unx     4990 b- defN 24-Apr-26 15:07 RepoAuditor/Query.py
+-rw-r--r--  2.0 unx     3227 b- defN 24-Apr-26 15:07 RepoAuditor/Requirement.py
+-rw-r--r--  2.0 unx      600 b- defN 24-Apr-26 15:08 RepoAuditor/__init__.py
+-rw-r--r--  2.0 unx     4511 b- defN 24-Apr-26 15:07 RepoAuditor/Impl/ParallelSequentialProcessor.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 15:07 RepoAuditor/Impl/__init__.py
+-rw-r--r--  2.0 unx     1132 b- defN 24-Apr-26 15:08 RepoAuditor-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2104 b- defN 24-Apr-26 15:08 RepoAuditor-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 15:08 RepoAuditor-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 24-Apr-26 15:08 RepoAuditor-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-26 15:08 RepoAuditor-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1165 b- defN 24-Apr-26 15:08 RepoAuditor-0.1.2.dist-info/RECORD
+14 files, 29607 bytes uncompressed, 9191 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,37 +1,43 @@
 Filename: BuildBinary.py
 Comment: 
 
 Filename: RepoAuditor/EntryPoint.py
 Comment: 
 
+Filename: RepoAuditor/Module.py
+Comment: 
+
+Filename: RepoAuditor/Query.py
+Comment: 
+
 Filename: RepoAuditor/Requirement.py
 Comment: 
 
 Filename: RepoAuditor/__init__.py
 Comment: 
 
 Filename: RepoAuditor/Impl/ParallelSequentialProcessor.py
 Comment: 
 
 Filename: RepoAuditor/Impl/__init__.py
 Comment: 
 
-Filename: RepoAuditor-0.1.1.dist-info/LICENSE.txt
+Filename: RepoAuditor-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: RepoAuditor-0.1.1.dist-info/METADATA
+Filename: RepoAuditor-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: RepoAuditor-0.1.1.dist-info/WHEEL
+Filename: RepoAuditor-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: RepoAuditor-0.1.1.dist-info/entry_points.txt
+Filename: RepoAuditor-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: RepoAuditor-0.1.1.dist-info/top_level.txt
+Filename: RepoAuditor-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: RepoAuditor-0.1.1.dist-info/RECORD
+Filename: RepoAuditor-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RepoAuditor/__init__.py

```diff
@@ -5,8 +5,8 @@
 # |
 # ----------------------------------------------------------------------
 # pylint: disable=missing-module-docstring,invalid-name
 
 # Note that this value will be overwritten by calls to `python ../../Build.py update_version` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `RepoAuditor-0.1.1.dist-info/LICENSE.txt` & `RepoAuditor-0.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `RepoAuditor-0.1.1.dist-info/METADATA` & `RepoAuditor-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepoAuditor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Audits repositories for best practices.
 Author-email: Scientific Software Engineering Center at Georgia Tech <sse-center@gatech.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/gt-sse-center/RepoAuditor
 Project-URL: Documentation, https://github.com/gt-sse-center/RepoAuditor
 Project-URL: Repository, https://github.com/gt-sse-center/RepoAuditor
 Classifier: License :: OSI Approved :: MIT License
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: RepoAuditor Version: 0.1.1 Summary: Audits
+Metadata-Version: 2.1 Name: RepoAuditor Version: 0.1.2 Summary: Audits
 repositories for best practices. Author-email: Scientific Software Engineering
 Center at Georgia Tech
 gatech.edu> License: MIT Project-URL: Homepage, https://github.com/gt-sse-
 center/RepoAuditor Project-URL: Documentation, https://github.com/gt-sse-
 center/RepoAuditor Project-URL: Repository, https://github.com/gt-sse-center/
 RepoAuditor Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
```

