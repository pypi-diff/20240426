# Comparing `tmp/mxbt-0.3.4.1.tar.gz` & `tmp/mxbt-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxbt-0.3.4.1.tar", last modified: Sat Apr 20 10:05:53 2024, max compression
+gzip compressed data, was "mxbt-0.3.5.tar", last modified: Fri Apr 26 15:43:47 2024, max compression
```

## Comparing `mxbt-0.3.4.1.tar` & `mxbt-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-20 10:05:53.888230 mxbt-0.3.4.1/
--rw-r--r--   0 warlock   (1000) warlock   (1000)    35149 2024-03-11 08:01:52.000000 mxbt-0.3.4.1/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)     3036 2024-04-20 10:05:53.888230 mxbt-0.3.4.1/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2287 2024-04-20 08:57:14.000000 mxbt-0.3.4.1/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-20 10:05:53.888230 mxbt-0.3.4.1/mxbt/
--rw-r--r--   0 warlock   (1000) warlock   (1000)      242 2024-04-20 10:05:30.000000 mxbt-0.3.4.1/mxbt/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)    20565 2024-04-20 10:05:16.000000 mxbt-0.3.4.1/mxbt/api.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5465 2024-04-06 15:56:45.000000 mxbt-0.3.4.1/mxbt/auth.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5897 2024-04-11 12:46:01.000000 mxbt-0.3.4.1/mxbt/bot.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     3372 2024-04-11 12:46:01.000000 mxbt-0.3.4.1/mxbt/callbacks.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     7211 2024-03-11 08:01:52.000000 mxbt-0.3.4.1/mxbt/context.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     9633 2024-04-06 16:48:20.000000 mxbt-0.3.4.1/mxbt/filters.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5682 2024-03-11 08:01:52.000000 mxbt-0.3.4.1/mxbt/listener.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     3938 2024-04-06 16:48:25.000000 mxbt-0.3.4.1/mxbt/match.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2425 2024-03-11 08:01:52.000000 mxbt-0.3.4.1/mxbt/module.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-20 10:05:53.888230 mxbt-0.3.4.1/mxbt/types/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       67 2024-04-06 16:48:53.000000 mxbt-0.3.4.1/mxbt/types/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      279 2024-03-11 08:01:52.000000 mxbt-0.3.4.1/mxbt/types/command.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)    10011 2024-04-20 10:04:48.000000 mxbt-0.3.4.1/mxbt/types/file.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      178 2024-04-06 16:47:24.000000 mxbt-0.3.4.1/mxbt/types/msgtype.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      281 2024-04-11 12:46:01.000000 mxbt-0.3.4.1/mxbt/utils.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-20 10:05:53.888230 mxbt-0.3.4.1/mxbt.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     3036 2024-04-20 10:05:53.000000 mxbt-0.3.4.1/mxbt.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      415 2024-04-20 10:05:53.000000 mxbt-0.3.4.1/mxbt.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-20 10:05:53.000000 mxbt-0.3.4.1/mxbt.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       80 2024-04-20 10:05:53.000000 mxbt-0.3.4.1/mxbt.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        5 2024-04-20 10:05:53.000000 mxbt-0.3.4.1/mxbt.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-20 10:05:53.888230 mxbt-0.3.4.1/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1032 2024-03-11 08:01:52.000000 mxbt-0.3.4.1/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-26 15:43:47.046463 mxbt-0.3.5/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)    35149 2024-04-26 15:33:21.000000 mxbt-0.3.5/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3130 2024-04-26 15:43:47.046463 mxbt-0.3.5/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2383 2024-04-26 15:38:14.000000 mxbt-0.3.5/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-26 15:43:47.046463 mxbt-0.3.5/mxbt/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      221 2024-04-26 15:42:57.000000 mxbt-0.3.5/mxbt/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     5465 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/auth.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)    22720 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/bot.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3395 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/callbacks.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     7431 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/context.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     9633 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/filters.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     7582 2024-04-26 15:37:31.000000 mxbt-0.3.5/mxbt/listener.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3938 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/match.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2441 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/module.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-26 15:43:47.046463 mxbt-0.3.5/mxbt/types/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       67 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/types/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      279 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/types/command.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)    10011 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/types/file.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      178 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/types/msgtype.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      281 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/utils.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-26 15:43:47.046463 mxbt-0.3.5/mxbt.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3130 2024-04-26 15:43:46.000000 mxbt-0.3.5/mxbt.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      403 2024-04-26 15:43:46.000000 mxbt-0.3.5/mxbt.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-26 15:43:46.000000 mxbt-0.3.5/mxbt.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       80 2024-04-26 15:43:46.000000 mxbt-0.3.5/mxbt.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        5 2024-04-26 15:43:46.000000 mxbt-0.3.5/mxbt.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-26 15:43:47.046463 mxbt-0.3.5/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1032 2024-04-26 15:33:21.000000 mxbt-0.3.5/setup.py
```

### Comparing `mxbt-0.3.4.1/LICENSE` & `mxbt-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.4.1/PKG-INFO` & `mxbt-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxbt
-Version: 0.3.4.1
+Version: 0.3.5
 Summary: Yet another Matrix bot library.
 Home-page: https://codeberg.org/librehub/mxbt
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,matrix-nio,matrix,bot,api
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -59,27 +59,30 @@
 ```
 
 ## Getting started
 
 More examples [here](examples/) or in [docs](https://librehub.codeberg.page/mxbt/).
 
 ```python
