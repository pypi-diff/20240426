# Comparing `tmp/rxdjango-0.0.7.tar.gz` & `tmp/rxdjango-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxdjango-0.0.7.tar", last modified: Mon Oct 16 12:45:46 2023, max compression
+gzip compressed data, was "rxdjango-0.0.8.tar", last modified: Fri Apr 26 14:55:17 2024, max compression
```

## Comparing `rxdjango-0.0.7.tar` & `rxdjango-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,60 @@
-drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2023-10-16 12:45:46.389697 rxdjango-0.0.7/
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1064 2022-10-23 15:25:56.000000 rxdjango-0.0.7/LICENSE.md
--rw-r--r--   0 lfagundes  (1000) lfagundes  (1000)     3181 2023-10-16 12:45:46.389697 rxdjango-0.0.7/PKG-INFO
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     2628 2023-10-16 12:31:42.000000 rxdjango-0.0.7/README.md
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)      589 2023-10-16 12:45:26.000000 rxdjango-0.0.7/pyproject.toml
-drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2023-10-16 12:45:46.385697 rxdjango-0.0.7/rxdjango/
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        0 2023-09-25 11:04:24.000000 rxdjango-0.0.7/rxdjango/__init__.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1181 2023-09-25 11:04:24.000000 rxdjango-0.0.7/rxdjango/apps.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     4092 2023-10-03 14:06:29.000000 rxdjango-0.0.7/rxdjango/channels.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     4959 2023-10-03 19:33:25.000000 rxdjango-0.0.7/rxdjango/consumers.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)       68 2023-09-25 11:04:24.000000 rxdjango-0.0.7/rxdjango/decorators.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)      179 2023-09-29 17:38:53.000000 rxdjango-0.0.7/rxdjango/exceptions.py
-drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2023-10-16 12:45:46.385697 rxdjango-0.0.7/rxdjango/management/
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        0 2023-09-23 14:04:36.000000 rxdjango-0.0.7/rxdjango/management/__init__.py
-drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2023-10-16 12:45:46.385697 rxdjango-0.0.7/rxdjango/management/commands/
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        0 2023-09-23 14:04:36.000000 rxdjango-0.0.7/rxdjango/management/commands/__init__.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1056 2023-09-25 11:04:24.000000 rxdjango-0.0.7/rxdjango/management/commands/makefrontend.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     3899 2023-10-03 19:33:25.000000 rxdjango-0.0.7/rxdjango/mongo.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)    14705 2023-09-25 11:04:24.000000 rxdjango-0.0.7/rxdjango/redis.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1605 2023-10-10 16:55:13.000000 rxdjango-0.0.7/rxdjango/related_properties.py
-drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2023-10-16 12:45:46.385697 rxdjango-0.0.7/rxdjango/rxdjango.egg-info/
--rw-r--r--   0 lfagundes  (1000) lfagundes  (1000)     3181 2023-10-16 12:45:46.000000 rxdjango-0.0.7/rxdjango/rxdjango.egg-info/PKG-INFO
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1441 2023-10-16 12:45:46.000000 rxdjango-0.0.7/rxdjango/rxdjango.egg-info/SOURCES.txt
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        1 2023-10-16 12:45:46.000000 rxdjango-0.0.7/rxdjango/rxdjango.egg-info/dependency_links.txt
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)      169 2023-10-16 12:45:46.000000 rxdjango-0.0.7/rxdjango/rxdjango.egg-info/top_level.txt
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     4952 2023-10-10 13:23:56.000000 rxdjango-0.0.7/rxdjango/signal_handler.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     4656 2023-10-03 19:33:25.000000 rxdjango-0.0.7/rxdjango/state_loader.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     8865 2023-10-10 18:35:45.000000 rxdjango-0.0.7/rxdjango/state_model.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)      497 2023-09-25 11:04:24.000000 rxdjango-0.0.7/rxdjango/transaction.py
-drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2023-10-16 12:45:46.385697 rxdjango-0.0.7/rxdjango/ts/
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1933 2023-09-29 17:38:53.000000 rxdjango-0.0.7/rxdjango/ts/__init__.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     5835 2023-10-16 12:31:42.000000 rxdjango-0.0.7/rxdjango/ts/channels.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     6372 2023-09-29 17:38:53.000000 rxdjango-0.0.7/rxdjango/ts/interfaces.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1954 2023-09-27 14:38:54.000000 rxdjango-0.0.7/rxdjango/websocket_router.py
--rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)       38 2023-10-16 12:45:46.389697 rxdjango-0.0.7/setup.cfg
+drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-26 14:55:17.029853 rxdjango-0.0.8/
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1064 2022-10-23 15:25:56.000000 rxdjango-0.0.8/LICENSE.md
+-rw-r--r--   0 lfagundes  (1000) lfagundes  (1000)      439 2024-04-26 14:55:17.029853 rxdjango-0.0.8/PKG-INFO
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     2628 2023-12-21 12:52:38.000000 rxdjango-0.0.8/README.md
+drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-26 14:55:17.025853 rxdjango-0.0.8/rxdjango/
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        0 2023-12-18 14:58:19.000000 rxdjango-0.0.8/rxdjango/__init__.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1181 2023-12-18 14:58:19.000000 rxdjango-0.0.8/rxdjango/apps.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     4092 2024-01-30 18:38:00.000000 rxdjango-0.0.8/rxdjango/channels.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     4995 2024-02-12 14:05:59.000000 rxdjango-0.0.8/rxdjango/consumers.py
+drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-26 14:55:17.029853 rxdjango-0.0.8/rxdjango/contrib/
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-25 20:41:25.000000 rxdjango-0.0.8/rxdjango/contrib/__init__.py
+drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-26 14:55:17.029853 rxdjango-0.0.8/rxdjango/contrib/celery/
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-25 20:41:28.000000 rxdjango-0.0.8/rxdjango/contrib/celery/__init__.py
+drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-26 14:55:17.029853 rxdjango-0.0.8/rxdjango/contrib/celery/backends/
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-25 20:41:31.000000 rxdjango-0.0.8/rxdjango/contrib/celery/backends/__init__.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)       68 2023-12-18 14:58:19.000000 rxdjango-0.0.8/rxdjango/decorators.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)      179 2023-12-18 14:58:19.000000 rxdjango-0.0.8/rxdjango/exceptions.py
+drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-26 14:55:17.029853 rxdjango-0.0.8/rxdjango/management/
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        0 2023-12-18 14:57:31.000000 rxdjango-0.0.8/rxdjango/management/__init__.py
+drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-26 14:55:17.029853 rxdjango-0.0.8/rxdjango/management/commands/
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        0 2023-12-18 14:57:31.000000 rxdjango-0.0.8/rxdjango/management/commands/__init__.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)      978 2024-04-24 13:16:00.000000 rxdjango-0.0.8/rxdjango/management/commands/runserver.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     6301 2024-04-09 08:19:45.000000 rxdjango-0.0.8/rxdjango/mongo.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)    14734 2024-02-12 14:05:59.000000 rxdjango-0.0.8/rxdjango/redis.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     2355 2024-02-12 14:05:59.000000 rxdjango-0.0.8/rxdjango/related_properties.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)      345 2024-02-12 14:05:59.000000 rxdjango-0.0.8/rxdjango/serialize.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     7653 2024-04-24 13:16:17.000000 rxdjango-0.0.8/rxdjango/signal_handler.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     4656 2024-01-30 14:34:47.000000 rxdjango-0.0.8/rxdjango/state_loader.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     9296 2024-02-14 17:59:54.000000 rxdjango-0.0.8/rxdjango/state_model.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)      497 2023-12-18 14:58:19.000000 rxdjango-0.0.8/rxdjango/transaction.py
+drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-26 14:55:17.029853 rxdjango-0.0.8/rxdjango/ts/
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1919 2024-04-24 13:17:34.000000 rxdjango-0.0.8/rxdjango/ts/__init__.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     6578 2024-04-24 13:16:00.000000 rxdjango-0.0.8/rxdjango/ts/channels.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     6963 2024-04-24 13:16:00.000000 rxdjango-0.0.8/rxdjango/ts/interfaces.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1984 2024-02-12 14:05:59.000000 rxdjango-0.0.8/rxdjango/websocket_router.py
+drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-26 14:55:17.021854 rxdjango-0.0.8/rxdjango-env/
+drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-26 14:55:17.021854 rxdjango-0.0.8/rxdjango-env/bin/
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1257 2023-10-09 13:26:19.000000 rxdjango-0.0.8/rxdjango-env/bin/activate_this.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)     1733 2023-10-09 14:40:50.000000 rxdjango-0.0.8/rxdjango-env/bin/jp.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)      640 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rst2html.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)      762 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rst2html4.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)     1097 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rst2html5.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)      839 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rst2latex.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)      662 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rst2man.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)      828 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rst2odt.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)      634 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)      647 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)      683 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rst2s5.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)      919 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rst2xetex.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)      648 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rst2xml.py
+-rwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)      716 2023-10-09 14:07:00.000000 rxdjango-0.0.8/rxdjango-env/bin/rstpep2html.py
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1215 2023-10-09 14:40:35.000000 rxdjango-0.0.8/rxdjango-env/setup.py
+drwxrwxr-x   0 lfagundes  (1000) lfagundes  (1000)        0 2024-04-26 14:55:17.029853 rxdjango-0.0.8/rxdjango.egg-info/
+-rw-r--r--   0 lfagundes  (1000) lfagundes  (1000)      439 2024-04-26 14:55:16.000000 rxdjango-0.0.8/rxdjango.egg-info/PKG-INFO
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)     1814 2024-04-26 14:55:16.000000 rxdjango-0.0.8/rxdjango.egg-info/SOURCES.txt
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        1 2024-04-26 14:55:16.000000 rxdjango-0.0.8/rxdjango.egg-info/dependency_links.txt
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)      102 2024-04-26 14:55:16.000000 rxdjango-0.0.8/rxdjango.egg-info/requires.txt
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)        9 2024-04-26 14:55:16.000000 rxdjango-0.0.8/rxdjango.egg-info/top_level.txt
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)       38 2024-04-26 14:55:17.029853 rxdjango-0.0.8/setup.cfg
+-rw-rw-r--   0 lfagundes  (1000) lfagundes  (1000)      655 2023-12-21 12:52:38.000000 rxdjango-0.0.8/setup.py
```

### Comparing `rxdjango-0.0.7/LICENSE.md` & `rxdjango-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rxdjango-0.0.7/PKG-INFO` & `rxdjango-0.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: rxdjango
-Version: 0.0.7
-Summary: A Django layer to synchronize models between back and frontend
-Author-email: Luis Fagundes <lhfagundes@gmail.com>
-Project-URL: Homepage, https://github.com/CDIGlobalTrack/rxdjango
-Project-URL: Bug Tracker, https://github.com/CDIGlobalTrack/rxdjango/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 RxDjango
 =========
 
 RxDjango is a layer over Django Channels aimed to make it as simple as possible to broadcast
 changes in Django models to browsers through websockets, with minimal latency.
 
 It's evolving in production for more than 2 years now and it's revised API has just been released
