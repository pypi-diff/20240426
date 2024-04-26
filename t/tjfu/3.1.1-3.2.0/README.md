# Comparing `tmp/tjfu-3.1.1.tar.gz` & `tmp/tjfu-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tjfu-3.1.1.tar", last modified: Tue Apr  9 18:42:56 2024, max compression
+gzip compressed data, was "tjfu-3.2.0.tar", last modified: Fri Apr 26 18:01:37 2024, max compression
```

## Comparing `tjfu-3.1.1.tar` & `tjfu-3.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-09 18:42:56.919653 tjfu-3.1.1/
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     7959 2024-04-09 18:42:56.919021 tjfu-3.1.1/PKG-INFO
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     7392 2024-04-09 18:39:57.000000 tjfu-3.1.1/README.md
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       38 2024-04-09 18:42:56.919796 tjfu-3.1.1/setup.cfg
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     1075 2024-04-09 18:41:20.000000 tjfu-3.1.1/setup.py
-drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-09 18:42:56.904963 tjfu-3.1.1/tjfu/
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       66 2024-04-07 12:46:51.000000 tjfu-3.1.1/tjfu/__init__.py
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     1222 2024-04-09 18:36:16.000000 tjfu-3.1.1/tjfu/route.py
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)      490 2024-04-07 12:46:51.000000 tjfu-3.1.1/tjfu/tj_socket.py
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     8156 2024-04-07 13:21:26.000000 tjfu-3.1.1/tjfu/tjfu.py
-drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-09 18:42:56.916678 tjfu-3.1.1/tjfu.egg-info/
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     7959 2024-04-09 18:42:56.000000 tjfu-3.1.1/tjfu.egg-info/PKG-INFO
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)      219 2024-04-09 18:42:56.000000 tjfu-3.1.1/tjfu.egg-info/SOURCES.txt
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        1 2024-04-09 18:42:56.000000 tjfu-3.1.1/tjfu.egg-info/dependency_links.txt
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       65 2024-04-09 18:42:56.000000 tjfu-3.1.1/tjfu.egg-info/requires.txt
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        5 2024-04-09 18:42:56.000000 tjfu-3.1.1/tjfu.egg-info/top_level.txt
+drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-26 18:01:37.613239 tjfu-3.2.0/
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     8624 2024-04-26 18:01:37.613239 tjfu-3.2.0/PKG-INFO
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     8058 2024-04-26 17:58:26.000000 tjfu-3.2.0/README.md
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)       38 2024-04-26 18:01:37.613239 tjfu-3.2.0/setup.cfg
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     1224 2024-04-25 19:29:35.000000 tjfu-3.2.0/setup.py
+drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-26 18:01:37.613239 tjfu-3.2.0/tjfu/
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      114 2024-04-25 19:29:52.000000 tjfu-3.2.0/tjfu/__init__.py
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     1222 2024-04-25 19:28:34.000000 tjfu-3.2.0/tjfu/route.py
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      490 2024-04-25 19:28:34.000000 tjfu-3.2.0/tjfu/tj_socket.py
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      461 2024-04-26 17:22:09.000000 tjfu-3.2.0/tjfu/tj_utils.py
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     9900 2024-04-26 17:52:20.000000 tjfu-3.2.0/tjfu/tjfu.py
+drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-26 18:01:37.613239 tjfu-3.2.0/tjfu.egg-info/
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     8624 2024-04-26 18:01:37.000000 tjfu-3.2.0/tjfu.egg-info/PKG-INFO
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      236 2024-04-26 18:01:37.000000 tjfu-3.2.0/tjfu.egg-info/SOURCES.txt
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)        1 2024-04-26 18:01:37.000000 tjfu-3.2.0/tjfu.egg-info/dependency_links.txt
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)       65 2024-04-26 18:01:37.000000 tjfu-3.2.0/tjfu.egg-info/requires.txt
+-rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)        5 2024-04-26 18:01:37.000000 tjfu-3.2.0/tjfu.egg-info/top_level.txt
```

### Comparing `tjfu-3.1.1/PKG-INFO` & `tjfu-3.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,9 @@
-Metadata-Version: 2.1
-Name: tjfu
-Version: 3.1.1
-Summary: Python library helps optimize Flask development to be flexible and object-oriented.
-Home-page: https://github.com/duynguyen02/tjfu
-Author: DuyNguyen02
-License: UNKNOWN
-Keywords: Python,Flask
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # TJFU
 Python library helps optimize Flask development to be flexible and object-oriented.
