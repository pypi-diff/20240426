# Comparing `tmp/pygooglehelper-0.0.5.tar.gz` & `tmp/pygooglehelper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygooglehelper-0.0.5.tar", last modified: Sat Oct 21 11:06:51 2023, max compression
+gzip compressed data, was "pygooglehelper-0.0.6.tar", last modified: Fri Apr 26 00:27:51 2024, max compression
```

## Comparing `pygooglehelper-0.0.5.tar` & `pygooglehelper-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-10-21 11:06:51.235607 pygooglehelper-0.0.5/
--rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-10-21 11:06:39.000000 pygooglehelper-0.0.5/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1529 2023-10-21 11:06:51.235607 pygooglehelper-0.0.5/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      426 2023-10-21 11:06:39.000000 pygooglehelper-0.0.5/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-10-21 11:06:51.235607 pygooglehelper-0.0.5/pygooglehelper/
--rw-r--r--   0 mark      (1000) mark      (1000)      236 2023-10-21 11:05:48.000000 pygooglehelper-0.0.5/pygooglehelper/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2946 2023-10-21 10:59:37.000000 pygooglehelper-0.0.5/pygooglehelper/auth.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1173 2023-10-21 10:48:16.000000 pygooglehelper-0.0.5/pygooglehelper/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      386 2023-10-21 10:53:57.000000 pygooglehelper-0.0.5/pygooglehelper/register_hook.py
--rw-r--r--   0 mark      (1000) mark      (1000)      187 2023-10-21 11:06:39.000000 pygooglehelper-0.0.5/pygooglehelper/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)      360 2020-11-15 12:57:38.000000 pygooglehelper-0.0.5/pygooglehelper/util.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-10-21 11:06:51.235607 pygooglehelper-0.0.5/pygooglehelper.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1529 2023-10-21 11:06:51.000000 pygooglehelper-0.0.5/pygooglehelper.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      382 2023-10-21 11:06:51.000000 pygooglehelper-0.0.5/pygooglehelper.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-10-21 11:06:51.000000 pygooglehelper-0.0.5/pygooglehelper.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       75 2023-10-21 11:06:51.000000 pygooglehelper-0.0.5/pygooglehelper.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       15 2023-10-21 11:06:51.000000 pygooglehelper-0.0.5/pygooglehelper.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-10-21 11:06:51.236607 pygooglehelper-0.0.5/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1550 2023-10-21 11:06:39.000000 pygooglehelper-0.0.5/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 00:27:51.347621 pygooglehelper-0.0.6/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1069 2024-04-26 00:27:38.000000 pygooglehelper-0.0.6/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1435 2024-04-26 00:27:51.347621 pygooglehelper-0.0.6/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      432 2024-04-26 00:27:38.000000 pygooglehelper-0.0.6/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 00:27:51.347621 pygooglehelper-0.0.6/pygooglehelper/
+-rw-r--r--   0 mark      (1000) mark      (1000)      236 2023-10-21 11:05:48.000000 pygooglehelper-0.0.6/pygooglehelper/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2917 2024-04-26 00:27:13.000000 pygooglehelper-0.0.6/pygooglehelper/auth.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1173 2023-10-21 10:48:16.000000 pygooglehelper-0.0.6/pygooglehelper/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      386 2023-10-21 10:53:57.000000 pygooglehelper-0.0.6/pygooglehelper/register_hook.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      187 2024-04-26 00:27:38.000000 pygooglehelper-0.0.6/pygooglehelper/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      360 2020-11-15 12:57:38.000000 pygooglehelper-0.0.6/pygooglehelper/util.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-26 00:27:51.347621 pygooglehelper-0.0.6/pygooglehelper.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1435 2024-04-26 00:27:51.000000 pygooglehelper-0.0.6/pygooglehelper.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      382 2024-04-26 00:27:51.000000 pygooglehelper-0.0.6/pygooglehelper.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-26 00:27:51.000000 pygooglehelper-0.0.6/pygooglehelper.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       75 2024-04-26 00:27:51.000000 pygooglehelper-0.0.6/pygooglehelper.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       15 2024-04-26 00:27:51.000000 pygooglehelper-0.0.6/pygooglehelper.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2024-04-26 00:27:51.347621 pygooglehelper-0.0.6/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1452 2024-04-26 00:27:38.000000 pygooglehelper-0.0.6/setup.py
```

### Comparing `pygooglehelper-0.0.5/LICENSE` & `pygooglehelper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygooglehelper-0.0.5/PKG-INFO` & `pygooglehelper-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: pygooglehelper
-Version: 0.0.5
+Version: 0.0.6
 Summary: help you with the google API
 Home-page: https://veltzer.github.io/pygooglehelper
 Download-URL: https://github.com/veltzer/pygooglehelper
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Keywords: API,google,python,auth,pagination
+Keywords: api,google,python,auth,pagination
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: google-api-python-client
 Requires-Dist: google-auth-httplib2
 Requires-Dist: google-auth-oauthlib
@@ -39,10 +37,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pygooglehelper
 
 author: Mark Veltzer
 
-version: 0.0.5
+version: 0.0.6
 
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023, 2024
```

### Comparing `pygooglehelper-0.0.5/pygooglehelper/auth.py` & `pygooglehelper-0.0.6/pygooglehelper/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         if credentials is not None:
             if credentials.expired and credentials.refresh_token:
                 logger.debug("refreshing credentials")
                 credentials.refresh(Request())
         else:
             client_secret = os.path.expanduser(f"~/.config/{app_name}/client_secret.json")
             if not os.path.isfile(client_secret):
-                raise IOError(f"missing client secret file [{client_secret}] for application [{app_name}]")
+                raise IOError(f"missing [{client_secret=}] for [{app_name=}]")
             logger.debug(f"creating credentials from client secret at {client_secret}")
             flow = InstalledAppFlow.from_client_secrets_file(
                 client_secret, scopes,
             )
             credentials = flow.run_local_server(
                 host=host,
                 port=port,
```

### Comparing `pygooglehelper-0.0.5/pygooglehelper/configs.py` & `pygooglehelper-0.0.6/pygooglehelper/configs.py`

 * *Files identical despite different names*

### Comparing `pygooglehelper-0.0.5/pygooglehelper.egg-info/PKG-INFO` & `pygooglehelper-0.0.6/pygooglehelper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: pygooglehelper
-Version: 0.0.5
+Version: 0.0.6
 Summary: help you with the google API
 Home-page: https://veltzer.github.io/pygooglehelper
 Download-URL: https://github.com/veltzer/pygooglehelper
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Keywords: API,google,python,auth,pagination
+Keywords: api,google,python,auth,pagination
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: google-api-python-client
 Requires-Dist: google-auth-httplib2
 Requires-Dist: google-auth-oauthlib
@@ -39,10 +37,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pygooglehelper
 
 author: Mark Veltzer
 
-version: 0.0.5
+version: 0.0.6
 
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023, 2024
```

### Comparing `pygooglehelper-0.0.5/setup.py` & `pygooglehelper-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
     with open("README.rst") as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pygooglehelper",
-    version="0.0.5",
+    version="0.0.6",
     packages=[
         "pygooglehelper",
     ],
     # from here all is optional
     description="help you with the google API",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
-        "API",
+        "api",
         "google",
         "python",
         "auth",
         "pagination",
     ],
     url="https://veltzer.github.io/pygooglehelper",
     download_url="https://github.com/veltzer/pygooglehelper",
@@ -43,14 +43,12 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
     ],
 )
```

