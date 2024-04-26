# Comparing `tmp/python_swidget-1.0.3.tar.gz` & `tmp/python_swidget-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_swidget-1.0.3.tar", max compression
+gzip compressed data, was "python_swidget-1.2.0.tar", max compression
```

## Comparing `python_swidget-1.0.3.tar` & `python_swidget-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      539 2024-04-10 14:24:43.925014 python_swidget-1.0.3/README.md
--rw-r--r--   0        0        0     2179 2024-04-14 23:44:52.509851 python_swidget-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1330 2024-04-10 14:24:43.935014 python_swidget-1.0.3/swidget/__init__.py
--rw-r--r--   0        0        0     8982 2024-04-14 18:19:53.397240 python_swidget-1.0.3/swidget/cli.py
--rw-r--r--   0        0        0     3865 2024-04-14 18:19:53.397240 python_swidget-1.0.3/swidget/discovery.py
--rw-r--r--   0        0        0       79 2023-01-11 19:11:12.359430 python_swidget-1.0.3/swidget/exceptions.py
--rw-r--r--   0        0        0     4591 2024-04-10 14:24:43.935014 python_swidget-1.0.3/swidget/provision.py
--rw-r--r--   0        0        0        0 2023-01-11 19:11:12.359430 python_swidget-1.0.3/swidget/py.typed
--rw-r--r--   0        0        0    19107 2024-04-14 18:19:53.397240 python_swidget-1.0.3/swidget/swidgetdevice.py
--rw-r--r--   0        0        0     1696 2024-04-14 18:19:53.397240 python_swidget-1.0.3/swidget/swidgetdimmer.py
--rw-r--r--   0        0        0      402 2024-04-10 14:24:43.935014 python_swidget-1.0.3/swidget/swidgetoutlet.py
--rw-r--r--   0        0        0      402 2024-04-14 18:19:53.397240 python_swidget-1.0.3/swidget/swidgetswitch.py
--rw-r--r--   0        0        0      820 2024-04-14 18:19:53.397240 python_swidget-1.0.3/swidget/swidgettimerswitch.py
--rw-r--r--   0        0        0     4229 2024-04-14 18:19:53.397240 python_swidget-1.0.3/swidget/websocket.py
--rw-r--r--   0        0        0     1853 1970-01-01 00:00:00.000000 python_swidget-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      539 2024-04-10 14:24:43.925014 python_swidget-1.2.0/README.md
+-rw-r--r--   0        0        0     2179 2024-04-26 14:40:32.968055 python_swidget-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1330 2024-04-10 14:24:43.935014 python_swidget-1.2.0/swidget/__init__.py
+-rw-r--r--   0        0        0     8951 2024-04-26 14:40:11.998055 python_swidget-1.2.0/swidget/cli.py
+-rw-r--r--   0        0        0     3865 2024-04-14 18:19:53.397240 python_swidget-1.2.0/swidget/discovery.py
+-rw-r--r--   0        0        0       79 2023-01-11 19:11:12.359430 python_swidget-1.2.0/swidget/exceptions.py
+-rw-r--r--   0        0        0     4591 2024-04-10 14:24:43.935014 python_swidget-1.2.0/swidget/provision.py
+-rw-r--r--   0        0        0        0 2023-01-11 19:11:12.359430 python_swidget-1.2.0/swidget/py.typed
+-rw-r--r--   0        0        0    22143 2024-04-26 14:40:11.998055 python_swidget-1.2.0/swidget/swidgetdevice.py
+-rw-r--r--   0        0        0     1969 2024-04-26 14:40:11.998055 python_swidget-1.2.0/swidget/swidgetdimmer.py
+-rw-r--r--   0        0        0      402 2024-04-10 14:24:43.935014 python_swidget-1.2.0/swidget/swidgetoutlet.py
+-rw-r--r--   0        0        0      402 2024-04-14 18:19:53.397240 python_swidget-1.2.0/swidget/swidgetswitch.py
+-rw-r--r--   0        0        0      820 2024-04-14 18:19:53.397240 python_swidget-1.2.0/swidget/swidgettimerswitch.py
+-rw-r--r--   0        0        0     5774 2024-04-26 14:40:11.998055 python_swidget-1.2.0/swidget/websocket.py
+-rw-r--r--   0        0        0     1853 1970-01-01 00:00:00.000000 python_swidget-1.2.0/PKG-INFO
```

### Comparing `python_swidget-1.0.3/README.md` & `python_swidget-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python_swidget-1.0.3/pyproject.toml` & `python_swidget-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-swidget"
-version = "1.0.3"
+version = "1.2.0"
 description = "Python API for Swidget smart devices"
 license = "GPL-3.0-or-later"
 authors = ["Swidget"]
 repository = "https://github.com/swidget/python-swidget"
 readme = "README.md"
 packages = [
   { include = "swidget" }
```

### Comparing `python_swidget-1.0.3/swidget/__init__.py` & `python_swidget-1.2.0/swidget/__init__.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.0.3/swidget/cli.py` & `python_swidget-1.2.0/swidget/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,16 +112,16 @@
 @click.option("--secret_key", prompt=True, hide_input=True)
 @click.option("--friendly_name", prompt=True, hide_input=False)
 def join(ssid, network_password, secret_key, friendly_name):
     """Join the given wifi network."""
     confirmation = click.prompt(f"Are you connected to a wifi network that stars with the name 'Swidget-' (y/n)")
     if confirmation == "y":
         click.echo(f"Asking the device to connect to network {ssid}..")
-        # def provision_wifi(ssid, network_password, token_name, secret_key, friendly_name):
         provision_wifi(friendly_name, ssid, network_password, secret_key)
+        click.echo(f"Disconnect from the `swidget` network and connect back your main WiFi network")
         return True
     else:
         click.echo("Not provisioning wifi")
         return False
 
 
 @cli.command()
@@ -160,15 +160,15 @@
 
     click.echo(click.style("\t== Generic information ==", bold=True))
     click.echo(f"\tHardware:     {dev.hw_info['model']}")
     click.echo(f"\tSoftware:     {dev.hw_info['version']}")
     click.echo(f"\tMAC (rssi):   {dev.mac_address} ({dev.rssi})")
 
     click.echo(click.style("\n\t== Current State ==", bold=True))
-    realtime_values = await dev.realtime_values
+    realtime_values = dev.realtime_values
     for info_name, info_data in realtime_values.items():
         if isinstance(info_data, list):
             click.echo(f"\t{info_name}:")
             for item in info_data:
                 click.echo(f"\t\t{item}")
         else:
             click.echo(f"\t{info_name}: {info_data}")
@@ -259,30 +259,30 @@
 
 
 @cli.command()
 @pass_dev
 async def check_for_updates(dev: SwidgetDevice):
     click.echo("Contacting Swidget servers to fetch for updates...")
     available_updates = await dev.check_for_updates()
-    if len(available_updates['updates']) == 0:
+    if len(available_updates) == 0:
         click.echo("No available updates")
     else:
         click.echo("The following versions are available to update to")
-        for version in available_updates['updates']:
+        for version in available_updates:
             click.echo(click.style(f"\t+ {version}", fg="green"))
 
 
 @cli.command()
 @click.option("--version", required=False)
 @pass_dev
 async def upgrade(dev: SwidgetDevice, version: str):
     if version is None:
         click.echo("Contacting Swidget servers to fetch for latest version")
         available_updates = await dev.check_for_updates()
-        if len(available_updates['updates']) == 0:
+        if len(available_updates) == 0:
             click.echo("No available updates")
         else:
             version = available_updates[-1]
     click.echo(f"Upgrading to version: {version}")
     response = await dev.update_version(version)
     click.echo(response)
```

### Comparing `python_swidget-1.0.3/swidget/discovery.py` & `python_swidget-1.2.0/swidget/discovery.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.0.3/swidget/provision.py` & `python_swidget-1.2.0/swidget/provision.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.0.3/swidget/swidgetdevice.py` & `python_swidget-1.2.0/swidget/swidgetdevice.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import logging
 import time
+from types import TracebackType
 
 from aiohttp import ClientSession, TCPConnector
-import asyncio
+from collections.abc import Callable
 from enum import Enum
 from typing import Any, Dict, List
 
 from .exceptions import SwidgetException
 from .websocket import SwidgetWebsocket
 
 _LOGGER = logging.getLogger(__name__)
@@ -19,38 +20,73 @@
     Outlet = "outlet"
     Switch = "switch"
     TimerSwitch = "pana_switch"
     RelaySwitch = "relay_switch"
     Unknown = -1
 
 
+class InsertType(Enum):
+    """Insert type enum."""
+    USB = "USB"
+    THM = "TEMP HUMI MOTION"
+    TH = "TEMP HUMI"
+    AQ = "AIR QUALITY"
+    GL = "GUIDE LIGHT"
+    PO = "POWER OUT"
+    Unknown = -1
+
+
+class SelfDiagnosticErrorCodes(Enum):
+    """Self-Diagnostic error codes"""
+    UNUSED = 0
+    AQ = 1
+    GUIDELIGHT = 2
+    LIGHT_SENSOR = 3
+    MOTION = 4
+    POWER_OUT = 5
+    PRESSURE = 6
+    TEMP = 7
+    USB = 8
+    VIBRATION = 9
+    VIDEO = 10
+    ADVANCED_GL = 11
+    HUMI = 12
+    CO2 = 13
+    PART_MATTER = 14
+
+
 class SwidgetDevice:
     def __init__(self, host, token_name, secret_key, use_https=True, use_websockets=True) -> None:
         self.token_name = token_name
         self.ip_address = host
         self.use_https = use_https
         self.uri_scheme = 'https' if self.use_https is True else 'http'
         self.secret_key = secret_key
         self.use_websockets = use_websockets
         self.device_type = DeviceType.Unknown
         self._friendly_name = "Unknown Swidget Device"
         self.assemblies: Dict[Any, Any] = dict()
+        self._subscribers: Callable[[Dict[str, Any]], Any] = list()
         headers = {self.token_name: self.secret_key,
                    'Connection': 'keep-alive'}
         connector = TCPConnector(verify_ssl=False, force_close=True)
         self._session = ClientSession(headers=headers, connector=connector)
         self._last_update: int = 0
         if self.use_websockets:
             self._websocket = SwidgetWebsocket(
                 host=self.ip_address,
                 token_name=self.token_name,
                 secret_key=self.secret_key,
                 callback=self.message_callback,
                 session=self._session)
 
+    @property
+    def connected(self) -> bool:
+        return self._websocket.connected
+
     def get_websocket(self) -> SwidgetWebsocket | None:
         if self.use_websockets:
             return self._websocket
         return None
 
     def set_countdown_timer(self, minutes) -> Any:
         raise NotImplementedError()
@@ -73,25 +109,45 @@
         if hasattr(self, '_websocket'):
             await self._websocket.close()
         await self._session.close()
 
     async def close(self) -> None:
         await self.stop()
 
+    async def add_event_callback(self, callback: Callable[[Dict, Any], None],) -> bool:
+        for c in self._subscribers:
+            if c == callback:
+                _LOGGER.warn(f"Callback has already been added, not adding the same callback function again")
+                return False
+        self._subscribers.append(callback)
+        return True
+
+    async def remove_event_callback(self, callback: Callable[[Dict, Any], None],) -> bool:
+        if callback in self._subscribers:
+            self._subscribers.remove(callback)
+            return True
+        return False
+
     async def message_callback(self, message) -> None:
         """Entrypoint for a websocket callback"""
         _LOGGER.debug("SwidgetDevice.message_callback() called")
         if message["request_id"] == "summary":
             _LOGGER.debug("Calling SwidgetDevice.process_summary()")
             await self.process_summary(message)
         elif message["request_id"] == "state" or message["request_id"] == "DYNAMIC_UPDATE" or message["request_id"] == "command":
             _LOGGER.debug("Calling SwidgetDevice.process_state()")
             await self.process_state(message)
         else:
             _LOGGER.error(f"Unknown message type from websocket. Type given was: {message["request_id"]}")
+        await self.signal_callbacks(message)
+
+    async def signal_callbacks(self, message):
+        _LOGGER.debug("SwidgetDevice.signal_callsbacks() called")
+        for callback in self._subscribers:
+            await callback(message)
 
     async def get_summary(self) -> None:
         """Get a summary of the device over HTTP"""
         _LOGGER.debug("SwidgetDevice.get_summary() called")
         if self.use_websockets:
             _LOGGER.debug("In websocket mode. Sending get_summary() command over websocket")
             await self._websocket.send_str(json.dumps({"type": "summary", "request_id": "summary"}))
@@ -209,28 +265,30 @@
             ) as response:
                 state = await response.json()
 
             # Do a hard set of the new state of the device. May change this in the future
             function_value = state[assembly]["components"][component][function]
             self.assemblies[assembly].components[component].functions[function] = function_value  # fmt: skip
 
