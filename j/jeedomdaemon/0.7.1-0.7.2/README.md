# Comparing `tmp/jeedomdaemon-0.7.1.tar.gz` & `tmp/jeedomdaemon-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeedomdaemon-0.7.1.tar", last modified: Fri Apr 26 12:28:12 2024, max compression
+gzip compressed data, was "jeedomdaemon-0.7.2.tar", last modified: Fri Apr 26 13:08:39 2024, max compression
```

## Comparing `jeedomdaemon-0.7.1.tar` & `jeedomdaemon-0.7.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/jeedomdaemon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/jeedomdaemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/jeedomdaemon/aio_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/jeedomdaemon/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/jeedomdaemon/base_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/jeedomdaemon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-26 12:28:12.000000 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-26 12:28:12.000000 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:28:12.000000 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 12:28:12.000000 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 12:28:12.000000 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/tests/base_daemon_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:39.000374 jeedomdaemon-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-26 13:08:39.000374 jeedomdaemon-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:38.996374 jeedomdaemon-0.7.2/jeedomdaemon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/jeedomdaemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/jeedomdaemon/aio_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/jeedomdaemon/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/jeedomdaemon/base_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/jeedomdaemon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:39.000374 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-26 13:08:38.000000 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-26 13:08:38.000000 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:08:38.000000 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 13:08:38.000000 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 13:08:38.000000 jeedomdaemon-0.7.2/jeedomdaemon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:08:39.000374 jeedomdaemon-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:39.000374 jeedomdaemon-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 13:08:34.000000 jeedomdaemon-0.7.2/tests/base_daemon_test.py
```

### Comparing `jeedomdaemon-0.7.1/LICENSE` & `jeedomdaemon-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.1/jeedomdaemon/aio_connector.py` & `jeedomdaemon-0.7.2/jeedomdaemon/aio_connector.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.1/jeedomdaemon/base_config.py` & `jeedomdaemon-0.7.2/jeedomdaemon/base_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         self.__parser = argparse.ArgumentParser(description='Daemon for Jeedom plugin')
         self.add_argument("--loglevel", help="Log Level for the daemon", type=str, default='error')
         self.add_argument("--sockethost", help="Socket host", type=str, default='127.0.0.1')
         self.add_argument("--socketport", help="Socket Port", type=int, default=0)
         self.add_argument("--callback", help="Jeedom callback url", type=str)
         self.add_argument("--apikey", help="Plugin API Key", type=str)
         self.add_argument("--pid", help="daemon pid", type=str)
+        self.add_argument("--cycle", help="cycle", type=float)
 
     def add_argument(self, *args, **kwargs):
         """Add a, argurment to parse.
 
         e.g. from your child class:
 
         self.add_argument("--clientId", type=str)
@@ -58,7 +59,12 @@
         """Return the api key."""
         return str(self._args.apikey)
 
     @property
     def pid_filename(self):
         """Return the pid."""
         return str(self._args.pid)
+
+    @property
+    def cycle(self):
+        """Return the cycle."""
+        return float(self._args.cycle)
```

### Comparing `jeedomdaemon-0.7.1/jeedomdaemon/base_daemon.py` & `jeedomdaemon-0.7.2/jeedomdaemon/base_daemon.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.1/jeedomdaemon/utils.py` & `jeedomdaemon-0.7.2/jeedomdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.1/setup.py` & `jeedomdaemon-0.7.2/setup.py`

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
-    version='0.7.1',
+    version='0.7.2',
     # The license can be anything you like
     license='MIT',
     description='A base to implement Jeedom daemon in python',
     # We will also need a readme eventually (there will be a warning)
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
 )
```

### Comparing `jeedomdaemon-0.7.1/tests/base_config_test.py` & `jeedomdaemon-0.7.2/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.1/tests/base_daemon_test.py` & `jeedomdaemon-0.7.2/tests/base_daemon_test.py`

 * *Files identical despite different names*

