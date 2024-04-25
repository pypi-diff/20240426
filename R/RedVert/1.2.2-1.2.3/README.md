# Comparing `tmp/redvert-1.2.2.tar.gz` & `tmp/redvert-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvert-1.2.2.tar", last modified: Thu Apr 25 23:27:50 2024, max compression
+gzip compressed data, was "redvert-1.2.3.tar", last modified: Thu Apr 25 23:31:45 2024, max compression
```

## Comparing `redvert-1.2.2.tar` & `redvert-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 23:27:50.863659 redvert-1.2.2/
--rw-rw-rw-   0        0        0     9172 2024-04-25 23:27:50.859822 redvert-1.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 23:27:50.853548 redvert-1.2.2/RedVert.egg-info/
--rw-rw-rw-   0        0        0     9172 2024-04-25 23:27:50.000000 redvert-1.2.2/RedVert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-25 23:27:50.000000 redvert-1.2.2/RedVert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 23:27:50.000000 redvert-1.2.2/RedVert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2024-04-25 23:27:50.000000 redvert-1.2.2/RedVert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 23:27:50.000000 redvert-1.2.2/RedVert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 23:27:50.849072 redvert-1.2.2/redvert/
--rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.2.2/redvert/__init__.py
--rw-rw-rw-   0        0        0     7928 2024-04-25 23:24:44.000000 redvert-1.2.2/redvert/main.py
--rw-rw-rw-   0        0        0       42 2024-04-25 23:27:50.864235 redvert-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      570 2024-04-25 23:24:52.000000 redvert-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:31:45.297961 redvert-1.2.3/
+-rw-rw-rw-   0        0        0     9172 2024-04-25 23:31:45.297961 redvert-1.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 23:31:45.295137 redvert-1.2.3/RedVert.egg-info/
+-rw-rw-rw-   0        0        0     9172 2024-04-25 23:31:45.000000 redvert-1.2.3/RedVert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-25 23:31:45.000000 redvert-1.2.3/RedVert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 23:31:45.000000 redvert-1.2.3/RedVert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2024-04-25 23:31:45.000000 redvert-1.2.3/RedVert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 23:31:45.000000 redvert-1.2.3/RedVert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 23:31:45.283379 redvert-1.2.3/redvert/
+-rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.2.3/redvert/__init__.py
+-rw-rw-rw-   0        0        0     7949 2024-04-25 23:31:34.000000 redvert-1.2.3/redvert/main.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 23:31:45.301921 redvert-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      570 2024-04-25 23:31:03.000000 redvert-1.2.3/setup.py
```

### Comparing `redvert-1.2.2/PKG-INFO` & `redvert-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.2.2
+Version: 1.2.3
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
```

### Comparing `redvert-1.2.2/RedVert.egg-info/PKG-INFO` & `redvert-1.2.3/RedVert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.2.2
+Version: 1.2.3
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
```

### Comparing `redvert-1.2.2/redvert/main.py` & `redvert-1.2.3/redvert/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,30 +116,30 @@
 def createNewFile(filename):
     removeEnvironments(filename)
 
 def remove_content_from_file(filename):
     removeEnvironments(filename)
 
 def Version():
-    print("RedVert Version 1.2.2")
+    print("RedVert Version 1.2.3")
 
 def LearnMore():
     print("Learn More At pypi.org/project/RedVert")
 
 def Initalize():
     i = 0
     parser = argparse.ArgumentParser()
-    parser.add_argument('--version', action='version', version='RedVert Version 1.2.2')
+    parser.add_argument('--version', action='version', version='RedVert Version 1.2.3')
     parser.add_argument('--learn-more', action='store_true', help='Learn More At pypi.org/project/RedVert')
     args = parser.parse_args()
     try:
         if args.version:
-            Version()
+            print(args.version)
         if args.learn_more:
-            LearnMore()
+            print(args.learn_more)
     except:
         print("")
     while True:
         print("Welcome To RedVert. What would you like to do?")
         print("Create Env, Access Env, Remove All Env, Clear Console")
         user_input = input('>>> ')
         if user_input == 'Create Env':
```

### Comparing `redvert-1.2.2/setup.py` & `redvert-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('readme.md', 'r') as file:
     description = file.read()
 
 setup(
     name='RedVert',
-    version='1.2.2',
+    version='1.2.3',
     packages=find_packages(),
     install_requires = [
         # nothing is here
     ],
     entry_points={
         "console_scripts": [
             'redvert = redvert:Initalize',
```