-    async def ping(self) -> int | SwidgetException:
+    async def ping(self) -> bool:
         """Ping the device to ensure it's devices
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
         """
         _LOGGER.debug("SwidgetDevice.ping() called")
         try:
             async with self._session.get(
                 url=f"{self.uri_scheme}://{self.ip_address}/ping",
                 ssl=False
             ) as response:
-                return response.status
+                if response.status == 200:
+                    return True
+                return False
         except:
-            raise SwidgetException
+            return False
 
     async def blink(self) -> Any:
         """Make the device LED blink
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
         """
         _LOGGER.debug("SwidgetDevice.blink() called")
@@ -250,15 +308,17 @@
         """
         _LOGGER.debug("SwidgetDevice.enable_debug_server() called")
         try:
             async with self._session.get(
                 url=f"{self.uri_scheme}://{self.ip_address}/debug?x-secret-key={self.secret_key}",
                 ssl=False
             ) as response:
-                return await response.json()
+                if response.status == 200:
+                    return True
+                return False
         except:
             raise SwidgetException
 
     async def factory_reset(self) -> Any:
         """Factory reset the Swidget device
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
@@ -280,33 +340,37 @@
         """
         try:
 
             async with self._session.get(
                 url=f"{self.uri_scheme}://{self.ip_address}/api/v1/update",
                 ssl=False
             ) as response:
-                return await response.json()
+                newer_versions = await response.json()
+                return sorted(newer_versions['updates'])
         except:
             raise SwidgetException
 
     async def update_version(self, version) -> Any:
         """Tell the device to download and apply an update
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
         """
         try:
             data = {
                 "version": version
             }
             async with self._session.post(
-                url=f"{self.uri_scheme}://{self.ip_address}/api/v1/update",
+                url=f"{self.uri_scheme}://{self.ip_address}/api/v1/update/version",
                 ssl=False,
                 data=json.dumps(data)
             ) as response:
-                return await response.json()
+                result = await response.status
+                if result == 200:
+                    return True
+                return False
         except:
             raise SwidgetException
 
     @property
     def hw_info(self) -> Dict:
         """
         Return hardware information.
