# Comparing `tmp/upycli-0.2.5.tar.gz` & `tmp/upycli-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upycli-0.2.5.tar", last modified: Thu Mar 21 14:23:39 2024, max compression
+gzip compressed data, was "upycli-0.2.6.tar", last modified: Fri Apr 26 14:35:38 2024, max compression
```

## Comparing `upycli-0.2.5.tar` & `upycli-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:23:39.930791 upycli-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-21 14:23:39.930791 upycli-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-21 14:23:32.000000 upycli-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 14:23:39.930791 upycli-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-21 14:23:32.000000 upycli-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:23:39.926791 upycli-0.2.5/upycli/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-21 14:23:32.000000 upycli-0.2.5/upycli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-21 14:23:32.000000 upycli-0.2.5/upycli/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-21 14:23:32.000000 upycli-0.2.5/upycli/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 14:23:39.930791 upycli-0.2.5/upycli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-21 14:23:39.000000 upycli-0.2.5/upycli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-21 14:23:39.000000 upycli-0.2.5/upycli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 14:23:39.000000 upycli-0.2.5/upycli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-21 14:23:39.000000 upycli-0.2.5/upycli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-21 14:23:39.000000 upycli-0.2.5/upycli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:35:38.850597 upycli-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-26 14:35:38.850597 upycli-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-26 14:35:34.000000 upycli-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:35:38.850597 upycli-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-26 14:35:34.000000 upycli-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:35:38.850597 upycli-0.2.6/upycli/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-26 14:35:34.000000 upycli-0.2.6/upycli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-26 14:35:34.000000 upycli-0.2.6/upycli/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-26 14:35:34.000000 upycli-0.2.6/upycli/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:35:38.850597 upycli-0.2.6/upycli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-26 14:35:38.000000 upycli-0.2.6/upycli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-26 14:35:38.000000 upycli-0.2.6/upycli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:35:38.000000 upycli-0.2.6/upycli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 14:35:38.000000 upycli-0.2.6/upycli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 14:35:38.000000 upycli-0.2.6/upycli.egg-info/top_level.txt
```

### Comparing `upycli-0.2.5/PKG-INFO` & `upycli-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upycli
-Version: 0.2.5
+Version: 0.2.6
 Summary: A microscopic library to turn any function into a CLI.
 Home-page: https://github.com/zrthxn/uPyCLI
 Maintainer: Alisamar Husian
 Maintainer-email: zrthxn@gmail.com
 Description-Content-Type: text/markdown
 
 # uPyCLI
```

### Comparing `upycli-0.2.5/README.md` & `upycli-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `upycli-0.2.5/setup.py` & `upycli-0.2.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='upycli',
-    version='0.2.5',
+    version='0.2.6',
     packages=find_packages(),
     
     # Descriptions
     description='A microscopic library to turn any function into a CLI.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `upycli-0.2.5/upycli/decorator.py` & `upycli-0.2.6/upycli/decorator.py`

 * *Files identical despite different names*

### Comparing `upycli-0.2.5/upycli/runner.py` & `upycli-0.2.6/upycli/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     --batch_size BATCH_SIZE
     --device DEVICE
     ```
 """
 
 
 def reflect(func: Callable):
-    annotations = func.__annotations__
-    defaults = func.__defaults__
+    annotations = func.__annotations__ or []
+    defaults = func.__defaults__ or []
     
     # Quickfix: If all args are optional, and so no type annotations, use code to inspect names 
     if len(annotations) == 0:
         annotations = {k: None for k in func.__code__.co_varnames[:func.__code__.co_argcount]}
 
     parser = ArgumentParser(description = func.__doc__)
```

### Comparing `upycli-0.2.5/upycli.egg-info/PKG-INFO` & `upycli-0.2.6/upycli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upycli
-Version: 0.2.5
+Version: 0.2.6
 Summary: A microscopic library to turn any function into a CLI.
 Home-page: https://github.com/zrthxn/uPyCLI
 Maintainer: Alisamar Husian
 Maintainer-email: zrthxn@gmail.com
 Description-Content-Type: text/markdown
 
 # uPyCLI
```

