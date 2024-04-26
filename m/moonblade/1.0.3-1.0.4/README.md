# Comparing `tmp/moonblade-1.0.3.tar.gz` & `tmp/moonblade-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonblade-1.0.3.tar", last modified: Tue Apr 23 08:59:14 2024, max compression
+gzip compressed data, was "moonblade-1.0.4.tar", last modified: Fri Apr 26 02:18:01 2024, max compression
```

## Comparing `moonblade-1.0.3.tar` & `moonblade-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 08:59:14.533739 moonblade-1.0.3/
--rw-rw-rw-   0        0        0     1090 2024-04-23 08:54:11.000000 moonblade-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3793 2024-04-23 08:59:14.523639 moonblade-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3071 2024-04-23 08:56:46.000000 moonblade-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 08:59:14.518738 moonblade-1.0.3/moonblade/
--rw-rw-rw-   0        0        0      547 2024-04-23 08:59:07.000000 moonblade-1.0.3/moonblade/__init__.py
--rw-rw-rw-   0        0        0      297 2024-04-23 06:56:09.000000 moonblade-1.0.3/moonblade/logger.py
--rw-rw-rw-   0        0        0     5444 2024-04-23 06:58:53.000000 moonblade-1.0.3/moonblade/moonblade.py
--rw-rw-rw-   0        0        0     5491 2024-04-23 07:01:00.000000 moonblade-1.0.3/moonblade/router.py
--rw-rw-rw-   0        0        0      741 2024-04-23 06:59:04.000000 moonblade-1.0.3/moonblade/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:59:14.522639 moonblade-1.0.3/moonblade.egg-info/
--rw-rw-rw-   0        0        0     3793 2024-04-23 08:59:14.000000 moonblade-1.0.3/moonblade.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-04-23 08:59:14.000000 moonblade-1.0.3/moonblade.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 08:59:14.000000 moonblade-1.0.3/moonblade.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-23 08:59:14.000000 moonblade-1.0.3/moonblade.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-23 08:59:14.000000 moonblade-1.0.3/moonblade.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 08:59:14.533739 moonblade-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1082 2024-04-23 08:59:10.000000 moonblade-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:18:01.925118 moonblade-1.0.4/
+-rw-rw-rw-   0        0        0     1090 2024-04-23 08:54:11.000000 moonblade-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3817 2024-04-26 02:18:01.924117 moonblade-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3095 2024-04-26 02:13:13.000000 moonblade-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 02:18:01.918118 moonblade-1.0.4/moonblade/
+-rw-rw-rw-   0        0        0      547 2024-04-26 02:16:36.000000 moonblade-1.0.4/moonblade/__init__.py
+-rw-rw-rw-   0        0        0      297 2024-04-23 06:56:09.000000 moonblade-1.0.4/moonblade/logger.py
+-rw-rw-rw-   0        0        0     5444 2024-04-23 06:58:53.000000 moonblade-1.0.4/moonblade/moonblade.py
+-rw-rw-rw-   0        0        0     5491 2024-04-23 07:01:00.000000 moonblade-1.0.4/moonblade/router.py
+-rw-rw-rw-   0        0        0      741 2024-04-23 06:59:04.000000 moonblade-1.0.4/moonblade/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:18:01.923118 moonblade-1.0.4/moonblade.egg-info/
+-rw-rw-rw-   0        0        0     3817 2024-04-26 02:18:01.000000 moonblade-1.0.4/moonblade.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-04-26 02:18:01.000000 moonblade-1.0.4/moonblade.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 02:18:01.000000 moonblade-1.0.4/moonblade.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-26 02:18:01.000000 moonblade-1.0.4/moonblade.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-26 02:18:01.000000 moonblade-1.0.4/moonblade.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 02:18:01.925118 moonblade-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2024-04-26 02:16:57.000000 moonblade-1.0.4/setup.py
```

### Comparing `moonblade-1.0.3/LICENSE` & `moonblade-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `moonblade-1.0.3/PKG-INFO` & `moonblade-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonblade
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python 3 asynchronous library committed to communicating with LOL server through the LCU API in a simple and flexible way .
 Home-page: https://github.com/gfk-sveyigey/moonblade
 Author: gfk-sveyigey
 Author-email: gfk_sveyigey@163.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -64,15 +64,15 @@
 ```
 
 #### register
 
 To receive events, we need to register asynchronous handlers.
 The handler should be able to accept a dict param.
 ```python
-def example(data: dict):
+async def example(data: dict):
     pass
 
 router = Router()
 router.register(route = "/moonblade/start", event_type = "All", handler = example)
 ```
 Note that Router is a singleton class that points to the same Router no matter how many times it is instantiated.
 
@@ -81,15 +81,15 @@
 Router.register(route = "/moonblade/start", event_type = "All", handler = example)
 ```
 
 Router can also be use as a decorator to register route.
 
 ```python
 @Router.register(route = "/moonblade/start", event_type = "All")
