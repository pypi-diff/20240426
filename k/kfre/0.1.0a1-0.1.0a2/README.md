# Comparing `tmp/kfre-0.1.0a1.tar.gz` & `tmp/kfre-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kfre-0.1.0a1.tar", last modified: Thu Apr 25 23:44:59 2024, max compression
+gzip compressed data, was "kfre-0.1.0a2.tar", last modified: Fri Apr 26 04:53:00 2024, max compression
```

## Comparing `kfre-0.1.0a1.tar` & `kfre-0.1.0a2.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 23:44:59.348065 kfre-0.1.0a1/
--rw-rw-rw-   0        0        0      551 2024-04-25 23:44:59.346065 kfre-0.1.0a1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 23:44:59.348065 kfre-0.1.0a1/setup.cfg
--rw-rw-rw-   0        0        0     1190 2024-04-25 23:44:34.000000 kfre-0.1.0a1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:44:59.329067 kfre-0.1.0a1/src/
-drwxrwxrwx   0        0        0        0 2024-04-25 23:44:59.334070 kfre-0.1.0a1/src/kfre/
--rw-rw-rw-   0        0        0       56 2024-04-25 23:42:13.000000 kfre-0.1.0a1/src/kfre/__init__.py
--rw-rw-rw-   0        0        0    12294 2024-04-25 22:12:43.000000 kfre-0.1.0a1/src/kfre/main.py
-drwxrwxrwx   0        0        0        0 2024-04-25 23:44:59.345065 kfre-0.1.0a1/src/kfre.egg-info/
--rw-rw-rw-   0        0        0      551 2024-04-25 23:44:59.000000 kfre-0.1.0a1/src/kfre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-04-25 23:44:59.000000 kfre-0.1.0a1/src/kfre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 23:44:59.000000 kfre-0.1.0a1/src/kfre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-25 23:44:59.000000 kfre-0.1.0a1/src/kfre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-25 23:44:59.000000 kfre-0.1.0a1/src/kfre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 04:53:00.229230 kfre-0.1.0a2/
+-rw-rw-rw-   0        0        0     4409 2024-04-26 04:53:00.227318 kfre-0.1.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-26 04:53:00.229230 kfre-0.1.0a2/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2024-04-26 04:52:56.000000 kfre-0.1.0a2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 04:53:00.209175 kfre-0.1.0a2/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 04:53:00.226234 kfre-0.1.0a2/src/kfre.egg-info/
+-rw-rw-rw-   0        0        0     4409 2024-04-26 04:53:00.000000 kfre-0.1.0a2/src/kfre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-04-26 04:53:00.000000 kfre-0.1.0a2/src/kfre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 04:53:00.000000 kfre-0.1.0a2/src/kfre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-26 04:53:00.000000 kfre-0.1.0a2/src/kfre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 04:53:00.000000 kfre-0.1.0a2/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.0a1/setup.py` & `kfre-0.1.0a2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kfre",
-    version="0.1.0-alpha1",
+    version="0.1.0-alpha2",
     author="Leonid Shpaner",
-    author_email="lshpaner@ucla.edu",
+    author_email="Lshpaner@ucla.edu",
     description="A Python library for kidney failure risk estimation using Tangri's KFRE model",
-    long_description=open("README.md").read(),  # Detailed description read from the README.md
+    long_description=open("README.md").read(),
     long_description_content_type="text/markdown",  # Type of the long description
     url="https://github.com/lshpaner/kfre",  # URL to the repository or documentation
     package_dir={"": "src"},  # Directory where your package files are located
-    packages=find_packages(where="src"),  # Automatically find packages in the specified directory
+    # Automatically find packages in the specified directory
+    packages=find_packages(where="src"),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],  # Classifiers for the package
-    python_requires='>=3.6',  # Minimum version of Python required
+    python_requires=">=3.6",  # Minimum version of Python required
     install_requires=[
         "numpy>=1.18.5",  # Example of a required library with a minimum version
-        "pandas>=1.0.5"  # Example of another required library with a minimum version
+        "pandas>=1.0.5",  # Example of another required library with a minimum version
     ],
-)
+)
```