@@ -424,53 +488,78 @@
     def friendly_name(self) -> str:
         """Return a friendly description of the device"""
         return self._friendly_name
 
     @property  # type: ignore
     def is_on(self) -> bool:
         """Return whether device is on."""
+        _LOGGER.debug("SwidgetDevice.is_on called")
         dimmer_state = self.assemblies['host'].components["0"].functions['toggle']["state"]
         if dimmer_state == "on":
             return True
         return False
 
     async def turn_on(self) -> None:
         """Turn the device on."""
         _LOGGER.debug("SwidgetDevice.turn_on() called")
+        self.assemblies['host'].components["0"].functions['toggle']["state"] = "on"
         await self.send_command(
             assembly="host", component="0", function="toggle", command={"state": "on"}
         )
 
     async def turn_off(self) -> None:
         """Turn the device off."""
         _LOGGER.debug("SwidgetDevice.turn_off() called")
+        self.assemblies['host'].components["0"].functions['toggle']["state"] = "off"
         await self.send_command(
             assembly="host", component="0", function="toggle", command={"state": "off"}
         )
 
     async def turn_on_usb_insert(self) -> None:
         """Turn the USB insert on."""
+        _LOGGER.debug("SwidgetDevice.turn_on_usb_insert() called")
+        self.assemblies['insert'].components["usb"].functions['toggle']["state"] = "on"
         await self.send_command(
             assembly="insert", component="usb", function="toggle", command={"state": "on"}
         )
 
     async def turn_off_usb_insert(self) -> None:
         """Turn the USB insert off."""