```

### Comparing `rxdjango-0.0.7/rxdjango/apps.py` & `rxdjango-0.0.8/rxdjango/apps.py`

 * *Files identical despite different names*

### Comparing `rxdjango-0.0.7/rxdjango/channels.py` & `rxdjango-0.0.8/rxdjango/channels.py`

 * *Files identical despite different names*

### Comparing `rxdjango-0.0.7/rxdjango/consumers.py` & `rxdjango-0.0.8/rxdjango/consumers.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django.db.models.query import QuerySet
 from asgiref.sync import sync_to_async, async_to_sync
 from channels.db import database_sync_to_async
 from channels.generic.websocket import AsyncWebsocketConsumer
 from rest_framework.authtoken.models import Token
 from .state_loader import StateLoader
 from .exceptions import UnauthorizedError, ForbiddenError, AnchorDoesNotExist
+from rxdjango.serialize import json_dumps
 
 
 class StateConsumer(AsyncWebsocketConsumer):
     """
     WebSocket consumer that manages user authentication, session management,
     and real-time data relay to clients. A subclass of StateConsumer will be
     dinamically created by StateChannel.as_asgi().
@@ -42,14 +43,15 @@
 
     async def receive_authentication(self, text_data):
         # If user is not logged, we expect credentials
         data = json.loads(text_data)
         token = data.get('token', None)
         last_update  = data.get('last_update', None)
 
+        user = None
         try:
             user = await self.authenticate(token=token)
         except UnauthorizedError:
             await self.send_connection_status(401, 'error/unauthorized')
         except ForbiddenError:
             await self.send_connection_status(403, 'error/forbidden')
 
@@ -79,23 +81,23 @@
 
         async with StateLoader(self.channel) as loader:
             await self.send_connection_status(200)
             await self.channel.on_connect(tstamp)
 
             async for instances in loader.list_instances():
                 if instances:
-                    data = json.dumps(instances, default=str)
+                    data = json_dumps(instances)
                     await self.send(text_data=data)
 
             self.tstamp = loader.tstamp
             await self.send(text_data=self.end_of_data)
 
     @property
     def end_of_data(self):
-        return json.dumps([{
+        return json_dumps([{
             '_instance_type': '',
             '_tstamp': self.tstamp,
             '_operation': 'end_initial_state',
             'id': 0,
         }])
 
     @database_sync_to_async
@@ -132,25 +134,25 @@
             raise ForbiddenError('error/forbidden')
             return
 
         return token.user
 
     async def relay(self, payload):
         payload = payload['payload']
-        await self.send(text_data=json.dumps(payload, default=str))
+        await self.send(text_data=json_dumps(payload))
 
     async def receive_command(self, text_data):
         # If user is logged, we expect a JSON command
         try:
             data = json.loads(text_data)
         except json.JSONDecodeError:
             await self.disconnect()
         await self.channel.receive(data)
 
     async def send_connection_status(self, status_code, error=None):
         data = {}
         data['status_code'] = status_code
         if error:
             data['error'] = error
-        text_data = json.dumps(data)
+        text_data = json_dumps(data)
         close = error != None
         await self.send(text_data=text_data, close=close)
```

### Comparing `rxdjango-0.0.7/rxdjango/redis.py` & `rxdjango-0.0.8/rxdjango/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import redis
 from asgiref.sync import async_to_sync
 from django.utils.functional import cached_property
 from django.conf import settings
+from rxdjango.serialize import json_dumps
 
 
 async def _connect():
     return await redis.asyncio.from_url(settings.REDIS_URL)
 
 def _sync_connect():
     return redis.from_url(settings.REDIS_URL)
@@ -257,15 +258,15 @@
 
     async def write_instances(self, instances):
         """Serialize a list of objects, append them to the instances list, and publish the size to the trigger pub/sub channel.
 
         Args:
             objects (list): List of objects to append to the instances list.
         """
-        serialized_instances = [json.dumps(instance, default=str) for instance in instances]
+        serialized_instances = [json_dumps(instance) for instance in instances]
 
         script = """
         -- Append the serialized instances to instances list
         for i, obj in ipairs(ARGV) do
             redis.call("RPUSH", KEYS[3], obj)
         end
