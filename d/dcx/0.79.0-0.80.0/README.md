# Comparing `tmp/dcx-0.79.0.tar.gz` & `tmp/dcx-0.80.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcx-0.79.0.tar", last modified: Tue Apr  9 09:27:31 2024, max compression
+gzip compressed data, was "dcx-0.80.0.tar", last modified: Fri Apr 26 20:20:50 2024, max compression
```

## Comparing `dcx-0.79.0.tar` & `dcx-0.80.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-09 09:27:31.673124 dcx-0.79.0/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-02-16 09:45:07.000000 dcx-0.79.0/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-09 09:27:31.672950 dcx-0.79.0/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      159 2024-02-25 22:16:23.000000 dcx-0.79.0/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      716 2024-04-09 09:27:29.000000 dcx-0.79.0/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-04-09 09:27:31.673298 dcx-0.79.0/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-09 09:27:31.670333 dcx-0.79.0/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-09 09:27:31.671119 dcx-0.79.0/src/dcx/
--rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-01-14 18:51:20.000000 dcx-0.79.0/src/dcx/__init__.py
--rw-r--r--   0 robertdegen   (501) staff       (20)    66377 2024-04-09 09:27:20.000000 dcx-0.79.0/src/dcx/__main__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-09 09:27:31.672650 dcx-0.79.0/src/dcx.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-09 09:27:31.000000 dcx-0.79.0/src/dcx.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      226 2024-04-09 09:27:31.000000 dcx-0.79.0/src/dcx.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-04-09 09:27:31.000000 dcx-0.79.0/src/dcx.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       83 2024-04-09 09:27:31.000000 dcx-0.79.0/src/dcx.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-04-09 09:27:31.000000 dcx-0.79.0/src/dcx.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-26 20:20:50.777127 dcx-0.80.0/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-02-16 09:45:07.000000 dcx-0.80.0/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-26 20:20:50.776964 dcx-0.80.0/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      159 2024-02-25 22:16:23.000000 dcx-0.80.0/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      716 2024-04-26 20:20:48.000000 dcx-0.80.0/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-04-26 20:20:50.777161 dcx-0.80.0/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-26 20:20:50.774454 dcx-0.80.0/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-26 20:20:50.775214 dcx-0.80.0/src/dcx/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-01-14 18:51:20.000000 dcx-0.80.0/src/dcx/__init__.py
+-rw-r--r--   0 robertdegen   (501) staff       (20)    66710 2024-04-26 20:20:31.000000 dcx-0.80.0/src/dcx/__main__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-26 20:20:50.776799 dcx-0.80.0/src/dcx.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-26 20:20:50.000000 dcx-0.80.0/src/dcx.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      226 2024-04-26 20:20:50.000000 dcx-0.80.0/src/dcx.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-04-26 20:20:50.000000 dcx-0.80.0/src/dcx.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       83 2024-04-26 20:20:50.000000 dcx-0.80.0/src/dcx.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-04-26 20:20:50.000000 dcx-0.80.0/src/dcx.egg-info/top_level.txt
```

### Comparing `dcx-0.79.0/PKG-INFO` & `dcx-0.80.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcx
-Version: 0.79.0
+Version: 0.80.0
 Summary: Minimalistic selenium wrapper
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert/dcx
 Project-URL: Issues, https://github.com/turbo-bert/dcx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcx-0.79.0/pyproject.toml` & `dcx-0.80.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dcx"
-version = "0.79.0"
+version = "0.80.0"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "Minimalistic selenium wrapper"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dcx-0.79.0/src/dcx/__main__.py` & `dcx-0.80.0/src/dcx/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import traceback
 import subprocess
 import datetime
 import argparse
 import shutil
 import getpass
 import tabulate
+import pathlib
 
 const_figlet = "IF9fXyAgIF9fX19fICBfXwp8ICAgXCAvIF9fXCBcLyAvCnwgfCkgfCAoX18gPiAgPCAKfF9fXy8gXF9fXy9fL1xfXAogICAgICAgICAgICAgICAgCg=="
 
 import rich
 from rich.console import Console
 
 from selenium.webdriver.firefox.options import Options as FFOptions
@@ -399,25 +400,30 @@
         the_page = 0
         the_page += 1
 
         pdf.page(the_page).text(1,15,"*** THIS DOCUMENT MAY CONTAIN CONFIDENTIAL DATA *** FOR INTERNAL USE ONLY *** DO NOT TRANSMIT AS UNENCRYPTED FILE ***")
         #pdf.page(the_page).text(4,55,"______________________________________")
         #pdf.page(the_page).text(34,55,"______________________________________")
         
+        user_id_from_os = -1
+        # win doesn't have this
+        if hasattr(os, "getuid") and callable(getattr(os, "getuid")):
+            user_id_from_os = os.getuid()
+
         testdata = tabulate.tabulate(tabular_data=[
             ["",""],
             ["Execution Result    : ", "[x] OK        [ ] Failed        [ ] Failed on internal error"],
             ["",""],
             ["Execution DURATION  : ", "8sec (=0d 0h 0min 8sec)"],
             ["Execution START     : ", "10:30"],
             ["Execution STOP      : ", "10:31"],
             ["",""],
             ["Python / Platform   : ", "%d.%d / %s" % (sys.version_info.major, sys.version_info.minor, sys.platform)],
             ["Hostname            : ", socket.gethostname()],
-            ["User (UID)          : ", "%s (%d)" % (getpass.getuser(), os.getuid())],
+            ["User (UID)          : ", "%s (%d)" % (getpass.getuser(), user_id_from_os)],
             ["Browser Mode        : ", driver_mode],
             ["Test Engine         : ", "dcx-" + const_appversion],
             ["",""],
             ["Directory           : ",envdata["PWD"]],
                                                    ], headers=["S U M M A R Y", ""])
         pdf.page(the_page).text(12,20,testdata)
 
@@ -593,15 +599,20 @@
     if idx+1 <= len(src)-1:
         content = content_provider_facade(content, src[idx+1])
     return content
 
 
 envdata = {}
 envdata["HOME"] = os.getenv("HOME")
+if envdata["HOME"] == None:
+    envdata["HOME"] = str(pathlib.Path.home())
+    
 envdata["PWD"] = os.getenv("PWD")
+if envdata["PWD"] == None:
+    envdata["PWD"] = os.getcwd()
 
 secdata = {}
 sec_hack = None
 sec_server = None
 
 
 if args.sec:
```

### Comparing `dcx-0.79.0/src/dcx.egg-info/PKG-INFO` & `dcx-0.80.0/src/dcx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcx
-Version: 0.79.0
+Version: 0.80.0
 Summary: Minimalistic selenium wrapper
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert/dcx
 Project-URL: Issues, https://github.com/turbo-bert/dcx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

