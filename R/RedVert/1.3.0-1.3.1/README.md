# Comparing `tmp/redvert-1.3.0.tar.gz` & `tmp/redvert-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvert-1.3.0.tar", last modified: Thu Apr 25 23:35:47 2024, max compression
+gzip compressed data, was "redvert-1.3.1.tar", last modified: Fri Apr 26 01:19:37 2024, max compression
```

## Comparing `redvert-1.3.0.tar` & `redvert-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 23:35:47.429163 redvert-1.3.0/
--rw-rw-rw-   0        0        0     9172 2024-04-25 23:35:47.425050 redvert-1.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 23:35:47.423036 redvert-1.3.0/RedVert.egg-info/
--rw-rw-rw-   0        0        0     9172 2024-04-25 23:35:47.000000 redvert-1.3.0/RedVert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-25 23:35:47.000000 redvert-1.3.0/RedVert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 23:35:47.000000 redvert-1.3.0/RedVert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2024-04-25 23:35:47.000000 redvert-1.3.0/RedVert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 23:35:47.000000 redvert-1.3.0/RedVert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 23:35:47.414121 redvert-1.3.0/redvert/
--rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.3.0/redvert/__init__.py
--rw-rw-rw-   0        0        0     7951 2024-04-25 23:33:30.000000 redvert-1.3.0/redvert/main.py
--rw-rw-rw-   0        0        0       42 2024-04-25 23:35:47.429163 redvert-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      570 2024-04-25 23:33:37.000000 redvert-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:19:37.808848 redvert-1.3.1/
+-rw-rw-rw-   0        0        0     9172 2024-04-26 01:19:37.802798 redvert-1.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 01:19:37.799799 redvert-1.3.1/RedVert.egg-info/
+-rw-rw-rw-   0        0        0     9172 2024-04-26 01:19:37.000000 redvert-1.3.1/RedVert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-26 01:19:37.000000 redvert-1.3.1/RedVert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 01:19:37.000000 redvert-1.3.1/RedVert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-26 01:19:37.000000 redvert-1.3.1/RedVert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 01:19:37.000000 redvert-1.3.1/RedVert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 01:19:37.798789 redvert-1.3.1/redvert/
+-rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.3.1/redvert/__init__.py
+-rw-rw-rw-   0        0        0     7779 2024-04-26 01:17:34.000000 redvert-1.3.1/redvert/main.py
+-rw-rw-rw-   0        0        0       42 2024-04-26 01:19:37.808848 redvert-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      462 2024-04-26 01:00:48.000000 redvert-1.3.1/setup.py
```

### Comparing `redvert-1.3.0/PKG-INFO` & `redvert-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.3.0
+Version: 1.3.1
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
```

### Comparing `redvert-1.3.0/RedVert.egg-info/PKG-INFO` & `redvert-1.3.1/RedVert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.3.0
+Version: 1.3.1
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
```

### Comparing `redvert-1.3.0/redvert/main.py` & `redvert-1.3.1/redvert/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ast
 import os
 import argparse
+import webbrowser
 from time import sleep as delay
 
 env_file = 'envs.txt'
 env_name = {}
 scriptcontainerfile = {}
 
 def interpret(program_filepath):
@@ -115,32 +116,22 @@
 
 def createNewFile(filename):
     removeEnvironments(filename)
 
 def remove_content_from_file(filename):
     removeEnvironments(filename)
 
-def Version():
-    print("RedVert Version 1.3.0")
-
-def LearnMore():
-    print("Learn More At pypi.org/project/RedVert")
-
 def Initalize():
     i = 0
     parser = argparse.ArgumentParser()
-    parser.add_argument('--version', action='version', version='RedVert Version 1.3.0')
+    parser.add_argument('--version', action='version', version='RedVert Version 1.3.1')
     parser.add_argument('--learn-more', action='store_true', help='Learn More At pypi.org/project/RedVert')
     args = parser.parse_args()
-    try:
-        if args.version:
-            print(args.version)
-        elif args.learn_more:
-            print(args.learn_more)
-    except:
+    if args.learn_more:
+        webbrowser.open('pypi.org/project/RedVert', new=2)
         print("")
     while True:
         print("Welcome To RedVert. What would you like to do?")
         print("Create Env, Access Env, Remove All Env, Clear Console")
         user_input = input('>>> ')
         if user_input == 'Create Env':
             print("Name Environment")
```

