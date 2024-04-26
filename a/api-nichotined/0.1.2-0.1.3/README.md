# Comparing `tmp/api-nichotined-0.1.2.tar.gz` & `tmp/api-nichotined-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-nichotined-0.1.2.tar", last modified: Fri Apr 26 10:37:13 2024, max compression
+gzip compressed data, was "api-nichotined-0.1.3.tar", last modified: Fri Apr 26 17:47:48 2024, max compression
```

## Comparing `api-nichotined-0.1.2.tar` & `api-nichotined-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 10:37:13.150215 api-nichotined-0.1.2/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1112 2024-04-26 10:37:13.149887 api-nichotined-0.1.2/PKG-INFO
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      648 2024-04-19 16:19:11.000000 api-nichotined-0.1.2/README.md
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 10:37:13.148062 api-nichotined-0.1.2/api_nichotined/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       65 2024-04-26 10:16:58.000000 api-nichotined-0.1.2/api_nichotined/__init__.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 10:37:13.149122 api-nichotined-0.1.2/api_nichotined/core/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 04:53:46.000000 api-nichotined-0.1.2/api_nichotined/core/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1749 2024-04-26 10:30:30.000000 api-nichotined-0.1.2/api_nichotined/core/core.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 10:37:13.149622 api-nichotined-0.1.2/api_nichotined.egg-info/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1112 2024-04-26 10:37:13.000000 api-nichotined-0.1.2/api_nichotined.egg-info/PKG-INFO
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      324 2024-04-26 10:37:13.000000 api-nichotined-0.1.2/api_nichotined.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        1 2024-04-26 10:37:13.000000 api-nichotined-0.1.2/api_nichotined.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       17 2024-04-26 10:37:13.000000 api-nichotined-0.1.2/api_nichotined.egg-info/requires.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       20 2024-04-26 10:37:13.000000 api-nichotined-0.1.2/api_nichotined.egg-info/top_level.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       38 2024-04-26 10:37:13.150282 api-nichotined-0.1.2/setup.cfg
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      718 2024-04-26 10:36:44.000000 api-nichotined-0.1.2/setup.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 10:37:13.149399 api-nichotined-0.1.2/test/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 05:21:55.000000 api-nichotined-0.1.2/test/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      451 2024-04-26 10:35:06.000000 api-nichotined-0.1.2/test/main.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 17:47:48.969874 api-nichotined-0.1.3/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1112 2024-04-26 17:47:48.969579 api-nichotined-0.1.3/PKG-INFO
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      648 2024-04-19 16:19:11.000000 api-nichotined-0.1.3/README.md
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 17:47:48.967057 api-nichotined-0.1.3/api_nichotined/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       65 2024-04-26 10:16:58.000000 api-nichotined-0.1.3/api_nichotined/__init__.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 17:47:48.968335 api-nichotined-0.1.3/api_nichotined/core/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 04:53:46.000000 api-nichotined-0.1.3/api_nichotined/core/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1713 2024-04-26 17:47:14.000000 api-nichotined-0.1.3/api_nichotined/core/core.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 17:47:48.969284 api-nichotined-0.1.3/api_nichotined.egg-info/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1112 2024-04-26 17:47:48.000000 api-nichotined-0.1.3/api_nichotined.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      324 2024-04-26 17:47:48.000000 api-nichotined-0.1.3/api_nichotined.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        1 2024-04-26 17:47:48.000000 api-nichotined-0.1.3/api_nichotined.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       17 2024-04-26 17:47:48.000000 api-nichotined-0.1.3/api_nichotined.egg-info/requires.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       20 2024-04-26 17:47:48.000000 api-nichotined-0.1.3/api_nichotined.egg-info/top_level.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       38 2024-04-26 17:47:48.969935 api-nichotined-0.1.3/setup.cfg
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      718 2024-04-26 17:47:24.000000 api-nichotined-0.1.3/setup.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 17:47:48.968872 api-nichotined-0.1.3/test/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 05:21:55.000000 api-nichotined-0.1.3/test/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      451 2024-04-26 10:35:06.000000 api-nichotined-0.1.3/test/main.py
```

### Comparing `api-nichotined-0.1.2/PKG-INFO` & `api-nichotined-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-nichotined
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple lib for testing rest API
 Home-page: https://github.com/nichotined/simple-api
 Author: Nicholas Frederich
 Author-email: nicholas.frederich.lagaunne@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `api-nichotined-0.1.2/README.md` & `api-nichotined-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `api-nichotined-0.1.2/api_nichotined/core/core.py` & `api-nichotined-0.1.3/api_nichotined/core/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
         response = self.session.request(method, url, params=params, data=data, json=json_data, headers=headers)
         curl = curlify.to_curl(response.request)
 
         self.logger.info(curl)
         self.logger.info(f"Response received for {method} request to {url} with status code {response.status_code}")
         self.logger.info(response.json())
-        response.raise_for_status()
         return response
 
     def get(self, path, params=None, data=None, json_data=None, headers=None) -> Response:
         return self._make_request("GET", path, params=params, data=data, headers=headers, json_data=json_data)
 
     def post(self, path, params=None, data=None, json_data=None, headers=None) -> Response:
         return self._make_request("POST", path, params=params, data=data, headers=headers, json_data=json_data)
```

### Comparing `api-nichotined-0.1.2/api_nichotined.egg-info/PKG-INFO` & `api-nichotined-0.1.3/api_nichotined.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-nichotined
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple lib for testing rest API
 Home-page: https://github.com/nichotined/simple-api
 Author: Nicholas Frederich
 Author-email: nicholas.frederich.lagaunne@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `api-nichotined-0.1.2/setup.py` & `api-nichotined-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="api-nichotined",
-    version="0.1.2",
+    version="0.1.3",
     author="Nicholas Frederich",
     author_email="nicholas.frederich.lagaunne@gmail.com",
     description="Simple lib for testing rest API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nichotined/simple-api",
     packages=setuptools.find_packages(),
```