+        _LOGGER.debug("SwidgetDevice.turn_off_usb_insert() called")
+        self.assemblies['insert'].components["usb"].functions['toggle']["state"] = "off"
         await self.send_command(
             assembly="insert", component="usb", function="toggle", command={"state": "off"}
         )
 
     @property  # type: ignore
     def usb_is_on(self) -> bool:
         """Return whether USB is on."""
+        _LOGGER.debug("SwidgetDevice.usb_is_on called")
         usb_state = self.assemblies['insert'].components["usb"].functions['toggle']["state"]
         if usb_state == "on":
             return True
         return False
 
+    async def __aenter__(self) -> "SwidgetDevice":
+        """Initialize and connect the Swidget Websocket client."""
+        await self.connect()
+        return self
+
+    async def __aexit__(
+        self, exc_type: Exception, exc_value: str, traceback: TracebackType
+    ) -> None:
+        """Disconnect from the websocket."""
+        await self.disconnect()
+
+    def __repr__(self) -> str:
+        """Return the representation."""
+        url = self.connection.ws_server_url
+        prefix = "" if self.connection.connected else "not "
+        return f"{type(self).__name__}(ws_server_url={url!r}, {prefix}connected)"
+
     def __repr__(self) -> str:
         if self._last_update == 0:
             return f"<{self.device_type} at {self.ip_address} - update() needed>"
         return f"<{self.device_type} model {self.model} at {self.ip_address}>"
 
 
 class SwidgetAssembly:
