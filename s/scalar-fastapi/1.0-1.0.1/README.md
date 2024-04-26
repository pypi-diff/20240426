# Comparing `tmp/scalar_fastapi-1.0.tar.gz` & `tmp/scalar_fastapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalar_fastapi-1.0.tar", last modified: Fri Apr 26 02:53:23 2024, max compression
+gzip compressed data, was "scalar_fastapi-1.0.1.tar", last modified: Fri Apr 26 07:10:43 2024, max compression
```

## Comparing `scalar_fastapi-1.0.tar` & `scalar_fastapi-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 marclaventure   (501) staff       (20)        0 2024-04-26 02:53:23.991056 scalar_fastapi-1.0/
--rw-r--r--   0 marclaventure   (501) staff       (20)      317 2024-04-26 02:53:23.990973 scalar_fastapi-1.0/PKG-INFO
--rw-r--r--   0 marclaventure   (501) staff       (20)        0 2024-04-26 02:12:06.000000 scalar_fastapi-1.0/README.md
-drwxr-xr-x   0 marclaventure   (501) staff       (20)        0 2024-04-26 02:53:23.989871 scalar_fastapi-1.0/scalar_fastapi/
--rw-r--r--   0 marclaventure   (501) staff       (20)        0 2024-04-26 02:11:52.000000 scalar_fastapi-1.0/scalar_fastapi/__init__.py
--rw-r--r--   0 marclaventure   (501) staff       (20)     2124 2024-04-26 02:41:39.000000 scalar_fastapi-1.0/scalar_fastapi/scalar_fastapi.py
-drwxr-xr-x   0 marclaventure   (501) staff       (20)        0 2024-04-26 02:53:23.990595 scalar_fastapi-1.0/scalar_fastapi.egg-info/
--rw-r--r--   0 marclaventure   (501) staff       (20)      317 2024-04-26 02:53:23.000000 scalar_fastapi-1.0/scalar_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 marclaventure   (501) staff       (20)      258 2024-04-26 02:53:23.000000 scalar_fastapi-1.0/scalar_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 marclaventure   (501) staff       (20)        1 2024-04-26 02:53:23.000000 scalar_fastapi-1.0/scalar_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 marclaventure   (501) staff       (20)       21 2024-04-26 02:53:23.000000 scalar_fastapi-1.0/scalar_fastapi.egg-info/top_level.txt
--rw-r--r--   0 marclaventure   (501) staff       (20)       38 2024-04-26 02:53:23.991246 scalar_fastapi-1.0/setup.cfg
--rw-r--r--   0 marclaventure   (501) staff       (20)      575 2024-04-26 02:53:18.000000 scalar_fastapi-1.0/setup.py
-drwxr-xr-x   0 marclaventure   (501) staff       (20)        0 2024-04-26 02:53:23.990725 scalar_fastapi-1.0/tests/
--rw-r--r--   0 marclaventure   (501) staff       (20)        0 2024-04-26 02:11:55.000000 scalar_fastapi-1.0/tests/__init__.py
+drwxr-xr-x   0 marclaventure   (501) staff       (20)        0 2024-04-26 07:10:43.321661 scalar_fastapi-1.0.1/
+-rw-r--r--   0 marclaventure   (501) staff       (20)      319 2024-04-26 07:10:43.321519 scalar_fastapi-1.0.1/PKG-INFO
+-rw-r--r--   0 marclaventure   (501) staff       (20)        0 2024-04-26 02:12:06.000000 scalar_fastapi-1.0.1/README.md
+drwxr-xr-x   0 marclaventure   (501) staff       (20)        0 2024-04-26 07:10:43.320501 scalar_fastapi-1.0.1/scalar_fastapi/
+-rw-r--r--   0 marclaventure   (501) staff       (20)       52 2024-04-26 07:00:13.000000 scalar_fastapi-1.0.1/scalar_fastapi/__init__.py
+-rw-r--r--   0 marclaventure   (501) staff       (20)     5334 2024-04-26 07:07:56.000000 scalar_fastapi-1.0.1/scalar_fastapi/scalar_fastapi.py
+drwxr-xr-x   0 marclaventure   (501) staff       (20)        0 2024-04-26 07:10:43.321051 scalar_fastapi-1.0.1/scalar_fastapi.egg-info/
+-rw-r--r--   0 marclaventure   (501) staff       (20)      319 2024-04-26 07:10:43.000000 scalar_fastapi-1.0.1/scalar_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 marclaventure   (501) staff       (20)      258 2024-04-26 07:10:43.000000 scalar_fastapi-1.0.1/scalar_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 marclaventure   (501) staff       (20)        1 2024-04-26 07:10:43.000000 scalar_fastapi-1.0.1/scalar_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 marclaventure   (501) staff       (20)       21 2024-04-26 07:10:43.000000 scalar_fastapi-1.0.1/scalar_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 marclaventure   (501) staff       (20)       38 2024-04-26 07:10:43.321902 scalar_fastapi-1.0.1/setup.cfg
+-rw-r--r--   0 marclaventure   (501) staff       (20)      577 2024-04-26 07:09:47.000000 scalar_fastapi-1.0.1/setup.py
+drwxr-xr-x   0 marclaventure   (501) staff       (20)        0 2024-04-26 07:10:43.321173 scalar_fastapi-1.0.1/tests/
+-rw-r--r--   0 marclaventure   (501) staff       (20)        0 2024-04-26 02:11:55.000000 scalar_fastapi-1.0.1/tests/__init__.py
```

### Comparing `scalar_fastapi-1.0/setup.py` & `scalar_fastapi-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='scalar_fastapi',
-    version='1.0',
+    version='1.0.1',
     packages=find_packages(),
     install_requires=[
         # Add your package dependencies here
     ],
     author='Marc Laventure',
     author_email='marc@scalar.com',
     description='This plugin provides an easy way to render a beautiful API reference based on a OpenAPI/Swagger file with FastAPI.',
```

