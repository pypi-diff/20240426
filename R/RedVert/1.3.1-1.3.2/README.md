# Comparing `tmp/redvert-1.3.1.tar.gz` & `tmp/redvert-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvert-1.3.1.tar", last modified: Fri Apr 26 01:19:37 2024, max compression
+gzip compressed data, was "redvert-1.3.2.tar", last modified: Fri Apr 26 01:43:37 2024, max compression
```

## Comparing `redvert-1.3.1.tar` & `redvert-1.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 01:19:37.808848 redvert-1.3.1/
--rw-rw-rw-   0        0        0     9172 2024-04-26 01:19:37.802798 redvert-1.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-26 01:19:37.799799 redvert-1.3.1/RedVert.egg-info/
--rw-rw-rw-   0        0        0     9172 2024-04-26 01:19:37.000000 redvert-1.3.1/RedVert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-26 01:19:37.000000 redvert-1.3.1/RedVert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 01:19:37.000000 redvert-1.3.1/RedVert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-26 01:19:37.000000 redvert-1.3.1/RedVert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-04-26 01:19:37.000000 redvert-1.3.1/RedVert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 01:19:37.798789 redvert-1.3.1/redvert/
--rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.3.1/redvert/__init__.py
--rw-rw-rw-   0        0        0     7779 2024-04-26 01:17:34.000000 redvert-1.3.1/redvert/main.py
--rw-rw-rw-   0        0        0       42 2024-04-26 01:19:37.808848 redvert-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      462 2024-04-26 01:00:48.000000 redvert-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 01:43:37.383014 redvert-1.3.2/
+-rw-rw-rw-   0        0        0    10298 2024-04-26 01:43:37.381744 redvert-1.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 01:43:37.376498 redvert-1.3.2/RedVert.egg-info/
+-rw-rw-rw-   0        0        0    10298 2024-04-26 01:43:37.000000 redvert-1.3.2/RedVert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-26 01:43:37.000000 redvert-1.3.2/RedVert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 01:43:37.000000 redvert-1.3.2/RedVert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-26 01:43:37.000000 redvert-1.3.2/RedVert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 01:43:37.000000 redvert-1.3.2/RedVert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 01:43:37.376498 redvert-1.3.2/redvert/
+-rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.3.2/redvert/__init__.py
+-rw-rw-rw-   0        0        0     7779 2024-04-26 01:43:11.000000 redvert-1.3.2/redvert/main.py
+-rw-rw-rw-   0        0        0       42 2024-04-26 01:43:37.383014 redvert-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      462 2024-04-26 01:43:12.000000 redvert-1.3.2/setup.py
```

### Comparing `redvert-1.3.1/PKG-INFO` & `redvert-1.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.3.1
+Version: 1.3.2
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
@@ -106,15 +106,15 @@
 
 filename = 'whateverfilenameyouwant.txt' # The extension of the file doesn't matter, in this case, I'm using .txt
 
 createNewFile(filename)
 
 ```
 Wala! The new file is created. Now we're going to learn more about the save to file and append to file functions.
-To save one file of code to the file, use the save to file cmd, otherwise use append to file to append multiple lines. (NOTE: Appending to the file doesn't do formatting, so later on, you may have to use extra spaces to format it correctly)
+To save one file of code to the file, use the save to file cmd, otherwise use append to file to append multiple lines.
 To use save_to_file you put the input in the first param, and put the file name in the second.
 ```
 from redvert import *
 
 filename = 'whateverfilenameyouwant.txt' # The extension of the file doesn't matter, in this case, I'm using .txt
 
 createNewFile(filename)
