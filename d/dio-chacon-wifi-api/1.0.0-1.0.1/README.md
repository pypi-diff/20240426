# Comparing `tmp/dio_chacon_wifi_api-1.0.0-py3-none-any.whl.zip` & `tmp/dio_chacon_wifi_api-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 22533 bytes, number of entries: 9
+Zip file size: 22644 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      120 b- defN 80-Jan-01 00:00 dio_chacon_wifi_api/__init__.py
 -rw-r--r--  2.0 unx    13108 b- defN 80-Jan-01 00:00 dio_chacon_wifi_api/client.py
 -rw-r--r--  2.0 unx     1205 b- defN 80-Jan-01 00:00 dio_chacon_wifi_api/const.py
--rw-r--r--  2.0 unx      190 b- defN 80-Jan-01 00:00 dio_chacon_wifi_api/exceptions.py
--rw-r--r--  2.0 unx     7074 b- defN 80-Jan-01 00:00 dio_chacon_wifi_api/session.py
--rw-r--r--  2.0 unx    35149 b- defN 80-Jan-01 00:00 dio_chacon_wifi_api-1.0.0.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 dio_chacon_wifi_api-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     5235 b- defN 16-Jan-01 00:00 dio_chacon_wifi_api-1.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      778 b- defN 16-Jan-01 00:00 dio_chacon_wifi_api-1.0.0.dist-info/RECORD
-9 files, 62942 bytes uncompressed, 21185 bytes compressed:  66.3%
+-rw-r--r--  2.0 unx      343 b- defN 80-Jan-01 00:00 dio_chacon_wifi_api/exceptions.py
+-rw-r--r--  2.0 unx     7399 b- defN 80-Jan-01 00:00 dio_chacon_wifi_api/session.py
+-rw-r--r--  2.0 unx    35149 b- defN 80-Jan-01 00:00 dio_chacon_wifi_api-1.0.1.dist-info/LICENSE
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 dio_chacon_wifi_api-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     5235 b- defN 16-Jan-01 00:00 dio_chacon_wifi_api-1.0.1.dist-info/METADATA
+?rw-r--r--  2.0 unx      778 b- defN 16-Jan-01 00:00 dio_chacon_wifi_api-1.0.1.dist-info/RECORD
+9 files, 63420 bytes uncompressed, 21296 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: dio_chacon_wifi_api/exceptions.py
 Comment: 
 
 Filename: dio_chacon_wifi_api/session.py
 Comment: 
 
-Filename: dio_chacon_wifi_api-1.0.0.dist-info/LICENSE
+Filename: dio_chacon_wifi_api-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: dio_chacon_wifi_api-1.0.0.dist-info/WHEEL
+Filename: dio_chacon_wifi_api-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: dio_chacon_wifi_api-1.0.0.dist-info/METADATA
+Filename: dio_chacon_wifi_api-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: dio_chacon_wifi_api-1.0.0.dist-info/RECORD
+Filename: dio_chacon_wifi_api-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dio_chacon_wifi_api/exceptions.py

```diff
@@ -1,8 +1,15 @@
-"""Exceptions for DIOChaconAPIClient."""
+"""Exceptions for DIOChacon API."""
 
 
 class DIOChaconAPIError(Exception):
     """Error from this api."""
 
     def __init__(self, *args) -> None:
         Exception.__init__(self, *args)
+
+
+class DIOChaconInvalidAuthError(Exception):
+    """Invalid auth detected"""
+
+    def __init__(self, *args) -> None:
+        Exception.__init__(self, *args)
```

## dio_chacon_wifi_api/session.py

```diff
@@ -5,14 +5,16 @@
 """
 import asyncio
 import json
 import logging
 
 import aiohttp
 
+from .exceptions import DIOChaconInvalidAuthError
+
 MAX_FAILED_ATTEMPTS = 5
 
 STATE_CONNECTED = "connected"
 STATE_DISCONNECTED = "disconnected"
 STATE_STARTING = "starting"
 STATE_STOPPED = "stopped"
 
@@ -84,14 +86,19 @@
         trace_config.on_request_end.append(on_request_end)
         trace_config.on_request_chunk_sent.append(on_request_chunk_sent)
         trace_config.on_response_chunk_received.append(on_response_chunk_received)
 
         self._aiohttp_session = aiohttp.ClientSession(trace_configs=[trace_config])
         async with self._aiohttp_session.post(url=self._auth_url, data=payload_data, headers=headers_token) as resp:
             resp_json = await resp.json()
+            if resp_json["status"] == 400:
+                err_msg = resp_json["data"]
+                _LOGGER.debug("Invalid auth response received : %s", err_msg)
+                await self._aiohttp_session.close()
+                raise DIOChaconInvalidAuthError(err_msg)
             self._sessionToken = str(resp_json["data"]["sessionToken"])
             _LOGGER.debug("SessionToken of authentication : " + self._sessionToken)
 
     async def ws_connect(self) -> None:
         """Make a connection to the server via websocket protocol."""
 
         # Starts a background parallel task to permanently listen to events
```

## Comparing `dio_chacon_wifi_api-1.0.0.dist-info/LICENSE` & `dio_chacon_wifi_api-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dio_chacon_wifi_api-1.0.0.dist-info/METADATA` & `dio_chacon_wifi_api-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dio-chacon-wifi-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library for DIO Chacon wifi's protocol for shutters and switches
 Home-page: https://github.com/cnico/dio-chacon-wifi-api
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: dio,chacon,shutter,switch,api
 Author: cnico
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