```

### Comparing `python_swidget-1.0.3/swidget/swidgetdimmer.py` & `python_swidget-1.2.0/swidget/swidgetdimmer.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,39 +9,42 @@
 _LOGGER = logging.getLogger(__name__)
 
 
 class SwidgetDimmer(SwidgetDevice):
 
     def __init__(self, host,  token_name: str, secret_key: str, use_https: bool, use_websockets: bool) -> None:
         super().__init__(host=host, token_name=token_name, secret_key=secret_key, use_https=use_https, use_websockets=use_websockets)
-        self._device_type = "dimmer"
+        self._device_type = DeviceType.Dimmer
 
     @property  # type: ignore
     def brightness(self) -> int:
         """Return current brightness on dimmers.
 
         Will return a range between 0 - 100.
         """
+        _LOGGER.debug("SwidgetDimmer.brightness called")
         if not self.is_dimmable:
             raise SwidgetException("Device is not dimmable.")
         try:
             return self.assemblies['host'].components["0"].functions["level"]["now"]
         except KeyError:
             return self.assemblies['host'].components["0"].functions["level"]["default"]
 
     async def set_brightness(self, brightness) -> None:
         """Set the brightness of the device."""
-        _LOGGER.debug("SwidgetDimmer.set_brightness() called")
+        _LOGGER.debug("SwidgetDimmer.set_brightness() called with brightness: {brightness}")
+        self.assemblies['host'].components["0"].functions["level"]["now"] = brightness
         await self.send_command(
             assembly="host", component="0", function="level", command={"now": brightness}
         )
 
     async def set_default_brightness(self, brightness) -> None:
-        _LOGGER.debug("SwidgetDimmer.set_default_brightness() called")
+        _LOGGER.debug("SwidgetDimmer.set_default_brightness() called with brightness: {brightness}")
         await self.send_command(
             assembly="host", component="0", function="level", command={"default": brightness}
         )
 
     @property  # type: ignore
     def is_dimmable(self) -> bool:
         """Whether the switch supports brightness changes."""
+        _LOGGER.debug("SwidgetDimmer.is_dimmable() called")
         return True
```

### Comparing `python_swidget-1.0.3/swidget/swidgettimerswitch.py` & `python_swidget-1.2.0/swidget/swidgettimerswitch.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.0.3/swidget/websocket.py` & `python_swidget-1.2.0/swidget/websocket.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import aiohttp
 from aiohttp import ClientWebSocketResponse, WSMsgType
 import logging
 import socket
+from typing import Any
 
 _LOGGER = logging.getLogger(__name__)
 
 
 async def cancel_task(*tasks: asyncio.Task | None) -> None:
     """Cancel task(s)."""
     for task in tasks:
