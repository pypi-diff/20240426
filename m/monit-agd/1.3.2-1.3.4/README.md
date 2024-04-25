# Comparing `tmp/monit-agd-1.3.2.tar.gz` & `tmp/monit-agd-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monit-agd-1.3.2.tar", last modified: Thu Apr 25 22:34:40 2024, max compression
+gzip compressed data, was "monit-agd-1.3.4.tar", last modified: Thu Apr 25 22:35:41 2024, max compression
```

## Comparing `monit-agd-1.3.2.tar` & `monit-agd-1.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 22:34:40.474790 monit-agd-1.3.2/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.3.2/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2235 2024-04-25 22:34:40.471457 monit-agd-1.3.2/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1598 2024-04-25 17:01:33.000000 monit-agd-1.3.2/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 22:34:40.471457 monit-agd-1.3.2/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 monit-agd-1.3.2/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      799 2024-04-25 16:26:23.000000 monit-agd-1.3.2/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      860 2024-04-25 17:07:54.000000 monit-agd-1.3.2/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1592 2024-04-25 16:30:27.000000 monit-agd-1.3.2/monit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 monit-agd-1.3.2/monit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3145 2024-04-22 21:01:19.000000 monit-agd-1.3.2/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 monit-agd-1.3.2/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 monit-agd-1.3.2/monit/logger.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      254 2024-04-25 16:25:13.000000 monit-agd-1.3.2/monit/verify_env.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 22:34:40.471457 monit-agd-1.3.2/monit_agd.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2235 2024-04-25 22:34:40.000000 monit-agd-1.3.2/monit_agd.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      339 2024-04-25 22:34:40.000000 monit-agd-1.3.2/monit_agd.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-25 22:34:40.000000 monit-agd-1.3.2/monit_agd.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-25 22:34:40.000000 monit-agd-1.3.2/monit_agd.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-04-25 22:34:40.000000 monit-agd-1.3.2/monit_agd.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-25 22:34:40.474790 monit-agd-1.3.2/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      867 2024-04-25 22:34:14.000000 monit-agd-1.3.2/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 22:35:41.117566 monit-agd-1.3.4/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.3.4/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2268 2024-04-25 22:35:41.117566 monit-agd-1.3.4/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1631 2024-04-25 22:35:22.000000 monit-agd-1.3.4/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 22:35:41.117566 monit-agd-1.3.4/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 monit-agd-1.3.4/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      799 2024-04-25 16:26:23.000000 monit-agd-1.3.4/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      860 2024-04-25 17:07:54.000000 monit-agd-1.3.4/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1592 2024-04-25 16:30:27.000000 monit-agd-1.3.4/monit/database.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 monit-agd-1.3.4/monit/error.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3145 2024-04-22 21:01:19.000000 monit-agd-1.3.4/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 monit-agd-1.3.4/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 monit-agd-1.3.4/monit/logger.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      254 2024-04-25 16:25:13.000000 monit-agd-1.3.4/monit/verify_env.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 22:35:41.117566 monit-agd-1.3.4/monit_agd.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2268 2024-04-25 22:35:41.000000 monit-agd-1.3.4/monit_agd.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      339 2024-04-25 22:35:41.000000 monit-agd-1.3.4/monit_agd.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-25 22:35:41.000000 monit-agd-1.3.4/monit_agd.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-25 22:35:41.000000 monit-agd-1.3.4/monit_agd.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-04-25 22:35:41.000000 monit-agd-1.3.4/monit_agd.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-25 22:35:41.117566 monit-agd-1.3.4/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      867 2024-04-25 22:35:29.000000 monit-agd-1.3.4/setup.py
```

### Comparing `monit-agd-1.3.2/LICENSE` & `monit-agd-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.2/PKG-INFO` & `monit-agd-1.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.3.2
+Version: 1.3.4
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -105,8 +105,11 @@
 ```bash
 SetupError
 DatabaseError
 HTTPError
 FileError
 FolderError
 TooManyRequests
+DataCreateError
+DataUpdateError
+
 ```
```

### Comparing `monit-agd-1.3.2/README.md` & `monit-agd-1.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -86,8 +86,11 @@
 ```bash
 SetupError
 DatabaseError
 HTTPError
 FileError
 FolderError
 TooManyRequests
+DataCreateError
+DataUpdateError
+
 ```
```

### Comparing `monit-agd-1.3.2/monit/config.py` & `monit-agd-1.3.4/monit/config.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.2/monit/core.py` & `monit-agd-1.3.4/monit/core.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.2/monit/database.py` & `monit-agd-1.3.4/monit/database.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.2/monit/func.py` & `monit-agd-1.3.4/monit/func.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.2/monit/log2file.py` & `monit-agd-1.3.4/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.2/monit/logger.py` & `monit-agd-1.3.4/monit/logger.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.2/monit_agd.egg-info/PKG-INFO` & `monit-agd-1.3.4/monit_agd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.3.2
+Version: 1.3.4
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -105,8 +105,11 @@
 ```bash
 SetupError
 DatabaseError
 HTTPError
 FileError
 FolderError
 TooManyRequests
+DataCreateError
+DataUpdateError
+
 ```
```

### Comparing `monit-agd-1.3.2/setup.py` & `monit-agd-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='monit-agd',
-    version='1.3.2',
+    version='1.3.4',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

