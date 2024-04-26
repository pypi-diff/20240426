# Comparing `tmp/flyerapi-1.0.7.tar.gz` & `tmp/flyerapi-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyerapi-1.0.7.tar", last modified: Sun Jan 21 11:32:24 2024, max compression
+gzip compressed data, was "flyerapi-1.0.8.tar", last modified: Fri Apr 26 10:37:53 2024, max compression
```

## Comparing `flyerapi-1.0.7.tar` & `flyerapi-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-01-21 11:32:24.939529 flyerapi-1.0.7/
--rw-rw-rw-   0        0        0     1210 2023-12-18 09:38:20.000000 flyerapi-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1980 2024-01-21 11:32:24.938161 flyerapi-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2023-12-23 21:37:03.000000 flyerapi-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-01-21 11:32:24.917545 flyerapi-1.0.7/flyerapi/
--rw-rw-rw-   0        0        0       27 2023-12-18 09:35:41.000000 flyerapi-1.0.7/flyerapi/__init__.py
--rw-rw-rw-   0        0        0     2811 2024-01-21 11:31:35.000000 flyerapi-1.0.7/flyerapi/flyerapi.py
-drwxrwxrwx   0        0        0        0 2024-01-21 11:32:24.936791 flyerapi-1.0.7/flyerapi.egg-info/
--rw-rw-rw-   0        0        0     1980 2024-01-21 11:32:24.000000 flyerapi-1.0.7/flyerapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2024-01-21 11:32:24.000000 flyerapi-1.0.7/flyerapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-21 11:32:24.000000 flyerapi-1.0.7/flyerapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-01-21 11:32:24.000000 flyerapi-1.0.7/flyerapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-01-21 11:32:24.000000 flyerapi-1.0.7/flyerapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-21 11:32:24.939529 flyerapi-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1220 2024-01-21 11:31:33.000000 flyerapi-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:37:53.671342 flyerapi-1.0.8/
+-rw-rw-rw-   0        0        0     1210 2023-12-18 09:38:20.000000 flyerapi-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2078 2024-04-26 10:37:53.670436 flyerapi-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1240 2024-04-26 10:37:04.000000 flyerapi-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 10:37:53.644053 flyerapi-1.0.8/flyerapi/
+-rw-rw-rw-   0        0        0       27 2023-12-18 09:35:41.000000 flyerapi-1.0.8/flyerapi/__init__.py
+-rw-rw-rw-   0        0        0     3248 2024-04-26 10:31:57.000000 flyerapi-1.0.8/flyerapi/flyerapi.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:37:53.668343 flyerapi-1.0.8/flyerapi.egg-info/
+-rw-rw-rw-   0        0        0     2078 2024-04-26 10:37:53.000000 flyerapi-1.0.8/flyerapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2024-04-26 10:37:53.000000 flyerapi-1.0.8/flyerapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 10:37:53.000000 flyerapi-1.0.8/flyerapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-26 10:37:53.000000 flyerapi-1.0.8/flyerapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-26 10:37:53.000000 flyerapi-1.0.8/flyerapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 10:37:53.671342 flyerapi-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2024-04-19 11:11:09.000000 flyerapi-1.0.8/setup.py
```

### Comparing `flyerapi-1.0.7/LICENSE` & `flyerapi-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flyerapi-1.0.7/PKG-INFO` & `flyerapi-1.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyerapi
-Version: 1.0.7
+Version: 1.0.8
 Summary: Asynchronous api of the Flyer service
 Home-page: https://github.com/EliCreator/flyerapi
 Author: Eli
 Author-email: <eli.dev.tg@gmail.com>
 Project-URL: Homepage, https://github.com/EliCreator/flyerapi
 Project-URL: Bug Tracker, https://github.com/EliCreator/flyerapi/issues
 Keywords: python,flyer,async,asyncio,cache
