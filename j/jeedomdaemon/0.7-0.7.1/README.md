# Comparing `tmp/jeedomdaemon-0.7.tar.gz` & `tmp/jeedomdaemon-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeedomdaemon-0.7.tar", last modified: Thu Apr 25 15:23:58 2024, max compression
+gzip compressed data, was "jeedomdaemon-0.7.1.tar", last modified: Fri Apr 26 12:28:12 2024, max compression
```

## Comparing `jeedomdaemon-0.7.tar` & `jeedomdaemon-0.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:23:58.666299 jeedomdaemon-0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-25 15:23:54.000000 jeedomdaemon-0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-25 15:23:58.666299 jeedomdaemon-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-25 15:23:54.000000 jeedomdaemon-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:23:58.666299 jeedomdaemon-0.7/jeedomdaemon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:23:54.000000 jeedomdaemon-0.7/jeedomdaemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-25 15:23:54.000000 jeedomdaemon-0.7/jeedomdaemon/aio_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-25 15:23:54.000000 jeedomdaemon-0.7/jeedomdaemon/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-25 15:23:54.000000 jeedomdaemon-0.7/jeedomdaemon/base_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 15:23:54.000000 jeedomdaemon-0.7/jeedomdaemon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:23:58.666299 jeedomdaemon-0.7/jeedomdaemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-25 15:23:58.000000 jeedomdaemon-0.7/jeedomdaemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-25 15:23:58.000000 jeedomdaemon-0.7/jeedomdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:23:58.000000 jeedomdaemon-0.7/jeedomdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:23:58.000000 jeedomdaemon-0.7/jeedomdaemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 15:23:58.000000 jeedomdaemon-0.7/jeedomdaemon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:23:58.666299 jeedomdaemon-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-25 15:23:54.000000 jeedomdaemon-0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:23:58.666299 jeedomdaemon-0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:23:54.000000 jeedomdaemon-0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-25 15:23:54.000000 jeedomdaemon-0.7/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-25 15:23:54.000000 jeedomdaemon-0.7/tests/base_daemon_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/jeedomdaemon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/jeedomdaemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/jeedomdaemon/aio_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/jeedomdaemon/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/jeedomdaemon/base_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/jeedomdaemon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-26 12:28:12.000000 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-26 12:28:12.000000 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:28:12.000000 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 12:28:12.000000 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 12:28:12.000000 jeedomdaemon-0.7.1/jeedomdaemon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:28:12.920565 jeedomdaemon-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 12:27:56.000000 jeedomdaemon-0.7.1/tests/base_daemon_test.py
```

### Comparing `jeedomdaemon-0.7/LICENSE` & `jeedomdaemon-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7/jeedomdaemon/aio_connector.py` & `jeedomdaemon-0.7.1/jeedomdaemon/aio_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,29 +67,29 @@
         return self
 
     async def __aexit__(self, *excinfo):
         await self._jeedom_session.close()
 
     def create_send_task(self):
         """ Helper function to create the send task"""
-        return asyncio.create_task(self._send_task())
+        return asyncio.create_task(self.__send_task())
 
     async def test_callback(self):
         """test_callback will return true if communication with Jeedom is sucessfull or false otherwise"""
         try:
             async with self._jeedom_session.get(self._callback_url + '?test=1&apikey=' + self._api_key) as resp:
                 if resp.status != 200:
                     self._logger.error("Please check your network configuration page: %s-%s", resp.status, resp.reason)
                     return False
         except aiohttp.ClientError as e:
             self._logger.error('Callback error: %s. Please check your network configuration page', e)
             return False
         return True
 
-    async def _send_task(self):
+    async def __send_task(self):
         self._logger.info("Send async started")
         try:
             last_send_on_error = False
             while True:
                 if len(self.__changes)>0:
                     changes = self.__changes
                     self.__changes = {}
```

### Comparing `jeedomdaemon-0.7/jeedomdaemon/base_config.py` & `jeedomdaemon-0.7.1/jeedomdaemon/base_config.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7/jeedomdaemon/base_daemon.py` & `jeedomdaemon-0.7.1/jeedomdaemon/base_daemon.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7/jeedomdaemon/utils.py` & `jeedomdaemon-0.7.1/jeedomdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7/setup.py` & `jeedomdaemon-0.7.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     author='Mips',
     # author_email='',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['aiohttp'],
     # *strongly* suggested for sharing
-    version='0.7',
+    version='0.7.1',
     # The license can be anything you like
     license='MIT',
     description='A base to implement Jeedom daemon in python',
     # We will also need a readme eventually (there will be a warning)
     long_description=open('README.md').read(),
+    long_description_content_type="text/markdown",
 )
```

### Comparing `jeedomdaemon-0.7/tests/base_config_test.py` & `jeedomdaemon-0.7.1/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7/tests/base_daemon_test.py` & `jeedomdaemon-0.7.1/tests/base_daemon_test.py`

 * *Files identical despite different names*