```

### Comparing `rxdjango-0.0.7/rxdjango/related_properties.py` & `rxdjango-0.0.8/rxdjango/related_properties.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,25 +6,32 @@
     return key in RelatedProperty.accessors
 
 
 def get_accessor(model, property_name):
     return RelatedProperty.get_accessor(model, property_name)
 
 
+def get_reverse_accessor(model, property_name):
+    return RelatedProperty.get_reverse_accessor(model, property_name)
+
+
 class RelatedProperty:
     accessors = {}
+    reverses = {}
     unknown_properties = set()
 
-    def __init__(self, accessor=None):
+    def __init__(self, accessor, reverse):
         self.accessor = accessor
+        self.reverse = reverse
 
     def __call__(self, fget):
         self.fget = fget
         key = (fget.__module__, fget.__qualname__)
         RelatedProperty.accessors[key] = self.accessor
+        RelatedProperty.reverses[key] = self.reverse
         return property(self._get_wrapper())
 
     def _get_wrapper(self):
         def wrapper(instance):
             return self.fget(instance)
         return wrapper
 
@@ -39,14 +46,28 @@
                 module = cls.__module__
                 raise UnknownProperty(
                     f'Unknown property {name}, use {module}.related_property '
                     'decorator instead to provide an acessor'
                 )
 
     @classmethod
