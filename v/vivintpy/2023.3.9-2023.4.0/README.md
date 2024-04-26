# Comparing `tmp/vivintpy-2023.3.9.tar.gz` & `tmp/vivintpy-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivintpy-2023.3.9.tar", max compression
+gzip compressed data, was "vivintpy-2023.4.0.tar", max compression
```

## Comparing `vivintpy-2023.3.9.tar` & `vivintpy-2023.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1076 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/LICENSE
--rw-r--r--   0        0        0     2658 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/README.md
--rw-r--r--   0        0        0     1049 2024-04-06 22:25:48.560179 vivintpy-2023.3.9/pyproject.toml
--rw-r--r--   0        0        0       64 2024-04-06 22:25:48.560179 vivintpy-2023.3.9/vivintpy/__init__.py
--rw-r--r--   0        0        0     7674 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/account.py
--rw-r--r--   0        0        0     4371 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/const.py
--rw-r--r--   0        0        0     8198 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/__init__.py
--rw-r--r--   0        0        0    12193 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/alarm_panel.py
--rw-r--r--   0        0        0    10352 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/camera.py
--rw-r--r--   0        0        0     1280 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/door_lock.py
--rw-r--r--   0        0        0     2069 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/garage_door.py
--rw-r--r--   0        0        0     1799 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/switch.py
--rw-r--r--   0        0        0     3326 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/thermostat.py
--rw-r--r--   0        0        0     3275 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/wireless_sensor.py
--rw-r--r--   0        0        0     1658 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/entity.py
--rw-r--r--   0        0        0    12804 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/enums.py
--rw-r--r--   0        0        0      705 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/exceptions.py
--rw-r--r--   0        0        0    81878 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/proto/beam_pb2.py
--rw-r--r--   0        0        0   102437 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/proto/beam_pb2.pyi
--rw-r--r--   0        0        0   168580 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/proto/beam_pb2_grpc.py
--rw-r--r--   0        0        0     1959 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/pubnub.py
--rw-r--r--   0        0        0        0 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/py.typed
--rw-r--r--   0        0        0     3665 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/system.py
--rw-r--r--   0        0        0     1289 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/utils.py
--rw-r--r--   0        0        0    19652 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/vivintskyapi.py
--rw-r--r--   0        0        0   429866 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/zjs_device_config_db.json
--rw-r--r--   0        0        0     1037 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/zjs_device_config_db.py
--rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 vivintpy-2023.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-26 18:36:41.482793 vivintpy-2023.4.0/LICENSE
+-rw-r--r--   0        0        0     2658 2024-04-26 18:36:41.482793 vivintpy-2023.4.0/README.md
+-rw-r--r--   0        0        0     1049 2024-04-26 18:36:55.338863 vivintpy-2023.4.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-04-26 18:36:55.342863 vivintpy-2023.4.0/vivintpy/__init__.py
+-rw-r--r--   0        0        0     7674 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/account.py
+-rw-r--r--   0        0        0     4371 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/const.py
+-rw-r--r--   0        0        0     8198 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/devices/__init__.py
+-rw-r--r--   0        0        0    12193 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/devices/alarm_panel.py
+-rw-r--r--   0        0        0    10535 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/devices/camera.py
+-rw-r--r--   0        0        0     1280 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/devices/door_lock.py
+-rw-r--r--   0        0        0     2069 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/devices/garage_door.py
+-rw-r--r--   0        0        0     1799 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/devices/switch.py
+-rw-r--r--   0        0        0     3326 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/devices/thermostat.py
+-rw-r--r--   0        0        0     3275 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/devices/wireless_sensor.py
+-rw-r--r--   0        0        0     1658 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/entity.py
+-rw-r--r--   0        0        0    12804 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/enums.py
+-rw-r--r--   0        0        0      705 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/exceptions.py
+-rw-r--r--   0        0        0    81878 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/proto/beam_pb2.py
+-rw-r--r--   0        0        0   102437 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/proto/beam_pb2.pyi
+-rw-r--r--   0        0        0   168580 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/proto/beam_pb2_grpc.py
+-rw-r--r--   0        0        0     1959 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/pubnub.py
+-rw-r--r--   0        0        0        0 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/py.typed
+-rw-r--r--   0        0        0     3665 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/system.py
+-rw-r--r--   0        0        0     1289 2024-04-26 18:36:41.486793 vivintpy-2023.4.0/vivintpy/utils.py
+-rw-r--r--   0        0        0    19994 2024-04-26 18:36:41.490793 vivintpy-2023.4.0/vivintpy/vivintskyapi.py
+-rw-r--r--   0        0        0   429866 2024-04-26 18:36:41.490793 vivintpy-2023.4.0/vivintpy/zjs_device_config_db.json
+-rw-r--r--   0        0        0     1037 2024-04-26 18:36:41.490793 vivintpy-2023.4.0/vivintpy/zjs_device_config_db.py
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 vivintpy-2023.4.0/PKG-INFO
```

### Comparing `vivintpy-2023.3.9/LICENSE` & `vivintpy-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/README.md` & `vivintpy-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/pyproject.toml` & `vivintpy-2023.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vivintpy"
-version = "2023.3.9"
+version = "2023.4.0"
 description = "Python library for interacting with a Vivint security and smart home system."
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/natekspencer/vivintpy"
 repository = "https://github.com/natekspencer/vivintpy"
 keywords = ["Vivint", "alarm system", "security", "smart home", "home automation", "asynchronous"]
