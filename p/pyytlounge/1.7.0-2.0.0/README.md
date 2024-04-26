# Comparing `tmp/pyytlounge-1.7.0.tar.gz` & `tmp/pyytlounge-2.0.0.tar.gz`

## Comparing `pyytlounge-1.7.0.tar` & `pyytlounge-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,26 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/test.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/variables_example.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/.vscode/launch.json
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/src/pyytlounge/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/src/pyytlounge/api.py
--rwxr-xr-x   0        0        0     1040 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/src/pyytlounge/manual_pairing.py
--rw-r--r--   0        0        0    20276 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/src/pyytlounge/wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/tests/__init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/tests/conftest.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/tests/devices.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/tests/test_process_event.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/LICENSE
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/README.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyytlounge-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/test.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/variables_example.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/.vscode/launch.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/docs/Makefile
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/docs/api.rst
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/docs/conf.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/docs/make.bat
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/docs/usage.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/src/pyytlounge/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/src/pyytlounge/api.py
+-rwxr-xr-x   0        0        0     1040 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/src/pyytlounge/manual_pairing.py
+-rw-r--r--   0        0        0    20164 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/src/pyytlounge/wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/tests/devices.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/tests/test_process_event.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/LICENSE
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 pyytlounge-2.0.0/PKG-INFO
```

### Comparing `pyytlounge-1.7.0/test.py` & `pyytlounge-2.0.0/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 import asyncio
 from src.pyytlounge.wrapper import YtLoungeApi, PlaybackState, State
 from ast import literal_eval
 import os
+import logging
 
 AUTH_STATE_FILE = "auth_state"
-
+logger = logging.getLogger(__name__)
+console_handler = logging.StreamHandler()
+console_handler.setLevel(logging.DEBUG)
+logger.addHandler(console_handler)
+logger.setLevel(logging.DEBUG)
 
 async def go():
-    api = YtLoungeApi("Test")
-    if os.path.exists(AUTH_STATE_FILE):
-        with open(AUTH_STATE_FILE, "r") as f:
-            content = f.read()
-            api.load_auth_state(literal_eval(content))
-            print("Loaded from file")
-    else:
-        pairing_code = input("Enter pairing code: ")
-        print(f"Pairing with code {pairing_code}...")
-        paired = await api.pair(pairing_code)
-        print(paired and "success" or "failed")
-        if not paired:
+    async with YtLoungeApi("Test", logger) as api:
+        if os.path.exists(AUTH_STATE_FILE):
+            with open(AUTH_STATE_FILE, "r") as f:
+                content = f.read()
+                api.load_auth_state(literal_eval(content))
+                print("Loaded from file")
+        else:
+            pairing_code = input("Enter pairing code: ")
+            print(f"Pairing with code {pairing_code}...")
+            paired = await api.pair(pairing_code)
+            print(paired and "success" or "failed")
+            if not paired:
+                exit()
+            auth_state = api.auth.serialize()
+            with open(AUTH_STATE_FILE, "w") as f:
+                f.write(str(auth_state))
+        print(api)
+        is_available = await api.is_available()
+        print(f"Screen availability: {is_available}")
+
+        print("Connecting...")
+        connected = await api.connect()
+        print(connected and "success" or "failed")
+        if not connected:
             exit()
-        auth_state = api.auth.serialize()
-        with open(AUTH_STATE_FILE, "w") as f:
-            f.write(str(auth_state))
-    print(api)
-    is_available = await api.is_available()
-    print(f"Screen availability: {is_available}")
-
-    print("Connecting...")
-    connected = await api.connect()
-    print(connected and "success" or "failed")
-    if not connected:
-        exit()
-
-    print(f"Screen: {api.screen_name}")
-    print(f"Device: {api.screen_device_name}")
-
-    async def receive_state(state: PlaybackState):
-        print(f"New state: {state}")
-        if state.videoId:
-            print(
-                f"Image should be at: https://img.youtube.com/vi/{state.videoId}/0.jpg"
-            )
 
-    await api.subscribe(receive_state)
+        print(f"Screen: {api.screen_name}")
+        print(f"Device: {api.screen_device_name}")
+
+        last_video_id = None
+        async def receive_state(state: PlaybackState):
+            nonlocal last_video_id
+            print(f"New state: {state}")
+            if state.videoId and state.videoId != last_video_id:
+                last_video_id = state.videoId
+                print(
+                    f"Image should be at: https://img.youtube.com/vi/{state.videoId}/0.jpg"
+                )
+
+        await api.subscribe(receive_state)
 
 
 asyncio.run(go())