+    def get_reverse_accessor(cls, model, property_name):
+        key = _make_key(model, property_name)
+        try:
+            return cls.reverses[key]
+        except KeyError:
+            if key in cls.unknown_properties:
+                name = '.'.join(key)
+                module = cls.__module__
+                raise UnknownProperty(
+                    f'Unknown property {name}, use {module}.related_property '
+                    'decorator instead to provide a reverse acessor'
+                )
+
+    @classmethod
     def register_unknown_property(cls, model, property_name):
         key = _make_key(model, property_name)
         cls.unknown_properties.add(key)
         return cls.accessors.get(key)
 
 def _make_key(model, property_name):
     qualname = '.'.join([model.__name__, property_name])
```

### Comparing `rxdjango-0.0.7/rxdjango/state_loader.py` & `rxdjango-0.0.8/rxdjango/state_loader.py`

 * *Files identical despite different names*

### Comparing `rxdjango-0.0.7/rxdjango/state_model.py` & `rxdjango-0.0.8/rxdjango/state_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import defaultdict
 from rest_framework import serializers
 from django.db import models, connection
 from django.db import ProgrammingError
 from django.db.models.fields import related_descriptors
 from .ts import export_interface
 from .exceptions import UnknownProperty
-from .related_properties import is_related_property, get_accessor
+from .related_properties import is_related_property, get_accessor, get_reverse_accessor
 
 class StateModel:
 
     def __init__(self, state_serializer, many=False, origin=None, instance_property=None, query_property=None, reverse_acessor=None):
         self.nested_serializer = state_serializer
         self.many = many
         self.origin = origin
