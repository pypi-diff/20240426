# Comparing `tmp/discord_limits-1.1.2.tar.gz` & `tmp/discord_limits-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_limits-1.1.2.tar", last modified: Mon May 30 18:57:08 2022, max compression
+gzip compressed data, was "discord_limits-2.0.1.tar", last modified: Fri Apr 26 03:48:48 2024, max compression
```

## Comparing `discord_limits-1.1.2.tar` & `discord_limits-2.0.1.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-05-30 18:57:08.355331 discord_limits-1.1.2/
--rw-rw-rw-   0        0        0     1088 2022-05-06 09:44:00.000000 discord_limits-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     1418 2022-05-30 18:57:08.354830 discord_limits-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2022-05-30 18:56:37.000000 discord_limits-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2022-05-30 18:57:08.338316 discord_limits-1.1.2/discord_limits/
--rw-rw-rw-   0        0        0       30 2022-05-24 12:38:22.000000 discord_limits-1.1.2/discord_limits/__init__.py
--rw-rw-rw-   0        0        0     6455 2022-05-30 18:56:13.000000 discord_limits-1.1.2/discord_limits/api.py
--rw-rw-rw-   0        0        0     1348 2022-05-23 18:12:56.000000 discord_limits-1.1.2/discord_limits/embed.py
--rw-rw-rw-   0        0        0      429 2022-05-23 18:12:56.000000 discord_limits-1.1.2/discord_limits/emoji.py
--rw-rw-rw-   0        0        0      682 2022-05-23 18:12:56.000000 discord_limits-1.1.2/discord_limits/errors.py
--rw-rw-rw-   0        0        0      813 2022-05-23 18:12:56.000000 discord_limits-1.1.2/discord_limits/member.py
--rw-rw-rw-   0        0        0     1373 2022-05-23 18:12:56.000000 discord_limits-1.1.2/discord_limits/message.py
--rw-rw-rw-   0        0        0   134776 2022-05-26 22:45:11.000000 discord_limits-1.1.2/discord_limits/paths.py
--rw-rw-rw-   0        0        0     2944 2022-05-30 17:13:55.000000 discord_limits-1.1.2/discord_limits/rate_limits.py
--rw-rw-rw-   0        0        0     1479 2022-05-23 18:12:56.000000 discord_limits-1.1.2/discord_limits/reactions.py
--rw-rw-rw-   0        0        0      647 2022-05-23 18:12:56.000000 discord_limits-1.1.2/discord_limits/route.py
--rw-rw-rw-   0        0        0     1047 2022-05-23 18:12:56.000000 discord_limits-1.1.2/discord_limits/thread.py
--rw-rw-rw-   0        0        0     1148 2022-05-23 18:12:56.000000 discord_limits-1.1.2/discord_limits/user.py
-drwxrwxrwx   0        0        0        0 2022-05-30 18:57:08.352829 discord_limits-1.1.2/discord_limits.egg-info/
--rw-rw-rw-   0        0        0     1418 2022-05-30 18:57:08.000000 discord_limits-1.1.2/discord_limits.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2022-05-30 18:57:08.000000 discord_limits-1.1.2/discord_limits.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-30 18:57:08.000000 discord_limits-1.1.2/discord_limits.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2022-05-30 18:57:08.000000 discord_limits-1.1.2/discord_limits.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-05-30 18:57:08.000000 discord_limits-1.1.2/discord_limits.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       89 2022-05-16 23:25:33.000000 discord_limits-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-05-30 18:57:08.355331 discord_limits-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      646 2022-05-30 18:56:27.000000 discord_limits-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:48:48.255498 discord_limits-2.0.1/
+-rw-rw-rw-   0        0        0     1088 2022-05-06 09:44:00.000000 discord_limits-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1143 2024-04-26 03:48:48.254998 discord_limits-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      819 2024-04-26 03:48:19.000000 discord_limits-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 03:48:48.224114 discord_limits-2.0.1/discord_limits/
+-rw-rw-rw-   0        0        0      191 2024-04-26 03:20:44.000000 discord_limits-2.0.1/discord_limits/__init__.py
+-rw-rw-rw-   0        0        0     9822 2024-04-26 03:42:18.000000 discord_limits-2.0.1/discord_limits/client.py
+-rw-rw-rw-   0        0        0      863 2024-04-26 02:09:02.000000 discord_limits-2.0.1/discord_limits/errors.py
+-rw-rw-rw-   0        0        0     1283 2024-04-26 03:33:26.000000 discord_limits-2.0.1/discord_limits/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:48:48.253996 discord_limits-2.0.1/discord_limits/paths/
+-rw-rw-rw-   0        0        0      499 2024-04-10 17:52:46.000000 discord_limits-2.0.1/discord_limits/paths/__init__.py
+-rw-rw-rw-   0        0        0    10829 2024-04-26 00:13:39.000000 discord_limits-2.0.1/discord_limits/paths/applicationPaths.py
+-rw-rw-rw-   0        0        0     1735 2024-04-25 13:16:04.000000 discord_limits-2.0.1/discord_limits/paths/auditPaths.py
+-rw-rw-rw-   0        0        0     3884 2024-04-25 13:16:29.000000 discord_limits-2.0.1/discord_limits/paths/autoModerationPaths.py
+-rw-rw-rw-   0        0        0    38908 2024-04-26 00:13:31.000000 discord_limits-2.0.1/discord_limits/paths/channelPaths.py
+-rw-rw-rw-   0        0        0     3856 2024-04-26 02:49:01.000000 discord_limits-2.0.1/discord_limits/paths/emojiPaths.py
+-rw-rw-rw-   0        0        0    54345 2024-04-25 13:52:49.000000 discord_limits-2.0.1/discord_limits/paths/guildPaths.py
+-rw-rw-rw-   0        0        0     9702 2024-04-25 14:47:20.000000 discord_limits-2.0.1/discord_limits/paths/interationsPaths.py
+-rw-rw-rw-   0        0        0     2318 2024-04-25 14:43:34.000000 discord_limits-2.0.1/discord_limits/paths/invitePaths.py
+-rw-rw-rw-   0        0        0     5059 2024-04-25 14:45:12.000000 discord_limits-2.0.1/discord_limits/paths/paths.py
+-rw-rw-rw-   0        0        0     3457 2024-04-25 14:47:56.000000 discord_limits-2.0.1/discord_limits/paths/stagePaths.py
+-rw-rw-rw-   0        0        0     4512 2024-04-25 14:51:36.000000 discord_limits-2.0.1/discord_limits/paths/stickerPaths.py
+-rw-rw-rw-   0        0        0     5247 2024-04-26 00:13:14.000000 discord_limits-2.0.1/discord_limits/paths/userPaths.py
+-rw-rw-rw-   0        0        0    13305 2024-04-26 00:13:01.000000 discord_limits-2.0.1/discord_limits/paths/webhookPaths.py
+-rw-rw-rw-   0        0        0     1817 2024-04-26 02:36:27.000000 discord_limits-2.0.1/discord_limits/rate_limits.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:48:48.238643 discord_limits-2.0.1/discord_limits.egg-info/
+-rw-rw-rw-   0        0        0     1143 2024-04-26 03:48:48.000000 discord_limits-2.0.1/discord_limits.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      873 2024-04-26 03:48:48.000000 discord_limits-2.0.1/discord_limits.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 03:48:48.000000 discord_limits-2.0.1/discord_limits.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-26 03:48:48.000000 discord_limits-2.0.1/discord_limits.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-26 03:48:48.000000 discord_limits-2.0.1/discord_limits.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       89 2024-04-26 03:43:46.000000 discord_limits-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 03:48:48.255998 discord_limits-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      699 2024-04-26 03:28:12.000000 discord_limits-2.0.1/setup.py
```

### Comparing `discord_limits-1.1.2/LICENSE` & `discord_limits-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord_limits-1.1.2/PKG-INFO` & `discord_limits-2.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,44 @@
 Metadata-Version: 2.1
 Name: discord_limits