-def example(data: dict):
+async def example(data: dict):
     pass
 ```
 In fact, I recommend using this way. It should be noted that when registering route with a decorator, the handler param should be `None`.
 
 We can also register asynchronous methods, which will be introduced later.
 
 ##### event_type
@@ -109,27 +109,27 @@
 class C(Node):
 
     def __init__(self) -> None:
         ...
         super().__init__()
 
     @Router.register('/moonblade/start')
-    def example(self, data: dict):
+    async def example(self, data: dict):
         pass
 ```
 
 Also, we can add `for key in self.__dir__(): getattr(self, key)` to the end of the `__init__` method to achieve the same effect.
 ```python
 class C:
     def __init__(self) -> None:
         for key in self.__dir__():
             getattr(self, key)
 
     @Router.register('/moonblade/start')
-    def example(self, data: dict):
+    async def example(self, data: dict):
         pass
 ```
 
 ## Application
 
 For more detailed usage instructions, reference the library [`Diana`](https://github.com/gfk-sveyigey/Diana) witch is based on moonblade.
```

### Comparing `moonblade-1.0.3/README.md` & `moonblade-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 ```
 
 #### register
 
 To receive events, we need to register asynchronous handlers.
 The handler should be able to accept a dict param.
 ```python
-def example(data: dict):
+async def example(data: dict):
     pass
 
 router = Router()
 router.register(route = "/moonblade/start", event_type = "All", handler = example)
 ```
 Note that Router is a singleton class that points to the same Router no matter how many times it is instantiated.
 
@@ -64,15 +64,15 @@
 Router.register(route = "/moonblade/start", event_type = "All", handler = example)
 ```
 
 Router can also be use as a decorator to register route.
 
 ```python
 @Router.register(route = "/moonblade/start", event_type = "All")
-def example(data: dict):
+async def example(data: dict):
     pass
 ```
 In fact, I recommend using this way. It should be noted that when registering route with a decorator, the handler param should be `None`.
 
 We can also register asynchronous methods, which will be introduced later.
 
 ##### event_type
@@ -92,27 +92,27 @@
 class C(Node):
 
     def __init__(self) -> None:
         ...
         super().__init__()
 
     @Router.register('/moonblade/start')
-    def example(self, data: dict):
+    async def example(self, data: dict):
         pass
 ```
 
 Also, we can add `for key in self.__dir__(): getattr(self, key)` to the end of the `__init__` method to achieve the same effect.
 ```python
 class C:
     def __init__(self) -> None:
         for key in self.__dir__():
             getattr(self, key)
 
     @Router.register('/moonblade/start')
-    def example(self, data: dict):
+    async def example(self, data: dict):
         pass
 ```
 
 ## Application
 
 For more detailed usage instructions, reference the library [`Diana`](https://github.com/gfk-sveyigey/Diana) witch is based on moonblade.
```

### Comparing `moonblade-1.0.3/moonblade/__init__.py` & `moonblade-1.0.4/moonblade/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .moonblade import MoonBlade, EventCode
 from .router import Router, Node
 
 __title__ = "moonblade"
 __description__ = "A Python 3 asynchronous library committed to communicating with LOL server through the LCU API in a simple and flexible way ."
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __author__ = "gfk-sveyigey"
 __author_email__ = "gfk_sveyigey@163.com"
 __url__ = "https://github.com/gfk-sveyigey/moonblade"
 
 
 __all__ = [
     "__title__",
```

### Comparing `moonblade-1.0.3/moonblade/moonblade.py` & `moonblade-1.0.4/moonblade/moonblade.py`

 * *Files identical despite different names*

### Comparing `moonblade-1.0.3/moonblade/router.py` & `moonblade-1.0.4/moonblade/router.py`

 * *Files identical despite different names*

### Comparing `moonblade-1.0.3/moonblade/utils.py` & `moonblade-1.0.4/moonblade/utils.py`

 * *Files identical despite different names*

### Comparing `moonblade-1.0.3/moonblade.egg-info/PKG-INFO` & `moonblade-1.0.4/moonblade.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonblade
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python 3 asynchronous library committed to communicating with LOL server through the LCU API in a simple and flexible way .
 Home-page: https://github.com/gfk-sveyigey/moonblade
 Author: gfk-sveyigey
 Author-email: gfk_sveyigey@163.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -64,15 +64,15 @@
 ```
 
 #### register
 
 To receive events, we need to register asynchronous handlers.
 The handler should be able to accept a dict param.
 ```python
-def example(data: dict):
+async def example(data: dict):
     pass
 
 router = Router()
 router.register(route = "/moonblade/start", event_type = "All", handler = example)
 ```
 Note that Router is a singleton class that points to the same Router no matter how many times it is instantiated.
 
@@ -81,15 +81,15 @@
 Router.register(route = "/moonblade/start", event_type = "All", handler = example)
 ```
 
 Router can also be use as a decorator to register route.
 
 ```python
 @Router.register(route = "/moonblade/start", event_type = "All")
-def example(data: dict):
+async def example(data: dict):
     pass
 ```
 In fact, I recommend using this way. It should be noted that when registering route with a decorator, the handler param should be `None`.
 
 We can also register asynchronous methods, which will be introduced later.
 
 ##### event_type
@@ -109,27 +109,27 @@
 class C(Node):
 
     def __init__(self) -> None:
         ...
         super().__init__()
 
     @Router.register('/moonblade/start')
-    def example(self, data: dict):
+    async def example(self, data: dict):
         pass
 ```
 
 Also, we can add `for key in self.__dir__(): getattr(self, key)` to the end of the `__init__` method to achieve the same effect.
 ```python
 class C:
     def __init__(self) -> None:
         for key in self.__dir__():
             getattr(self, key)
 
     @Router.register('/moonblade/start')
-    def example(self, data: dict):
+    async def example(self, data: dict):
         pass
 ```
 
 ## Application
 
 For more detailed usage instructions, reference the library [`Diana`](https://github.com/gfk-sveyigey/Diana) witch is based on moonblade.
```

### Comparing `moonblade-1.0.3/setup.py` & `moonblade-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 path = pathlib.Path(__file__).parent
 
 long_description = (path / "README.md").read_text(encoding="utf-8")
 
 setup(
     name = "moonblade",
-    version = "1.0.3",
+    version = "1.0.4",
     description = "A Python 3 asynchronous library committed to communicating with LOL server through the LCU API in a simple and flexible way .",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/gfk-sveyigey/moonblade",
     author = "gfk-sveyigey",
     author_email = "gfk_sveyigey@163.com",
     license = "MIT",
```