```

### Comparing `pyytlounge-1.7.0/.github/workflows/python-publish.yml` & `pyytlounge-2.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyytlounge-1.7.0/.github/workflows/test.yml` & `pyytlounge-2.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyytlounge-1.7.0/src/pyytlounge/manual_pairing.py` & `pyytlounge-2.0.0/src/pyytlounge/manual_pairing.py`

 * *Files identical despite different names*

### Comparing `pyytlounge-1.7.0/src/pyytlounge/wrapper.py` & `pyytlounge-2.0.0/src/pyytlounge/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import logging
 from enum import Enum
 from typing import Any, AsyncIterator, List, TypedDict, Union, Callable
 from dataclasses import dataclass
 
 import aiohttp
-from aiohttp import ClientTimeout, StreamReader
+from aiohttp import ClientTimeout, StreamReader, ClientPayloadError
 
 from .api import api_base
 
 
 class State(Enum):
     """Playback state"""
 
@@ -180,17 +180,29 @@
         self._last_event_id = None
         self.state = PlaybackState(logger)
         self.state_update = 0
         self._command_offset = 1
         self._screen_name: str = None
         self._device_info: __DeviceInfo = None
         self._logger = logger or logging.Logger(__package__, logging.DEBUG)
+        self.conn = aiohttp.TCPConnector(ttl_dns_cache=300)
+        self.session = aiohttp.ClientSession(connector=self.conn)
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        await self.close()
+
+    async def close(self):
+        await self.session.close()
+        await self.conn.close()
 
     def paired(self) -> bool:
-        """Returns true if screen id and lounge id token are known."""
+        """Returns true if screen id is known."""
         return self.auth.screen_id is not None
 
     def linked(self) -> bool:
         """Returns true if paired and lounge id token is known."""
         return self.paired() and self.auth.lounge_id_token is not None
 
     def connected(self) -> bool:
@@ -221,52 +233,50 @@
         brand = self._device_info["brand"]
         model = self._device_info["model"]
         return f"{brand} {model}"
 
     async def pair(self, pairing_code) -> bool:
         """Pair with a device using a manual input pairing code"""
 
-        async with aiohttp.ClientSession() as session:
-            pair_url = f"{api_base}/pairing/get_screen"
-            pair_data = {"pairing_code": pairing_code}
-            async with session.post(url=pair_url, data=pair_data) as resp:
-                try:
-                    screens = await resp.json()
-                    screen = screens["screen"]
-                    self._screen_name = screen["name"]
-                    self.auth.screen_id = screen["screenId"]
-                    self.auth.lounge_id_token = screen["loungeToken"]
-                    return self.linked()
-                except:
-                    self._logger.exception("Pairing failed")
-                    return False
+        pair_url = f"{api_base}/pairing/get_screen"
+        pair_data = {"pairing_code": pairing_code}
+        async with self.session.post(url=pair_url, data=pair_data) as resp:
+            try:
+                screens = await resp.json()
+                screen = screens["screen"]
+                self._screen_name = screen["name"]
+                self.auth.screen_id = screen["screenId"]
+                self.auth.lounge_id_token = screen["loungeToken"]
+                return self.linked()
+            except:
+                self._logger.exception("Pairing failed")
+                raise
 
     async def refresh_auth(self) -> bool:
         """Refresh lounge token using stored refresh token."""
         if not self.paired():
             raise NotPairedException("Must be paired")
 
