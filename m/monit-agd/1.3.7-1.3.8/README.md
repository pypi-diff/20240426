# Comparing `tmp/monit-agd-1.3.7.tar.gz` & `tmp/monit-agd-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monit-agd-1.3.7.tar", last modified: Fri Apr 26 01:29:41 2024, max compression
+gzip compressed data, was "monit-agd-1.3.8.tar", last modified: Fri Apr 26 01:33:49 2024, max compression
```

## Comparing `monit-agd-1.3.7.tar` & `monit-agd-1.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-26 01:29:41.317516 monit-agd-1.3.7/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.3.7/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2268 2024-04-26 01:29:41.317516 monit-agd-1.3.7/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1631 2024-04-25 22:35:22.000000 monit-agd-1.3.7/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-26 01:29:41.314183 monit-agd-1.3.7/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 monit-agd-1.3.7/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      934 2024-04-26 01:29:09.000000 monit-agd-1.3.7/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      860 2024-04-25 17:07:54.000000 monit-agd-1.3.7/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1592 2024-04-25 16:30:27.000000 monit-agd-1.3.7/monit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 monit-agd-1.3.7/monit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3145 2024-04-22 21:01:19.000000 monit-agd-1.3.7/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 monit-agd-1.3.7/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 monit-agd-1.3.7/monit/logger.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      266 2024-04-25 23:01:36.000000 monit-agd-1.3.7/monit/verify_env.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-26 01:29:41.317516 monit-agd-1.3.7/monit_agd.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2268 2024-04-26 01:29:41.000000 monit-agd-1.3.7/monit_agd.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      339 2024-04-26 01:29:41.000000 monit-agd-1.3.7/monit_agd.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-26 01:29:41.000000 monit-agd-1.3.7/monit_agd.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-26 01:29:41.000000 monit-agd-1.3.7/monit_agd.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-04-26 01:29:41.000000 monit-agd-1.3.7/monit_agd.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-26 01:29:41.317516 monit-agd-1.3.7/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      867 2024-04-26 01:29:15.000000 monit-agd-1.3.7/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-26 01:33:49.304427 monit-agd-1.3.8/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.3.8/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2268 2024-04-26 01:33:49.301093 monit-agd-1.3.8/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1631 2024-04-25 22:35:22.000000 monit-agd-1.3.8/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-26 01:33:49.301093 monit-agd-1.3.8/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 monit-agd-1.3.8/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1074 2024-04-26 01:33:37.000000 monit-agd-1.3.8/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      860 2024-04-25 17:07:54.000000 monit-agd-1.3.8/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1592 2024-04-25 16:30:27.000000 monit-agd-1.3.8/monit/database.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 monit-agd-1.3.8/monit/error.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3145 2024-04-22 21:01:19.000000 monit-agd-1.3.8/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 monit-agd-1.3.8/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 monit-agd-1.3.8/monit/logger.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      266 2024-04-25 23:01:36.000000 monit-agd-1.3.8/monit/verify_env.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-26 01:33:49.301093 monit-agd-1.3.8/monit_agd.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2268 2024-04-26 01:33:49.000000 monit-agd-1.3.8/monit_agd.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      339 2024-04-26 01:33:49.000000 monit-agd-1.3.8/monit_agd.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-26 01:33:49.000000 monit-agd-1.3.8/monit_agd.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-26 01:33:49.000000 monit-agd-1.3.8/monit_agd.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-04-26 01:33:49.000000 monit-agd-1.3.8/monit_agd.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-26 01:33:49.304427 monit-agd-1.3.8/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      867 2024-04-26 01:33:45.000000 monit-agd-1.3.8/setup.py
```

### Comparing `monit-agd-1.3.7/LICENSE` & `monit-agd-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.7/PKG-INFO` & `monit-agd-1.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.3.7
+Version: 1.3.8
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `monit-agd-1.3.7/README.md` & `monit-agd-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.7/monit/config.py` & `monit-agd-1.3.8/monit/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from dotenv import load_dotenv
 import os
 import json
+import inspect
 
 load_dotenv()
 
-script_dir = os.path.dirname(os.path.abspath(__file__))
-env_path = os.path.join(script_dir, '.env')
+# script_dir = os.path.dirname(os.path.abspath(__file__))
+calling_script_dir = os.path.dirname(os.path.abspath(inspect.stack()[1].filename))
+env_path = os.path.join(calling_script_dir, '.env')
 load_dotenv(dotenv_path=env_path)
 
+insp = inspect.stack()
+
 # Code info
 project = os.getenv('PROJECT')
 company = os.getenv('COMPANY')
 location = os.getenv('LOCATION')
 dev = os.getenv('DEV')
 
 # Database info
@@ -22,12 +26,12 @@
 
 db_url = f'mysql+pymysql://{user}:{password}@{host}/{database}'
 
 # Email info
 email = os.getenv('EMAIL')
 email_password = os.getenv('EMAIL_PASSWORD')
 
-if not project or not company or not location or not dev:
-    raise Exception("Por favor, as informações do código não podem ficar em branco.")
+# if not project or not company or not location or not dev:
+#     raise Exception("Por favor, as informações do código não podem ficar em branco.")
 
-if not user or not password or not host or not database:
-    raise Exception("Por favor, as informações do banco de dados não podem ficar em branco.")
+# if not user or not password or not host or not database:
+#     raise Exception("Por favor, as informações do banco de dados não podem ficar em branco.")
```

### Comparing `monit-agd-1.3.7/monit/core.py` & `monit-agd-1.3.8/monit/core.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.7/monit/database.py` & `monit-agd-1.3.8/monit/database.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.7/monit/func.py` & `monit-agd-1.3.8/monit/func.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.7/monit/log2file.py` & `monit-agd-1.3.8/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.7/monit/logger.py` & `monit-agd-1.3.8/monit/logger.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.7/monit_agd.egg-info/PKG-INFO` & `monit-agd-1.3.8/monit_agd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.3.7
+Version: 1.3.8
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `monit-agd-1.3.7/setup.py` & `monit-agd-1.3.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='monit-agd',
-    version='1.3.7',
+    version='1.3.8',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

