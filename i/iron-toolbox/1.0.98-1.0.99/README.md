# Comparing `tmp/iron_toolbox-1.0.98.tar.gz` & `tmp/iron_toolbox-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iron_toolbox-1.0.98.tar", last modified: Fri Apr 19 16:31:36 2024, max compression
+gzip compressed data, was "iron_toolbox-1.0.99.tar", last modified: Fri Apr 26 21:03:34 2024, max compression
```

## Comparing `iron_toolbox-1.0.98.tar` & `iron_toolbox-1.0.99.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:31:36.587547 iron_toolbox-1.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 16:31:30.000000 iron_toolbox-1.0.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-19 16:31:36.587547 iron_toolbox-1.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-19 16:31:30.000000 iron_toolbox-1.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:31:36.587547 iron_toolbox-1.0.98/iron_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 16:31:30.000000 iron_toolbox-1.0.98/iron_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-19 16:31:30.000000 iron_toolbox-1.0.98/iron_toolbox/aws_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-19 16:31:30.000000 iron_toolbox-1.0.98/iron_toolbox/domo_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19748 2024-04-19 16:31:30.000000 iron_toolbox-1.0.98/iron_toolbox/iron_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)   110645 2024-04-19 16:31:30.000000 iron_toolbox-1.0.98/iron_toolbox/mongo_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-19 16:31:30.000000 iron_toolbox-1.0.98/iron_toolbox/sftp_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:31:36.587547 iron_toolbox-1.0.98/iron_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-19 16:31:36.000000 iron_toolbox-1.0.98/iron_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-19 16:31:36.000000 iron_toolbox-1.0.98/iron_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:31:36.000000 iron_toolbox-1.0.98/iron_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 16:31:36.000000 iron_toolbox-1.0.98/iron_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 16:31:36.000000 iron_toolbox-1.0.98/iron_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 16:31:36.591547 iron_toolbox-1.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-19 16:31:30.000000 iron_toolbox-1.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:03:34.565451 iron_toolbox-1.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-26 21:03:28.000000 iron_toolbox-1.0.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-26 21:03:34.565451 iron_toolbox-1.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-26 21:03:28.000000 iron_toolbox-1.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:03:34.557451 iron_toolbox-1.0.99/iron_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 21:03:28.000000 iron_toolbox-1.0.99/iron_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-26 21:03:28.000000 iron_toolbox-1.0.99/iron_toolbox/aws_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-26 21:03:28.000000 iron_toolbox-1.0.99/iron_toolbox/domo_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19748 2024-04-26 21:03:28.000000 iron_toolbox-1.0.99/iron_toolbox/iron_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110733 2024-04-26 21:03:28.000000 iron_toolbox-1.0.99/iron_toolbox/mongo_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-26 21:03:28.000000 iron_toolbox-1.0.99/iron_toolbox/sftp_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:03:34.561451 iron_toolbox-1.0.99/iron_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-26 21:03:34.000000 iron_toolbox-1.0.99/iron_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-26 21:03:34.000000 iron_toolbox-1.0.99/iron_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:03:34.000000 iron_toolbox-1.0.99/iron_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-26 21:03:34.000000 iron_toolbox-1.0.99/iron_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 21:03:34.000000 iron_toolbox-1.0.99/iron_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 21:03:34.565451 iron_toolbox-1.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-26 21:03:28.000000 iron_toolbox-1.0.99/setup.py
```

### Comparing `iron_toolbox-1.0.98/LICENSE.txt` & `iron_toolbox-1.0.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.98/PKG-INFO` & `iron_toolbox-1.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iron_toolbox
-Version: 1.0.98
+Version: 1.0.99
 Summary: Functions to be used by Iron Data Analytics Team
 Home-page: https://github.com/IronTrainers/iron_data_toolbox
 Download-URL: https://github.com/IronTrainers/iron_data_toolbox/archive/refs/tags/iron_data_toolboox.tar.gz
 Author: Luciano Siqueira
 Author-email: lucianosiqueira@iron.fit
 License: MIT
 Project-URL: Bug Tracker, https://github.com/IronTrainers/iron_data_toolbox/issues
```

### Comparing `iron_toolbox-1.0.98/README.md` & `iron_toolbox-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.98/iron_toolbox/aws_functions.py` & `iron_toolbox-1.0.99/iron_toolbox/aws_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.98/iron_toolbox/domo_functions.py` & `iron_toolbox-1.0.99/iron_toolbox/domo_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.98/iron_toolbox/iron_functions.py` & `iron_toolbox-1.0.99/iron_toolbox/iron_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.98/iron_toolbox/mongo_functions.py` & `iron_toolbox-1.0.99/iron_toolbox/mongo_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,16 @@
                                                                         '_p_personalHealthCoach': 1,
                                                                         'cardEmissionDate': 1,
                                                                         'cardExpirationDate': 1,
                                                                         'cardHistory': 1,
                                                                         'isPatientCaptated': 1,
                                                                         'captationDate': 1,
                                                                         'captationInteractionId': 1,
-                                                                        'isStaff': 1,}), desc="Total itens recebidos:"))
+                                                                        'baseOrigem': 1,
+                                                                        'isStaff': 1}), desc="Total itens recebidos:"))
 
         dbuser = dbuser.replace({'_p_corporation': r'^Corporation\$'}, {'_p_corporation': ''},
                                 regex=True)
         dbuser = dbuser.replace({'_p_userPublic': r'^UserPublic\$'}, {'_p_userPublic': ''}, regex=True)
         dbuser = dbuser.replace({'_p_establishment': r'^EstablishmentData\$'}, {'_p_establishment': ''},
                                 regex=True)
     else:
```

### Comparing `iron_toolbox-1.0.98/iron_toolbox/sftp_functions.py` & `iron_toolbox-1.0.99/iron_toolbox/sftp_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.98/iron_toolbox.egg-info/PKG-INFO` & `iron_toolbox-1.0.99/iron_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iron_toolbox
-Version: 1.0.98
+Version: 1.0.99
 Summary: Functions to be used by Iron Data Analytics Team
 Home-page: https://github.com/IronTrainers/iron_data_toolbox
 Download-URL: https://github.com/IronTrainers/iron_data_toolbox/archive/refs/tags/iron_data_toolboox.tar.gz
 Author: Luciano Siqueira
 Author-email: lucianosiqueira@iron.fit
 License: MIT
 Project-URL: Bug Tracker, https://github.com/IronTrainers/iron_data_toolbox/issues
```

### Comparing `iron_toolbox-1.0.98/setup.py` & `iron_toolbox-1.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='iron_toolbox',
     packages=['iron_toolbox'],
-    version='1.0.98',
+    version='1.0.99',
     license='MIT',
     description='Functions to be used by Iron Data Analytics Team',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Luciano Siqueira',
     author_email='lucianosiqueira@iron.fit',
     url='https://github.com/IronTrainers/iron_data_toolbox',
```