```

### Comparing `vivintpy-2023.3.9/vivintpy/account.py` & `vivintpy-2023.4.0/vivintpy/account.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/const.py` & `vivintpy-2023.4.0/vivintpy/const.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/devices/__init__.py` & `vivintpy-2023.4.0/vivintpy/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/devices/alarm_panel.py` & `vivintpy-2023.4.0/vivintpy/devices/alarm_panel.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/devices/camera.py` & `vivintpy-2023.4.0/vivintpy/devices/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,20 @@
     async def get_direct_rtsp_url(
         self,
         hd: bool = False,  # pylint: disable=invalid-name
     ) -> str | None:
         """Return the direct rtsp url for this camera, in HD if requested, if any."""
         return self.get_rtsp_access_url(RtspUrlType.LOCAL, hd)
 
+    async def reboot(self) -> None:
+        """Reboot the camera."""
+        await self.api.reboot_camera(
+            self.alarm_panel.id, self.id, self.device_type.value
+        )
+
     async def set_as_doorbell_chime_extender(self, state: bool) -> None:
         """Set use as doorbell chime extender."""
         await self.api.set_camera_as_doorbell_chime_extender(
             self.alarm_panel.id, self.id, state
         )
 
     async def set_privacy_mode(self, state: bool) -> None:
```

### Comparing `vivintpy-2023.3.9/vivintpy/devices/door_lock.py` & `vivintpy-2023.4.0/vivintpy/devices/door_lock.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/devices/garage_door.py` & `vivintpy-2023.4.0/vivintpy/devices/garage_door.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/devices/switch.py` & `vivintpy-2023.4.0/vivintpy/devices/switch.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/devices/thermostat.py` & `vivintpy-2023.4.0/vivintpy/devices/thermostat.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/devices/wireless_sensor.py` & `vivintpy-2023.4.0/vivintpy/devices/wireless_sensor.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/entity.py` & `vivintpy-2023.4.0/vivintpy/entity.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/enums.py` & `vivintpy-2023.4.0/vivintpy/enums.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/exceptions.py` & `vivintpy-2023.4.0/vivintpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/proto/beam_pb2.py` & `vivintpy-2023.4.0/vivintpy/proto/beam_pb2.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/proto/beam_pb2.pyi` & `vivintpy-2023.4.0/vivintpy/proto/beam_pb2.pyi`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/proto/beam_pb2_grpc.py` & `vivintpy-2023.4.0/vivintpy/proto/beam_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/pubnub.py` & `vivintpy-2023.4.0/vivintpy/pubnub.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/system.py` & `vivintpy-2023.4.0/vivintpy/system.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/utils.py` & `vivintpy-2023.4.0/vivintpy/utils.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/vivintskyapi.py` & `vivintpy-2023.4.0/vivintpy/vivintskyapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Any, cast
 
 import aiohttp
 import certifi
 import grpc
 from aiohttp import ClientResponseError
 from aiohttp.client import _RequestContextManager
+from google.protobuf.message import Message  # type: ignore
 
 from .const import (
     AuthenticationResponse,
     MfaVerificationResponse,
     SwitchAttribute,
     VivintDeviceAttribute,
 )
@@ -131,14 +132,31 @@
         return resp
 
     async def update_panel_software(self, panel_id: int) -> None:
         """Request a panel software update."""
         if not await self.__post(f"systems/{panel_id}/system-update"):
             raise VivintSkyApiError("Unable to update panel software")
 
+    async def reboot_camera(
+        self, panel_id: int, device_id: int, device_type: str
+    ) -> None:
+        """Reboot a camera."""
+
+        async def _callback(
+            stub: beam_pb2_grpc.BeamStub, metadata: list[tuple[str, str]]
+        ) -> Message:
+            return await stub.RebootCamera(
+                beam_pb2.RebootCameraRequest(  # pylint: disable=no-member
+                    panel_id=panel_id, device_id=device_id, device_type=device_type
+                ),
+                metadata=metadata,
+            )
+
+        await self._send_grpc(_callback)
+
     async def reboot_panel(self, panel_id: int) -> None:
         """Reboot a panel."""
         if not await self.__post(f"systems/{panel_id}/reboot-panel"):
             raise VivintSkyApiError("Unable to reboot panel")
 
     async def get_device_data(self, panel_id: int, device_id: int) -> dict:
         """Get the raw data for a device."""
@@ -180,71 +198,62 @@
             _LOGGER.error("Failed to trigger alarm for panel %s", panel_id)
             raise VivintSkyApiError("Failed to trigger alarm")
 
     async def set_camera_as_doorbell_chime_extender(
         self, panel_id: int, device_id: int, state: bool
     ) -> None:
         """Set the camera to be used as a doorbell chime extender."""
-        creds = grpc.ssl_channel_credentials()
-        assert (cookie := self._get_session_cookie())
 
-        async with grpc.aio.secure_channel(GRPC_ENDPOINT, credentials=creds) as channel:
-            stub: beam_pb2_grpc.BeamStub = beam_pb2_grpc.BeamStub(channel)  # type: ignore
-            response: beam_pb2.SetUseAsDoorbellChimeExtenderResponse = (
-                await stub.SetUseAsDoorbellChimeExtender(
-                    beam_pb2.SetUseAsDoorbellChimeExtenderRequest(  # pylint: disable=no-member
-                        panel_id=panel_id,
-                        device_id=device_id,
-                        use_as_doorbell_chime_extender=state,
-                    ),
-                    metadata=[("session", cookie.value)],
-                )
+        async def _callback(
+            stub: beam_pb2_grpc.BeamStub, metadata: list[tuple[str, str]]
+        ) -> Message:
+            return await stub.SetUseAsDoorbellChimeExtender(
+                beam_pb2.SetUseAsDoorbellChimeExtenderRequest(  # pylint: disable=no-member
+                    panel_id=panel_id,
+                    device_id=device_id,
+                    use_as_doorbell_chime_extender=state,
+                ),
+                metadata=metadata,
             )
 
-        _LOGGER.debug("Response received: %s", str(response))
+        await self._send_grpc(_callback)
 
     async def set_camera_privacy_mode(
         self, panel_id: int, device_id: int, state: bool
     ) -> None:
         """Set the camera privacy mode."""
-        creds = grpc.ssl_channel_credentials()
-        assert (cookie := self._get_session_cookie())
 
-        async with grpc.aio.secure_channel(GRPC_ENDPOINT, credentials=creds) as channel:
-            stub: beam_pb2_grpc.BeamStub = beam_pb2_grpc.BeamStub(channel)  # type: ignore
-            response: beam_pb2.SetCameraPrivacyModeResponse = (
-                await stub.SetCameraPrivacyMode(
-                    beam_pb2.SetCameraPrivacyModeRequest(  # pylint: disable=no-member
-                        panel_id=panel_id,
-                        device_id=device_id,
-                        privacy_mode=state,
-                    ),
-                    metadata=[("session", cookie.value)],
-                )
+        async def _callback(
+            stub: beam_pb2_grpc.BeamStub, metadata: list[tuple[str, str]]
+        ) -> Message:
+            return await stub.SetCameraPrivacyMode(
+                beam_pb2.SetCameraPrivacyModeRequest(  # pylint: disable=no-member
+                    panel_id=panel_id, device_id=device_id, privacy_mode=state
+                ),
+                metadata=metadata,
             )
 
-        _LOGGER.debug("Response received: %s", str(response))
+        await self._send_grpc(_callback)
 
     async def set_camera_deter_mode(
         self, panel_id: int, device_id: int, state: bool
     ) -> None:
         """Set the camera deter mode."""
-        creds = grpc.ssl_channel_credentials()
-        assert (cookie := self._get_session_cookie())
 
-        async with grpc.aio.secure_channel(GRPC_ENDPOINT, credentials=creds) as channel:
-            stub: beam_pb2_grpc.BeamStub = beam_pb2_grpc.BeamStub(channel)  # type: ignore
-            response: beam_pb2.SetDeterOverrideResponse = await stub.SetDeterOverride(
+        async def _callback(
+            stub: beam_pb2_grpc.BeamStub, metadata: list[tuple[str, str]]
+        ) -> Message:
+            return await stub.SetDeterOverride(
                 beam_pb2.SetDeterOverrideRequest(  # pylint: disable=no-member
                     panel_id=panel_id, device_id=device_id, enabled=state
                 ),
-                metadata=[("session", cookie.value)],
+                metadata=metadata,
             )
 
-        _LOGGER.debug("Response received: %s", str(response))
+        await self._send_grpc(_callback)
 
     async def set_garage_door_state(
         self, panel_id: int, partition_id: int, device_id: int, state: int
     ) -> None:
         """Open/Close garage door."""
         resp = await self.__put(
             f"{panel_id}/{partition_id}/door/{device_id}",
@@ -527,7 +536,20 @@
                     self.__mfa_pending = True
                     raise VivintSkyApiMfaRequiredError(message)
                 if resp.status == 400:
                     raise VivintSkyApiError(message)
                 raise VivintSkyApiAuthenticationError(message)
             resp.raise_for_status()
             return None
+
+    async def _send_grpc(
+        self,
+        callback: Callable[[beam_pb2_grpc.BeamStub, list[tuple[str, str]]], Message],
+    ) -> None:
+        """Send gRPC."""
+        creds = grpc.ssl_channel_credentials()
+        assert (cookie := self._get_session_cookie())
+
+        async with grpc.aio.secure_channel(GRPC_ENDPOINT, credentials=creds) as channel:
+            stub: beam_pb2_grpc.BeamStub = beam_pb2_grpc.BeamStub(channel)  # type: ignore
+            response = await callback(stub, [("session", cookie.value)])
+            _LOGGER.debug("Response received: %s", str(response))
```

### Comparing `vivintpy-2023.3.9/vivintpy/zjs_device_config_db.json` & `vivintpy-2023.4.0/vivintpy/zjs_device_config_db.json`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/vivintpy/zjs_device_config_db.py` & `vivintpy-2023.4.0/vivintpy/zjs_device_config_db.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.9/PKG-INFO` & `vivintpy-2023.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivintpy
-Version: 2023.3.9
+Version: 2023.4.0
 Summary: Python library for interacting with a Vivint security and smart home system.
 Home-page: https://github.com/natekspencer/vivintpy
 License: MIT
 Keywords: Vivint,alarm system,security,smart home,home automation,asynchronous
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vivintpy Version: 2023.3.9 Summary: Python library
+Metadata-Version: 2.1 Name: vivintpy Version: 2023.4.0 Summary: Python library
 for interacting with a Vivint security and smart home system. Home-page: https:
 //github.com/natekspencer/vivintpy License: MIT Keywords: Vivint,alarm
 system,security,smart home,home automation,asynchronous Author: Nathan Spencer
 Author-email: natekspencer@gmail.com Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

