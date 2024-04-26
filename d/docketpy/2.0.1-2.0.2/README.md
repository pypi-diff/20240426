# Comparing `tmp/docketpy-2.0.1.tar.gz` & `tmp/docketpy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/docketpy-2.0.1.tar", last modified: Tue Mar 12 15:39:58 2024, max compression
+gzip compressed data, was "dist/docketpy-2.0.2.tar", last modified: Fri Apr 26 18:06:50 2024, max compression
```

## Comparing `docketpy-2.0.1.tar` & `docketpy-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 st201n     (503) staff       (20)        0 2024-03-12 15:39:58.463253 docketpy-2.0.1/
--rw-r--r--   0 st201n     (503) staff       (20)     1068 2024-03-12 07:00:02.000000 docketpy-2.0.1/LICENSE
--rw-r--r--   0 st201n     (503) staff       (20)      130 2024-03-12 15:39:58.463116 docketpy-2.0.1/PKG-INFO
--rw-r--r--   0 st201n     (503) staff       (20)      303 2024-03-12 15:39:27.000000 docketpy-2.0.1/README.md
-drwxr-xr-x   0 st201n     (503) staff       (20)        0 2024-03-12 15:39:58.460878 docketpy-2.0.1/docketpy/
--rw-r--r--   0 st201n     (503) staff       (20)       22 2024-03-12 15:39:06.000000 docketpy-2.0.1/docketpy/__init__.py
--rw-r--r--   0 st201n     (503) staff       (20)      931 2024-03-12 14:57:07.000000 docketpy-2.0.1/docketpy/core.py
--rw-r--r--   0 st201n     (503) staff       (20)     1029 2024-03-12 10:54:37.000000 docketpy-2.0.1/docketpy/mathx.py
-drwxr-xr-x   0 st201n     (503) staff       (20)        0 2024-03-12 15:39:58.462037 docketpy-2.0.1/docketpy.egg-info/
--rw-r--r--   0 st201n     (503) staff       (20)      130 2024-03-12 15:39:58.000000 docketpy-2.0.1/docketpy.egg-info/PKG-INFO
--rw-r--r--   0 st201n     (503) staff       (20)      259 2024-03-12 15:39:58.000000 docketpy-2.0.1/docketpy.egg-info/SOURCES.txt
--rw-r--r--   0 st201n     (503) staff       (20)        1 2024-03-12 15:39:58.000000 docketpy-2.0.1/docketpy.egg-info/dependency_links.txt
--rw-r--r--   0 st201n     (503) staff       (20)        9 2024-03-12 15:39:58.000000 docketpy-2.0.1/docketpy.egg-info/top_level.txt
--rw-r--r--   0 st201n     (503) staff       (20)       63 2024-03-12 15:39:58.463700 docketpy-2.0.1/setup.cfg
--rw-r--r--   0 st201n     (503) staff       (20)      354 2024-03-12 15:38:31.000000 docketpy-2.0.1/setup.py
-drwxr-xr-x   0 st201n     (503) staff       (20)        0 2024-03-12 15:39:58.462667 docketpy-2.0.1/tests/
--rw-r--r--   0 st201n     (503) staff       (20)      281 2024-03-12 15:39:11.000000 docketpy-2.0.1/tests/test_core.py
--rw-r--r--   0 st201n     (503) staff       (20)      375 2024-03-12 15:39:07.000000 docketpy-2.0.1/tests/test_mathx.py
+drwxr-xr-x   0 st201n     (503) staff       (20)        0 2024-04-26 18:06:50.529922 docketpy-2.0.2/
+-rw-r--r--   0 st201n     (503) staff       (20)     1068 2024-03-12 07:00:02.000000 docketpy-2.0.2/LICENSE
+-rw-r--r--   0 st201n     (503) staff       (20)      130 2024-04-26 18:06:50.529816 docketpy-2.0.2/PKG-INFO
+-rw-r--r--   0 st201n     (503) staff       (20)      330 2024-04-04 22:06:13.000000 docketpy-2.0.2/README.md
+drwxr-xr-x   0 st201n     (503) staff       (20)        0 2024-04-26 18:06:50.528027 docketpy-2.0.2/docketpy/
+-rw-r--r--   0 st201n     (503) staff       (20)       22 2024-04-04 22:09:25.000000 docketpy-2.0.2/docketpy/__init__.py
+-rw-r--r--   0 st201n     (503) staff       (20)      931 2024-03-12 14:57:07.000000 docketpy-2.0.2/docketpy/core.py
+-rw-r--r--   0 st201n     (503) staff       (20)     1029 2024-03-12 10:54:37.000000 docketpy-2.0.2/docketpy/mathx.py
+drwxr-xr-x   0 st201n     (503) staff       (20)        0 2024-04-26 18:06:50.528864 docketpy-2.0.2/docketpy.egg-info/
+-rw-r--r--   0 st201n     (503) staff       (20)      130 2024-04-26 18:06:50.000000 docketpy-2.0.2/docketpy.egg-info/PKG-INFO
+-rw-r--r--   0 st201n     (503) staff       (20)      259 2024-04-26 18:06:50.000000 docketpy-2.0.2/docketpy.egg-info/SOURCES.txt
+-rw-r--r--   0 st201n     (503) staff       (20)        1 2024-04-26 18:06:50.000000 docketpy-2.0.2/docketpy.egg-info/dependency_links.txt
+-rw-r--r--   0 st201n     (503) staff       (20)        9 2024-04-26 18:06:50.000000 docketpy-2.0.2/docketpy.egg-info/top_level.txt
+-rw-r--r--   0 st201n     (503) staff       (20)       63 2024-04-26 18:06:50.530242 docketpy-2.0.2/setup.cfg
+-rw-r--r--   0 st201n     (503) staff       (20)      354 2024-04-04 22:05:57.000000 docketpy-2.0.2/setup.py
+drwxr-xr-x   0 st201n     (503) staff       (20)        0 2024-04-26 18:06:50.529373 docketpy-2.0.2/tests/
+-rw-r--r--   0 st201n     (503) staff       (20)      281 2024-03-12 15:39:11.000000 docketpy-2.0.2/tests/test_core.py
+-rw-r--r--   0 st201n     (503) staff       (20)      375 2024-03-12 15:39:07.000000 docketpy-2.0.2/tests/test_mathx.py
```

### Comparing `docketpy-2.0.1/LICENSE` & `docketpy-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docketpy-2.0.1/docketpy/core.py` & `docketpy-2.0.2/docketpy/core.py`

 * *Files identical despite different names*

### Comparing `docketpy-2.0.1/docketpy/mathx.py` & `docketpy-2.0.2/docketpy/mathx.py`

 * *Files identical despite different names*