@@ -232,14 +232,51 @@
 
 L1:
 print "equal"
 halt
 ```
 Congrats! You just wrote a pretty complex program. If you run it it will prompt you with two values, and it will tell you if they are equal or not. (NOTE: this is only a beginner intermediate program so errors will occur if the input is not a int or float.) We will go over pop and push later on!
 
+# Coding Through Python Itself
+
+If you are wondering how to code manually through python this is the section for you! First import the module and create the variable containing the filepath.
+```
+import redvert as rv
+redvertFile = 'file.redvert'
+
+```
+Next create the file using the redvert.createNewFile function
+```
+import redvert as rv
+redvertFile = 'file.redvert'
+rv.createNewFile(redvertFile)
+```
+Next, you have to save the multiple lines of code. To do this, use the save_to_file function and the triple apostrophe.
+```
+import redvert as rv
+redvertFile = 'file.redvert'
+rv.createNewFile(redvertFile)
+rv.save_to_file('''
+print "Hello, World!"
+halt
+''')
+```
+This script will now create a new file with the file name, "file.redvert" and save a redvert command to print, "Hello, World!" Finally, you have to run it through the interpret function.
+```
+import redvert as rv
+redvertFile = 'file.redvert'
+rv.createNewFile(redvertFile)
+rv.save_to_file('''
+print "Hello, World!"
+halt
+''')
+rv.interpret(redvertFile)
+```
+When you run this code a new redvert file will be created and it will run! In the terminal it should say Hello World! If it worked, congrats! You have successfully created a script through python!
+
 # Other RedVert Flags
 
 In the cmd prompt or terminal, you can type in this
 ```
 redvert -h
 ```
 To learn more about the flags in RedVert. One flag is the version. To see the version, just input
```

### Comparing `redvert-1.3.1/RedVert.egg-info/PKG-INFO` & `redvert-1.3.2/RedVert.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.3.1
+Version: 1.3.2
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
@@ -106,15 +106,15 @@
 
 filename = 'whateverfilenameyouwant.txt' # The extension of the file doesn't matter, in this case, I'm using .txt
 
 createNewFile(filename)
 
 ```
 Wala! The new file is created. Now we're going to learn more about the save to file and append to file functions.
-To save one file of code to the file, use the save to file cmd, otherwise use append to file to append multiple lines. (NOTE: Appending to the file doesn't do formatting, so later on, you may have to use extra spaces to format it correctly)
+To save one file of code to the file, use the save to file cmd, otherwise use append to file to append multiple lines.
 To use save_to_file you put the input in the first param, and put the file name in the second.
 ```
 from redvert import *
 
 filename = 'whateverfilenameyouwant.txt' # The extension of the file doesn't matter, in this case, I'm using .txt
 
 createNewFile(filename)
@@ -232,14 +232,51 @@
 
 L1:
 print "equal"
 halt
 ```
 Congrats! You just wrote a pretty complex program. If you run it it will prompt you with two values, and it will tell you if they are equal or not. (NOTE: this is only a beginner intermediate program so errors will occur if the input is not a int or float.) We will go over pop and push later on!
 
+# Coding Through Python Itself
+
+If you are wondering how to code manually through python this is the section for you! First import the module and create the variable containing the filepath.
+```
+import redvert as rv
+redvertFile = 'file.redvert'
+
+```
+Next create the file using the redvert.createNewFile function
+```
+import redvert as rv
+redvertFile = 'file.redvert'
+rv.createNewFile(redvertFile)
+```
+Next, you have to save the multiple lines of code. To do this, use the save_to_file function and the triple apostrophe.
+```
+import redvert as rv
+redvertFile = 'file.redvert'
+rv.createNewFile(redvertFile)
+rv.save_to_file('''
+print "Hello, World!"
+halt
+''')
+```
+This script will now create a new file with the file name, "file.redvert" and save a redvert command to print, "Hello, World!" Finally, you have to run it through the interpret function.
+```
+import redvert as rv
+redvertFile = 'file.redvert'
+rv.createNewFile(redvertFile)
+rv.save_to_file('''
+print "Hello, World!"
+halt
+''')
+rv.interpret(redvertFile)
+```
+When you run this code a new redvert file will be created and it will run! In the terminal it should say Hello World! If it worked, congrats! You have successfully created a script through python!
+
 # Other RedVert Flags
 
 In the cmd prompt or terminal, you can type in this
 ```
 redvert -h
 ```
 To learn more about the flags in RedVert. One flag is the version. To see the version, just input
```

### Comparing `redvert-1.3.1/redvert/main.py` & `redvert-1.3.2/redvert/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 def remove_content_from_file(filename):
     removeEnvironments(filename)
 
 def Initalize():
     i = 0
     parser = argparse.ArgumentParser()
-    parser.add_argument('--version', action='version', version='RedVert Version 1.3.1')
+    parser.add_argument('--version', action='version', version='RedVert Version 1.3.2')
     parser.add_argument('--learn-more', action='store_true', help='Learn More At pypi.org/project/RedVert')
     args = parser.parse_args()
     if args.learn_more:
         webbrowser.open('pypi.org/project/RedVert', new=2)
         print("")
     while True:
         print("Welcome To RedVert. What would you like to do?")
```

