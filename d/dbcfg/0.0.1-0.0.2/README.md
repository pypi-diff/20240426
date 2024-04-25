# Comparing `tmp/dbcfg-0.0.1.tar.gz` & `tmp/dbcfg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbcfg-0.0.1.tar", last modified: Sun Feb 18 03:38:18 2024, max compression
+gzip compressed data, was "dbcfg-0.0.2.tar", last modified: Thu Apr 25 23:49:21 2024, max compression
```

## Comparing `dbcfg-0.0.1.tar` & `dbcfg-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 03:38:17.000000 dbcfg-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     9688 2024-02-17 00:45:56.000000 dbcfg-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1097 2024-02-18 03:38:17.000000 dbcfg-0.0.1/PKG-INFO
--rwxrw-rw-   0 root         (0) root         (0)      731 2024-02-14 03:00:31.000000 dbcfg-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 03:38:17.000000 dbcfg-0.0.1/dbcfg/
--rwxrw-rw-   0 root         (0) root         (0)       60 2024-02-18 02:16:40.000000 dbcfg-0.0.1/dbcfg/dbcfg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 03:38:17.000000 dbcfg-0.0.1/dbcfg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1097 2024-02-18 03:38:17.000000 dbcfg-0.0.1/dbcfg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2024-02-18 03:38:17.000000 dbcfg-0.0.1/dbcfg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-18 03:38:17.000000 dbcfg-0.0.1/dbcfg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-02-18 03:38:17.000000 dbcfg-0.0.1/dbcfg.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-18 03:34:58.000000 dbcfg-0.0.1/dbcfg.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       11 2024-02-18 03:38:17.000000 dbcfg-0.0.1/dbcfg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-18 03:38:17.000000 dbcfg-0.0.1/setup.cfg
--rwxrw-rw-   0 root         (0) root         (0)      815 2024-02-18 03:38:07.000000 dbcfg-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 23:49:21.000000 dbcfg-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     9688 2024-02-17 00:45:56.000000 dbcfg-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2710 2024-04-25 23:49:21.000000 dbcfg-0.0.2/PKG-INFO
+-rwxrw-rw-   0 root         (0) root         (0)     2344 2024-04-25 06:57:12.000000 dbcfg-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 23:49:20.000000 dbcfg-0.0.2/dbcfg/
+-rwxrw-rw-   0 root         (0) root         (0)       81 2024-04-18 23:58:07.000000 dbcfg-0.0.2/dbcfg/__init__.py
+-rwxrw-rw-   0 root         (0) root         (0)     1982 2024-04-21 09:15:21.000000 dbcfg-0.0.2/dbcfg/dbcfgmain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 23:49:21.000000 dbcfg-0.0.2/dbcfg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2710 2024-04-25 23:49:20.000000 dbcfg-0.0.2/dbcfg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      279 2024-04-25 23:49:20.000000 dbcfg-0.0.2/dbcfg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 23:49:20.000000 dbcfg-0.0.2/dbcfg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-25 23:49:20.000000 dbcfg-0.0.2/dbcfg.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-18 03:34:58.000000 dbcfg-0.0.2/dbcfg.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-25 23:49:20.000000 dbcfg-0.0.2/dbcfg.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 23:49:21.000000 dbcfg-0.0.2/script/
+-rwxrw-rw-   0 root         (0) root         (0)      585 2024-04-21 09:06:37.000000 dbcfg-0.0.2/script/dbcfgdemo.py
+-rwxrw-rw-   0 root         (0) root         (0)       60 2024-02-18 02:16:40.000000 dbcfg-0.0.2/script/dbcfgtool.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 23:49:21.000000 dbcfg-0.0.2/setup.cfg
+-rwxrw-rw-   0 root         (0) root         (0)      867 2024-04-21 00:31:06.000000 dbcfg-0.0.2/setup.py
```

### Comparing `dbcfg-0.0.1/LICENSE` & `dbcfg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbcfg-0.0.1/setup.py` & `dbcfg-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools,distutils,shutil,re,os
 
 with open("README.md", "r",encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dbcfg",
-    version="0.0.1",
+    version="0.0.2",
     author="Chen chuan",
     author_email="kcchen@139.com",
     description="数据库连接信息管理",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_namespace_packages(),
     classifiers=[
@@ -20,11 +20,12 @@
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
     zip_safe= False,
     include_package_data = True,
     entry_points={
         'console_scripts':  [
-            'dbcfg=dbcfg.dbcfg:main',
+            'dbcfg=script.dbcfgtool:main',
+            'dbcfgdemo=script.dbcfgdemo:main',
         ],
     },
 )
```