-from mxbt import Bot, Context, Creds, Filter
+from mxbt import Bot, Context, Creds, Filter, Listener
+import asyncio
 
 bot = Bot(
     prefix="!",          # Standart command prefix, commands can setup it own prefix
     creds=Creds.from_json_file("credits.json")
 )
+lr = Listener(bot)
 
-@bot.on_command(prefix="?", aliases=["test", "t"])
+@lr.on_command(prefix="?", aliases=["test", "t"])
 @Filter.from_users(['@username:homeserver'])    # Event works only with this senders
 async def ctx_echo(ctx: Context) -> None:       # Context object contains main info about event
     await ctx.reply(ctx.body)                   # Reply message to event room
 
-bot.run()
+if __name__ == "__main__":
+    asyncio.run(lr.start_polling())
 ```
 
 **credits.json** structure
 ```json
 {
     "homeserver" : "https://matrix.org",
     "user_id" : "user",
```

### Comparing `mxbt-0.3.4.1/README.md` & `mxbt-0.3.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -36,27 +36,30 @@
 ```
 
 ## Getting started
 
 More examples [here](examples/) or in [docs](https://librehub.codeberg.page/mxbt/).
 
 ```python
-from mxbt import Bot, Context, Creds, Filter
+from mxbt import Bot, Context, Creds, Filter, Listener
+import asyncio
 
 bot = Bot(
     prefix="!",          # Standart command prefix, commands can setup it own prefix
     creds=Creds.from_json_file("credits.json")
 )
+lr = Listener(bot)
 
-@bot.on_command(prefix="?", aliases=["test", "t"])
+@lr.on_command(prefix="?", aliases=["test", "t"])
 @Filter.from_users(['@username:homeserver'])    # Event works only with this senders
 async def ctx_echo(ctx: Context) -> None:       # Context object contains main info about event
     await ctx.reply(ctx.body)                   # Reply message to event room
 
-bot.run()
+if __name__ == "__main__":
+    asyncio.run(lr.start_polling())
 ```
 
 **credits.json** structure
 ```json
 {
     "homeserver" : "https://matrix.org",
     "user_id" : "user",
```

### Comparing `mxbt-0.3.4.1/mxbt/api.py` & `mxbt-0.3.5/mxbt/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,98 @@
-from nio import AsyncClient, Event, MatrixRoom, OlmUnverifiedDeviceError, AsyncClientConfig, RoomGetEventResponse, RoomMessageFile, RoomMessageImage, RoomMessageText, RoomMessageVideo, RoomSendResponse
+from nio import (AsyncClient, Event, MatrixRoom,
+                 OlmUnverifiedDeviceError,
+                 AsyncClientConfig,
+                 RoomGetEventResponse,
+                 RoomMessageFile, RoomMessageImage,
+                 RoomMessageText, RoomMessageVideo,
+                 RoomSendResponse, SyncResponse)
 from nio.crypto import ENCRYPTION_ENABLED
 from typing import List, Union, Tuple 
+import cryptography
 import markdown
 import aiohttp
 import json
 import nio
-import os
 import re
+import os
 
 from .types.file import File, FileUrl
+from .callbacks import Callbacks
 from .utils import info, error
 
 def split_mxid(mxid: str) -> Union[Tuple[str, str], Tuple[None, None]]:
     # s = mxid.split(':')
     # if len(s) != 2 or s[0][0] != '@':
     #     return None, None
     # s[0] = s[0][1:]
     match = re.match(
         r'@(?P<localpart>[^:]*):(?P<hostname>(?P<ipv4>\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})|(?P<ipv6>\[[\da-fA-F:.]{2,45}\])|(?P<dns>[a-zA-Z\d\-.]{1,255}))(?P<port>:\d{1,5})?',
         mxid)
     if match is None:
         return None, None
     return match.group('localpart'), match.group('hostname')
 
+class Bot:
 
-class Api:
-
-    def __init__(self, creds) -> None:
-        self.creds = creds
-        self.async_client: AsyncClient | None = None
+    def __init__(self, creds, prefix: str="!", selfbot: bool=False, config: dict=dict()) -> None:
+        self.prefix = prefix
+        self.selfbot = selfbot
+        self.creds = creds 
+        self.config = config
         self.user_emotes = dict()
         self.room_emotes = dict()
 
+        self.async_client: AsyncClient | None = None
+        self.callbacks: Callbacks | None = None
+
+    async def connect(self, listener) -> None:
+        """
+        Main method of mxbt.Bot. Implements bot login and forever sync.
+
+        Can be runed with mxbt.Bot.run method or with asyncio.run(bot.connect())
+
+        Implementation from:
+        https://codeberg.org/imbev/simplematrixbotlib/src/branch/master/simplematrixbotlib/bot.py
+        """
+        try:
+            self.creds.session_read_file()
+        except cryptography.fernet.InvalidToken:
+            print("Invalid Stored Token")
+            print("Regenerating token from provided credentials")
+            os.remove(self.creds._session_stored_file)
+            self.creds.session_read_file()
+
+        await self.login()
+
+        if self.async_client is None: 
+            raise Exception("AsyncClient is None!")
+
+        resp = await self.async_client.sync(full_state=True)  #Ignore prior messages
+
+        if isinstance(resp, SyncResponse):
+            info(
+                f"Connected to {self.async_client.homeserver} as {self.async_client.user_id} ({self.async_client.device_id})"
+            )
+            if ENCRYPTION_ENABLED:
+                if self.async_client.olm is None:
+                    raise Exception("AsyncClient doesn't have olm module")
+                key = self.async_client.olm.account.identity_keys['ed25519']
+                info(
+                    f"This bot's public fingerprint (\"Session key\") for one-sided verification is: "
+                    f"{' '.join([key[i:i+4] for i in range(0, len(key), 4)])}")
+
+        self.creds.session_write_file()
+
+        self.callbacks = Callbacks(self.async_client, self, listener)
+        await self.callbacks.setup()
+        await listener.startup()
+
+        await self.async_client.sync_forever(timeout=3000, full_state=True)
+
+
     def get_user_emote(self, name: str) -> str | None:
         if (not 'images' in self.user_emotes.keys()
             or
             not name in self.user_emotes['images'].keys()):
             return None
         return self.user_emotes['images'][name]['url']
 
@@ -466,15 +523,16 @@
         content = self._add_relations(
             content, reply_to, edit_id
         )
 
         content = self._add_mentions(
             content, mentions
         )
-        content['formatted_body'] = self._add_emotes(str(content['body']), emotes)
+
+        content['formatted_body'] = self._add_emotes(str(content['formatted_body']), emotes)
     
         result = await self._send_room(room_id=room_id, content=content)
         room = self.async_client.rooms[room_id]
         if isinstance(result, RoomMessageText):
             return room, result
 
     async def send_reaction(self, room_id: str, event_id: str, key: str) -> Event | None:
@@ -512,8 +570,10 @@
             res = await self._send_room(room_id, content)
             room = self.async_client.rooms[room_id]
             if isinstance(res, (RoomMessageImage, RoomMessageVideo, RoomMessageFile)):
                 return room, res
         except:
             error("Failed to send file.")
 
- 
+
+
+
```

### Comparing `mxbt-0.3.4.1/mxbt/auth.py` & `mxbt-0.3.5/mxbt/auth.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.4.1/mxbt/bot.py` & `mxbt-0.3.5/mxbt/context.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,198 +1,262 @@
-from nio import SyncResponse, AsyncClient
-from inspect import isclass
-import cryptography
-import importlib
-import asyncio
-import os
-
-from nio.crypto import ENCRYPTION_ENABLED
-
-from .callbacks import Callbacks
-from .listener import Listener
-from .module import Module
-from .api import Api
-
-from .utils import info
-
-class Bot:
-
-    def __init__(self, creds, prefix: str="!", selfbot: bool=False, config: dict=dict()) -> None:
-        self.prefix = prefix
-        self.selfbot = selfbot
-        self.creds = creds 
-        self.config = config
-
-        self.api = Api(self.creds)
-        self.listener = Listener(self)
-        self.async_client: AsyncClient | None = None
-        self.callbacks: Callbacks | None = None
-
-    def mount_module(self, module: str) -> None:
-        """
-        Mount module by module name (without .py):
-            {modules_dir}.{filename}
-        Example:
-            modules.help
-        """
-        mod_file = importlib.import_module(module)
-        for it in dir(mod_file):
-            obj = getattr(mod_file, it)
-            if isclass(obj) and issubclass(obj, Module) and obj != Module:
-                info(f"Setup {obj.__name__} module")
-                obj(self)
-
-    def mount_modules(self, dirpath: str) -> None:
+from nio import MatrixRoom, Event, RoomMessageAudio, RoomMessageEmote, RoomMessageFile, RoomMessageFormatted, RoomMessageImage, RoomMessageNotice, RoomMessageText, RoomMessageVideo
+from dataclasses import dataclass, field
+from typing import Dict, List
+
+from .types.command import Command
+from .types.file import File
+from .bot import Bot
+
+@dataclass
+class Context:
+    """
+    Event context class
+
+    Parameters:
+    -------------
+    bot: mxbt.Bot
+        Bot object for sending events
+    room: nio.MatrixRoom
+        Event room object
+    event: nio.Event
+        Event object
+    sender: str
+        User id of event author
+    event_id: str
+        Id of received event
+    body: str
+        Body of received event
+    command: mxbt.Command, optional
+        Command object with args, prefix and aliases
+    mentions: list[str], optional
+        List of all mentioned users in event
+    info: dict, optional
+        Dict with media file info
+    """
+    bot: Bot 
+    room: MatrixRoom
+    room_id: str
+    event: Event
+    sender: str
+    event_id: str
+    body: str=str()
+    command: Command | None=None
+    mentions: List[str]=field(
+        default_factory=lambda: list()
+    )
+
+    # Media file info
+    info: Dict=field(
+        default_factory=lambda: dict()
+    )
+
+    async def _pack_result(self, result):
+        if result is None: return None 
+        room_id, event = result
+
+        if isinstance(event, RoomMessageText):
+            return Context.from_text(self.bot, room_id, event)
+        else:
+            return Context.from_media(self.bot, room_id, event)
+
+    async def send(self, body: str | File,
+                   use_html: bool=False,
+                   mentions: list[str]=list(),
+                   emotes: list[str]=list()):
         """
-        Mount all modules in dir
+        Send text or file to context room
 
         Parameters:
         -------------
-        dirpath: str - Path to modules directory.
+        body: str | mxbt.types.File
+            Text of message or File object to send
+        use_html: bool, optional
+            Use html formatting or not
+        """
+        result = await self.bot.send(
+            self.room_id,
+            body,
+            use_html,
+            mentions,
+            emotes
+        )
+        return await self._pack_result(result)
+
+    async def reply(self, body: str | File,
+                    use_html: bool=False,
+                    mentions: list[str]=list(),
+                    emotes: list[str]=list()):
         """
-        dirname = os.path.basename(dirpath)
-        for filename in os.listdir(dirpath):
-            if filename.endswith(".py"):
-                self.mount_module(f"{dirname}.{filename[:-3]}")
-
-    def on_custom_event(self, event):
-        def wrapper(func) -> None:
-            @self.listener.on_custom_event(event)
-            async def on_custom_event(*args) -> None:
-                await func(*args)
-            return on_custom_event
-        return wrapper
+        Reply context message with text or file
 
-    def on_member_join(self):
-        """
-        on_member_join event listener
-
-        func params:
-        --------------
-        room: MatrixRoom
-        event: InviteMemberEvent
-        """
-        def wrapper(func) -> None:
-            self.listener.on_member_join(func)
-        return wrapper
-
-    def on_member_leave(self):
+        Parameters:
+        -------------
+        body: str | mxbt.types.File
+            Text of message or File object to send
+        use_html: bool, optional
+            Use html formatting or not
+        """
+        result = await self.bot.reply(
+            self.room_id,
+            body,
+            self.event_id,
+            use_html,
+            mentions,
+            emotes
+        )
+        return await self._pack_result(result) 
+
+    async def edit(self, body: str | File,
+                   use_html: bool=False,
+                   mentions: list[str]=list(),
+                   emotes: list[str]=list()):
         """
-        on_member_leave event listener
+        Edit context message with text or file
 
-        func params:
-        --------------
-        room: MatrixRoom
-        event: InviteMemberEvent
-        """
-        def wrapper(func) -> None:
-            self.listener.on_member_leave(func)
-        return wrapper
+        Parameters:
+        -------------
+        body: str | mxbt.types.File
+            Text of message or File object to send
+        use_html: bool, optional
+            Use html formatting or not
+        """
+        result = await self.bot.edit(
+            self.room_id,
+            body,
+            self.event_id,
+            use_html,
+            mentions,
+            emotes
+        )
+        return await self._pack_result(result)
 
-    def on_command(self, **kwargs):
+    async def delete(self, reason: str | None=None):
         """
-        Custom on_command event listener
-
-        listener params:
-        ------------------
-        aliases: list[str] - list of command aliases
-        prefix: str, optional - custom command prefix (empty - use standart bot prefix)
+        Delete context event
 
-        func params:
-        ------------------
-        ctx: mxbt.Context
+        Parameters:
+        -------------
+        reason: str | None - optional
+            Reason, why message is deleted
         """
-        def wrapper(func):
-            @self.listener.on_command(**kwargs)
-            async def command_func(*args) -> None:
-                await func(*args)
-            return command_func
-        return wrapper
-
-    def on_message_text(self):
+        return await self.bot.delete(
+            self.room.room_id,
+            self.event.event_id,
+            reason
+        )
+    
+    async def react(self, body: str):
         """
-        On text message event listener
+        Send reaction to context message.
 
-        func params:
+        Parameters:
         --------------
-        room: MatrixRoom
-        event: RoomMessageText
-        """
-        def wrapper(func) -> None:
-            self.listener.on_message_text(func)
-        return wrapper
-
-    def on_message(self):
+        body : str
+            Reaction emoji.
         """
-        On any message event listener
+        return await self.bot.send_reaction(
+            self.room.room_id,
+            self.event.event_id,
+            body
+        )
 
-        func params:
-        --------------
-        room: MatrixRoom
-        event: RoomMessage
+    async def ban(self, reason: str | None=None):
         """
-        def wrapper(func) -> None:
-            self.listener.on_message(func)
-        return wrapper
+        Ban sender of this event
 
-    def on_reaction(self):
-        """
-        On reaction event listener
+        Parameters:
+        -------------
+        reason: str | None - optional
+            Reason, why sender is banned
         """
-        def wrapper(func) -> None:
-           self.listener.on_reaction(func) 
-        return wrapper
+        return await self.bot.ban(
+            self.room.room_id,
+            self.sender,
+            reason
+        )
 
-    async def connect(self) -> None:
+    async def kick(self, reason: str | None=None):
         """
-        Main method of mxbt.Bot. Implements bot login and forever sync.
-
-        Can be runed with mxbt.Bot.run method or with asyncio.run(bot.connect())
+        Kick sender of this event
 
-        Implementation from:
-        https://codeberg.org/imbev/simplematrixbotlib/src/branch/master/simplematrixbotlib/bot.py
+        Parameters:
+        -------------
+        reason: str | None - optional
+            Reason, why sender is kicked
         """
-        try:
-            self.creds.session_read_file()
-        except cryptography.fernet.InvalidToken:
-            print("Invalid Stored Token")
-            print("Regenerating token from provided credentials")
-            os.remove(self.creds._session_stored_file)
-            self.creds.session_read_file()
-
-        await self.api.login()
-
-        self.async_client = self.api.async_client
-        if self.async_client is None: 
-            raise Exception("AsyncClient is None!")
-
-        resp = await self.async_client.sync(full_state=True)  #Ignore prior messages
-
-        if isinstance(resp, SyncResponse):
-            info(
-                f"Connected to {self.async_client.homeserver} as {self.async_client.user_id} ({self.async_client.device_id})"
-            )
-            if ENCRYPTION_ENABLED:
-                if self.async_client.olm is None:
-                    raise Exception("AsyncClient doesn't have olm module")
-                key = self.async_client.olm.account.identity_keys['ed25519']
-                info(
-                    f"This bot's public fingerprint (\"Session key\") for one-sided verification is: "
-                    f"{' '.join([key[i:i+4] for i in range(0, len(key), 4)])}")
-
-        self.creds.session_write_file()
+        return await self.bot.kick(
+            self.room.room_id,
+            self.sender,
+            reason
+        )
+
+    @staticmethod
+    def __parse_command(message: RoomMessageText, prefix: str, aliases: list) -> Command:
+        command = Command(prefix, aliases)
+        args = message.body.split(" ")
+        if len(args) > 1:
+            args = args[1:]
+        else:
+            args = list()
+        command.args = args
+        command.substring = ' '.join(args)
+        return command
+
+    @staticmethod
+    def __parse_mentions(message: RoomMessageText | RoomMessageNotice | RoomMessageEmote | RoomMessageFormatted) -> list:
+        mentions = list()
+        content = message.source['content']
+        if 'm.mentions' in content.keys():
+            if 'user_ids' in content['m.mentions'].keys():
+                mentions = content['m.mentions']['user_ids']
+        return mentions
+
+    @staticmethod
+    def from_command(bot: Bot, room: MatrixRoom, message: RoomMessageText, prefix: str, aliases: list):
+        command = Context.__parse_command(message, prefix, aliases)
+        mentions = Context.__parse_mentions(message)
+        return Context(
+            bot=bot,
+            room=room, 
+            room_id=room.room_id,
+            event=message,
+            sender=message.sender,
+            event_id=message.event_id,
+            body=message.body,
+            command=command,
+            mentions=mentions
+        )
+
+    @classmethod
+    def from_text(cls, bot: Bot, room: MatrixRoom, message: RoomMessageText | RoomMessageNotice | RoomMessageEmote | RoomMessageFormatted):
+        mentions = cls.__parse_mentions(message)
+        return cls(
+            bot=bot,
+            room=room,
+            room_id=room.room_id,
+            event=message,
+            sender=message.sender,
+            event_id=message.event_id,
+            body=message.body,
+            mentions=mentions
+        )
+
+    @classmethod
+    def from_media(cls, bot: Bot,
+                   room: MatrixRoom,
+                   message: RoomMessageImage | RoomMessageVideo | RoomMessageFile | RoomMessageAudio):
+        source = message.source
+        info = source['content']['info']
+        if 'external_url' in source.keys():
+            info['external_url'] = source['external_url']
+        return cls(
+            bot=bot,
+            room=room,
+            room_id=room.room_id,
+            event=message,
+            sender=message.sender,
+            event_id=message.event_id,
+            body=message.body,
+            info=info
+        )
 
-        self.callbacks = Callbacks(self.async_client, self)
-        await self.callbacks.setup()
-
-        for action in self.listener._startup_registry:
-            for room_id in self.async_client.rooms:
-                await action(room_id)
-
-        await self.async_client.sync_forever(timeout=3000, full_state=True)
-
-    def run(self) -> None:
-        """
-        Run mxbt.Bot.connect method with asyncio.run
-        """
-        asyncio.run(self.connect())
```

### Comparing `mxbt-0.3.4.1/mxbt/callbacks.py` & `mxbt-0.3.5/mxbt/callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 from .utils import info, error
 
 class Callbacks:
     """
     A class for handling callbacks.
     """
 
-    def __init__(self, async_client, bot) -> None:
+    def __init__(self, async_client, bot, listener) -> None:
         self.async_client = async_client
         self.bot = bot
+        self.listener = listener
 
     async def setup(self) -> None:
         """
         Add callbacks to async_client
         """
         self.async_client.add_event_callback(self.invite_callback,
                                                  InviteMemberEvent)
         self.async_client.add_global_account_data_callback(
             self.custom_emotes_callback, AccountDataEvent
         )
 
-        for event_listener in self.bot.listener._registry:
+        for event_listener in self.listener._registry:
             if issubclass(event_listener[1],
                           nio.events.to_device.ToDeviceEvent):
                 self.async_client.add_to_device_callback(
                     event_listener[0], event_listener[1])
             else:
                 self.async_client.add_event_callback(event_listener[0],
                                                      event_listener[1])
@@ -41,25 +42,25 @@
             - im.ponies.emote_rooms: Custom emojis from a bot rooms
                 We need to receive room_get_state event with 'im.ponies.room_emotes' event type
                 and emoji pack name as state_key
                 Then emojis dict from this room will be saved to Api.room_emotes[room_id][pack_name]
         """
         if hasattr(event, 'type'):
             if event.type == 'im.ponies.user_emotes':
-                if self.bot.api.user_emotes != event.content:
-                    self.bot.api.user_emotes = event.content
+                if self.bot.user_emotes != event.content:
+                    self.bot.user_emotes = event.content
             elif event.type == 'im.ponies.emote_rooms':
                 for room_id, packs in event.content['rooms'].items():
-                    self.bot.api.room_emotes[room_id] = dict()
+                    self.bot.room_emotes[room_id] = dict()
                     for pack in packs.keys():
                         result = await self.async_client.room_get_state_event(
                             room_id, 'im.ponies.room_emotes', pack
                         )
                         emojis = result.content
-                        self.bot.api.room_emotes[room_id][pack] = emojis
+                        self.bot.room_emotes[room_id][pack] = emojis
 
     async def invite_callback(self, room, event, tries=1) -> None:
         """
         Callback for handling invites.
 
         Parameters
         ----------
```

### Comparing `mxbt-0.3.4.1/mxbt/filters.py` & `mxbt-0.3.5/mxbt/filters.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.4.1/mxbt/match.py` & `mxbt-0.3.5/mxbt/match.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.4.1/mxbt/module.py` & `mxbt-0.3.5/mxbt/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,39 +44,41 @@
     def wrapper(func):
         func.__event__ = kwargs
         return func
     return wrapper
 
 class Module:
 
-    def __init__(self, bot) -> None:
+    def __init__(self, bot, listener) -> None:
         self.bot = bot
+        self.listener = listener
         self.__setup__()
 
     def add_command(self, method) -> None:
         kwargs = method.__command__
-        @self.bot.listener.on_command(**kwargs)
+
+        @self.listener.on_command(**kwargs)
         async def _(ctx) -> None:
             await method(ctx)
 
     def add_event(self, method) -> None:
         event_type = method.__event__['event_type']
         methods = {
-            Event.onMessage : self.bot.listener.on_message,
-            Event.onMemberJoin : self.bot.listener.on_member_join,
-            Event.onMemberLeave : self.bot.listener.on_member_leave,
-            Event.onReaction : self.bot.listener.on_reaction,
-            Event.onStartup : self.bot.listener.on_startup,
+            Event.onMessage : self.listener.on_message,
+            Event.onMemberJoin : self.listener.on_member_join,
+            Event.onMemberLeave : self.listener.on_member_leave,
+            Event.onReaction : self.listener.on_reaction,
+            Event.onStartup : self.listener.on_startup,
         }
         if event_type in methods.keys():
             methods[event_type](method)
         elif event_type == Event.onCustomEvent:
             event = method.__event__['event']
 
-            @self.bot.listener.on_custom_event(event)
+            @self.listener.on_custom_event(event)
             async def _(*args) -> None:
                 await method(*args)
 
     def __setup__(self) -> None:
         methods = inspect.getmembers(self, predicate=inspect.ismethod)
         for method_tuple in methods:
             method = method_tuple[1]
```

### Comparing `mxbt-0.3.4.1/mxbt/types/file.py` & `mxbt-0.3.5/mxbt/types/file.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.4.1/mxbt.egg-info/PKG-INFO` & `mxbt-0.3.5/mxbt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxbt
-Version: 0.3.4.1
+Version: 0.3.5
 Summary: Yet another Matrix bot library.
 Home-page: https://codeberg.org/librehub/mxbt
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,matrix-nio,matrix,bot,api
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -59,27 +59,30 @@
 ```
 
 ## Getting started
 
 More examples [here](examples/) or in [docs](https://librehub.codeberg.page/mxbt/).
 
 ```python
-from mxbt import Bot, Context, Creds, Filter
+from mxbt import Bot, Context, Creds, Filter, Listener
+import asyncio
 
 bot = Bot(
     prefix="!",          # Standart command prefix, commands can setup it own prefix
     creds=Creds.from_json_file("credits.json")
 )
+lr = Listener(bot)
 
-@bot.on_command(prefix="?", aliases=["test", "t"])
+@lr.on_command(prefix="?", aliases=["test", "t"])
 @Filter.from_users(['@username:homeserver'])    # Event works only with this senders
 async def ctx_echo(ctx: Context) -> None:       # Context object contains main info about event
     await ctx.reply(ctx.body)                   # Reply message to event room
 
-bot.run()
+if __name__ == "__main__":
+    asyncio.run(lr.start_polling())
 ```
 
 **credits.json** structure
 ```json
 {
     "homeserver" : "https://matrix.org",
     "user_id" : "user",
```

### Comparing `mxbt-0.3.4.1/setup.py` & `mxbt-0.3.5/setup.py`

 * *Files identical despite different names*

