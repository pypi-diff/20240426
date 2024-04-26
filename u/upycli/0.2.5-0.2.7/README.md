# Comparing `tmp/upycli-0.2.5.tar.gz` & `tmp/upycli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upycli-0.2.5.tar", last modified: Thu Mar 21 14:23:39 2024, max compression
+gzip compressed data, was "upycli-0.2.7.tar", last modified: Fri Apr 26 16:17:52 2024, max compression
```

## Comparing `upycli-0.2.5.tar` & `upycli-0.2.7.tar`

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
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:17:52.010899 upycli-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-26 16:17:52.010899 upycli-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-26 16:17:48.000000 upycli-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:17:52.010899 upycli-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-26 16:17:48.000000 upycli-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:17:52.006899 upycli-0.2.7/upycli/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-26 16:17:48.000000 upycli-0.2.7/upycli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-26 16:17:48.000000 upycli-0.2.7/upycli/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-26 16:17:48.000000 upycli-0.2.7/upycli/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:17:52.006899 upycli-0.2.7/upycli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-26 16:17:51.000000 upycli-0.2.7/upycli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-26 16:17:52.000000 upycli-0.2.7/upycli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:17:51.000000 upycli-0.2.7/upycli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 16:17:51.000000 upycli-0.2.7/upycli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 16:17:51.000000 upycli-0.2.7/upycli.egg-info/top_level.txt
```

### Comparing `upycli-0.2.5/PKG-INFO` & `upycli-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upycli
-Version: 0.2.5
+Version: 0.2.7
 Summary: A microscopic library to turn any function into a CLI.
 Home-page: https://github.com/zrthxn/uPyCLI
 Maintainer: Alisamar Husian
 Maintainer-email: zrthxn@gmail.com
 Description-Content-Type: text/markdown
 
 # uPyCLI
```

### Comparing `upycli-0.2.5/README.md` & `upycli-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `upycli-0.2.5/setup.py` & `upycli-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='upycli',
-    version='0.2.5',
+    version='0.2.7',
     packages=find_packages(),
     
     # Descriptions
     description='A microscopic library to turn any function into a CLI.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `upycli-0.2.5/upycli/decorator.py` & `upycli-0.2.7/upycli/decorator.py`

 * *Files identical despite different names*

### Comparing `upycli-0.2.5/upycli/runner.py` & `upycli-0.2.7/upycli/runner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Callable
+from typing import Callable, Union
 from argparse import ArgumentParser
 from importlib.util import spec_from_file_location, module_from_spec
 
 """
 Runner Module
 -------------
 
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
 
@@ -69,15 +69,15 @@
                             type=atype, 
                             help='%(type)s (default %(default)s)',
                             default=dvalue)
     
     return parser
 
 
-def execute(target: str | Callable, argv = []):
+def execute(target: Union[str, Callable], argv = []):
     if callable(target):
         func = target
     elif '.' in target:
         path, name = target.rsplit('.', 1)
         target_path = os.path.abspath(os.path.curdir)
         
         # specify the module that needs to be imported relative to the path of the module
```

### Comparing `upycli-0.2.5/upycli.egg-info/PKG-INFO` & `upycli-0.2.7/upycli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upycli
-Version: 0.2.5
+Version: 0.2.7
 Summary: A microscopic library to turn any function into a CLI.
 Home-page: https://github.com/zrthxn/uPyCLI
 Maintainer: Alisamar Husian
 Maintainer-email: zrthxn@gmail.com
 Description-Content-Type: text/markdown
 
 # uPyCLI
```

