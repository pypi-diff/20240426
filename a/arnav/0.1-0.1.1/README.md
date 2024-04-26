# Comparing `tmp/arnav-0.1.tar.gz` & `tmp/arnav-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arnav-0.1.tar", last modified: Fri Apr 26 16:35:28 2024, max compression
+gzip compressed data, was "arnav-0.1.1.tar", last modified: Fri Apr 26 17:57:53 2024, max compression
```

## Comparing `arnav-0.1.tar` & `arnav-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 16:35:28.426985 arnav-0.1/
--rw-rw-rw-   0        0        0     1079 2024-04-26 16:35:14.000000 arnav-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      759 2024-04-26 16:35:28.427997 arnav-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-26 16:25:54.000000 arnav-0.1/README.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 16:35:28.397187 arnav-0.1/arnav/
--rw-rw-rw-   0        0        0       29 2024-04-26 16:24:46.000000 arnav-0.1/arnav/__init__.py
--rw-rw-rw-   0        0        0       40 2024-04-26 16:22:39.000000 arnav-0.1/arnav/slang.py
-drwxrwxrwx   0        0        0        0 2024-04-26 16:35:28.425980 arnav-0.1/arnav.egg-info/
--rw-rw-rw-   0        0        0      759 2024-04-26 16:35:28.000000 arnav-0.1/arnav.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-26 16:35:28.000000 arnav-0.1/arnav.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 16:35:28.000000 arnav-0.1/arnav.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 16:35:28.000000 arnav-0.1/arnav.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-26 16:35:28.428998 arnav-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1628 2024-04-26 16:34:47.000000 arnav-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:57:53.856388 arnav-0.1.1/
+-rw-rw-rw-   0        0        0     1079 2024-04-26 16:35:14.000000 arnav-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      763 2024-04-26 17:57:53.857396 arnav-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-26 16:25:54.000000 arnav-0.1.1/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 17:57:53.840081 arnav-0.1.1/arnav/
+-rw-rw-rw-   0        0        0       67 2024-04-26 17:52:12.000000 arnav-0.1.1/arnav/__init__.py
+-rw-rw-rw-   0        0        0       60 2024-04-26 17:51:54.000000 arnav-0.1.1/arnav/mathutils.py
+-rw-rw-rw-   0        0        0       68 2024-04-26 17:56:15.000000 arnav-0.1.1/arnav/slang.py
+drwxrwxrwx   0        0        0        0 2024-04-26 17:57:53.855356 arnav-0.1.1/arnav.egg-info/
+-rw-rw-rw-   0        0        0      763 2024-04-26 17:57:53.000000 arnav-0.1.1/arnav.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-26 17:57:53.000000 arnav-0.1.1/arnav.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 17:57:53.000000 arnav-0.1.1/arnav.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 17:57:53.000000 arnav-0.1.1/arnav.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-26 17:57:53.858796 arnav-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1632 2024-04-26 17:57:47.000000 arnav-0.1.1/setup.py
```

### Comparing `arnav-0.1/LICENSE.txt` & `arnav-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arnav-0.1/PKG-INFO` & `arnav-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arnav
-Version: 0.1
+Version: 0.1.1
 Summary: resting purposes
 Home-page: https://github.com/arnavjain2710/Pypi-Demo
-Download-URL: https://github.com/arnavjain2710/Pypi-Demo/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/arnavjain2710/Pypi-Demo/archive/refs/tags/v_01.1.tar.gz
 Author: Arnav Jain
 Author-email: jainarnav2710@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `arnav-0.1/arnav.egg-info/PKG-INFO` & `arnav-0.1.1/arnav.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arnav
-Version: 0.1
+Version: 0.1.1
 Summary: resting purposes
 Home-page: https://github.com/arnavjain2710/Pypi-Demo
-Download-URL: https://github.com/arnavjain2710/Pypi-Demo/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/arnavjain2710/Pypi-Demo/archive/refs/tags/v_01.1.tar.gz
 Author: Arnav Jain
 Author-email: jainarnav2710@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `arnav-0.1/setup.py` & `arnav-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'arnav',         # How you named your package folder (MyLib)
   packages = ['arnav'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'resting purposes',   # Give a short description about your library
   author = 'Arnav Jain',                   # Type in your name
   author_email = 'jainarnav2710@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/arnavjain2710/Pypi-Demo',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/arnavjain2710/Pypi-Demo/archive/refs/tags/v_01.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/arnavjain2710/Pypi-Demo/archive/refs/tags/v_01.1.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
```