@@ -40,14 +40,16 @@
         ])
         #modu = self.nested_serializer.__module__.replace('.serializers', '')
         #print(f"""perl -pi -e "s/instance_type === '{modu}.{self.model.__name__}/instance_type === '{self.instance_type}/" $1""")
 
         self.index[self.instance_type].append(self)
 
         self.user_key = getattr(meta, 'user_key', None)
+        if self.user_key and self.user_key not in meta.fields:
+            raise ProgrammingError(f'{state_serializer.__class__.__name__}.Meta declares user_key="{self.user_key}", but "{self.user_key}" is not in fields')
         self.optimistic = getattr(meta, 'optimistic', False)
         self.optimistic_timeout = getattr(meta, 'optimistic_timeout', 3)
 
         self.flat_serializer, fields = self._disassemble_nested()
 
         self.children = {}
         for field_name, serializer in fields.items():
@@ -127,16 +129,19 @@
                     continue
                 for serialized in peer_model.serialize_state(peer_instance, tstamp):
                     yield serialized
 
     def _mark(self, serialized, tstamp):
         serialized['_instance_type'] = self.instance_type
         serialized['_tstamp'] = tstamp
-        serialized['_user_key'] = self.user_key
         serialized['_operation'] = 'initial_state'
+        if self.user_key:
+            serialized['_user_key'] = serialized.get(self.user_key, None)
+        else:
+            serialized['_user_key'] = None
         return serialized
 
     def _disassemble_nested(self):
         serializer_fields = {}
         declared_fields = {}
 
         for field_name in self.nested_serializer.fields.keys():
@@ -214,19 +219,20 @@
         if isinstance(descriptor, related_descriptors.ReverseOneToOneDescriptor):
             return StateModel(
                 serializer,
                 False,
                 self,
                 field_name,
                 field_name,
-                descriptor.related.get_related_field().name,
+                descriptor.related.remote_field.name,
             )
 
         if isinstance(descriptor, property):
             query_property = get_accessor(self.model, field_name)