-        async with aiohttp.ClientSession() as session:
-            refresh_url = f"{api_base}/pairing/get_lounge_token_batch"
-            refresh_data = {"screen_ids": self.auth.screen_id}
-            async with session.post(url=refresh_url, data=refresh_data) as resp:
-                try:
-                    screens = await resp.json()
-                    screen = screens["screens"][0]
-                    self.auth.screen_id = screen["screenId"]
-                    self.auth.lounge_id_token = screen["loungeToken"]
-
-                    self._logger.info(
-                        "Refreshed auth, lounge id token %s", self.auth.lounge_id_token
-                    )
-
-                    return self.linked()
-                except:
-                    self._logger.exception("Refresh auth failed")
-                    return False
+        refresh_url = f"{api_base}/pairing/get_lounge_token_batch"
+        refresh_data = {"screen_ids": self.auth.screen_id}
+        async with self.session.post(url=refresh_url, data=refresh_data) as resp:
+            try:
+                screens = await resp.json()
+                screen = screens["screens"][0]
+                self.auth.screen_id = screen["screenId"]
+                self.auth.lounge_id_token = screen["loungeToken"]
+
+                self._logger.info(
+                    "Refreshed auth, lounge id token %s", self.auth.lounge_id_token
+                )
+
+                return self.linked()
+            except:
+                self._logger.exception("Refresh auth failed")
+                raise
 
     def store_auth_state(self) -> dict:
         """Return auth parameters as dict which can be serialized for later use"""
         return {
             "screenId": self.auth.screen_id,
             "lounge_id_token": self.auth.lounge_id_token,
             "refresh_token": self.auth.refresh_token,
@@ -305,14 +315,15 @@
                     self._screen_name = device["name"]
                     self._device_info = json.loads(device.get("deviceInfo", "null"))
                     break
         elif event_type == "loungeScreenDisconnected":
             self.state = PlaybackState(self._logger)
             self._update_state()
             self._connection_lost()
+            self._lounge_token_expired()
         elif event_type == "noop":
             pass  # no-op
         else:
             self._logger.debug("Unprocessed event %s %s", event_type, args)
 
     def _process_events(self, events):
         for event in events:
@@ -350,21 +361,20 @@
         if not self.linked():
             raise NotConnectedException("Not connected")
 
         body = {"lounge_token": self.auth.lounge_id_token}
 
         url = f"{api_base}/pairing/get_screen_availability"
 
-        async with aiohttp.ClientSession() as session:
-            result = await session.post(url=url, data=body)
-            status = await result.json()
-            if "screens" in status and len(status["screens"]) > 0:
-                return status["screens"][0]["status"] == "online"
+        result = await self.session.post(url=url, data=body)
+        status = await result.json()
+        if "screens" in status and len(status["screens"]) > 0:
+            return status["screens"][0]["status"] == "online"
 
-            return False
+        return False
 
     def get_thumbnail_url(self, thumbnail_idx=0) -> str:
         """Returns thumbnail for current video. Use thumbnail idx to get different thumbnails.
         Returns None if no video is set."""
         if not self.state.videoId:
             return None
         return get_thumbnail_url(self.state.videoId, thumbnail_idx)
@@ -387,39 +397,38 @@
             "deviceContext": "user_agent=dunno&window_width_points=&window_height_points=&os_name=android&ms=",
             "theme": "cl",
             "loungeIdToken": self.auth.lounge_id_token,
         }
         connect_url = (
             f"{api_base}/bc/bind?RID=1&VER=8&CVER=1&auth_failure_option=send_error"
         )
-        async with aiohttp.ClientSession() as session:
-            async with session.post(url=connect_url, data=connect_body) as resp:
-                try:
-                    text = await resp.text()
-                    if resp.status == 401:
-                        self._lounge_token_expired()
-                        return False
-
-                    if resp.status != 200:
-                        self._logger.warning(
-                            "Unknown reply to connect %i %s", resp.status, resp.reason
-                        )
-                        return False
-                    lines = text.splitlines()
-                    async for events in self._parse_event_chunks(desync(lines)):
-                        self._process_events(events)
-                    self._command_offset = 1
-                    return self.connected()
-                except:
-                    self._logger.exception(
-                        "Handle connect failed, status %s reason %s",
-                        resp.status,
-                        resp.reason,
+        async with self.session.post(url=connect_url, data=connect_body) as resp:
+            try:
+                text = await resp.text()
+                if resp.status == 401:
+                    self._lounge_token_expired()
+                    return False
+
+                if resp.status != 200:
+                    self._logger.warning(
+                        "Unknown reply to connect %i %s", resp.status, resp.reason
                     )
                     return False
+                lines = text.splitlines()
+                async for events in self._parse_event_chunks(desync(lines)):
+                    self._process_events(events)
+                self._command_offset = 1
+                return self.connected()
+            except:
+                self._logger.exception(
+                    "Handle connect failed, status %s reason %s",
+                    resp.status,
+                    resp.reason,
+                )
+                raise
 
     def _handle_session_result(self, status_code: int, reason: str) -> bool:
         if status_code == 400 and "Unknown SID" in reason:
             self._connection_lost()
             return False
         if status_code == 410 and "Gone" in reason:
             self._connection_lost()
@@ -447,39 +456,44 @@
             "CI": "0",
             "AID": self._last_event_id,
             "gsessionid": self._gsession,
             "TYPE": "xmlhttp",
         }
         url = f"{api_base}/bc/bind"
         self._logger.info("Subscribing to lounge id %s", self.auth.lounge_id_token)