@@ -59,16 +59,18 @@
 
 from aiogram import types
 
 
 flyer = Flyer(KEY)
 
 async def message_handler(message: types.Message):
+    # Use it wherever verification is necessary
     if not await flyer.check(message.from_user.id):
         return
 
 async def callback_handler(call: types.CallbackQuery):
+    # Use it wherever verification is necessary
     if not await flyer.check(call.from_user.id):
         return
 ```
 
 Developed by Eli (c) 2023
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flyerapi Version: 1.0.7 Summary: Asynchronous api
+Metadata-Version: 2.1 Name: flyerapi Version: 1.0.8 Summary: Asynchronous api
 of the Flyer service Home-page: https://github.com/EliCreator/flyerapi Author:
 Eli Author-email:
 gmail.com> Project-URL: Homepage, https://github.com/EliCreator/flyerapi
 Project-URL: Bug Tracker, https://github.com/EliCreator/flyerapi/issues
 Keywords: python,flyer,async,asyncio,cache Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
@@ -11,11 +11,12 @@
 Requires-Dist: aiohttp Requires-Dist: cachetools
 ************ FFllyyeerrAAPPII[[hhttttppss::////tteelleeggrraa..pphh//ffiillee//ee22aa22ff00552266dd22993377997733aa7700bb..ppnngg]] ************
 _[_P_y_P_I_]_[_P_y_P_I_]
 ## Usage With ``flyerapi`` you can use _F_l_y_e_r_A_P_I together with Telegram ##
 Installation ```bash pip install flyerapi ``` ## Requirements - ``Python 3.7+``
 - ``aiohttp`` ## Features - ``Asynchronous`` - ``Exception handling`` ## Basic
 example with aiogram ```python from flyerapi import Flyer from aiogram import
-types flyer = Flyer(KEY) async def message_handler(message: types.Message): if
-not await flyer.check(message.from_user.id): return async def callback_handler
-(call: types.CallbackQuery): if not await flyer.check(call.from_user.id):
-return ``` Developed by Eli (c) 2023
+types flyer = Flyer(KEY) async def message_handler(message: types.Message): #
+Use it wherever verification is necessary if not await flyer.check
+(message.from_user.id): return async def callback_handler(call:
+types.CallbackQuery): # Use it wherever verification is necessary if not await
+flyer.check(call.from_user.id): return ``` Developed by Eli (c) 2023
```

### Comparing `flyerapi-1.0.7/flyerapi/flyerapi.py` & `flyerapi-1.0.8/flyerapi/flyerapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,39 @@
 
         self._cache = TTLCache(maxsize=10000, ttl=self.service_cache_answer)
         self._service_shutdown = 0
 
         self.debug = debug
 
 
+    async def _request(self, method: str, params: dict = {}, **kwargs) -> dict:
+        url = f'https://api.flyerservice.io/{method}'
+        headers = {'Content-Type': 'application/json'}
+        data = {'key': self.key, **params}
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(url, headers=headers, json=data, **kwargs) as response:
+                result = await response.json()
+
+                if self.debug:
+                    print(result)
+
+        return result
+
+
+    async def get_me(self) -> dict:
+        """
+        Get bot info.
+
+        :return: dict information
+        """
+
+        return await self._request('get_me')
+
+
     async def check(self, user_id: int, timeout: float=5) -> bool:
         """
         Check user subscription status.
 
         :param user_id: User ID
         :return: True if subscribed, False otherwise
         """
@@ -55,24 +80,19 @@
 
         # If cached response
         if self._cache.get(user_id, False):
             return True
 
 
         try:
-            url = 'https://api.flyerservice.io/check'
-            headers = {'Content-Type': 'application/json'}
-            data = {'key': self.key, 'user_id': user_id}
-
-            async with aiohttp.ClientSession() as session:
-                async with session.post(url, headers=headers, json=data, timeout=timeout) as response:
-                    result = await response.json()
-
-                    if self.debug:
-                        print(result)
+            result = await self._request(
+                method='check',
+                params={'user_id': user_id},
+                timeout=timeout,
+            )
 
         # The server is not responding
         except (ClientConnectorError, TimeoutError):
             self._service_shutdown = time.time()
             return True
 
         # Answer error
