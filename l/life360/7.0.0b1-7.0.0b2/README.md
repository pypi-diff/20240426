# Comparing `tmp/life360-7.0.0b1.tar.gz` & `tmp/life360-7.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "life360-7.0.0b1.tar", last modified: Tue Apr 16 15:21:12 2024, max compression
+gzip compressed data, was "life360-7.0.0b2.tar", last modified: Fri Apr 26 15:33:12 2024, max compression
```

## Comparing `life360-7.0.0b1.tar` & `life360-7.0.0b2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:12.506760 life360-7.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 15:21:07.000000 life360-7.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-16 15:21:12.506760 life360-7.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-16 15:21:07.000000 life360-7.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:12.506760 life360-7.0.0b1/life360/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-16 15:21:07.000000 life360-7.0.0b1/life360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-04-16 15:21:07.000000 life360-7.0.0b1/life360/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-16 15:21:07.000000 life360-7.0.0b1/life360/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-16 15:21:07.000000 life360-7.0.0b1/life360/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 15:21:07.000000 life360-7.0.0b1/life360/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:12.506760 life360-7.0.0b1/life360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-16 15:21:12.000000 life360-7.0.0b1/life360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 15:21:12.000000 life360-7.0.0b1/life360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:21:12.000000 life360-7.0.0b1/life360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 15:21:12.000000 life360-7.0.0b1/life360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 15:21:12.000000 life360-7.0.0b1/life360.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:21:12.506760 life360-7.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-16 15:21:07.000000 life360-7.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:33:12.641570 life360-7.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 15:33:09.000000 life360-7.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-26 15:33:12.641570 life360-7.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 15:33:09.000000 life360-7.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:33:12.637570 life360-7.0.0b2/life360/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-26 15:33:09.000000 life360-7.0.0b2/life360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-26 15:33:09.000000 life360-7.0.0b2/life360/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-26 15:33:09.000000 life360-7.0.0b2/life360/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-26 15:33:09.000000 life360-7.0.0b2/life360/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-26 15:33:09.000000 life360-7.0.0b2/life360/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:33:12.641570 life360-7.0.0b2/life360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-26 15:33:12.000000 life360-7.0.0b2/life360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-26 15:33:12.000000 life360-7.0.0b2/life360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:33:12.000000 life360-7.0.0b2/life360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 15:33:12.000000 life360-7.0.0b2/life360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 15:33:12.000000 life360-7.0.0b2/life360.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:33:12.641570 life360-7.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-26 15:33:09.000000 life360-7.0.0b2/setup.py
```

### Comparing `life360-7.0.0b1/LICENSE` & `life360-7.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b1/PKG-INFO` & `life360-7.0.0b2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 7.0.0b1
+Version: 7.0.0b2
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `life360-7.0.0b1/README.md` & `life360-7.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b1/life360/__init__.py` & `life360-7.0.0b2/life360/__init__.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b1/life360/api.py` & `life360-7.0.0b2/life360/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Life360 API."""
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Iterable, Mapping
+from collections.abc import Iterable, Mapping, MutableMapping
 from contextlib import suppress
 from json import JSONDecodeError
 import logging
 import re
 import traceback
 from typing import Any, cast
 
@@ -48,14 +48,15 @@
 }
 
 _RETRY_EXCEPTIONS = (ClientConnectionError, asyncio.TimeoutError)
 _RETRY_CLIENT_RESPONSE_ERRORS = (
     HTTP_Error.BAD_GATEWAY,
     HTTP_Error.SERVICE_UNAVAILABLE,
     HTTP_Error.GATEWAY_TIME_OUT,
+    HTTP_Error.SERVER_UNKNOWN_ERROR,
 )
 
 _URL_REDACTIONS = (re.compile(r"/(?:(?:circles)|(?:members))/(?!REDACTED)([\w-]+)"),)
 _RESP_REPR_REDACTIONS = (
     *_URL_REDACTIONS,
     re.compile(r"'Bearer (?!REDACTED')([^']+)'"),
     re.compile(r"'Set-Cookie': '[^=]+=(?!REDACTED[;'])([^;']+)[;']"),
@@ -89,39 +90,58 @@
 
 
 def _format_exc(exc: Exception) -> str:
     """Format an exception."""
     return "; ".join(s.strip() for s in traceback.format_exception_only(exc))
 
 
+class NameAdapter(logging.LoggerAdapter):
+    """Logging adapter to add name prefix."""
+
+    def process(
+        self, msg: Any, kwargs: MutableMapping[str, Any]
+    ) -> tuple[Any, MutableMapping[str, Any]]:
+        """Add name prefix."""
+        return f"{cast(Mapping[str, object], self.extra)['name']}: {msg}", kwargs
+
+
 class Life360:
     """Life360 API."""
 
+    _logger: logging.Logger | logging.LoggerAdapter
+
     def __init__(
         self,
         session: ClientSession,
         max_retries: int,
         authorization: str | None = None,
         *,
+        name: str | None = None,
         verbosity: int = 0,
     ) -> None:
         """Initialize API.
 
+        name: Prefix for log messages, not affected by verbosity.
+
         verbosity:
         0 -> Minimal DEBUG messages with redactions
         1 -> Add client response headers
         2 -> Add client response text/json
         3 -> No informational redactions
         4 -> No redactions
         """
         self._session = session
         if max_retries < 0:
             raise ValueError("max_retries must be non-negative")
         self._max_attempts = max_retries + 1
-        self._authorization = authorization
+        self.authorization = authorization
+        if name:
+            self._logger = NameAdapter(_LOGGER, {"name": name})
+        else:
+            self._logger = _LOGGER
         self.verbosity = verbosity
         self._etags: dict[str, str] = {}
 
     @property
     def verbosity(self) -> int:
         """Return verbosity level."""
         return self._verbosity
@@ -129,19 +149,14 @@
     @verbosity.setter
     def verbosity(self, value: int) -> None:
         """Set verbosity level."""
         if not (0 <= value <= 4):
             raise ValueError("verbosity must be between 0 and 4, inclusive")
         self._verbosity = value
 
-    @property
-    def authorization(self) -> str | None:
-        """Return authorization."""
-        return self._authorization
-
     async def login_by_username(self, username: str, password: str) -> str:
         """Log into Life360 server using username & password."""
         reply = cast(
             Mapping[str, str],
             await self._request(
                 _TOKEN_URL,
                 method="post",
@@ -151,20 +166,20 @@
                     "username": username,
                     "password": password,
                 },
                 authorization=f"Basic {CLIENT_TOKEN}",
             ),
         )
         try:
-            self._authorization = f"{reply['token_type']} {reply['access_token']}"
+            self.authorization = f"{reply['token_type']} {reply['access_token']}"
         except KeyError:
             raise Life360Error(
                 f"Unexpected response while logging in by username: {reply}"
             ) from None
-        return self._authorization
+        return self.authorization
 
     async def get_circles(
         self, *, raise_not_modified: bool = False
     ) -> list[dict[str, str]]:
         """Get basic data about all Circles."""
         return cast(
             dict[str, list[dict[str, str]]],
@@ -201,15 +216,15 @@
         method: str = "get",
         *,
         authorization: str | None = None,
         **kwargs: dict[str, Any],
     ) -> Any:
         """Make a request to server."""
         if authorization is None:
-            authorization = self._authorization
+            authorization = self.authorization
         if authorization is None:
             raise LoginError("Must login")
 
         headers = _HEADERS
         if authorization != "":
             headers["authorization"] = authorization
         if raise_not_modified and (etag := self._etags.get(url)):
@@ -223,15 +238,15 @@
                 resp = cast(
                     ClientResponse,
                     await getattr(self._session, method)(url, **kwargs),
                 )
                 status = resp.status
                 resp.raise_for_status()
             except ClientError as exc:
-                _LOGGER.debug(
+                self._logger.debug(
                     "Request error: %s(%s), attempt %i: %s",
                     method.upper(),
                     self._redact(url, _URL_REDACTIONS),
                     attempt,
                     self._redact(repr(exc), _EXC_REPR_REDACTIONS),
                 )
                 await self._dump_resp_text(resp)
@@ -278,15 +293,15 @@
             try:
                 return await resp.json()
             except (ClientError, JSONDecodeError) as exc:
                 try:
                     resp_ = await resp.text()
                 except ClientError:
                     resp_ = str(resp)
-                _LOGGER.debug(
+                self._logger.debug(
                     "While parsing response: %r: %s",
                     resp_,
                     self._redact(repr(exc), _EXC_REPR_REDACTIONS),
                 )
                 raise Life360Error(
                     self._redact(_format_exc(exc), _URL_REDACTIONS)
                 ) from None
@@ -296,30 +311,30 @@
         if resp is None or self.verbosity < 2:
             return
         try:
             if not (text := await resp.text()):
                 return
         except ClientError:
             return
-        _LOGGER.debug(
-            "resp data: %s",
+        self._logger.debug(
+            "Response data: %s",
             self._redact(
                 text,
                 _RESP_TEXT_ALL_REDACTIONS
                 if self.verbosity < 3
                 else _RESP_TEXT_BASIC_REDACTIONS,
             ),
         )
 
     async def _dump_resp(self, resp: ClientResponse) -> None:
         """Dump response to log."""
         if self.verbosity < 1:
             return
         resp_repr = repr(resp).replace("\n", " ")
-        _LOGGER.debug("resp: %s", self._redact(resp_repr, _RESP_REPR_REDACTIONS))
+        self._logger.debug("Response headers: %s", self._redact(resp_repr, _RESP_REPR_REDACTIONS))
         await self._dump_resp_text(resp)
 
     def _redact(self, string: str, redactions: Iterable[re.Pattern]) -> str:
         """Redact string for lower verbosity levels."""
         if self.verbosity >= 4:
             return string
         for redaction in redactions:
```

### Comparing `life360-7.0.0b1/life360/const.py` & `life360-7.0.0b2/life360/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,7 +18,8 @@
     UNAUTHORIZED = 401
     FORBIDDEN = 403
     NOT_FOUND = 404
     TOO_MANY_REQUESTS = 429
     BAD_GATEWAY = 502
     SERVICE_UNAVAILABLE = 503
     GATEWAY_TIME_OUT = 504
+    SERVER_UNKNOWN_ERROR = 520
```

### Comparing `life360-7.0.0b1/life360/exceptions.py` & `life360-7.0.0b2/life360/exceptions.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b1/life360.egg-info/PKG-INFO` & `life360-7.0.0b2/life360.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 7.0.0b1
+Version: 7.0.0b2
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `life360-7.0.0b1/setup.py` & `life360-7.0.0b2/setup.py`

 * *Files identical despite different names*