-        async with aiohttp.ClientSession(timeout=ClientTimeout()) as session:
-            async with session.get(url=url, params=params) as resp:
-                try:
-                    if not self._handle_session_result(resp.status, resp.reason):
-                        return
-
-                    async for events in self._parse_event_chunks(
-                        iter_response_lines(resp.content)
-                    ):
-                        pre_state_update = self.state_update
-                        self._process_events(events)
-                        if pre_state_update != self.state_update:
-                            await callback(self.state)
-                        if not self.connected():
-                            break
-                    self._logger.info(
-                        "Subscribe completed, status %i %s", resp.status, resp.reason
-                    )
-
-                except:
-                    self._logger.exception(
-                        "Handle subscribe failed, status %s reason %s",
-                        resp.status,
-                        resp.reason,
-                    )
+        async with self.session.get(url=url, params=params, timeout=ClientTimeout()) as resp:
+            try:
+                if not self._handle_session_result(resp.status, resp.reason):
+                    return
+
+                async for events in self._parse_event_chunks(
+                    iter_response_lines(resp.content)
+                ):
+                    pre_state_update = self.state_update
+                    self._process_events(events)
+                    if pre_state_update != self.state_update:
+                        await callback(self.state)
+                    if not self.connected():
+                        break
+                self._logger.info(
+                    "Subscribe completed, status %i %s", resp.status, resp.reason
+                )
+            except ClientPayloadError:
+                self._logger.exception(
+                    "Handle subscribe payload error, status %s reason %s",
+                    resp.status,
+                    resp.reason
+                )
+            except:
+                self._logger.exception(
+                    "Handle subscribe failed, status %s reason %s",
+                    resp.status,
+                    resp.reason,
+                )
+                raise
 
     async def disconnect(self) -> bool:
         """Disconnect from the current session"""
         if not self.connected():
             raise NotConnectedException("Not connected")
 
         command_body = {
@@ -498,25 +512,24 @@
             "RID": self._command_offset,
             "SID": self._sid,
             "AID": self._last_event_id,
             "gsessionid": self._gsession,
             "auth_failure_option": "send_error",
         }
         url = f"{api_base}/bc/bind"
-        async with aiohttp.ClientSession() as session:
-            async with session.post(url=url, data=command_body, params=params) as resp:
-                try:
-                    response_text = await resp.text()
-                    if not self._handle_session_result(resp.status, response_text):
-                        return False
-                    resp.raise_for_status()
-                    return True
-                except:
-                    self._logger.exception("Disconnect failed")
+        async with self.session.post(url=url, data=command_body, params=params) as resp:
+            try:
+                response_text = await resp.text()
+                if not self._handle_session_result(resp.status, response_text):
                     return False
+                resp.raise_for_status()
+                return True
+            except:
+                self._logger.exception("Disconnect failed")
+                raise
 
     async def _command(self, command: str, command_parameters: dict = None) -> bool:
         if not self.connected():
             raise NotConnectedException("Not connected")
 
         command_body = {"count": 1, "ofs": self._command_offset, "req0__sc": command}
         if command_parameters:
@@ -534,25 +547,24 @@
             "v": "2",
             "RID": self._command_offset,
             "SID": self._sid,
             "AID": self._last_event_id,
             "gsessionid": self._gsession,
         }
         url = f"{api_base}/bc/bind"
-        async with aiohttp.ClientSession() as session:
-            async with session.post(url=url, data=command_body, params=params) as resp:
-                try:
-                    response_text = await resp.text()
-                    if not self._handle_session_result(resp.status, response_text):
-                        return False
-                    resp.raise_for_status()
-                    return True
-                except:
-                    self._logger.exception("Command failed")
+        async with self.session.post(url=url, data=command_body, params=params) as resp:
+            try:
+                response_text = await resp.text()
+                if not self._handle_session_result(resp.status, response_text):
                     return False
+                resp.raise_for_status()
+                return True
+            except:
+                self._logger.exception("Command failed")
+                raise
 
     async def play(self) -> bool:
         """Sends play command to screen"""
         return await self._command("play")
 
     async def pause(self) -> bool:
         """Sends pause command to screen"""
```

### Comparing `pyytlounge-1.7.0/tests/devices.py` & `pyytlounge-2.0.0/tests/devices.py`

 * *Files identical despite different names*

### Comparing `pyytlounge-1.7.0/LICENSE` & `pyytlounge-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyytlounge-1.7.0/pyproject.toml` & `pyytlounge-2.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyytlounge"
-version = "1.7.0"
+version = "2.0.0"
 authors = [
   { name="Fabio", email="example@example.com" },
 ]
 description = "YouTube Lounge API wrapper"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -21,11 +21,14 @@
 "Bug Tracker" = "https://github.com/FabioGNR/pyytlounge/issues"
 
 [project.optional-dependencies]
 tests = [
   'pytest',
   'pytest-mock',
 ]
+docs = [
+  'sphinx'
+]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `pyytlounge-1.7.0/PKG-INFO` & `pyytlounge-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pyytlounge
-Version: 1.7.0
+Version: 2.0.0
 Summary: YouTube Lounge API wrapper
 Project-URL: Homepage, https://github.com/FabioGNR/pyytlounge
 Project-URL: Bug Tracker, https://github.com/FabioGNR/pyytlounge/issues
 Author-email: Fabio <example@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: aiohttp>=3.8.4
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-mock; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # YouTube Lounge API wrapper written in Python (WIP)
```

