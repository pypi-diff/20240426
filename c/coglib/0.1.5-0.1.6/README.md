# Comparing `tmp/coglib-0.1.5.tar.gz` & `tmp/coglib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coglib-0.1.5.tar", last modified: Mon Apr 15 08:45:20 2024, max compression
+gzip compressed data, was "coglib-0.1.6.tar", last modified: Fri Apr 26 02:51:58 2024, max compression
```

## Comparing `coglib-0.1.5.tar` & `coglib-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 08:45:20.196085 coglib-0.1.5/
--rw-rw-rw-   0        0        0      548 2024-04-15 08:45:20.190087 coglib-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      110 2024-04-15 03:28:49.000000 coglib-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 08:45:20.162715 coglib-0.1.5/coglib/
--rw-rw-rw-   0        0        0        0 2024-04-15 03:17:14.000000 coglib-0.1.5/coglib/__init__.py
--rw-rw-rw-   0        0        0     5443 2024-04-15 08:44:40.000000 coglib-0.1.5/coglib/coglib.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:45:20.185125 coglib-0.1.5/coglib.egg-info/
--rw-rw-rw-   0        0        0      548 2024-04-15 08:45:20.000000 coglib-0.1.5/coglib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-04-15 08:45:20.000000 coglib-0.1.5/coglib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 08:45:20.000000 coglib-0.1.5/coglib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 08:45:20.000000 coglib-0.1.5/coglib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 08:45:20.000000 coglib-0.1.5/coglib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 08:45:20.197084 coglib-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      649 2024-04-15 08:45:09.000000 coglib-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:51:58.788264 coglib-0.1.6/
+-rw-rw-rw-   0        0        0      548 2024-04-26 02:51:58.785262 coglib-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2024-04-15 03:28:49.000000 coglib-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 02:51:58.744306 coglib-0.1.6/coglib/
+-rw-rw-rw-   0        0        0        0 2024-04-15 03:17:14.000000 coglib-0.1.6/coglib/__init__.py
+-rw-rw-rw-   0        0        0     5684 2024-04-26 02:51:18.000000 coglib-0.1.6/coglib/coglib.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:51:58.783258 coglib-0.1.6/coglib.egg-info/
+-rw-rw-rw-   0        0        0      548 2024-04-26 02:51:58.000000 coglib-0.1.6/coglib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-04-26 02:51:58.000000 coglib-0.1.6/coglib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 02:51:58.000000 coglib-0.1.6/coglib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-26 02:51:58.000000 coglib-0.1.6/coglib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 02:51:58.000000 coglib-0.1.6/coglib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 02:51:58.789265 coglib-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      649 2024-04-26 02:51:34.000000 coglib-0.1.6/setup.py
```

### Comparing `coglib-0.1.5/PKG-INFO` & `coglib-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coglib
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `coglib-0.1.5/coglib/coglib.py` & `coglib-0.1.6/coglib/coglib.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,15 +109,21 @@
         
 
     def get_command(self,route:str,querystring:str):
         url = f"{self.base_url}{route}?{querystring}"     
         response = requests.get(url,headers=self.headers)   
         return response
         
+    def write_json_to_csv(data, output_file):
+        df = pd.DataFrame(data)
+        df.to_csv(output_file, index=False)
 
+    def write_dataframe_to_csv(data, output_file):        
+        df.to_csv(data, index=False)        
+        
 class EconData:    
     def __init__(self, data,as_dataframe=False):        
         self.baseunit=data['baseunit'];
         self.country=data['country'];
         self.countryCode=data['countryCode'];
         self.frequency=data['frequency'];
         self.name=data['name'];
```

### Comparing `coglib-0.1.5/coglib.egg-info/PKG-INFO` & `coglib-0.1.6/coglib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coglib
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `coglib-0.1.5/setup.py` & `coglib-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='coglib',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=['requests', 'pandas'],  # Add any dependencies
     author='Kannan M',
     author_email='kannan.m@cogencis.com',
     description='Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