+            reverse_acessor = get_reverse_accessor(self.model, field_name)
             if not query_property:
                 my_module = self.__class__.__module__
                 raise UnknownProperty(
                     f'Unknown property {field_name} in '
                     f'{self.model.__module__}.{self.model.__name__}.\n'
                     f'Use {my_module}.decorators.related_property '
                     'to provide an acessor'
@@ -235,15 +241,15 @@
             many = getattr(serializer, 'many', False)
             return StateModel(
                 serializer.child if many else serializer,
                 many,
                 self,
                 field_name,
                 query_property,
-                None,
+                reverse_acessor,
             )
 
 
 def is_model_serializer(field):
     try:
         return isinstance(field.child, serializers.ModelSerializer)
     except AttributeError:
```

### Comparing `rxdjango-0.0.7/rxdjango/ts/__init__.py` & `rxdjango-0.0.8/rxdjango/ts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     return '.'.join([Serializer.__module__, Serializer.__name__])
 
 def header(app, *middle):
     now = timezone.now().strftime('%Y-%m-%d %H:%M')
     tz = timezone.now().tzinfo
 
     header = [
-        f' * Generated by Django React Framework on {now} ({tz})',
+        f' * Generated by RxDjango on {now} ({tz})',
     ] + [
         f' * {line}' for line in middle
     ]
 
     footer = [
         f' * To rebuild it, run:',
         f' *     ./manage.py makefrontend [{app}]',
```

### Comparing `rxdjango-0.0.7/rxdjango/ts/channels.py` & `rxdjango-0.0.8/rxdjango/ts/channels.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,31 @@
 
 def create_app_channels(app):
     consumer_urlpatterns = list_consumer_patterns(app)
 
     if not consumer_urlpatterns:
         return
 
-    path = os.path.join(settings.RX_FRONTEND_DIR, f'{app}/{app}.channels.ts')
+    channel_module_name = f'{app}.channels'
+    channel_path = channel_module_name.replace('.', '/') + '.py'
+
+    ts_file_path = os.path.join(settings.RX_FRONTEND_DIR, f'{app}/{app}.channels.ts')
+    py_mtime = None
+
+    if os.path.exists(channel_path):
+        py_mtime = os.path.getmtime(channel_path)
+
+
+    existing = []
+
+    if os.path.exists(ts_file_path):
+        if py_mtime == os.path.getmtime(ts_file_path):
+            return
+        with open(ts_file_path, 'r') as file:
+            existing = file.read().split('\n')
 
     code = header(
         app,
         f'Based on all StateChannel.as_asgi() calls in {settings.ASGI_APPLICATION}',
         f'This is expected to match {app}/channels.py',
     )
 
@@ -44,21 +60,29 @@
 
     code.append('')  # line break
     code.extend(build_imports(import_types, app))
     code.extend(body)
 
     content = '\n'.join(code)
 
+    if content.split('\n')[2:] == existing[2:]:
+        if py_mtime:
+            os.utime(ts_file_path, (py_mtime, py_mtime))
+        return
+
     try:
-        fh = open(path, 'w')
+        with open(ts_file_path, 'w') as fh:
+            fh.write(content)
     except FileNotFoundError:
-        os.mkdir(os.path.dirname(path))
-        fh = open(path, 'w')
-    fh.write(content)
-    fh.close()
+        os.makedirs(os.path.dirname(ts_file_path), exist_ok=True)
+        with open(ts_file_path, 'w') as fh:
+            fh.write(content)
+
+    if py_mtime:
+        os.utime(ts_file_path, (py_mtime, py_mtime))
 
 
 def get_root_routing():
     asgi_app = settings.ASGI_APPLICATION
     module_name, app_name = asgi_app.rsplit('.', 1)
     module = __import__(module_name, fromlist=[app_name])
     return getattr(module, app_name)
```

### Comparing `rxdjango-0.0.7/rxdjango/ts/interfaces.py` & `rxdjango-0.0.8/rxdjango/ts/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,71 +7,89 @@
 from django.utils import timezone
 from django.db.models.query import QuerySet
 from django.db.models.fields import related_descriptors
 from django.conf import settings
 from rest_framework import serializers, relations, fields
 from . import ts_exported, header, interface_name
 
-
 def create_app_interfaces(app):
+    serializer_module_name = f'{app}.serializers'
+    serializer_path = serializer_module_name.replace('.', '/') + '.py'
+
+    ts_file_path = os.path.join(settings.RX_FRONTEND_DIR, f'{app}/{app}.interfaces.d.ts')
+    py_mtime = None
+
+    if os.path.exists(serializer_path):
+        py_mtime = os.path.getmtime(serializer_path)
+
+    existing = []
+
+    if os.path.exists(ts_file_path):
+        if py_mtime == os.path.getmtime(ts_file_path):
+            return
+        with open(ts_file_path, 'r') as file:
+            existing = file.read().split('\n')
+
     try:
-        module = importlib.import_module(f'{app}.serializers')
+        module = importlib.import_module(serializer_module_name)
     except ModuleNotFoundError:
         return
 
-    path = os.path.join(settings.RX_FRONTEND_DIR, f'{app}/{app}.interfaces.d.ts')
-
     serializers = get_serializers(module)
 
     try:
         module_serializers = serializers.pop(app)
     except KeyError:
         return
 
-    now = timezone.now().strftime('%Y-%m-%d %H:%M')
-    tz = timezone.now().tzinfo
-
     code = header(
         app,
         f'Based on {app}/serializers.py',
     )
 
     initial_length = len(code)
 
-    code.append(f"import {{ InstanceType }} from 'lib/django-react';\n")
+    code.append(f"import {{ InstanceType }} from '@rxdjango/react';\n")
 
     for external_app, dependencies in serializers.items():
-        dependencies = [ dep for dep in dependencies if ts_exported(dep) ]
+        dependencies = [dep for dep in dependencies if ts_exported(dep)]
         if not dependencies:
             continue
         code.append(''.join([
             'import { ',
-            ', '.join([ interface_name(d) for d in dependencies ]),
+            ', '.join([interface_name(d) for d in dependencies]),
             ' } from ',
             f"'../{external_app}/{external_app}.interfaces';",
-            ]))
+        ]))
 
     code.append('')  # line break
 
     for Serializer in module_serializers:
         if ts_exported(Serializer):
             code.append(serialize_type(Serializer))
 
