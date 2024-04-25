# Comparing `tmp/redvert-1.0.4.tar.gz` & `tmp/redvert-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvert-1.0.4.tar", last modified: Thu Apr 25 21:40:46 2024, max compression
+gzip compressed data, was "redvert-1.2.0.tar", last modified: Thu Apr 25 22:21:56 2024, max compression
```

## Comparing `redvert-1.0.4.tar` & `redvert-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 21:40:46.126664 redvert-1.0.4/
--rw-rw-rw-   0        0        0     8808 2024-04-25 21:40:46.123894 redvert-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 21:40:46.123201 redvert-1.0.4/RedVert.egg-info/
--rw-rw-rw-   0        0        0     8808 2024-04-25 21:40:45.000000 redvert-1.0.4/RedVert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-25 21:40:46.000000 redvert-1.0.4/RedVert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 21:40:45.000000 redvert-1.0.4/RedVert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-25 21:40:45.000000 redvert-1.0.4/RedVert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 21:40:45.000000 redvert-1.0.4/RedVert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 21:40:46.120193 redvert-1.0.4/redvert/
--rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.0.4/redvert/__init__.py
--rw-rw-rw-   0        0        0     7381 2024-04-25 21:13:40.000000 redvert-1.0.4/redvert/main.py
--rw-rw-rw-   0        0        0       42 2024-04-25 21:40:46.128104 redvert-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-04-25 21:25:41.000000 redvert-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 22:21:56.467166 redvert-1.2.0/
+-rw-rw-rw-   0        0        0     8808 2024-04-25 22:21:56.463710 redvert-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 22:21:56.458821 redvert-1.2.0/RedVert.egg-info/
+-rw-rw-rw-   0        0        0     8808 2024-04-25 22:21:56.000000 redvert-1.2.0/RedVert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-25 22:21:56.000000 redvert-1.2.0/RedVert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 22:21:56.000000 redvert-1.2.0/RedVert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-25 22:21:56.000000 redvert-1.2.0/RedVert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 22:21:56.000000 redvert-1.2.0/RedVert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 22:21:56.457008 redvert-1.2.0/redvert/
+-rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.2.0/redvert/__init__.py
+-rw-rw-rw-   0        0        0     7454 2024-04-25 22:21:36.000000 redvert-1.2.0/redvert/main.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 22:21:56.467166 redvert-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-04-25 22:21:47.000000 redvert-1.2.0/setup.py
```

### Comparing `redvert-1.0.4/PKG-INFO` & `redvert-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.0.4
+Version: 1.2.0
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
```

### Comparing `redvert-1.0.4/RedVert.egg-info/PKG-INFO` & `redvert-1.2.0/RedVert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.0.4
+Version: 1.2.0
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
```

### Comparing `redvert-1.0.4/redvert/main.py` & `redvert-1.2.0/redvert/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 def remove_content_from_file(filename):
     removeEnvironments(filename)
 
 def Initalize():
     i = 0
     while True:
         print("Welcome To RedVert. What would you like to do?")
-        print("Create Env, Access Env, Remove All Env, Clear Console")
+        print("Create Env, Access Env, Remove All Env, Clear Console, Exit")
         user_input = input('>>> ')
         if user_input == 'Create Env':
             print("Name Environment")
             env_name[f'env{i}'] = input('>>> ')
             save_to_file(str(env_name), env_file)
             print("Successfully Created Environment\n")
             i += 1
@@ -201,9 +201,11 @@
                         except:
                             print("RedVert File Is Non Existent\n")
                     else:
                         print("Unknown Command Please Try Again\n")
                         continue
             except:
                 print("Unable To Open Environments File\n")
+        elif user_input == "Exit":
+            os.system('exit')
         else:
             print("Unknown RedVert Command Try Again.\n")
```