-#### Version: 3.1.1
 ### Extensions have been integrated
 1. [JWT](https://flask-jwt-extended.readthedocs.io/en/stable/)
 2. [SocketIO](https://flask-socketio.readthedocs.io/en/latest/)
 3. [Limiter](https://flask-limiter.readthedocs.io/en/stable/)
 ### Installation
 ```
 pip install tjfu
@@ -44,38 +26,41 @@
 
 """
     The TJFU configuration must be placed
     at the beginning of the main function.
     Absolutely do not define or import any Route
     before calling the build() function because an error may occur.
 """
-(
-    TJFU
+{
+TJFU
     .host_name("0.0.0.0") # required
     .host_port(3100) # required        
     .root_path(HERE) # optinal (default: '.')        
     .template_folder("templates") # optinal (default: 'templates')
     .static_folder("static") # optinal (default: 'static')
     .jwt_secret_key("your_jwt_secret_key")
         # optinal / enter value if you want to use JWT, 
         # Otherwise the jwt_required function will throw an error
     .jwt_access_token_expires(timedelta(days=7)) # optinal (default: 'timedelta(days=7)')
     .jwt_refresh_token_expires(timedelta(days=14)) # optinal (default: 'timedelta(days=14)')
     .socket_root("socket") # optinal (default: 'socket') 
     .ignore_cors(True) # optinal (default: 'True')
     .add_error_handler(404, error_404) # optional
     .add_error_handler(500, error_500) # optional
+    .add_status_code_handler(500, error_500) # optional (>=3.2.0)
     .limiter_storage_uri("memory://") # optinal (default: 'memory://')
     .default_limits(["200 per day", "50 per hour"]) # optinal (default: '[]')
     .log_output(False) # optinal (default: 'True')
     .debug(False) # optinal (default: 'True')
     .use_reloader(False) # optinal (default: 'True')
     .allow_unsafe_werkzeug(False) # optinal (default: 'True')
+    .app_config('MY_SECRET_KEY', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY'] = 'my_secret_key'
+    .app_config('MY_SECRET_KEY_2', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY_2'] = 'my_secret_key'
     .build()
-)
+}
 
 from tjfu import Route
 
 app = TJFU.init_app(Route("index", "/"))
 
 IS_PRODUCTION = False
 
@@ -189,15 +174,21 @@
             "hello_world.html"
         ): None
     }
 )
 
 # OTHER CODE...
 ```
-
+Get Flask App after TJFU.build() (>=3.2.0)
+```Python
+# Example
+from tjfu import TJFU
+from flask_mail import Mail, Message
+mail = Mail(TJFU.app())
+```
 Define a Socket Handle:
 ```Python
 # OTHER CODE...
 
 from tjfu import SocketEvent, SocketHandle
 from flask import request
 class MySocketHandle(SocketHandle):
@@ -275,9 +266,8 @@
 
 ### Changelog
 - `1.0.0`: First version released. There is a problem in Socket implementation.
 - `2.0.0`: Edit the Socket structure. There is a problem deploying the application to the production environment.
 - `3.0.0`: The version is relatively stable, overcoming the problem of deploying applications in production environments.
 - `3.1.0`: Added the function of registering Routes using Routes Map
 - `3.1.1`: Fixed an issue where additional variables could not be added when inheriting the _index function in Route.
-
-
+- `3.2.0`: Assign keys/values to Flask App Config using TJFU.app_config(...,...), add function TJFU.app() to get Flask App after calling TJFU.build(), use the add_status_code_handler function instead of the add_error_handler function.
```

### Comparing `tjfu-3.1.1/README.md` & `tjfu-3.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,26 @@
+Metadata-Version: 2.1
+Name: tjfu
+Version: 3.2.0
+Summary: Python library helps optimize Flask development to be flexible and object-oriented.
+Home-page: https://github.com/duynguyen02/tjfu
+Author: Duy Nguyen
+License: UNKNOWN
+Keywords: Python,Flask
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # TJFU
 Python library helps optimize Flask development to be flexible and object-oriented.
-#### Version: 3.1.1
 ### Extensions have been integrated
 1. [JWT](https://flask-jwt-extended.readthedocs.io/en/stable/)
 2. [SocketIO](https://flask-socketio.readthedocs.io/en/latest/)
 3. [Limiter](https://flask-limiter.readthedocs.io/en/stable/)
 ### Installation
 ```
 pip install tjfu
@@ -27,38 +43,41 @@
 
 """
     The TJFU configuration must be placed
     at the beginning of the main function.
     Absolutely do not define or import any Route
     before calling the build() function because an error may occur.
 """
-(
-    TJFU
+{
+TJFU
     .host_name("0.0.0.0") # required
     .host_port(3100) # required        
     .root_path(HERE) # optinal (default: '.')        
     .template_folder("templates") # optinal (default: 'templates')
     .static_folder("static") # optinal (default: 'static')
     .jwt_secret_key("your_jwt_secret_key")
         # optinal / enter value if you want to use JWT, 
         # Otherwise the jwt_required function will throw an error
     .jwt_access_token_expires(timedelta(days=7)) # optinal (default: 'timedelta(days=7)')
     .jwt_refresh_token_expires(timedelta(days=14)) # optinal (default: 'timedelta(days=14)')
     .socket_root("socket") # optinal (default: 'socket') 
     .ignore_cors(True) # optinal (default: 'True')
     .add_error_handler(404, error_404) # optional
     .add_error_handler(500, error_500) # optional
+    .add_status_code_handler(500, error_500) # optional (>=3.2.0)
     .limiter_storage_uri("memory://") # optinal (default: 'memory://')
     .default_limits(["200 per day", "50 per hour"]) # optinal (default: '[]')
     .log_output(False) # optinal (default: 'True')
     .debug(False) # optinal (default: 'True')
     .use_reloader(False) # optinal (default: 'True')
     .allow_unsafe_werkzeug(False) # optinal (default: 'True')
+    .app_config('MY_SECRET_KEY', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY'] = 'my_secret_key'
+    .app_config('MY_SECRET_KEY_2', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY_2'] = 'my_secret_key'
     .build()
-)
+}
 
 from tjfu import Route
 
 app = TJFU.init_app(Route("index", "/"))
 
 IS_PRODUCTION = False
 
@@ -172,15 +191,21 @@
             "hello_world.html"
         ): None
     }
 )
 
 # OTHER CODE...
 ```
-
+Get Flask App after TJFU.build() (>=3.2.0)
+```Python
+# Example
+from tjfu import TJFU
+from flask_mail import Mail, Message
+mail = Mail(TJFU.app())
+```
 Define a Socket Handle:
 ```Python
 # OTHER CODE...
 
 from tjfu import SocketEvent, SocketHandle
 from flask import request
 class MySocketHandle(SocketHandle):
@@ -258,7 +283,10 @@
 
 ### Changelog
 - `1.0.0`: First version released. There is a problem in Socket implementation.
 - `2.0.0`: Edit the Socket structure. There is a problem deploying the application to the production environment.
 - `3.0.0`: The version is relatively stable, overcoming the problem of deploying applications in production environments.
 - `3.1.0`: Added the function of registering Routes using Routes Map
 - `3.1.1`: Fixed an issue where additional variables could not be added when inheriting the _index function in Route.
+- `3.2.0`: Assign keys/values to Flask App Config using TJFU.app_config(...,...), add function TJFU.app() to get Flask App after calling TJFU.build(), use the add_status_code_handler function instead of the add_error_handler function.
+
+
```

### Comparing `tjfu-3.1.1/setup.py` & `tjfu-3.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 from setuptools import find_packages, setup
 from codecs import open
 from os import path
+import glob
+
+from tjfu import __version__, __author__
 
 HERE = path.abspath(path.dirname(__file__))
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
+    
+SCRIPTS = [
+    
+]
+    
+PACKAGES = [
+    'tjfu'
+]
+
+REQUIRED_PACKAGES = [
+    "flask",
+    "flask_cors",
+    "flask_jwt_extended",
+    "flask_socketio",
+    "flask_limiter"
+]
 
 setup(
     name='tjfu',
-    packages=find_packages(include=['tjfu']),
-    version='3.1.1',
+    packages=find_packages(include=PACKAGES),
+    scripts = SCRIPTS,
+    version=__version__,
     description='Python library helps optimize Flask development to be flexible and object-oriented.',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author='DuyNguyen02',
+    author=__author__,
     url="https://github.com/duynguyen02/tjfu",
-    install_requires=[
-        "flask",
-        "flask_cors",
-        "flask_jwt_extended",
-        "flask_socketio",
-        "flask_limiter"
-    ],
+    install_requires=REQUIRED_PACKAGES,
     python_requires=">=3.9",
     keywords=[
         "Python",
         "Flask"
     ],
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ]
-)
+)
```

### Comparing `tjfu-3.1.1/tjfu/route.py` & `tjfu-3.2.0/tjfu/route.py`

 * *Files identical despite different names*

### Comparing `tjfu-3.1.1/tjfu/tjfu.py` & `tjfu-3.2.0/tjfu/tjfu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from functools import wraps
 from flask import Flask
 from flask_cors import CORS
 from flask_jwt_extended import JWTManager
 from flask_socketio import SocketIO, emit
 from flask_limiter import Limiter
 from flask_limiter.util import get_remote_address
 
 from datetime import timedelta
 
 from .route import Route
 from .tj_socket import SocketEvent, SocketHandle
+from .tj_utils import deprecated
 
 class MissingPropertyException(Exception):
     def __init__(self, err) -> None:
-        super().__init__(f"Missing property: {err}")    
+        super().__init__(f"Missing property: {err}")
 
 class TJFU:
     # app properties
     _HOST_NAME: str = None
     _HOST_PORT: int = None
     _ROOT_PATH: str = '.'
     _FLASK_APP: Flask = None
@@ -49,143 +51,209 @@
     _USE_RELOADER: bool = True
     _LOG_OUTPUT: bool = True
     _ALLOW_UNSAFE_WERKZEUG: bool = True
     
     # error handler
     _ERROR_HANDLER: dict[int, any] = {}
     
+    # app config
+    _APP_CONFIG = {}
+    
+    
+    def _after_build_func(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            if TJFU._FLASK_APP is None:
+                raise Exception("TJFU has not been built yet, please call TJFU.build() before using this function.")
+            return func(*args, **kwargs)
+        return wrapper
+    
+    def _build_func(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            if TJFU._FLASK_APP is not None:
+                raise Exception("This function cannot be used after TJFU.build()")
+            return func(*args, **kwargs)
+        return wrapper
+    
     @staticmethod
+    @_after_build_func
     def limiter():
         return TJFU._LIMITER
     
     @staticmethod
+    @_after_build_func
+    def app():
+        return TJFU._FLASK_APP
+    
+    @staticmethod
+    @_build_func
+    def app_config(key: str, value: str):
+        TJFU._APP_CONFIG[key] = value
+        return TJFU
+    
+    @staticmethod
+    @_build_func
+    @deprecated("Use method add_status_code_handler instead")
     def add_error_handler(code:int, handler):
         TJFU._ERROR_HANDLER[code] = handler
         return TJFU
     
     @staticmethod
+    @_build_func
+    def add_status_code_handler(code:int, handler):
+        TJFU._ERROR_HANDLER[code] = handler
+        return TJFU
+    
+    @staticmethod
+    @_build_func
     def limiter_storage_uri(limiter_storage_uri: str):
         TJFU._LIMITER_STORAGE_URI = limiter_storage_uri
         return TJFU
     
     @staticmethod
+    @_build_func
     def default_limits(default_limits: list[str]):
         TJFU._DEFAULT_LIMITS = default_limits
         return TJFU
     
     @staticmethod
+    @_build_func
     def host_name(host_name: str):
         TJFU._HOST_NAME = host_name
         return TJFU
 
     @staticmethod
+    @_build_func
     def host_port(host_port: int):
         TJFU._HOST_PORT = host_port
         return TJFU
     
     @staticmethod
+    @_build_func
     def root_path(root_path: str):
         TJFU._ROOT_PATH = root_path
         return TJFU
 
     @staticmethod
+    @_build_func
     def template_folder(template_folder: str):
         TJFU._TEMPLATE_FOLDER = template_folder
         return TJFU
     
     @staticmethod
+    @_build_func
     def static_folder(static_folder: str):
         TJFU._STATIC_FOLDER = static_folder
         return TJFU
 
     @staticmethod
+    @_build_func
     def jwt_secret_key(jwt_secret_key: str):
         TJFU._JWT_SECRET_KEY = jwt_secret_key
         return TJFU
     
     @staticmethod
+    @_build_func
     def jwt_access_token_expires(jwt_access_token_expires: timedelta):
         TJFU._JWT_ACCESS_TOKEN_EXPIRES = jwt_access_token_expires
         return TJFU
     
     @staticmethod
+    @_build_func
     def jwt_refresh_token_expires(jwt_refresh_token_expires: timedelta):
         TJFU._JWT_REFRESH_TOKEN_EXPIRES = jwt_refresh_token_expires
         return TJFU
     
     @staticmethod
+    @_build_func
     def socket_root(socket_root: str):
         TJFU._SOCKET_ROOT = socket_root
         return TJFU
     
     @staticmethod
+    @_build_func
     def ignore_cors(ignore_cors: bool):
         TJFU._IGNORE_CORS = ignore_cors
         return TJFU
     
     @staticmethod
+    @_build_func
     def debug(debug: bool):
         TJFU._DEBUG = debug
         return TJFU
     
     @staticmethod
+    @_build_func
     def use_reloader(use_reloader: bool):
         TJFU._USE_RELOADER = use_reloader
         return TJFU
     
     @staticmethod
+    @_build_func
     def log_output(log_output: bool):
         TJFU._LOG_OUTPUT = log_output
         return TJFU
     
     @staticmethod
+    @_build_func
     def allow_unsafe_werkzeug(allow_unsafe_werkzeug: bool):
         TJFU._ALLOW_UNSAFE_WERKZEUG = allow_unsafe_werkzeug
         return TJFU
     
     _IS_RUNNING = False
     
     @staticmethod
     def build():
         if TJFU._HOST_NAME is None:
             raise MissingPropertyException("host_name")
         if TJFU._HOST_PORT is None:
             raise MissingPropertyException("host_port")
         
+        # init flask app
         TJFU._FLASK_APP = Flask(
             __name__,
             root_path=TJFU._ROOT_PATH,
             template_folder=TJFU._TEMPLATE_FOLDER,
             static_folder=TJFU._STATIC_FOLDER
         )
         
+        # add app config
+        for key, value in TJFU._APP_CONFIG.items():
+            TJFU._FLASK_APP.config[key] = value
+        
+        # add status code handler
         for code in TJFU._ERROR_HANDLER.keys():
             TJFU._FLASK_APP.errorhandler(code)(TJFU._ERROR_HANDLER[code])
         
+        # ignore CORS
         if TJFU._IGNORE_CORS:
             CORS(TJFU._FLASK_APP, origins='*')
             TJFU._CORS = CORS(TJFU._FLASK_APP, resource={
                 r"/*":{
                     "origins":"*"
                 }
             })
-            
+        
+        # init jwt
         if TJFU._JWT_SECRET_KEY is not None:
             TJFU._FLASK_APP.config['JWT_SECRET_KEY'] = TJFU._JWT_SECRET_KEY
             TJFU._FLASK_APP.config['JWT_ACCESS_TOKEN_EXPIRES'] = TJFU._JWT_ACCESS_TOKEN_EXPIRES
             TJFU._FLASK_APP.config['JWT_REFRESH_TOKEN_EXPIRES'] = TJFU._JWT_REFRESH_TOKEN_EXPIRES
             TJFU._JWT = JWTManager(TJFU._FLASK_APP)
             
+        # init limiter
         TJFU._LIMITER = Limiter(
             get_remote_address,
             app=TJFU._FLASK_APP,
             default_limits=TJFU._DEFAULT_LIMITS,
             storage_uri=TJFU._LIMITER_STORAGE_URI,
         )
         
+        # init socketio
         TJFU._SOCKET_IO = SocketIO(
             TJFU._FLASK_APP,
             cors_allowed_origins="*",
             async_mode=TJFU._SOCKET_ASYNC_MODE
         )
     
     def _routes_map_register(index_route: Route, routes_map: dict):
```

### Comparing `tjfu-3.1.1/tjfu.egg-info/PKG-INFO` & `tjfu-3.2.0/tjfu.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: tjfu
-Version: 3.1.1
+Version: 3.2.0
 Summary: Python library helps optimize Flask development to be flexible and object-oriented.
 Home-page: https://github.com/duynguyen02/tjfu
-Author: DuyNguyen02
+Author: Duy Nguyen
 License: UNKNOWN
 Keywords: Python,Flask
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # TJFU
 Python library helps optimize Flask development to be flexible and object-oriented.
-#### Version: 3.1.1
 ### Extensions have been integrated
 1. [JWT](https://flask-jwt-extended.readthedocs.io/en/stable/)
 2. [SocketIO](https://flask-socketio.readthedocs.io/en/latest/)
 3. [Limiter](https://flask-limiter.readthedocs.io/en/stable/)
 ### Installation
 ```
 pip install tjfu
@@ -44,38 +43,41 @@
 
 """
     The TJFU configuration must be placed
     at the beginning of the main function.
     Absolutely do not define or import any Route
     before calling the build() function because an error may occur.
 """
-(
-    TJFU
+{
+TJFU
     .host_name("0.0.0.0") # required
     .host_port(3100) # required        
     .root_path(HERE) # optinal (default: '.')        
     .template_folder("templates") # optinal (default: 'templates')
     .static_folder("static") # optinal (default: 'static')
     .jwt_secret_key("your_jwt_secret_key")
         # optinal / enter value if you want to use JWT, 
         # Otherwise the jwt_required function will throw an error
     .jwt_access_token_expires(timedelta(days=7)) # optinal (default: 'timedelta(days=7)')
     .jwt_refresh_token_expires(timedelta(days=14)) # optinal (default: 'timedelta(days=14)')
     .socket_root("socket") # optinal (default: 'socket') 
     .ignore_cors(True) # optinal (default: 'True')
     .add_error_handler(404, error_404) # optional
     .add_error_handler(500, error_500) # optional
+    .add_status_code_handler(500, error_500) # optional (>=3.2.0)
     .limiter_storage_uri("memory://") # optinal (default: 'memory://')
     .default_limits(["200 per day", "50 per hour"]) # optinal (default: '[]')
     .log_output(False) # optinal (default: 'True')
     .debug(False) # optinal (default: 'True')
     .use_reloader(False) # optinal (default: 'True')
     .allow_unsafe_werkzeug(False) # optinal (default: 'True')
+    .app_config('MY_SECRET_KEY', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY'] = 'my_secret_key'
+    .app_config('MY_SECRET_KEY_2', 'my_secret_key') # optional (>=3.2.0): use as app['MY_SECRET_KEY_2'] = 'my_secret_key'
     .build()
-)
+}
 
 from tjfu import Route
 
 app = TJFU.init_app(Route("index", "/"))
 
 IS_PRODUCTION = False
 
@@ -189,15 +191,21 @@
             "hello_world.html"
         ): None
     }
 )
 
 # OTHER CODE...
 ```
-
+Get Flask App after TJFU.build() (>=3.2.0)
+```Python
+# Example
+from tjfu import TJFU
+from flask_mail import Mail, Message
+mail = Mail(TJFU.app())
+```
 Define a Socket Handle:
 ```Python
 # OTHER CODE...
 
 from tjfu import SocketEvent, SocketHandle
 from flask import request
 class MySocketHandle(SocketHandle):
@@ -275,9 +283,10 @@
 
 ### Changelog
 - `1.0.0`: First version released. There is a problem in Socket implementation.
 - `2.0.0`: Edit the Socket structure. There is a problem deploying the application to the production environment.
 - `3.0.0`: The version is relatively stable, overcoming the problem of deploying applications in production environments.
 - `3.1.0`: Added the function of registering Routes using Routes Map
 - `3.1.1`: Fixed an issue where additional variables could not be added when inheriting the _index function in Route.
+- `3.2.0`: Assign keys/values to Flask App Config using TJFU.app_config(...,...), add function TJFU.app() to get Flask App after calling TJFU.build(), use the add_status_code_handler function instead of the add_error_handler function.
```

