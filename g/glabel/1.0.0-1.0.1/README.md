# Comparing `tmp/glabel-1.0.0.tar.gz` & `tmp/glabel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glabel-1.0.0.tar", last modified: Fri Apr 26 16:08:47 2024, max compression
+gzip compressed data, was "glabel-1.0.1.tar", last modified: Fri Apr 26 16:14:49 2024, max compression
```

## Comparing `glabel-1.0.0.tar` & `glabel-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 16:08:47.863229 glabel-1.0.0/
--rw-rw-rw-   0        0        0     3189 2024-04-26 16:08:47.860220 glabel-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2412 2024-04-26 16:06:32.000000 glabel-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 16:08:47.855130 glabel-1.0.0/glabel.egg-info/
--rw-rw-rw-   0        0        0     3189 2024-04-26 16:08:47.000000 glabel-1.0.0/glabel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-26 16:08:47.000000 glabel-1.0.0/glabel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 16:08:47.000000 glabel-1.0.0/glabel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-26 16:08:47.000000 glabel-1.0.0/glabel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2024-04-26 16:08:47.000000 glabel-1.0.0/glabel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 16:08:47.000000 glabel-1.0.0/glabel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 16:08:47.864220 glabel-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1737 2024-04-26 16:07:45.000000 glabel-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:14:49.885374 glabel-1.0.1/
+-rw-rw-rw-   0        0        0     3189 2024-04-26 16:14:49.881358 glabel-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2412 2024-04-26 16:06:32.000000 glabel-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 16:14:49.785133 glabel-1.0.1/glabel/
+-rw-rw-rw-   0        0        0       22 2024-04-26 16:13:24.000000 glabel-1.0.1/glabel/__init__.py
+-rw-rw-rw-   0        0        0      322 2024-04-26 16:13:13.000000 glabel-1.0.1/glabel/cli.py
+-rw-rw-rw-   0        0        0     6457 2024-04-26 15:48:47.000000 glabel-1.0.1/glabel/main.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:14:49.876291 glabel-1.0.1/glabel.egg-info/
+-rw-rw-rw-   0        0        0     3189 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 16:14:49.000000 glabel-1.0.1/glabel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 16:14:49.885374 glabel-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1779 2024-04-26 16:14:40.000000 glabel-1.0.1/setup.py
```

### Comparing `glabel-1.0.0/PKG-INFO` & `glabel-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glabel
-Version: 1.0.0
+Version: 1.0.1
 Summary: FastAPI-based image classification app for annotation
 Home-page: https://github.com/gaurang157/glabel
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Keywords: image-classification,annotation,fastapi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `glabel-1.0.0/README.md` & `glabel-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `glabel-1.0.0/glabel.egg-info/PKG-INFO` & `glabel-1.0.1/glabel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glabel
-Version: 1.0.0
+Version: 1.0.1
 Summary: FastAPI-based image classification app for annotation
 Home-page: https://github.com/gaurang157/glabel
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Keywords: image-classification,annotation,fastapi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `glabel-1.0.0/setup.py` & `glabel-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 from setuptools import setup, find_packages
 # Read the README.md content
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='glabel',  # Name of your package
-    version='1.0.0',  # Initial version
+    version='1.0.1',  # Initial version
     author='Gaurang Ingle',  # Your name
     author_email='gaurang.ingle@gmail.com',  # Your email
     description='FastAPI-based image classification app for annotation',  # Short description
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/gaurang157/glabel',  # Link to the project (e.g., GitHub)
     packages=find_packages(),  # Finds all packages in your source code
+    package_data={'glabel': ['cli.py']},
     include_package_data=True,  # Include additional data files specified in MANIFEST.in
     classifiers=[  # Classifiers to categorize your package
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