-    if len(code) == initial_length + 1:
+    if len(code) == initial_length + 2:
         return
 
     content = '\n'.join(code)
 
+    if content.split('\n')[2:] == existing[2:]:
+        return
+
     try:
-        fh = open(path, 'w')
+        with open(ts_file_path, 'w') as fh:
+            fh.write(content)
     except FileNotFoundError:
-        os.mkdir(os.path.dirname(path))
-        fh = open(path, 'w')
-    fh.write(content)
-    fh.close()
+        os.makedirs(os.path.dirname(ts_file_path), exist_ok=True)
+        with open(ts_file_path, 'w') as fh:
+            fh.write(content)
+
+    if py_mtime:
+        os.utime(ts_file_path, (py_mtime, py_mtime))
+
 
 def get_serializers(module):
     apps = {}
 
     for klass in _get_serializer_classes(module):
         app = klass.__module__.split('.')[0]
         try:
```

### Comparing `rxdjango-0.0.7/rxdjango/websocket_router.py` & `rxdjango-0.0.8/rxdjango/websocket_router.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 from asgiref.sync import async_to_sync
 import channels.layers
+from rxdjango.serialize import json_dumps
+
 
 def get_channel_key(name, anchor_id, user_id=None):
     if user_id is None:
         return f'{name}_{anchor_id}'
     return f'{name}_{anchor_id}_{user_id}'
 
 
@@ -32,15 +34,15 @@
 
     async def dispatch(self, payload, anchor_id, user_id=None):
         channel_key = get_channel_key(self.name, anchor_id, user_id)
         channel_layer = channels.layers.get_channel_layer()
 
         # FIXME: Datetime fields should be handled prior to this
         # This is probably due to properties such as launch_time
-        payload = json.dumps(payload, default=str)
+        payload = json_dumps(payload)
         payload = json.loads(payload)
 
         await channel_layer.group_send(
             channel_key,
             {
                 'type': 'relay',
                 'payload': payload,
```

