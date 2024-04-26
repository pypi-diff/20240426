# Comparing `tmp/jeedomdaemon-0.7.2.tar.gz` & `tmp/jeedomdaemon-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeedomdaemon-0.7.2.tar", last modified: Fri Apr 26 13:08:39 2024, max compression
+gzip compressed data, was "jeedomdaemon-0.7.3.tar", last modified: Fri Apr 26 13:23:42 2024, max compression
```

## Comparing `jeedomdaemon-0.7.2.tar` & `jeedomdaemon-0.7.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:39.000374 jeedomdaemon-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-26 13:08:39.000374 jeedomdaemon-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:38.996374 jeedomdaemon-0.7.2/jeedomdaemon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/jeedomdaemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/jeedomdaemon/aio_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/jeedomdaemon/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/jeedomdaemon/base_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/jeedomdaemon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:39.000374 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-26 13:08:38.000000 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-26 13:08:38.000000 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:08:38.000000 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 13:08:38.000000 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 13:08:38.000000 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:08:39.000374 jeedomdaemon-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:39.000374 jeedomdaemon-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/tests/base_daemon_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:42.885746 jeedomdaemon-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-26 13:23:42.885746 jeedomdaemon-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:42.881746 jeedomdaemon-0.7.3/jeedomdaemon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/jeedomdaemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/jeedomdaemon/aio_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/jeedomdaemon/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/jeedomdaemon/base_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/jeedomdaemon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:42.885746 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-26 13:23:42.000000 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-26 13:23:42.000000 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:23:42.000000 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 13:23:42.000000 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 13:23:42.000000 jeedomdaemon-0.7.3/jeedomdaemon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:23:42.885746 jeedomdaemon-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:42.885746 jeedomdaemon-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 13:23:38.000000 jeedomdaemon-0.7.3/tests/base_daemon_test.py
```

### Comparing `jeedomdaemon-0.7.2/LICENSE` & `jeedomdaemon-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.2/PKG-INFO` & `jeedomdaemon-0.7.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,16 @@
-Metadata-Version: 2.1
-Name: jeedomdaemon
-Version: 0.7.2
-Summary: A base to implement Jeedom daemon in python
-Home-page: https://github.com/Mips2648/jeedom-daemon-py
-Author: Mips
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp
-
 # jeedom-daemon-py
 
 ![pytest 3.9](https://github.com/Mips2648/jeedom-daemon-py/actions/workflows/pytest-3.9.yml/badge.svg)
 ![pytest 3.11](https://github.com/Mips2648/jeedom-daemon-py/actions/workflows/pytest-3.11.yml/badge.svg)
 
 ## Description
 
-This library provide everything is needed to build a daemon for a plugin for Jeedom in python.
+This library provide everything needed to build a daemon for a plugin for Jeedom in python.
+It's possible to get a daemon skeleton by typing literally less than 5 lines of code.
 
 ## Requirements
 
 * **Python 3.9+**
 
 ## How to install
 
@@ -47,9 +37,24 @@
   "post-install": {}
 }
 ```
 
 ### Via requirements.txt
 
 ```txt
-jeedomdaemon~=0.7
+jeedomdaemon~=0.7.3
+```
+
+## Create a daemon skeleton
+
+Create a file `myDaemon.py` and copy/past the 4 lines of code below and that's it, nothing else to do, your daemon is good to start.
+
+```python
+from jeedomdaemon.base_daemon import BaseDaemon
+
+class myDaemon(BaseDaemon):
+    pass
+
+myDaemon().run()
 ```
+
+Of course, this does nothing so far except starting, accepting incoming requests from your php code and stopping when it is needed.
```

### Comparing `jeedomdaemon-0.7.2/jeedomdaemon/aio_connector.py` & `jeedomdaemon-0.7.3/jeedomdaemon/aio_connector.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.2/jeedomdaemon/base_config.py` & `jeedomdaemon-0.7.3/jeedomdaemon/base_config.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.2/jeedomdaemon/base_daemon.py` & `jeedomdaemon-0.7.3/jeedomdaemon/base_daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .utils import Utils
 from .aio_connector import Publisher, Listener
 from .base_config import BaseConfig
 
 class BaseDaemon:
     """Base daemon class"""
     def __init__(self,
-                 config: BaseConfig,
+                 config: BaseConfig = BaseConfig(),
                  on_start_cb: Callable[...,Awaitable[None]] | None = None,
                  on_message_cb: Callable[[list], Awaitable[None]] | None = None,
                  on_stop_cb: Callable[..., None] | None = None,
                  ) -> None:
         self._config = config
         self._config.parse()
         self._listen_task: asyncio.Task[None] | None = None
```

### Comparing `jeedomdaemon-0.7.2/jeedomdaemon/utils.py` & `jeedomdaemon-0.7.3/jeedomdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.2/setup.py` & `jeedomdaemon-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author='Mips',
     # author_email='',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['aiohttp'],
     # *strongly* suggested for sharing
-    version='0.7.2',
+    version='0.7.3',
     # The license can be anything you like
     license='MIT',
     description='A base to implement Jeedom daemon in python',
     # We will also need a readme eventually (there will be a warning)
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
 )
```

### Comparing `jeedomdaemon-0.7.2/tests/base_config_test.py` & `jeedomdaemon-0.7.3/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.2/tests/base_daemon_test.py` & `jeedomdaemon-0.7.3/tests/base_daemon_test.py`

 * *Files identical despite different names*