-Version: 1.1.2
-Summary: Make requests API requests to Discord without having to worry about ratelimits.
+Version: 2.0.1
+Summary: Make Discord API calls without having to worry about ratelimits.
 Home-page: https://github.com/ninjafella/discord-API-limits
 Author: ninjafella
 License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Documentation Status](https://readthedocs.org/projects/discord-limits/badge/?version=latest)](https://discord-limits.readthedocs.io/en/latest/?badge=latest)
-[![Version](https://img.shields.io/badge/Version-v1.1.2-blue)](https://img.shields.io/badge/Version-v1.1.2-blue)
+[![Documentation Status]](https://discord-limits.readthedocs.io/en/latest/?badge=latest)
+[![Version](https://img.shields.io/badge/Version-v2.0.1-blue)](https://img.shields.io/badge/Version-v2.0.1-blue)
 
 # discord_limits
 
 ### A simple library to asynchronously make API requests to Discord without having to worry about ratelimits.
 
 <br>
 
-### Currently this library has only been tested on Python 3.9
-
 ---
 
 # Basic usage
 
 ```py
 import discord_limits
-import os
 import asyncio
 
-limitsClient = discord_limits.DiscordClient(os.environ.get('TOKEN'))
+limits_client = discord_limits.DiscordClient("YOUR_TOKEN", "bot")
 
 async def main():
-    await limitsClient.create_message(123456789012345678, content='Hello World!')
+    await limits_client.channel.create_message("CHANNEL_ID", "Hello World!")
 
+asyncio.run(main())
 
-asyncio.get_event_loop().run_until_complete(main())
 ```
 
 ---
 ### Requires:
 - [aiolimiter](https://pypi.org/project/aiolimiter/)
 - [aiohttp](https://pypi.org/project/aiohttp/)
 
----
-### Based off of:
-- [unbelipy](https://github.com/chrisdewa/unbelipy)
-- [discord.py](https://github.com/Rapptz/discord.py)
-
 
+[def]: https://readthedocs.org/projects/discord-limits/badge/?version=latest
```

### Comparing `discord_limits-1.1.2/README.md` & `discord_limits-2.0.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,33 @@
-[![Documentation Status](https://readthedocs.org/projects/discord-limits/badge/?version=latest)](https://discord-limits.readthedocs.io/en/latest/?badge=latest)
-[![Version](https://img.shields.io/badge/Version-v1.1.2-blue)](https://img.shields.io/badge/Version-v1.1.2-blue)
+[![Documentation Status]](https://discord-limits.readthedocs.io/en/latest/?badge=latest)
+[![Version](https://img.shields.io/badge/Version-v2.0.1-blue)](https://img.shields.io/badge/Version-v2.0.1-blue)
 
 # discord_limits
 
 ### A simple library to asynchronously make API requests to Discord without having to worry about ratelimits.
 
 <br>
 
-### Currently this library has only been tested on Python 3.9
-
 ---
 
 # Basic usage
 
 ```py
 import discord_limits
-import os
 import asyncio
 
-limitsClient = discord_limits.DiscordClient(os.environ.get('TOKEN'))
+limits_client = discord_limits.DiscordClient("YOUR_TOKEN", "bot")
 
 async def main():
-    await limitsClient.create_message(123456789012345678, content='Hello World!')
+    await limits_client.channel.create_message("CHANNEL_ID", "Hello World!")
 
+asyncio.run(main())
 
-asyncio.get_event_loop().run_until_complete(main())
 ```
 
 ---
 ### Requires:
 - [aiolimiter](https://pypi.org/project/aiolimiter/)
 - [aiohttp](https://pypi.org/project/aiohttp/)
 
----
-### Based off of:
-- [unbelipy](https://github.com/chrisdewa/unbelipy)
-- [discord.py](https://github.com/Rapptz/discord.py)
+
+[def]: https://readthedocs.org/projects/discord-limits/badge/?version=latest
```

### Comparing `discord_limits-1.1.2/discord_limits/api.py` & `discord_limits-2.0.1/discord_limits/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,260 @@
 import asyncio
-from aiohttp import ClientSession, ClientResponse
 import warnings
+import datetime
+from sys import version_info as python_version
 
+from aiohttp import ClientResponse, ClientSession
+from aiohttp import __version__ as aiohttp_version
+from aiolimiter import AsyncLimiter
+from requests import head
+
+from . import __version__
 from .errors import *
-from .rate_limits import BucketHandler, ClientRateLimits
 from .paths import Paths
+from .rate_limits import BucketHandler, ClientRateLimits
+
+from typing import Optional
+
 
 class DiscordClient(Paths):
     """
     Parameters
     ----------
     token : str
         The token to use for the request.
     token_type : str, optional
-        The type of token provided, by default 'bot'
-    prevent_rate_limits : bool, optional
-        Whether the client will sleep through ratelimits to prevent 429 errors, by default True
-    retry_rate_limits : bool, optional
-        Whether the client will sleep and retry after 429 errors, by default True
+        The type of token provided ('bot', 'bearer', 'user', None), by default 'bot'
     api_version : int, optional
-        The Discord API version to use, by default 9
+        The Discord API version to use (6, 7, 8, 9, 10), by default 10
+
+    Attributes
+    ----------
+    token : str
+        The token to use for the request.
+    token_type : str
+        The type of token provided. Can be 'bot', 'bearer' or 'user'.
+    api_version : int
+        The Discord API version to use. Default is 10.
+    suppress_warnings : bool
+        Whether to suppress warnings or not. Default is False.
+    max_attempts : int
+        The maximum number of attempts to make a request. Default is 3.
     """
 
-    def __init__(self, token: str, token_type: str = 'bot', prevent_rate_limits: bool = True, retry_rate_limits: bool = True, api_version: int = 9):
+    def __init__(
+        self,
+        token: Optional[str],
+        token_type: Optional[str] = "bot",
+        api_version: int = 10,
+        suppress_warnings: bool = False,
+        max_attempts: int = 3,
+    ):
         super().__init__(self)
-        if token_type == 'bot':
+
+        if api_version < 6:
+            raise InvalidParams("API version must be 6 or higher.")
+        elif api_version < 9 and not suppress_warnings:
+            warnings.warn(
+                f"API version {api_version} is now deprecated by Discord, some endpoints may not work as expected.",
+                UserWarning,
+            )
+
+        if token_type == "bot":
             self.token = f"Bot {token}"
             self.token_type = token_type
-        elif token_type == 'bearer':
+        elif token_type == "bearer":
             self.token = f"Bearer {token}"
             self.token_type = token_type
-        elif token_type == 'user':
-            warnings.warn("Use a user token at your own risk as (depending on your usage) it could be against Discord's ToS. If you are using this token for a bot, you should use the 'bot' token_type instead.", UserWarning)
+        elif token_type == "user":
+            if not suppress_warnings:
+                warnings.warn(
+                    "Use a user token at your own risk as (depending on your usage) it could be against Discord's ToS. If you are using this token for a bot, you should use the 'bot' token_type instead.",
+                    UserWarning,
+                )
             self.token = f"{token}"
             self.token_type = token_type
         else:
             self.token = None
             self.token_type = None
 
-        self._prevent_rate_limits = prevent_rate_limits
-        self._retry_rate_limits = retry_rate_limits
-        self.rate_limits = ClientRateLimits(prevent_rate_limits=prevent_rate_limits)
+        self.rate_limits = ClientRateLimits()
         self._base_url = f"https://discord.com/api/v{api_version}"
         self._base_url_len = len(self._base_url)
 
-    def _set_token(self, token: str, token_type: str = 'bot'):
-        if token_type == 'bot':
-            self.token = f"Bot {token}"
-        elif token_type == 'bearer':
-            self.token = f"Bearer {token}"
-        elif token_type == 'user':
-            warnings.warn("Use a user token at your own risk as (depending on your usage) it could be against Discord's ToS. If you are using this token for a bot, you should use the 'bot' token_type instead.", UserWarning)
-            self.token = f"{token}"
-        else:
-            self.token = None
+        self._user_agent: str = (
+            f"DiscordBot (https://github.com/ninjafella/discord-API-limits {__version__}) Python/{python_version[0]}.{python_version[1]}.{python_version[2]} aiohttp/{aiohttp_version}"
+        )
 
-    def _get_bucket_handler(self, bucket: str):
-        bucket_handler = self.rate_limits.buckets.get(bucket)
-        if bucket_handler is None:
-            bucket_handler = self.rate_limits.buckets[bucket] = BucketHandler(bucket=bucket)
-        return bucket_handler
+        self.global_limiter = AsyncLimiter(50, 1)
+
+        self.suppress_warnings = suppress_warnings  #: bool: Whether to suppress warnings or not. Default is False.
+        self.max_attempts = max_attempts  #: int: The maximum number of attempts to make a request. Default is 3.
+
+    def _create_bucket_handler(self, r: ClientResponse, bucket_path: str):
+        status = r.status
+
+        if status == 400:
+            raise BadRequest
+        elif status == 401:
+            raise Unauthorized
+        elif status == 403:
+            raise Forbidden
+        elif status == 404:
+            raise NotFound
+        elif status == 500:
+            raise InternalServerError
+
+        if self.rate_limits.buckets.get(r.headers["X-RateLimit-Bucket"]) is not None:
+            bucket_hash = r.headers["X-RateLimit-Bucket"]
+            self.rate_limits.bucket_relations[bucket_path] = bucket_hash
+            self._check_response(r, self.rate_limits.buckets[bucket_hash])
+        else:
+            bh = BucketHandler()
+            self._check_response(r, bh)
+            self.rate_limits.buckets[bh.bucket_hash] = bh
+            self.rate_limits.bucket_relations[bucket_path] = bh.bucket_hash
+
+    async def _request(
+        self,
+        method: str,
+        path: str,
+        headers: dict = {},
+        json: Optional[dict] = None,
+        params: Optional[dict] = None,
+        auth: bool = True,
+        metadata: Optional[str] = None,
+        _attempts: int = 0,
+    ) -> ClientResponse:  # type: ignore
+
+        if _attempts >= self.max_attempts:
+            raise MaxAttemptsReached
+
+        headers["User-Agent"] = self._user_agent
+        headers["Accept"] = "application/json"
+        headers["Content-Type"] = "application/json"
 
-    async def _request(self, method: str, path: str, bucket: str, headers: dict = None, json: dict = None, params: dict = None, auth: bool = True):
         if auth:
             if self.token_type is None:
-                raise InvalidParams("No token has been set. Please set the auth parameter to False or set a token with _set_token().")
-            if headers is None:
-                headers = {'Authorization': self.token}
-            else:
-                headers['Authorization'] = self.token
+                raise InvalidParams(
+                    "No token has been set. Please set a token with set_new_token()."
+                )
+            headers["Authorization"] = self.token
         cs = ClientSession()
 
         url = self._base_url + path
 
-        request_manager = cs.request(method, url, json=json, params=params, headers=headers)
+        request_manager = cs.request(
+            method, url, json=json, params=params, headers=headers
+        )
+
+        if metadata is not None:
+            bucket_path = f"{method}:{path}:{metadata}"
+        bucket_path = f"{method}:{path}"
+
+        bucket_hash = self.rate_limits.bucket_relations.get(bucket_path)
+        if bucket_hash is not None:
+            bucket_handler = self.rate_limits.buckets[bucket_hash]
+
+            async with self.rate_limits.global_limiter:
+                async with bucket_handler:
+                    async with cs:
+                        response = await request_manager
+                        try:
+                            self._check_response(response, bucket_handler)
+                        except TooManyRequests:
+                            await self._request(
+                                method,
+                                path,
+                                headers=headers,
+                                json=json,
+                                params=params,
+                                auth=auth,
+                                metadata=metadata,
+                                _attempts=_attempts + 1,
+                            )
+                        except Exception as e:
+                            raise e
 
-        bucket_handler = self._get_bucket_handler(bucket)
-        bucket_handler.prevent_429 = self._prevent_rate_limits
-        async with self.rate_limits.global_limiter:
-            async with bucket_handler as bh:
+        else:
+            async with self.rate_limits.global_limiter:
                 async with cs:
-                    r = await request_manager
-                    bh.check_limit_headers(r)  # sets up the bucket rate limit attributes w/ response headers
-                try:
-                    if await self._check_response(response=r, bucket=bucket):
-                        return r
-                except TooManyRequests as e:
-                    if self._retry_rate_limits is True:
-                        response_data = await r.json()
-                        timeout = response_data['retry_after'] / 1000 + 1
-                        await asyncio.sleep(timeout)
-                        # reschedule same request
-                        return await self._request(method, path, bucket, headers=headers, json=json, params=params, auth=auth)
-                    else:
+                    response = await request_manager
+                    try:
+                        self._create_bucket_handler(response, bucket_path)
+                    except TooManyRequests:
+                        await self._request(
+                            method,
+                            path,
+                            headers=headers,
+                            json=json,
+                            params=params,
+                            auth=auth,
+                            metadata=metadata,
+                            _attempts=_attempts + 1,
+                        )
+                    except Exception as e:
                         raise e
-                except NotFound as e:
-                    raise e
-                except UnknownError as e:
-                    raise e
-
-    async def _check_response(self, response: ClientResponse, bucket: str):
-        """Checks API response for errors. Returns True only on 300 > status >= 200"""
-        status = response.status
-        reason = response.reason
-
-
-        if 300 > status >= 200:
-            return True
-        elif status == 429:
-            data = await response.json()
-            message = data['message']
-            if 'global' in data:
-                text = f"Global rate limit. {data['message']}"
-            elif retry_after == data.get('retry_after'):
-                retry_after = int(retry_after) / 1000
-                bucket_handler = self._get_bucket_handler(bucket)
-                bucket_handler.retry_after = retry_after
-                text = f"{message} retry after: {retry_after}s"
-            else:
-                text = f"{message}"
-            raise TooManyRequests(text + f', bucket: {bucket}')
-        elif status == 400:
-            raise BadRequest(f'Error Code: "{status}" Reason: "{reason}", bucket {bucket}')
+
+    def _check_response(self, r: ClientResponse, bh: BucketHandler):
+        headers = r.headers
+        status = r.status
+
+        if status == 400:
+            raise BadRequest
         elif status == 401:
-            raise Unauthorized(f'Error Code: "{status}" Reason: "{reason}", bucket {bucket}')
+            raise Unauthorized
         elif status == 403:
-            raise Forbidden(f'Error Code: "{status}" Reason: "{reason}", bucket {bucket}')
+            raise Forbidden
         elif status == 404:
-            raise NotFound(f'Error Code: "{status}" Reason: "{reason}", bucket {bucket}')
+            raise NotFound
         elif status == 500:
-            raise InternalServerError(f'Error Code: "{status}" Reason: "{reason}", bucket {bucket}')
+            raise InternalServerError
+
+        for header in headers:
+            if header == "X-RateLimit-Limit":
+                bh.limit = int(headers["X-RateLimit-Limit"])
+            elif header == "X-RateLimit-Remaining":
+                bh.remaining = int(headers["X-RateLimit-Remaining"])
+            elif header == "X-RateLimit-Reset":
+                bh.reset = datetime.datetime.fromtimestamp(
+                    float(headers["X-RateLimit-Reset"]), datetime.UTC
+                )
+            elif header == "X-RateLimit-Bucket" and header != bh.bucket_hash:
+                if bh.bucket_hash == "":
+                    bh.bucket_hash = headers["X-RateLimit-Bucket"]
+                old_hash = bh.bucket_hash
+                bh.bucket_hash = headers["X-RateLimit-Bucket"]
+                self.rate_limits.update_bucket_relations(old_hash, bh.bucket_hash)
+
+        if status == 429:
+            bh.retry_after = float(headers["X-RateLimit-Reset-After"])
+            asyncio.ensure_future(bh.trigger_lock())
+            raise TooManyRequests
+        elif not (300 > status >= 200):
+            raise UnknownError
+
+    def set_new_token(
+        self, token: Optional[str], token_type: Optional[str] = "bot"
+    ) -> None:
+        """Set a new token to use.
+
+        Parameters
+        ----------
+        token : str
+            The new token to use for the request.
+        token_type : str, optional
+            The type of token provided ('bot', 'bearer', 'user', None), by default 'bot'
+        """
+        if token_type == "bot":
+            self.token = f"Bot {token}"
+        elif token_type == "bearer":
+            self.token = f"Bearer {token}"
+        elif token_type == "user":
+            if not self.suppress_warnings:
+                warnings.warn(
+                    "Use a user token at your own risk as (depending on your usage) it could be against Discord's ToS. If you are using this token for a bot, you should use the 'bot' token_type instead.",
+                    UserWarning,
+                )
+            self.token = token
         else:
-            error_text = f'Error code: "{status}" Reason: "{reason}"'
-            if status in api_errors:
-                raise api_errors[status](error_text)
-            else:
-                raise UnknownError(error_text)
+            self.token = None
```

### Comparing `discord_limits-1.1.2/discord_limits/rate_limits.py` & `discord_limits-2.0.1/discord_limits/rate_limits.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,53 @@
 import asyncio
-from collections import defaultdict
-from datetime import datetime, timedelta
-from typing import Dict, List
+import datetime
+import stat
+from typing import Dict, Optional
 
 from aiohttp import ClientResponse
 from aiolimiter import AsyncLimiter
+from .errors import *
 
 
 class BucketHandler:
-    """
-    Handles bucket specific rate limits
-    flow:
-        dict {
-            bucket_name: BucketHandler
-        }
-    """
-    limit: int = None
-    remaining: int = None
-    reset: datetime = None
-    retry_after: float = None
-    cond = None
-    prevent_429 = False
-
-    def __init__(self, bucket: str):
-        self.bucket = bucket
-
-    def __repr__(self):
-        return (f"RateLimit(bucket={self.bucket}, limit={self.limit}, remaining={self.remaining}, "
-                f"reset={self.reset}, retry_after={self.retry_after})")
-
-    def check_limit_headers(self, r: ClientResponse):
-        limits = {}
-        header_attrs = {
-            'X-RateLimit-Limit': 'limit',
-            'X-RateLimit-Remaining': 'remaining',
-            'X-RateLimit-Reset': 'reset',
-        }
-        for key in header_attrs:
-            value = r.headers.get(key)
-            if value is not None:
-                if key == 'X-RateLimit-Reset':
-                    value = datetime.utcfromtimestamp(float(value))
-            limits[header_attrs[key]] = value
-        for k, v in limits.items():
-            setattr(self, k, v)
+    limit: Optional[int] = None  # The rate limit
+    remaining: Optional[int] = None  # Remaining requests
+    reset: Optional[datetime.datetime] = None  # When the rate limit resets
+    retry_after: Optional[float] = None  # How long to wait before retrying the request
+    bucket_hash: str = ""  # The bucket hash from Discord
+    lock: asyncio.Event = (
+        asyncio.Event()
+    )  # Used to lock the bucket if a rate limit is hit
+
+    def __init__(self):
+        self.lock.set()
+
+    async def trigger_lock(self):
+        self.lock.clear()
+        await asyncio.sleep(self.retry_after)  # type: ignore
+        self.lock.set()
 
     async def __aenter__(self):
-        self.cond = self.cond or asyncio.Condition(loop=asyncio.get_running_loop())
-        if self.prevent_429 is True:
-            await self.cond.acquire()
-            if self.remaining is not None and self.remaining == 0:
-                now = datetime.utcnow()
-                to_wait = (self.reset - now).total_seconds() + 1
-                await asyncio.sleep(to_wait)
+        await self.lock.wait()
+        if self.remaining is not None and self.remaining == 0:
+            now = datetime.datetime.now(datetime.UTC)
+            to_wait = (self.reset - now).total_seconds() + 1  # type: ignore
+            await asyncio.sleep(to_wait)
         return self
 
     async def __aexit__(self, *args):
-        if self.prevent_429 is True:
-            self.cond.release()
-
-
-class AsyncNonLimiter:
-    async def __aenter__(self):
-        pass
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
         pass
 
 
 class ClientRateLimits:
-    buckets: Dict[str, BucketHandler] = dict()
+    buckets: Dict[str, BucketHandler] = dict()  # {bucket_hash: BucketHandler}
+    bucket_relations: Dict[str, str] = dict()  # {path: bucket_hash}
 
-    def __init__(self, prevent_rate_limits: bool):
-        self.global_limiter = AsyncLimiter(50, 1) if prevent_rate_limits is True else AsyncNonLimiter()
+    def __init__(self):
+        self.global_limiter = AsyncLimiter(50, 1)  # 50 requests per second
 
-    def currently_limited(self) -> List[str]:
-        """
-        Returns:
-            Returns a list of the buckets (str) that are currently being limited.
-        """
-        now = datetime.utcnow()
-        limited = [k for k, v in self.buckets.items() if v.reset is not None and v.reset > now and v.remaining == 0]
-        return limited
-
-    def any_limited(self) -> bool:
-        """
-        Returns:
-            True if any bucket is being rate limited
-        """
-        return any(self.currently_limited())
+    def update_bucket_relations(self, old_hash: str, new_hash: str):
+        for path, bucket_hash in self.bucket_relations.items():
+            if bucket_hash == old_hash:
+                self.bucket_relations[path] = new_hash
 
-    def is_limited(self, bucket: str):
-        return bucket in self.currently_limited()
+        self.buckets[new_hash] = self.buckets.pop(old_hash)
```

### Comparing `discord_limits-1.1.2/discord_limits.egg-info/PKG-INFO` & `discord_limits-2.0.1/discord_limits.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,44 @@
 Metadata-Version: 2.1
 Name: discord-limits
-Version: 1.1.2
-Summary: Make requests API requests to Discord without having to worry about ratelimits.
+Version: 2.0.1
+Summary: Make Discord API calls without having to worry about ratelimits.
 Home-page: https://github.com/ninjafella/discord-API-limits
 Author: ninjafella
 License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Documentation Status](https://readthedocs.org/projects/discord-limits/badge/?version=latest)](https://discord-limits.readthedocs.io/en/latest/?badge=latest)
-[![Version](https://img.shields.io/badge/Version-v1.1.2-blue)](https://img.shields.io/badge/Version-v1.1.2-blue)
+[![Documentation Status]](https://discord-limits.readthedocs.io/en/latest/?badge=latest)
+[![Version](https://img.shields.io/badge/Version-v2.0.1-blue)](https://img.shields.io/badge/Version-v2.0.1-blue)
 
 # discord_limits
 
 ### A simple library to asynchronously make API requests to Discord without having to worry about ratelimits.
 
 <br>
 
-### Currently this library has only been tested on Python 3.9
-
 ---
 
 # Basic usage
 
 ```py
 import discord_limits
-import os
 import asyncio
 
-limitsClient = discord_limits.DiscordClient(os.environ.get('TOKEN'))
+limits_client = discord_limits.DiscordClient("YOUR_TOKEN", "bot")
 
 async def main():
-    await limitsClient.create_message(123456789012345678, content='Hello World!')
+    await limits_client.channel.create_message("CHANNEL_ID", "Hello World!")
 
+asyncio.run(main())
 
-asyncio.get_event_loop().run_until_complete(main())
 ```
 
 ---
 ### Requires:
 - [aiolimiter](https://pypi.org/project/aiolimiter/)
 - [aiohttp](https://pypi.org/project/aiohttp/)
 
----
-### Based off of:
-- [unbelipy](https://github.com/chrisdewa/unbelipy)
-- [discord.py](https://github.com/Rapptz/discord.py)
-
 
+[def]: https://readthedocs.org/projects/discord-limits/badge/?version=latest
```

