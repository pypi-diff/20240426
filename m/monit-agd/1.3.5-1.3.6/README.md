# Comparing `tmp/monit-agd-1.3.5.tar.gz` & `tmp/monit-agd-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monit-agd-1.3.5.tar", last modified: Thu Apr 25 23:01:45 2024, max compression
+gzip compressed data, was "monit-agd-1.3.6.tar", last modified: Fri Apr 26 01:20:31 2024, max compression
```

## Comparing `monit-agd-1.3.5.tar` & `monit-agd-1.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 23:01:45.682584 monit-agd-1.3.5/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.3.5/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2268 2024-04-25 23:01:45.682584 monit-agd-1.3.5/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1631 2024-04-25 22:35:22.000000 monit-agd-1.3.5/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 23:01:45.679251 monit-agd-1.3.5/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 monit-agd-1.3.5/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      799 2024-04-25 16:26:23.000000 monit-agd-1.3.5/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      860 2024-04-25 17:07:54.000000 monit-agd-1.3.5/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1592 2024-04-25 16:30:27.000000 monit-agd-1.3.5/monit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 monit-agd-1.3.5/monit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3145 2024-04-22 21:01:19.000000 monit-agd-1.3.5/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 monit-agd-1.3.5/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 monit-agd-1.3.5/monit/logger.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      266 2024-04-25 23:01:36.000000 monit-agd-1.3.5/monit/verify_env.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-25 23:01:45.682584 monit-agd-1.3.5/monit_agd.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2268 2024-04-25 23:01:45.000000 monit-agd-1.3.5/monit_agd.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      339 2024-04-25 23:01:45.000000 monit-agd-1.3.5/monit_agd.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-25 23:01:45.000000 monit-agd-1.3.5/monit_agd.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-25 23:01:45.000000 monit-agd-1.3.5/monit_agd.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-04-25 23:01:45.000000 monit-agd-1.3.5/monit_agd.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-25 23:01:45.682584 monit-agd-1.3.5/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      867 2024-04-25 23:01:41.000000 monit-agd-1.3.5/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-26 01:20:31.247828 monit-agd-1.3.6/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.3.6/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2268 2024-04-26 01:20:31.247828 monit-agd-1.3.6/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1631 2024-04-25 22:35:22.000000 monit-agd-1.3.6/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-26 01:20:31.247828 monit-agd-1.3.6/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 monit-agd-1.3.6/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      807 2024-04-26 01:18:08.000000 monit-agd-1.3.6/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      860 2024-04-25 17:07:54.000000 monit-agd-1.3.6/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1592 2024-04-25 16:30:27.000000 monit-agd-1.3.6/monit/database.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 monit-agd-1.3.6/monit/error.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3145 2024-04-22 21:01:19.000000 monit-agd-1.3.6/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 monit-agd-1.3.6/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 monit-agd-1.3.6/monit/logger.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      266 2024-04-25 23:01:36.000000 monit-agd-1.3.6/monit/verify_env.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-26 01:20:31.247828 monit-agd-1.3.6/monit_agd.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2268 2024-04-26 01:20:31.000000 monit-agd-1.3.6/monit_agd.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      339 2024-04-26 01:20:31.000000 monit-agd-1.3.6/monit_agd.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-26 01:20:31.000000 monit-agd-1.3.6/monit_agd.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-26 01:20:31.000000 monit-agd-1.3.6/monit_agd.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-04-26 01:20:31.000000 monit-agd-1.3.6/monit_agd.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-26 01:20:31.247828 monit-agd-1.3.6/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      867 2024-04-26 01:20:26.000000 monit-agd-1.3.6/setup.py
```

### Comparing `monit-agd-1.3.5/LICENSE` & `monit-agd-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.5/PKG-INFO` & `monit-agd-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.3.5
+Version: 1.3.6
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `monit-agd-1.3.5/README.md` & `monit-agd-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.5/monit/config.py` & `monit-agd-1.3.6/monit/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 
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

### Comparing `monit-agd-1.3.5/monit/core.py` & `monit-agd-1.3.6/monit/core.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.5/monit/database.py` & `monit-agd-1.3.6/monit/database.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.5/monit/func.py` & `monit-agd-1.3.6/monit/func.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.5/monit/log2file.py` & `monit-agd-1.3.6/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.5/monit/logger.py` & `monit-agd-1.3.6/monit/logger.py`

 * *Files identical despite different names*

### Comparing `monit-agd-1.3.5/monit_agd.egg-info/PKG-INFO` & `monit-agd-1.3.6/monit_agd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.3.5
+Version: 1.3.6
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `monit-agd-1.3.5/setup.py` & `monit-agd-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='monit-agd',
-    version='1.3.5',
+    version='1.3.6',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