@@ -94,12 +114,12 @@
             logger.warning(result['warning'])
 
         elif 'info' in result:
             logger.info(result['info'])
 
 
         # If response is True, writing in cache
-        if result['skip']:
+        if result['skip'] and 'error' not in result:
             self._cache[user_id] = True
 
 
         return result['skip']
```

### Comparing `flyerapi-1.0.7/flyerapi.egg-info/PKG-INFO` & `flyerapi-1.0.8/flyerapi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyerapi
-Version: 1.0.7
+Version: 1.0.8
 Summary: Asynchronous api of the Flyer service
 Home-page: https://github.com/EliCreator/flyerapi
 Author: Eli
 Author-email: <eli.dev.tg@gmail.com>
 Project-URL: Homepage, https://github.com/EliCreator/flyerapi
 Project-URL: Bug Tracker, https://github.com/EliCreator/flyerapi/issues
 Keywords: python,flyer,async,asyncio,cache
@@ -59,16 +59,18 @@
 
 from aiogram import types
 
 
 flyer = Flyer(KEY)
 
 async def message_handler(message: types.Message):
+    # Use it wherever verification is necessary
     if not await flyer.check(message.from_user.id):
         return
 
 async def callback_handler(call: types.CallbackQuery):
+    # Use it wherever verification is necessary
     if not await flyer.check(call.from_user.id):
         return
 ```
 
 Developed by Eli (c) 2023
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flyerapi Version: 1.0.7 Summary: Asynchronous api
+Metadata-Version: 2.1 Name: flyerapi Version: 1.0.8 Summary: Asynchronous api
 of the Flyer service Home-page: https://github.com/EliCreator/flyerapi Author:
 Eli Author-email:
 gmail.com> Project-URL: Homepage, https://github.com/EliCreator/flyerapi
 Project-URL: Bug Tracker, https://github.com/EliCreator/flyerapi/issues
 Keywords: python,flyer,async,asyncio,cache Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
@@ -11,11 +11,12 @@
 Requires-Dist: aiohttp Requires-Dist: cachetools
 ************ FFllyyeerrAAPPII[[hhttttppss::////tteelleeggrraa..pphh//ffiillee//ee22aa22ff00552266dd22993377997733aa7700bb..ppnngg]] ************
 _[_P_y_P_I_]_[_P_y_P_I_]
 ## Usage With ``flyerapi`` you can use _F_l_y_e_r_A_P_I together with Telegram ##
 Installation ```bash pip install flyerapi ``` ## Requirements - ``Python 3.7+``
 - ``aiohttp`` ## Features - ``Asynchronous`` - ``Exception handling`` ## Basic
 example with aiogram ```python from flyerapi import Flyer from aiogram import
-types flyer = Flyer(KEY) async def message_handler(message: types.Message): if
-not await flyer.check(message.from_user.id): return async def callback_handler
-(call: types.CallbackQuery): if not await flyer.check(call.from_user.id):
-return ``` Developed by Eli (c) 2023
+types flyer = Flyer(KEY) async def message_handler(message: types.Message): #
+Use it wherever verification is necessary if not await flyer.check
+(message.from_user.id): return async def callback_handler(call:
+types.CallbackQuery): # Use it wherever verification is necessary if not await
+flyer.check(call.from_user.id): return ``` Developed by Eli (c) 2023
```

### Comparing `flyerapi-1.0.7/setup.py` & `flyerapi-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import codecs
 
 from setuptools import setup, find_packages
 
 
-VERSION = '1.0.7'
+VERSION = '1.0.8'
 DESCRIPTION = 'Asynchronous api of the Flyer service'
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as file:
     long_description = file.read()
```

