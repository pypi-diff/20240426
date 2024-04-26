# Comparing `tmp/streply_sdk-0.0.1.tar.gz` & `tmp/streply_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streply_sdk-0.0.1.tar", last modified: Tue Apr 23 09:06:10 2024, max compression
+gzip compressed data, was "streply_sdk-0.0.3.tar", last modified: Fri Apr 26 10:13:57 2024, max compression
```

## Comparing `streply_sdk-0.0.1.tar` & `streply_sdk-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-23 09:06:10.397413 streply_sdk-0.0.1/
--rw-r--r--   0 michalmolenda   (501) staff       (20)     2994 2024-04-23 09:06:10.396927 streply_sdk-0.0.1/PKG-INFO
--rw-r--r--   0 michalmolenda   (501) staff       (20)     1874 2024-04-23 07:10:58.000000 streply_sdk-0.0.1/README.md
--rw-r--r--   0 michalmolenda   (501) staff       (20)       38 2024-04-23 09:06:10.397491 streply_sdk-0.0.1/setup.cfg
--rw-r--r--   0 michalmolenda   (501) staff       (20)     1554 2024-04-23 08:56:46.000000 streply_sdk-0.0.1/setup.py
-drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-23 09:06:10.392822 streply_sdk-0.0.1/streply/
--rw-r--r--   0 michalmolenda   (501) staff       (20)      325 2024-04-23 05:15:43.000000 streply_sdk-0.0.1/streply/__init__.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)      492 2024-04-22 12:50:57.000000 streply_sdk-0.0.1/streply/capture.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)      741 2024-04-22 14:38:58.000000 streply_sdk-0.0.1/streply/debug.py
-drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-23 09:06:10.393294 streply_sdk-0.0.1/streply/entity/
--rw-r--r--   0 michalmolenda   (501) staff       (20)        0 2024-04-21 06:14:30.000000 streply_sdk-0.0.1/streply/entity/__init__.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)     2765 2024-04-23 05:05:06.000000 streply_sdk-0.0.1/streply/entity/entity.py
-drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-23 09:06:10.393716 streply_sdk-0.0.1/streply/enum/
--rw-r--r--   0 michalmolenda   (501) staff       (20)        0 2024-04-21 05:41:17.000000 streply_sdk-0.0.1/streply/enum/__init__.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)      118 2024-04-21 05:42:36.000000 streply_sdk-0.0.1/streply/enum/level.py
-drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-23 09:06:10.394274 streply_sdk-0.0.1/streply/handler/
--rw-r--r--   0 michalmolenda   (501) staff       (20)        0 2024-04-22 10:08:40.000000 streply_sdk-0.0.1/streply/handler/__init__.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)      668 2024-04-22 10:05:12.000000 streply_sdk-0.0.1/streply/handler/log_handler.py
-drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-23 09:06:10.395193 streply_sdk-0.0.1/streply/input/
--rw-r--r--   0 michalmolenda   (501) staff       (20)        0 2024-04-21 04:57:34.000000 streply_sdk-0.0.1/streply/input/__init__.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)      811 2024-04-21 04:57:04.000000 streply_sdk-0.0.1/streply/input/dsn.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)      385 2024-04-22 14:53:27.000000 streply_sdk-0.0.1/streply/input/options.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)      664 2024-04-22 10:31:26.000000 streply_sdk-0.0.1/streply/request.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)      679 2024-04-23 05:04:40.000000 streply_sdk-0.0.1/streply/response.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)      514 2024-04-22 05:06:36.000000 streply_sdk-0.0.1/streply/session.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)      495 2024-04-22 14:51:08.000000 streply_sdk-0.0.1/streply/source.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)     2691 2024-04-22 18:12:28.000000 streply_sdk-0.0.1/streply/streply.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)     1239 2024-04-22 14:59:08.000000 streply_sdk-0.0.1/streply/trace.py
--rw-r--r--   0 michalmolenda   (501) staff       (20)      212 2024-04-22 18:11:17.000000 streply_sdk-0.0.1/streply/utils.py
-drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-23 09:06:10.396462 streply_sdk-0.0.1/streply_sdk.egg-info/
--rw-r--r--   0 michalmolenda   (501) staff       (20)     2994 2024-04-23 09:06:10.000000 streply_sdk-0.0.1/streply_sdk.egg-info/PKG-INFO
--rw-r--r--   0 michalmolenda   (501) staff       (20)      573 2024-04-23 09:06:10.000000 streply_sdk-0.0.1/streply_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 michalmolenda   (501) staff       (20)        1 2024-04-23 09:06:10.000000 streply_sdk-0.0.1/streply_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 michalmolenda   (501) staff       (20)        8 2024-04-23 09:06:10.000000 streply_sdk-0.0.1/streply_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-26 10:13:57.562045 streply_sdk-0.0.3/
+-rw-r--r--   0 michalmolenda   (501) staff       (20)     2994 2024-04-26 10:13:57.561766 streply_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 michalmolenda   (501) staff       (20)     1874 2024-04-23 07:10:58.000000 streply_sdk-0.0.3/README.md
+-rw-r--r--   0 michalmolenda   (501) staff       (20)       38 2024-04-26 10:13:57.562104 streply_sdk-0.0.3/setup.cfg
+-rw-r--r--   0 michalmolenda   (501) staff       (20)     1553 2024-04-26 10:06:45.000000 streply_sdk-0.0.3/setup.py
+drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-26 10:13:57.557628 streply_sdk-0.0.3/streply/
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      325 2024-04-26 10:06:58.000000 streply_sdk-0.0.3/streply/__init__.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      519 2024-04-26 07:09:47.000000 streply_sdk-0.0.3/streply/capture.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      741 2024-04-22 14:38:58.000000 streply_sdk-0.0.3/streply/debug.py
+drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-26 10:13:57.558149 streply_sdk-0.0.3/streply/entity/
+-rw-r--r--   0 michalmolenda   (501) staff       (20)        0 2024-04-21 06:14:30.000000 streply_sdk-0.0.3/streply/entity/__init__.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)     3364 2024-04-26 07:30:18.000000 streply_sdk-0.0.3/streply/entity/entity.py
+drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-26 10:13:57.558898 streply_sdk-0.0.3/streply/enum/
+-rw-r--r--   0 michalmolenda   (501) staff       (20)        0 2024-04-21 05:41:17.000000 streply_sdk-0.0.3/streply/enum/__init__.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)       59 2024-04-26 08:43:49.000000 streply_sdk-0.0.3/streply/enum/flags.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      118 2024-04-21 05:42:36.000000 streply_sdk-0.0.3/streply/enum/level.py
+drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-26 10:13:57.559353 streply_sdk-0.0.3/streply/handler/
+-rw-r--r--   0 michalmolenda   (501) staff       (20)        0 2024-04-22 10:08:40.000000 streply_sdk-0.0.3/streply/handler/__init__.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      668 2024-04-22 10:05:12.000000 streply_sdk-0.0.3/streply/handler/log_handler.py
+drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-26 10:13:57.560347 streply_sdk-0.0.3/streply/input/
+-rw-r--r--   0 michalmolenda   (501) staff       (20)        0 2024-04-21 04:57:34.000000 streply_sdk-0.0.3/streply/input/__init__.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      811 2024-04-21 04:57:04.000000 streply_sdk-0.0.3/streply/input/dsn.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      385 2024-04-22 14:53:27.000000 streply_sdk-0.0.3/streply/input/options.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      664 2024-04-26 07:10:44.000000 streply_sdk-0.0.3/streply/request.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      679 2024-04-23 05:04:40.000000 streply_sdk-0.0.3/streply/response.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      835 2024-04-26 07:30:11.000000 streply_sdk-0.0.3/streply/scope.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      514 2024-04-22 05:06:36.000000 streply_sdk-0.0.3/streply/session.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      495 2024-04-22 14:51:08.000000 streply_sdk-0.0.3/streply/source.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)     2833 2024-04-26 08:42:01.000000 streply_sdk-0.0.3/streply/streply.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)     1239 2024-04-22 14:59:08.000000 streply_sdk-0.0.3/streply/trace.py
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      212 2024-04-22 18:11:17.000000 streply_sdk-0.0.3/streply/utils.py
+drwxr-xr-x   0 michalmolenda   (501) staff       (20)        0 2024-04-26 10:13:57.561456 streply_sdk-0.0.3/streply_sdk.egg-info/
+-rw-r--r--   0 michalmolenda   (501) staff       (20)     2994 2024-04-26 10:13:57.000000 streply_sdk-0.0.3/streply_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 michalmolenda   (501) staff       (20)      612 2024-04-26 10:13:57.000000 streply_sdk-0.0.3/streply_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 michalmolenda   (501) staff       (20)        1 2024-04-26 10:13:57.000000 streply_sdk-0.0.3/streply_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 michalmolenda   (501) staff       (20)        8 2024-04-26 10:13:57.000000 streply_sdk-0.0.3/streply_sdk.egg-info/top_level.txt
```

### Comparing `streply_sdk-0.0.1/PKG-INFO` & `streply_sdk-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streply-sdk
-Version: 0.0.1
+Version: 0.0.3
 Summary: The all-in-one monitoring app for smart devs (https://streply.com)
 Author: Streply
 Author-email: support@streply.com
 Project-URL: Documentation, https://docs.streply.com/
 Project-URL: Changelog, https://streply.com/changelog
 Project-URL: Help & Support, https://streply.com/help
 Classifier: Environment :: Web Environment
```

### Comparing `streply_sdk-0.0.1/README.md` & `streply_sdk-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `streply_sdk-0.0.1/setup.py` & `streply_sdk-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def read_file(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 setup(
     name='streply-sdk',
-    version='0.0.01',
+    version='0.0.3',
     author='Streply',
     author_email='support@streply.com',
     project_urls={
         "Documentation": "https://docs.streply.com/",
         "Changelog": "https://streply.com/changelog",
         "Help & Support": "https://streply.com/help",
     },
```

### Comparing `streply_sdk-0.0.1/streply/debug.py` & `streply_sdk-0.0.3/streply/debug.py`

 * *Files identical despite different names*

### Comparing `streply_sdk-0.0.1/streply/entity/entity.py` & `streply_sdk-0.0.3/streply/entity/entity.py`

 * *Files 21% similar despite different names*

```diff
@@ -49,46 +49,67 @@
         self._line = line
 
     def trace(self, trace: object):
         self._trace = trace
 
     def toJson(self):
         if self._message is None:
-            print('error')  # @TODO:
+            raise Exception('Message cannot be empty')
 
         _time = microtime()
         _loadTime = _time - __start_time__
+        _scope = sys.streply.scope()
+        _flag = None
+        _url = None
+        _channel = None
+        _environment = self._options.environment()
+        _release = self._options.release()
+
+        if _scope is not None:
+            _flag = _scope.flag
+            _url = _scope.url
+            _channel = _scope.channel
+
+            if _scope.environment is not None:
+                _environment = _scope.environment
+
+            if _scope.release is not None:
+                _release = _scope.release
+
+            if not _scope.global_scope:
+                sys.streply.set_scope(None)
 
         return {
             'eventType': 'event',
             'traceId': __session__.traceId(),
             'traceUniqueId': __session__.traceUniqueId(),
-            'sessionId': __session__.sessionId(),  # @TODO:
-            'userId': __session__.userId(),  # @TODO:
+            'sessionId': __session__.sessionId(),
+            'userId': __session__.userId(),
             'status': 0,
             'dateTimeZone': str(datetime.datetime.now().astimezone().tzname()),
             'date': str(datetime.datetime.now()),
             'startTime': __start_time__,
             'time': _time,
             'loadTime': _loadTime,
             'technology': 'python',
             'technologyVersion': platform.python_version(),
-            'environment': self._options.environment(),
-            'release': self._options.release(),
+            'environment': _environment,
+            'release': _release,
             'projectId': self._dsn.getProjectId(),
             'httpStatusCode': 200,
             'apiClientVersion': __streply_version__,
             'type': self._type,
             'level': self._level,
             'params': parseParams(self._params),
             'message': self._message,
             'requestUserAgent': socket.gethostname(),
             'requestParams': sys.argv,
             'dir': os.getcwd(),
             'user': self._user,
-            'url': None,
-            'flag': None,
+            'url': _url,
+            'flag': _flag,
             'file': self._file,
             'line': self._line,
             'exceptionName': self._exception_name,
             'trace': self._trace,
+            'channel': _channel,
         }
```

### Comparing `streply_sdk-0.0.1/streply/handler/log_handler.py` & `streply_sdk-0.0.3/streply/handler/log_handler.py`

 * *Files identical despite different names*

### Comparing `streply_sdk-0.0.1/streply/input/dsn.py` & `streply_sdk-0.0.3/streply/input/dsn.py`

 * *Files identical despite different names*

### Comparing `streply_sdk-0.0.1/streply/request.py` & `streply_sdk-0.0.3/streply/request.py`

 * *Files identical despite different names*

### Comparing `streply_sdk-0.0.1/streply/response.py` & `streply_sdk-0.0.3/streply/response.py`

 * *Files identical despite different names*

### Comparing `streply_sdk-0.0.1/streply/session.py` & `streply_sdk-0.0.3/streply/session.py`

 * *Files identical despite different names*

### Comparing `streply_sdk-0.0.1/streply/streply.py` & `streply_sdk-0.0.3/streply/streply.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,28 @@
 from streply.enum.level import level
 from streply.entity.entity import entity
 from streply.trace import trace
 from streply.utils import parseParams
 
 
 class streply:
-    def __init__(self, _dsn: str, _options: object):
+    def __init__(self, _dsn: str, _options: object = {}):
         self._dsn = dsn(_dsn)
         self._options = options(_options)
         self._request = request(self._dsn, self._options)
         self._user = None
+        self._scope = None
         sys.streply = self
 
+    def set_scope(self, scope):
+        self._scope = scope
+
+    def scope(self):
+        return self._scope
+
     def set_option(self, name: str, value):
         self._options.set(name, value)
 
     def set_user(self, user_id: str, user_name: str = None, params: object = {}):
         if user_name is None:
             user_name = user_id
         self._user = {'userId': user_id, 'userName': user_name, 'params': parseParams(params)}
```

### Comparing `streply_sdk-0.0.1/streply/trace.py` & `streply_sdk-0.0.3/streply/trace.py`

 * *Files identical despite different names*

### Comparing `streply_sdk-0.0.1/streply_sdk.egg-info/PKG-INFO` & `streply_sdk-0.0.3/streply_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streply-sdk
-Version: 0.0.1
+Version: 0.0.3
 Summary: The all-in-one monitoring app for smart devs (https://streply.com)
 Author: Streply
 Author-email: support@streply.com
 Project-URL: Documentation, https://docs.streply.com/
 Project-URL: Changelog, https://streply.com/changelog
 Project-URL: Help & Support, https://streply.com/help
 Classifier: Environment :: Web Environment
```

### Comparing `streply_sdk-0.0.1/streply_sdk.egg-info/SOURCES.txt` & `streply_sdk-0.0.3/streply_sdk.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 README.md
 setup.py
 streply/__init__.py
 streply/capture.py
 streply/debug.py
 streply/request.py
 streply/response.py
+streply/scope.py
 streply/session.py
 streply/source.py
 streply/streply.py
 streply/trace.py
 streply/utils.py
 streply/entity/__init__.py
 streply/entity/entity.py
 streply/enum/__init__.py
+streply/enum/flags.py
 streply/enum/level.py
 streply/handler/__init__.py
 streply/handler/log_handler.py
 streply/input/__init__.py
 streply/input/dsn.py
 streply/input/options.py
 streply_sdk.egg-info/PKG-INFO
```

