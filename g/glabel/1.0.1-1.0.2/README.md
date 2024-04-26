# Comparing `tmp/glabel-1.0.1.tar.gz` & `tmp/glabel-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glabel-1.0.1.tar", last modified: Fri Apr 26 16:14:49 2024, max compression
+gzip compressed data, was "glabel-1.0.2.tar", last modified: Fri Apr 26 16:21:11 2024, max compression
```

## Comparing `glabel-1.0.1.tar` & `glabel-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 16:14:49.885374 glabel-1.0.1/
--rw-rw-rw-   0        0        0     3189 2024-04-26 16:14:49.881358 glabel-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2412 2024-04-26 16:06:32.000000 glabel-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 16:14:49.785133 glabel-1.0.1/glabel/
--rw-rw-rw-   0        0        0       22 2024-04-26 16:13:24.000000 glabel-1.0.1/glabel/__init__.py
--rw-rw-rw-   0        0        0      322 2024-04-26 16:13:13.000000 glabel-1.0.1/glabel/cli.py
--rw-rw-rw-   0        0        0     6457 2024-04-26 15:48:47.000000 glabel-1.0.1/glabel/main.py
-drwxrwxrwx   0        0        0        0 2024-04-26 16:14:49.876291 glabel-1.0.1/glabel.egg-info/
--rw-rw-rw-   0        0        0     3189 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 16:14:49.885374 glabel-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1779 2024-04-26 16:14:40.000000 glabel-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:21:11.408021 glabel-1.0.2/
+-rw-rw-rw-   0        0        0     3189 2024-04-26 16:21:11.406025 glabel-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2412 2024-04-26 16:06:32.000000 glabel-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 16:21:11.350605 glabel-1.0.2/glabel/
+-rw-rw-rw-   0        0        0       22 2024-04-26 16:13:24.000000 glabel-1.0.2/glabel/__init__.py
+-rw-rw-rw-   0        0        0      393 2024-04-26 16:20:51.000000 glabel-1.0.2/glabel/cli.py
+-rw-rw-rw-   0        0        0     6457 2024-04-26 15:48:47.000000 glabel-1.0.2/glabel/main.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:21:11.398959 glabel-1.0.2/glabel.egg-info/
+-rw-rw-rw-   0        0        0     3189 2024-04-26 16:21:10.000000 glabel-1.0.2/glabel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-26 16:21:11.000000 glabel-1.0.2/glabel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 16:21:10.000000 glabel-1.0.2/glabel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-26 16:21:10.000000 glabel-1.0.2/glabel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-04-26 16:21:10.000000 glabel-1.0.2/glabel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 16:21:11.000000 glabel-1.0.2/glabel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 16:21:11.408021 glabel-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1780 2024-04-26 16:21:03.000000 glabel-1.0.2/setup.py
```

### Comparing `glabel-1.0.1/PKG-INFO` & `glabel-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glabel
-Version: 1.0.1
+Version: 1.0.2
 Summary: FastAPI-based image classification app for annotation
 Home-page: https://github.com/gaurang157/glabel
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Keywords: image-classification,annotation,fastapi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `glabel-1.0.1/README.md` & `glabel-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `glabel-1.0.1/glabel/main.py` & `glabel-1.0.2/glabel/main.py`

 * *Files identical despite different names*

### Comparing `glabel-1.0.1/glabel.egg-info/PKG-INFO` & `glabel-1.0.2/glabel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glabel
-Version: 1.0.1
+Version: 1.0.2
 Summary: FastAPI-based image classification app for annotation
 Home-page: https://github.com/gaurang157/glabel
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Keywords: image-classification,annotation,fastapi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `glabel-1.0.1/setup.py` & `glabel-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 # Read the README.md content
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='glabel',  # Name of your package
-    version='1.0.1',  # Initial version
+    version='1.0.2',  # Initial version
     author='Gaurang Ingle',  # Your name
     author_email='gaurang.ingle@gmail.com',  # Your email
     description='FastAPI-based image classification app for annotation',  # Short description
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/gaurang157/glabel',  # Link to the project (e.g., GitHub)
     packages=find_packages(),  # Finds all packages in your source code
@@ -30,12 +30,12 @@
     keywords='image-classification, annotation, fastapi',  # Keywords for search
     install_requires=[  # Dependencies for your package
         'fastapi>=0.68.0',
         'uvicorn>=0.15.0',
     ],
     entry_points={
         'console_scripts': [
-            'glabel=glabel.main:app',  # CLI command to launch the app
+            'glabel=glabel.cli:main2',  # CLI command to launch the app
         ],
     },
     python_requires='>=3.6',  # Minimum Python version required
 )
```