@@ -65,18 +66,22 @@
         _LOGGER.debug("websocket.connect() called")
         """Create a new connection and, optionally, start the monitor."""
         await cancel_task(self._receiver_task)
         if self.connected:
             _LOGGER.debug("Websocket already connected")
             return
 
+        if self._client is not None:
+            raise ConnectionError("Already connected")
+
         if not self.session:
-            raise
+            raise ConnectionError("No aiohttp session available")
 
         try:
+            _LOGGER.debug("Trying to connect")
             self._client = await self.session.ws_connect(url=self.uri, headers=self.headers, verify_ssl=self._verify_ssl, heartbeat=30)
             _LOGGER.debug("Websocket now connected")
         except aiohttp.WSServerHandshakeError as handshake_error:
             _LOGGER.error(f"Error occurred during websocket handshake: {handshake_error}")
             raise
         except aiohttp.ClientConnectionError as connection_error:
             _LOGGER.error(f"Error connecting to the websocket server: {connection_error}")
@@ -87,21 +92,26 @@
         except Exception as e:
             _LOGGER.error(f"An unexpected error occurred: {e}")
             raise
         self._receiver_task = asyncio.ensure_future(self.listen())
 
     async def close(self) -> None:
         _LOGGER.debug("websocket.close() called")
-        if not self._client or not self.connected:
-            return
-        await self._client.close()
+        if self._client is not None and not self._client.closed:
+            await self._client.close()
+        self._client = None
+
+    async def disconnect(self) -> None:
+        await self.close()
 
     async def send_str(self, message):
         """Send a message through the websocket."""
         _LOGGER.debug("websocket.send_str() called")
+        if not self.connected:
+            raise ConnectionError
         message = str(message)
         _LOGGER.debug(f"Sending messsage over websocket: {message}")
         await self._client.send_str(f'{message}')
 
     async def listen(self):
         _LOGGER.debug("websocket.listen() called")
         if not self._client or not self.connected:
@@ -111,15 +121,47 @@
             message = await self._client.receive()
 
             if message.type == aiohttp.WSMsgType.ERROR:
                 raise
 
             if message.type == aiohttp.WSMsgType.TEXT:
                 message_data = message.json()
+                _LOGGER.debug(f"Received from websocket: {message_data}")
                 await self.callback(message_data)
 
             if message.type in (
                 aiohttp.WSMsgType.CLOSE,
                 aiohttp.WSMsgType.CLOSED,
                 aiohttp.WSMsgType.CLOSING,
             ):
-                _LOGGER.debug("Connection to the Swidget WebSocket on has been closed")
+                _LOGGER.error("Connection to the Swidget WebSocket on has been closed")
+
+    async def receive_message_or_raise(self) -> Any:
+        """Receive ONE (raw) message or raise."""
+        assert self._ws_client
+        ws_msg = await self._ws_client.receive()
+
+        if ws_msg.type in (WSMsgType.CLOSE, WSMsgType.CLOSED, WSMsgType.CLOSING):
+            raise ConnectionError("Connection was closed.")
+
+        if ws_msg.type == WSMsgType.ERROR:
+            raise ConnectionError
+
+        if ws_msg.type != WSMsgType.TEXT:
+            raise ValueError(
+                f"Received non-Text message: {ws_msg.type}: {ws_msg.data}"
+            )
+
+        try:
+            msg = ws_msg.json()
+        except TypeError as err:
+            raise TypeError(f"Received unsupported JSON: {err}") from err
+        except ValueError as err:
+            raise ValueError("Received invalid JSON.") from err
+
+        _LOGGER.debug(f"Received message:\n{msg}\n")
+        return msg
+
+    def __repr__(self) -> str:
+        """Return the representation."""
+        prefix = "" if self.connected else "not "
+        return f"{type(self).__name__}(ws_server_url={self.host}, {prefix}connected)"
```

### Comparing `python_swidget-1.0.3/PKG-INFO` & `python_swidget-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-swidget
-Version: 1.0.3
+Version: 1.2.0
 Summary: Python API for Swidget smart devices
 Home-page: https://github.com/swidget/python-swidget
 License: GPL-3.0-or-later
 Author: Swidget
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

