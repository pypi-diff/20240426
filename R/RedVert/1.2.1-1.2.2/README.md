# Comparing `tmp/redvert-1.2.1.tar.gz` & `tmp/redvert-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvert-1.2.1.tar", last modified: Thu Apr 25 22:26:01 2024, max compression
+gzip compressed data, was "redvert-1.2.2.tar", last modified: Thu Apr 25 23:27:50 2024, max compression
```

## Comparing `redvert-1.2.1.tar` & `redvert-1.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 22:26:01.449126 redvert-1.2.1/
--rw-rw-rw-   0        0        0     8808 2024-04-25 22:26:01.437993 redvert-1.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 22:26:01.437993 redvert-1.2.1/RedVert.egg-info/
--rw-rw-rw-   0        0        0     8808 2024-04-25 22:26:01.000000 redvert-1.2.1/RedVert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-25 22:26:01.000000 redvert-1.2.1/RedVert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 22:26:01.000000 redvert-1.2.1/RedVert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-25 22:26:01.000000 redvert-1.2.1/RedVert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 22:26:01.000000 redvert-1.2.1/RedVert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 22:26:01.434168 redvert-1.2.1/redvert/
--rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.2.1/redvert/__init__.py
--rw-rw-rw-   0        0        0     7381 2024-04-25 22:24:10.000000 redvert-1.2.1/redvert/main.py
--rw-rw-rw-   0        0        0       42 2024-04-25 22:26:01.449126 redvert-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-04-25 22:25:35.000000 redvert-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:27:50.863659 redvert-1.2.2/
+-rw-rw-rw-   0        0        0     9172 2024-04-25 23:27:50.859822 redvert-1.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 23:27:50.853548 redvert-1.2.2/RedVert.egg-info/
+-rw-rw-rw-   0        0        0     9172 2024-04-25 23:27:50.000000 redvert-1.2.2/RedVert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-25 23:27:50.000000 redvert-1.2.2/RedVert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 23:27:50.000000 redvert-1.2.2/RedVert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2024-04-25 23:27:50.000000 redvert-1.2.2/RedVert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 23:27:50.000000 redvert-1.2.2/RedVert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 23:27:50.849072 redvert-1.2.2/redvert/
+-rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.2.2/redvert/__init__.py
+-rw-rw-rw-   0        0        0     7928 2024-04-25 23:24:44.000000 redvert-1.2.2/redvert/main.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 23:27:50.864235 redvert-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      570 2024-04-25 23:24:52.000000 redvert-1.2.2/setup.py
```

### Comparing `redvert-1.2.1/PKG-INFO` & `redvert-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.2.1
+Version: 1.2.2
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
@@ -25,15 +25,15 @@
 
 To init RedVert in the terminal, first open file explorer and go to the file location you want your RedVert files and database environments to be stored. Next at the top, click it and type cmd. It will open a cmd prompt in that location. If this doesn't work, open a normal cmd and use this code,
 ```
 cd ('your folder path goes here')
 ```
 Now here, type in terminal,
 ```
-initredvert
+redvert
 ```
 This will init it! I will now show you how to use it in terminal.
 
 # How to use in terminal
 
 When Inited, it will probably show up something like this,
 ```
@@ -232,10 +232,26 @@
 
 L1:
 print "equal"
 halt
 ```
 Congrats! You just wrote a pretty complex program. If you run it it will prompt you with two values, and it will tell you if they are equal or not. (NOTE: this is only a beginner intermediate program so errors will occur if the input is not a int or float.) We will go over pop and push later on!
 
+# Other RedVert Flags
+
+In the cmd prompt or terminal, you can type in this
+```
+redvert -h
+```
+To learn more about the flags in RedVert. One flag is the version. To see the version, just input
+```
+redvert --version
+```
+Or you can input,
+```
+redvert --learn-more
+```
+To Learn More About It. (NOTE: The learn more will only bring you back to this page.)
+
 # Conclusion
 
 If you read through this entire description. Well Done! You have learned a lot. This project has taken me over 3 days to make, and it is still in the beta phase. That's all for RedVert. Goodbye!
```

### Comparing `redvert-1.2.1/RedVert.egg-info/PKG-INFO` & `redvert-1.2.2/RedVert.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.2.1
+Version: 1.2.2
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
@@ -25,15 +25,15 @@
 
 To init RedVert in the terminal, first open file explorer and go to the file location you want your RedVert files and database environments to be stored. Next at the top, click it and type cmd. It will open a cmd prompt in that location. If this doesn't work, open a normal cmd and use this code,
 ```
 cd ('your folder path goes here')
 ```
 Now here, type in terminal,
 ```
-initredvert
+redvert
 ```
 This will init it! I will now show you how to use it in terminal.
 
 # How to use in terminal
 
 When Inited, it will probably show up something like this,
 ```
@@ -232,10 +232,26 @@
 
 L1:
 print "equal"
 halt
 ```
 Congrats! You just wrote a pretty complex program. If you run it it will prompt you with two values, and it will tell you if they are equal or not. (NOTE: this is only a beginner intermediate program so errors will occur if the input is not a int or float.) We will go over pop and push later on!
 
+# Other RedVert Flags
+
+In the cmd prompt or terminal, you can type in this
+```
+redvert -h
+```
+To learn more about the flags in RedVert. One flag is the version. To see the version, just input
+```
+redvert --version
+```
+Or you can input,
+```
+redvert --learn-more
+```
+To Learn More About It. (NOTE: The learn more will only bring you back to this page.)
+
 # Conclusion
 
 If you read through this entire description. Well Done! You have learned a lot. This project has taken me over 3 days to make, and it is still in the beta phase. That's all for RedVert. Goodbye!
```

### Comparing `redvert-1.2.1/redvert/main.py` & `redvert-1.2.2/redvert/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ast
 import os
-import sys
+import argparse
 from time import sleep as delay
 
 env_file = 'envs.txt'
 env_name = {}
 scriptcontainerfile = {}
 
 def interpret(program_filepath):
@@ -115,16 +115,33 @@
 
 def createNewFile(filename):
     removeEnvironments(filename)
 
 def remove_content_from_file(filename):
     removeEnvironments(filename)
 
+def Version():
+    print("RedVert Version 1.2.2")
+
+def LearnMore():
+    print("Learn More At pypi.org/project/RedVert")
+
 def Initalize():
     i = 0
+    parser = argparse.ArgumentParser()
+    parser.add_argument('--version', action='version', version='RedVert Version 1.2.2')
+    parser.add_argument('--learn-more', action='store_true', help='Learn More At pypi.org/project/RedVert')
+    args = parser.parse_args()
+    try:
+        if args.version:
+            Version()
+        if args.learn_more:
+            LearnMore()
+    except:
+        print("")
     while True:
         print("Welcome To RedVert. What would you like to do?")
         print("Create Env, Access Env, Remove All Env, Clear Console")
         user_input = input('>>> ')
         if user_input == 'Create Env':
             print("Name Environment")
             env_name[f'env{i}'] = input('>>> ')
```

