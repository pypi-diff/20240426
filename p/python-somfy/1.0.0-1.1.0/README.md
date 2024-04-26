# Comparing `tmp/python_somfy-1.0.0.tar.gz` & `tmp/python_somfy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_somfy-1.0.0.tar", last modified: Sat Apr 20 10:23:29 2024, max compression
+gzip compressed data, was "python_somfy-1.1.0.tar", last modified: Fri Apr 26 04:05:13 2024, max compression
```

## Comparing `python_somfy-1.0.0.tar` & `python_somfy-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:23:29.085619 python_somfy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 10:23:25.000000 python_somfy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-20 10:23:29.085619 python_somfy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-20 10:23:25.000000 python_somfy-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-20 10:23:25.000000 python_somfy-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:23:29.085619 python_somfy-1.0.0/python_somfy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-20 10:23:29.000000 python_somfy-1.0.0/python_somfy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-20 10:23:29.000000 python_somfy-1.0.0/python_somfy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 10:23:29.000000 python_somfy-1.0.0/python_somfy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 10:23:28.000000 python_somfy-1.0.0/python_somfy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-20 10:23:29.000000 python_somfy-1.0.0/python_somfy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 10:23:29.000000 python_somfy-1.0.0/python_somfy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-20 10:23:29.089619 python_somfy-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:23:29.085619 python_somfy-1.0.0/somfy/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-20 10:23:25.000000 python_somfy-1.0.0/somfy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10555 2024-04-20 10:23:25.000000 python_somfy-1.0.0/somfy/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-20 10:23:25.000000 python_somfy-1.0.0/somfy/enumutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-20 10:23:25.000000 python_somfy-1.0.0/somfy/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-04-20 10:23:25.000000 python_somfy-1.0.0/somfy/payloads.py
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-20 10:23:25.000000 python_somfy-1.0.0/somfy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-20 10:23:25.000000 python_somfy-1.0.0/somfy/recognizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-20 10:23:25.000000 python_somfy-1.0.0/somfy/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:23:29.085619 python_somfy-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-04-20 10:23:25.000000 python_somfy-1.0.0/tests/test_decoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:05:13.252845 python_somfy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 04:05:08.000000 python_somfy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-26 04:05:13.252845 python_somfy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-26 04:05:08.000000 python_somfy-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 04:05:08.000000 python_somfy-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:05:13.252845 python_somfy-1.1.0/python_somfy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-26 04:05:13.252845 python_somfy-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:05:13.248845 python_somfy-1.1.0/somfy/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16043 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/enumutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22061 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:05:13.252845 python_somfy-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-04-26 04:05:08.000000 python_somfy-1.1.0/tests/test_decoding.py
```

### Comparing `python_somfy-1.0.0/LICENSE` & `python_somfy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_somfy-1.0.0/PKG-INFO` & `python_somfy-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: python-somfy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python library for local control of Somfy SDN shades
 Home-page: https://github.com/Cyberax/py-somfy-sdn
 Author: Aleksei Besogonov
 Author-email: b@alex.net
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Cyberax/py-somfy-sdn
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.11
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing-extensions; python_version < "3.8"
 
 # Somfy SDN protocol support
 
 This library implements Somfy SDN protocol used to control Somfy RS-485 connected blinds and shades. 
@@ -27,29 +27,31 @@
 
 # Using the library
 
 The library supports both directly-connected RS-485 adapters (typically implemented as USB-serial adapters), and
 connections via Ethernet-to-Serial converters. The library properly implements the timing restrictions specified
 in the SDN Integration Guide, with full `asyncio` support.
 
-To use the library, create a channel, a connector, and then exchange the messages:
+To use the library, create a connection factory, a connector, and then exchange the messages:
 
 ```python
-from somfy import SocketChannel
-ch = SocketChannel(host=host, port=port)
-async with ch:
-    async with SomfyConnector(ch) as conn:
-        await conn.do_exchange(...)
-        await conn.do_exchange(...)
-        await conn.do_exchange(...)
+from somfy import SocketConnectionFactory, SomfyConnector
+ch = SocketConnectionFactory(host=host, port=port)
+async with SomfyConnector(ch) as conn:
+    await conn.exchange(...)
+    await conn.exchange(...)
+    await conn.exchange(...)
 ```
 
 The channel (socket or serial) is physically opened in the context manager's `__aenter__` and freed in the `__aexit__`,
-there is no support for reconnection. If the socket is closed or the serial device becomes unavailable, you need to
-close the `SomfyConnector`, `Channel`, and then create new ones.
+there is no support for reconnection. Alternatively, `start` and `stop` methods can be used to control the connection. 
+
+If the socket is closed or the serial device becomes unavailable, you need to close the `SomfyConnector`,
+and then create a new one. Alternatively, you can use automatically reconnecting `ReconnectingSomfyConnector`. It
+will automatically reconnect the channel if it's closed, but it will NOT retry any failed `exchange` calls.
 
 `SomfyConnector` is stateless, but it launches a background task that drains the data from the SDN bus. You can
 optionally specify a `sniffer_callback` that will be called each time the "drainer" task recognizes a valid SDN 
 message. The drainer task is paused during the message exchanges.
 
 # Tools
```

### Comparing `python_somfy-1.0.0/README.md` & `python_somfy-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 
 # Using the library
 
 The library supports both directly-connected RS-485 adapters (typically implemented as USB-serial adapters), and
 connections via Ethernet-to-Serial converters. The library properly implements the timing restrictions specified
 in the SDN Integration Guide, with full `asyncio` support.
 
-To use the library, create a channel, a connector, and then exchange the messages:
+To use the library, create a connection factory, a connector, and then exchange the messages:
 
 ```python
-from somfy import SocketChannel
-ch = SocketChannel(host=host, port=port)
-async with ch:
-    async with SomfyConnector(ch) as conn:
-        await conn.do_exchange(...)
-        await conn.do_exchange(...)
-        await conn.do_exchange(...)
+from somfy import SocketConnectionFactory, SomfyConnector
+ch = SocketConnectionFactory(host=host, port=port)
+async with SomfyConnector(ch) as conn:
+    await conn.exchange(...)
+    await conn.exchange(...)
+    await conn.exchange(...)
 ```
 
 The channel (socket or serial) is physically opened in the context manager's `__aenter__` and freed in the `__aexit__`,
-there is no support for reconnection. If the socket is closed or the serial device becomes unavailable, you need to
-close the `SomfyConnector`, `Channel`, and then create new ones.
+there is no support for reconnection. Alternatively, `start` and `stop` methods can be used to control the connection. 
+
+If the socket is closed or the serial device becomes unavailable, you need to close the `SomfyConnector`,
+and then create a new one. Alternatively, you can use automatically reconnecting `ReconnectingSomfyConnector`. It
+will automatically reconnect the channel if it's closed, but it will NOT retry any failed `exchange` calls.
 
 `SomfyConnector` is stateless, but it launches a background task that drains the data from the SDN bus. You can
 optionally specify a `sniffer_callback` that will be called each time the "drainer" task recognizes a valid SDN 
 message. The drainer task is paused during the message exchanges.
 
 # Tools
 
@@ -113,8 +115,8 @@
 interval between messages transmitted by the master node is 25ms. The reply timeout for devices is 280ms.
 
 The node addresses are 3 byte-long. The broadcast address ix `FFFFFF`, the MASTER node is typically `7F7F7F`. A typical 
 exchange starts with `SET/GET_....` message sent by the MASTER node, to which the destination node (or nodes) reply 
 with the appropriate `POST_...` messages.
 
 The format of the message serialization is documented in `somfy/messages.py`. One thing to note, is that message bytes
-are bitwise-inverted prior to computing the checksum and sending them.
+are bitwise-inverted prior to computing the checksum and sending them.
```

### Comparing `python_somfy-1.0.0/python_somfy.egg-info/PKG-INFO` & `python_somfy-1.1.0/python_somfy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: python-somfy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python library for local control of Somfy SDN shades
 Home-page: https://github.com/Cyberax/py-somfy-sdn
 Author: Aleksei Besogonov
 Author-email: b@alex.net
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Cyberax/py-somfy-sdn
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.11
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing-extensions; python_version < "3.8"
 
 # Somfy SDN protocol support
 
 This library implements Somfy SDN protocol used to control Somfy RS-485 connected blinds and shades. 
@@ -27,29 +27,31 @@
 
 # Using the library
 
 The library supports both directly-connected RS-485 adapters (typically implemented as USB-serial adapters), and
 connections via Ethernet-to-Serial converters. The library properly implements the timing restrictions specified
 in the SDN Integration Guide, with full `asyncio` support.
 
-To use the library, create a channel, a connector, and then exchange the messages:
+To use the library, create a connection factory, a connector, and then exchange the messages:
 
 ```python
-from somfy import SocketChannel
-ch = SocketChannel(host=host, port=port)
-async with ch:
-    async with SomfyConnector(ch) as conn:
-        await conn.do_exchange(...)
-        await conn.do_exchange(...)
-        await conn.do_exchange(...)
+from somfy import SocketConnectionFactory, SomfyConnector
+ch = SocketConnectionFactory(host=host, port=port)
+async with SomfyConnector(ch) as conn:
+    await conn.exchange(...)
+    await conn.exchange(...)
+    await conn.exchange(...)
 ```
 
 The channel (socket or serial) is physically opened in the context manager's `__aenter__` and freed in the `__aexit__`,
-there is no support for reconnection. If the socket is closed or the serial device becomes unavailable, you need to
-close the `SomfyConnector`, `Channel`, and then create new ones.
+there is no support for reconnection. Alternatively, `start` and `stop` methods can be used to control the connection. 
+
+If the socket is closed or the serial device becomes unavailable, you need to close the `SomfyConnector`,
+and then create a new one. Alternatively, you can use automatically reconnecting `ReconnectingSomfyConnector`. It
+will automatically reconnect the channel if it's closed, but it will NOT retry any failed `exchange` calls.
 
 `SomfyConnector` is stateless, but it launches a background task that drains the data from the SDN bus. You can
 optionally specify a `sniffer_callback` that will be called each time the "drainer" task recognizes a valid SDN 
 message. The drainer task is paused during the message exchanges.
 
 # Tools
```

### Comparing `python_somfy-1.0.0/setup.cfg` & `python_somfy-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-somfy
-version = 1.0.0
+version = 1.1.0
 author = Aleksei Besogonov
 author_email = b@alex.net
 description = Python library for local control of Somfy SDN shades
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache-2.0
 platforms = any
@@ -21,15 +21,15 @@
 
 [options]
 zip_safe = False
 packages = find:
 requires = 
 	pyserial
 	pyserial-asyncio
-python_requires = >=3.11
+python_requires = >=3.12
 install_requires = 
 	typing-extensions;python_version<'3.8'
 
 [options.package_data]
 * = py.typed
 
 [flake8]
```

### Comparing `python_somfy-1.0.0/somfy/messages.py` & `python_somfy-1.1.0/somfy/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Messages specification
 from binascii import unhexlify
 from typing import List, Optional, Any
 
-from somfy.enumutils import EnumWithMissing, hex_enum
+from somfy.enumutils import enum_or_int, hex_enum, IntEnumWithStr
 
 
 # The destination flag. Only the matching devices will process the message if the flag is set.
-class NodeType(EnumWithMissing):
+class NodeType(IntEnumWithStr):
     TYPE_ALL = 0x00
     TYPE_30DC_SERIES = 0x02
     TYPE_RTS_TRANSMITTER = 0x05
     TYPE_GLYDEA = 0x06
     TYPE_50AC_SERIES = 0x07
     TYPE_50DC_SERIES = 0x08
     TYPE_40AC_SERIES = 0x09
 
 
 ########################################################################
 # SDN message types defined in the spec for window covers (DOC155888/2)
 ########################################################################
-class SomfyMessageId(EnumWithMissing):
+class SomfyMessageId(IntEnumWithStr):
     GET_NODE_ADDR = 0x40
     POST_NODE_ADDR = 0x60
 
     SET_GROUP_ADDR = 0x51
     GET_GROUP_ADDR = 0x41
     POST_GROUP_ADDR = 0x61
 
@@ -190,18 +190,18 @@
 # The 16-bit payload values (such as the pulse counts) are apparently sent in the LSB order.
 ####################################################################################################
 class SomfyMessage(object):
     def __init__(self, msgid: SomfyMessageId | int,
                  from_node_type: NodeType | int = NodeType.TYPE_ALL, from_addr: SomfyAddress = None,
                  to_node_type: NodeType | int = NodeType.TYPE_ALL, to_addr: SomfyAddress = None,
                  need_ack: bool = False, payload: SomfyPayload = SomfyPayload([])):
-        self.msgid = SomfyMessageId(msgid)
-        self.from_node_type = NodeType(from_node_type)
+        self.msgid = enum_or_int(SomfyMessageId, msgid)
+        self.from_node_type = enum_or_int(NodeType, from_node_type)
         self.from_addr = from_addr
-        self.to_node_type = NodeType(to_node_type)
+        self.to_node_type = enum_or_int(NodeType, to_node_type)
         self.to_addr = to_addr
         self.need_ack = need_ack
         self.payload = payload
 
     def serialize(self):
         content_data = self.payload.serialize()
         ack_flag = 0x80 if self.need_ack else 0x00
@@ -236,24 +236,24 @@
         checksum = SomfyMessage.compute_checksum(data[:-2])
         if checksum[0] != data[-2] or checksum[1] != data[-1]:
             return None  # Checksum mismatch
 
         # First, invert the data (except the checksum) to make parsing easier
         inverted = [~i & 0xFF for i in data[:-2]]
 
-        msg_id = SomfyMessageId(inverted[0])
+        msg_id = enum_or_int(SomfyMessageId, inverted[0])
 
         needs_ack = (inverted[1] & 0x80) != 0
         msg_len = inverted[1] & 0x7F  # Clear the ACK_REQUIRED bit
 
         if msg_len != len(data):
             return None  # The length field disagrees with the message length
 
-        from_node_type = NodeType(inverted[2] >> 4 & 0xF)
-        to_node_type = NodeType(inverted[2] & 0xF)
+        from_node_type = enum_or_int(NodeType, inverted[2] >> 4 & 0xF)
+        to_node_type = enum_or_int(NodeType, inverted[2] & 0xF)
 
         from_addr = SomfyAddress.parse_bytes(inverted[3:6])
         to_addr = SomfyAddress.parse_bytes(inverted[6:9])
 
         payload = inverted[9:]
         parsed_payload = attempt_to_parse_payload(msg_id, payload)
```

### Comparing `python_somfy-1.0.0/somfy/payloads.py` & `python_somfy-1.1.0/somfy/payloads.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ###############################################################################################
 # Typesafe wrappers for message payloads, based on the SDN Integration Guide
 # (and a bit of reverse engineering).
 ###############################################################################################
-from typing import Optional, List
+from typing import Optional, List, override
 
-from somfy.enumutils import EnumWithMissing
+from somfy.enumutils import enum_or_int, IntEnumWithStr
 from somfy.messages import SomfyPayload, SomfyMessageId, SomfyAddress, register_message_payloads
 
 
 class EmptyPayload(SomfyPayload):
     expected_lengths = [0]
 
     def __init__(self, *ignored, **ignored_kwargs):
@@ -20,40 +20,40 @@
 
     def get_group_index(self):
         return self.content[0]
 
     def get_group_id(self):
         return self.content[1] << 16 + self.content[2] << 8 + self.content[3]
 
-    # @override
+    @override
     def as_dict(self):
         return {"group_index": self.get_group_index(), "group_id": self.get_group_id()}
 
     @staticmethod
     def make(group_index: int, group_id: int) -> 'GroupAddrPayload':
         return GroupAddrPayload([group_index, group_id >> 16 & 0xFF, group_id >> 8 & 0xFF, group_id & 0xFF])
 
 
 class GroupIndexPayload(SomfyPayload):
     expected_lengths = [1]
 
     def get_group_index(self):
         return self.content[0]
 
-    # @override
+    @override
     def as_dict(self):
         return {"group_index": self.get_group_index()}
 
     @staticmethod
     def make(group_index: int) -> 'GroupIndexPayload':
         return GroupIndexPayload([group_index])
 
 
 # Some message processing fault reasons
-class SomfyNackReason(EnumWithMissing):
+class SomfyNackReason(IntEnumWithStr):
     NACK_DATA_OUT_OF_RANGE = 0x01
     NACK_UNKNOWN_MESSAGE = 0x10
     NACK_MESSAGE_LENGTH_ERROR = 0x11
     NACK_BUSY = 0xFF
 # Other NACK text codes that I gleaned from the Internet. Don't have numeric values yet.
 #     NACK_ACK
 #     NACK_RNG
@@ -69,23 +69,25 @@
 #     NACK_FEATURE_NOT_SUPPORTED
 #     NACK_IN_MOTION
 #     NACK_IN_SECURITY
 #     NACK_LAST_IP_REACHED
 #     NACK_THRESHOLD_REACHED
 #     NACK_LOW_PRIORITY
 #     NACK_WINK_IN_PROGRESS
+    NACK_IN_SECURITY = 0x27  # Thermal protection, obstacle detection, etc.
+    NACK_LAST_IP_REACHED = 0x28
 
 
 class NackPayload(SomfyPayload):
     expected_lengths = [1]
 
-    def get_nack_code(self) -> SomfyNackReason:
-        return SomfyNackReason(self.content[0])
+    def get_nack_code(self) -> SomfyNackReason | int:
+        return enum_or_int(SomfyNackReason, self.content[0])
 
-    # @override
+    @override
     def as_dict(self):
         return {"nack_code": self.get_nack_code()}
 
     @staticmethod
     def make(nack_code: SomfyNackReason | int) -> 'NackPayload':
         return NackPayload([int(nack_code)])
 
@@ -100,145 +102,146 @@
 
 class NodeLabelPayload(SomfyPayload):
     expected_lengths = [16]
 
     def get_label(self):
         return bytes(self.content).decode('utf-8').strip()
 
-    # @override
+    @override
     def as_dict(self):
         return {"label": self.get_label()}
 
     @staticmethod
     def make(label: str) -> 'NodeLabelPayload':
         label_bytes = label.encode('utf-8')
         if len(label_bytes) > 16:
             raise ValueError("Label too long")
         return NodeLabelPayload([b for b in label_bytes])
 
 
-class SomfyUIFunction(EnumWithMissing):
+class SomfyUIFunction(IntEnumWithStr):
     ENABLE = 0x0
     DISABLE = 0x1
 
 
-class SomfyUIIndex(EnumWithMissing):
+class SomfyUIIndex(IntEnumWithStr):
     ALL_CONTROLS = 0x0
     DCT_INPUT = 0x1
     LOCAL_STIMULI = 0x2
     LOCAL_RADIO = 0x03
     TOUCH_MOTION = 0x04
     LEDS = 0x05
 
 
 class SetLocalUIPayload(SomfyPayload):
     expected_lengths = [3]
 
-    def get_function(self) -> SomfyUIFunction:
-        return SomfyUIFunction(self.content[0])
+    def get_function(self) -> SomfyUIFunction | int:
+        return enum_or_int(SomfyUIFunction, self.content[0])
 
-    def get_ui_index(self) -> SomfyUIIndex:
-        return SomfyUIIndex(self.content[1])
+    def get_ui_index(self) -> SomfyUIIndex | int:
+        return enum_or_int(SomfyUIIndex, self.content[1])
 
     def get_priority(self) -> int:
         return self.content[2]
 
-    # @override
+    @override
     def as_dict(self):
         return {"function": self.get_function(), "ui_index": self.get_ui_index(), "priority": self.get_priority()}
 
     @staticmethod
-    def make(func: SomfyUIIndex, ui_index: SomfyUIIndex, priority: int) -> 'SetLocalUIPayload':
+    def make(func: SomfyUIFunction | int, ui_index: SomfyUIIndex | int, priority: int) -> 'SetLocalUIPayload':
         return SetLocalUIPayload([func, ui_index, priority])
 
 
 class GetLocalUIPayload(SomfyPayload):
     expected_lengths = [1]
 
-    def get_ui_index(self) -> SomfyUIIndex:
-        return SomfyUIIndex(self.content[0])
+    def get_ui_index(self) -> SomfyUIIndex | int:
+        return enum_or_int(SomfyUIIndex, self.content[0])
 
-    # @override
+    @override
     def as_dict(self):
         return {"ui_index": self.get_ui_index()}
 
     @staticmethod
-    def make(ui_index: SomfyUIIndex) -> 'GetLocalUIPayload':
+    def make(ui_index: SomfyUIIndex | int) -> 'GetLocalUIPayload':
         return GetLocalUIPayload([ui_index])
 
 
 class PostLocalUIPayload(SomfyPayload):
     expected_lengths = [5]
 
-    def get_function(self) -> SomfyUIFunction:
-        return SomfyUIFunction(self.content[0])
+    def get_function(self) -> SomfyUIFunction | int:
+        return enum_or_int(SomfyUIFunction, self.content[0])
 
     def get_source_addr(self) -> SomfyAddress:
         return SomfyAddress.parse_bytes(self.content[1:4])
 
     def get_priority(self) -> int:
         return self.content[4]
 
-    # @override
+    @override
     def as_dict(self):
         return {"function": self.get_function(),
                 "source_addr": self.get_source_addr(), "priority": self.get_priority()}
 
     @staticmethod
-    def make(func: SomfyUIFunction, source_address: SomfyAddress, priority: int) -> 'PostLocalUIPayload':
+    def make(func: SomfyUIFunction | int, source_address: SomfyAddress, priority: int) -> 'PostLocalUIPayload':
         return PostLocalUIPayload([func] + source_address.serialize() + [priority])
 
 
-class SomfyMotorIPFunction(EnumWithMissing):
+class SomfyMotorIPFunction(IntEnumWithStr):
     DELETE = 0x0
     SET_IP_AT_CURRENT = 0x01
     SET_IP_AT_SPECIFIED_PERCENT = 0x03  # Tilt value is ignored
     DIVIDE_INTO_EQUAL_RANGES = 0x04  # Position specifies the count of ranges, IP index and Tilt value are ignored
     SET_AT_CURRENT_POSITION_AND_ANGLE = 0x05  # Position and tilt value are ignored
     SET_AT_SPECIFIED_POSITION_AND_ANGLE_IN_PERCENTS = 0x0A
     SET_AT_SPECIFIED_POSITION_AND_ANGLE_IN_DEGREES = 0x0B
 
 
 class SetMotorIPPayload(SomfyPayload):
     expected_lengths = [4, 6]
 
     IP_POSITION_UNDEFINED = 0xFFFF
 
-    def get_function(self) -> SomfyMotorIPFunction:
-        return SomfyMotorIPFunction(self.content[0])
+    def get_function(self) -> SomfyMotorIPFunction | int:
+        return enum_or_int(SomfyMotorIPFunction, self.content[0])
 
     def get_ip_index(self) -> int:
         return self.content[1]
 
     def get_position(self) -> int:
         return self.content[3] << 8 | self.content[2]
 
     def get_angle(self) -> Optional[int]:
         if len(self.content) != 6:
             return None
         return self.content[5] << 8 | self.content[4]
 
-    # @override
+    @override
     def as_dict(self):
         return {"function": self.get_function(), "ip_index": self.get_ip_index(), "position": self.get_position(),
                 "angle": self.get_angle()}
 
     @staticmethod
-    def make(func: SomfyUIFunction, ip_index: int, position: int, angle: Optional[int]) -> 'SetMotorIPPayload':
+    def make(func: SomfyMotorIPFunction | int, ip_index: int, position: int,
+             angle: Optional[int]) -> 'SetMotorIPPayload':
         angle_list = [angle >> 8 & 0xFF, angle & 0xFF] if angle else []
         return SetMotorIPPayload([func, ip_index, position >> 8 & 0xFF, position & 0xFF] + angle_list)
 
 
 class GetMotorIPPayload(SomfyPayload):
     expected_lengths = [1]
 
     def get_ip_index(self):
         return self.content[0]
 
-    # @override
+    @override
     def as_dict(self):
         return {"ip_index": self.get_ip_index()}
 
     @staticmethod
     def make(ip_index: int) -> 'GetMotorIPPayload':
         return GetMotorIPPayload([ip_index])
 
@@ -257,15 +260,15 @@
 
     def get_angle(self) -> Optional[int]:
         if len(self.content) != 9:
             return None
         angle = self.content[8] << 8 | self.content[7]
         return angle
 
-    # @override
+    @override
     def as_dict(self):
         return {"ip_index": self.get_ip_index(), "position": self.get_position(), "angle": self.get_angle()}
 
     @staticmethod
     def make(ip_index: int, position: int, angle: Optional[int]) -> 'PostMotorIPPayload':
         angle_list = [0, 0, 0, angle & 0xFF, angle >> 8 & 0xFF] if angle else []
         return PostMotorIPPayload([ip_index, 0, 0, position] + angle_list)
@@ -279,47 +282,47 @@
 
     def get_down_speed_rpm(self) -> int:
         return self.content[1]
 
     def get_slow_speed_rpm(self) -> int:
         return self.content[2]
 
-    # @override
+    @override
     def as_dict(self):
         return {"up_speed_rpm": self.get_up_speed_rpm(), "down_speed_rpm": self.get_down_speed_rpm(),
                 "slow_speed_rpm": self.get_slow_speed_rpm()}
 
     @staticmethod
     def make(up_speed_rpm: int, down_speed_rpm: int, slow_speed_rpm: int) -> 'MotorSpeedPayload':
         return MotorSpeedPayload([up_speed_rpm, down_speed_rpm, slow_speed_rpm])
 
 
-class LockNetworkFunction(EnumWithMissing):
+class LockNetworkFunction(IntEnumWithStr):
     UNLOCK = 0x00
     LOCK = 0x01
     PRESERVE_LOCK_ON_POWER_CYCLE = 0x03  # Priority is ignored
     UNPRESERVE_LOCK_ON_POWER_CYCLE = 0x04  # Priority is ignored
 
 
 class SetNetworkLockPayload(SomfyPayload):
     expected_lengths = [2]
 
-    def get_function(self) -> LockNetworkFunction:
-        return LockNetworkFunction(self.content[0])
+    def get_function(self) -> LockNetworkFunction | int:
+        return enum_or_int(LockNetworkFunction, self.content[0])
 
     def get_priority(self) -> int:
         return self.content[1]
 
-    # @override
+    @override
     def as_dict(self):
         return {"function": self.get_function(), "priority": self.get_priority()}
 
     @staticmethod
-    def make(function: LockNetworkFunction, priority: int) -> 'SetNetworkLockPayload':
-        return SetNetworkLockPayload([function, priority])
+    def make(func: LockNetworkFunction | int, priority: int) -> 'SetNetworkLockPayload':
+        return SetNetworkLockPayload([func, priority])
 
 
 class PostNetworkLockPayload(SomfyPayload):
     expected_lengths = [6]
 
     def is_locked(self) -> bool:
         return self.content[0] != 0
@@ -329,68 +332,68 @@
 
     def get_priority(self) -> int:
         return self.content[4]
 
     def is_persistent_across_power_cycle(self) -> bool:
         return self.content[5] != 0
 
-    # @override
+    @override
     def as_dict(self):
         return {"is_locked": self.is_locked(), "lock_holder": self.get_lock_holder(), "priority": self.get_priority(),
                 "is_persistent_across_power_cycle": self.is_persistent_across_power_cycle()}
 
     @staticmethod
     def make(locked: bool, lock_holder: SomfyAddress, priority: int,
              persistent_across_power_cycle: bool) -> 'PostNetworkLockPayload':
         return PostNetworkLockPayload([int(locked), lock_holder.serialize(), priority,
                                        int(persistent_across_power_cycle)])
 
 
-class CtrlMoveToFunction(EnumWithMissing):
+class CtrlMoveToFunction(IntEnumWithStr):
     DOWN_LIMIT = 0x00  # Position and angle are ignored
     UP_LIMIT = 0x01  # Position and angle are ignored
     IP = 0x02  # Position contains the Intermediate Position index
     POSITION_PERCENT = 0x04  # Tilt is ignored
     POSITION_PERCENT_ANGLE_PERCENT = 0x0C
     POSITION_PERCENT_ANGLE_DEGREES = 0x0D
     CURRENT_POSITION_ANGLE_PERCENT = 0x0F  # Position is ignored
     CURRENT_POSITION_ANGLE_DEGREES = 0x10  # Position is ignored
 
 
 class CtrlMoveToPayload(SomfyPayload):
     expected_lengths = [4, 6]
 
-    def get_function(self) -> CtrlMoveToFunction:
-        return CtrlMoveToFunction(self.content[0])
+    def get_function(self) -> CtrlMoveToFunction | int:
+        return enum_or_int(CtrlMoveToFunction, self.content[0])
 
     def get_position(self) -> int:
         return self.content[2] << 8 | self.content[1]
 
     def get_angle(self) -> Optional[int]:
         if len(self.content) != 6:
             return None
         return self.content[5] << 8 | self.content[4]
 
-    # @override
+    @override
     def as_dict(self):
         return {"function": self.get_function(), "position": self.get_position(), "angle": self.get_angle()}
 
     @staticmethod
-    def make(func: CtrlMoveToFunction, position: int, angle: Optional[int] = None) -> 'CtrlMoveToPayload':
+    def make(func: CtrlMoveToFunction | int, position: int, angle: Optional[int] = None) -> 'CtrlMoveToPayload':
         angle_list = [angle & 0xFF, angle >> 8 & 0xFF] if angle else []
         return CtrlMoveToPayload([func, position & 0xFF, position >> 8 & 0xFF, 0] + angle_list)
 
 
 class CtrlStopPayload(SomfyPayload):
     expected_lengths = [1]
 
     def get_reserved(self) -> int:
         return self.content[0]
 
-    # @override
+    @override
     def as_dict(self):
         return {"reserved": self.get_reserved()}
 
     @staticmethod
     def make(reserved: int = 0) -> 'CtrlStopPayload':
         return CtrlStopPayload([reserved])
 
@@ -416,157 +419,157 @@
         return ip
 
     def get_tilt_degrees(self) -> Optional[int]:
         if len(self.content) != 11:
             return None
         return self.content[8] << 8 | self.content[7]
 
-    # @override
+    @override
     def as_dict(self):
         return {"position_pulses": self.get_position_pulses(), "position_percent": self.get_position_percent(),
                 "tilt_percent": self.get_tilt_percent(), "ip": self.get_ip(), "tilt_degrees": self.get_tilt_degrees()}
 
     @staticmethod
     def make(position_pulses: int, position_percent: int, tilt_percent: int,
              ip: int, tilt_degrees: Optional[int]) -> 'PostMotorPositionPayload':
         angle_list = [0, 0, tilt_degrees & 0xFF, tilt_degrees >> 8 & 0xFF, 0, 0] if tilt_degrees else []
         return PostMotorPositionPayload(
             [position_pulses & 0xFF, position_pulses >> 8 & 0xFF, position_percent, tilt_percent, ip] + angle_list)
 
 
-class MotorStatus(EnumWithMissing):
+class MotorStatus(IntEnumWithStr):
     STOPPED = 0x00
     RUNNING = 0x01
     BLOCKED = 0x02  # Blocked from movement by an obstacle or thermal protection
     LOCKED = 0x03  # Locked by another device
 
 
-class MotorDirection(EnumWithMissing):
+class MotorDirection(IntEnumWithStr):
     DOWN = 0x00
     UP = 0x01
     UNKNOWN = 0xFF
 
 
-class MotorCommandSource(EnumWithMissing):
+class MotorCommandSource(IntEnumWithStr):
     INTERNAL = 0x00  # Limit/IP/Position reached, Over-current, obstacle detection, thermal protection, ...
     NETWORK_MESSAGE = 0x01  # Any message received from the SDN bus
     LOCAL_UI = 0x02  # DCT, Local stimulus, local wireless
 
 
-class MotorStatusCause(EnumWithMissing):
+class MotorStatusCause(IntEnumWithStr):
     TARGET_REACHED = 0x00  # Successful completion of a command
     EXPLICIT_COMMAND = 0x01  # Network or Local UI command
     WINK = 0x02
     OBSTACLE_DETECTION = 0x20
     OVERCURRENT_PROTECTION = 0x21
     THERMAL_PROTECTION = 0x22
     RUNTIME_EXCEEDED = 0x30  # Continuous runtime exceeded limit
     TIMEOUT_EXCEEDED = 0x32  # When using CTRL_MOVE and more than 2min. elapsed
     POWER_CYCLE = 0xFF  # No command after startup
 
 
 class PostMotorStatusPayload(SomfyPayload):
     expected_lengths = [4]
 
-    def get_status(self) -> MotorStatus:
-        return MotorStatus(self.content[0])
+    def get_status(self) -> MotorStatus | int:
+        return enum_or_int(MotorStatus, self.content[0])
 
-    def get_direction(self) -> MotorDirection:
-        return MotorDirection(self.content[1])
+    def get_direction(self) -> MotorDirection | int:
+        return enum_or_int(MotorDirection, self.content[1])
 
-    def get_command_source(self) -> MotorCommandSource:
-        return MotorCommandSource(self.content[2])
+    def get_command_source(self) -> MotorCommandSource | int:
+        return enum_or_int(MotorCommandSource, self.content[2])
 
-    def get_status_cause(self) -> MotorStatusCause:
-        return MotorStatusCause(self.content[3])
+    def get_status_cause(self) -> MotorStatusCause | int:
+        return enum_or_int(MotorStatusCause, self.content[3])
 
-    # @override
+    @override
     def as_dict(self):
         return {"status": self.get_status(), "direction": self.get_direction(),
                 "command_source": self.get_command_source(), "status_cause": self.get_status_cause()}
 
     @staticmethod
-    def make(status: MotorStatus, direction: MotorDirection, source: MotorCommandSource,
-             cause: MotorStatusCause) -> 'PostMotorStatusPayload':
+    def make(status: MotorStatus | int, direction: MotorDirection | int, source: MotorCommandSource | int,
+             cause: MotorStatusCause | int) -> 'PostMotorStatusPayload':
         return PostMotorStatusPayload([status, direction, source, cause])
 
 
 #############################################################################################
 # Reverse-engineered payloads
 #############################################################################################
 
-class SomfyDirection(EnumWithMissing):
+class SomfyDirection(IntEnumWithStr):
     DOWN = 0x00
     UP = 0x01
 
 
 class CtrlMoveForcedPayload(SomfyPayload):
     expected_lengths = [3]
 
-    def get_direction(self) -> SomfyDirection:
-        return SomfyDirection(self.content[0])
+    def get_direction(self) -> SomfyDirection | int:
+        return enum_or_int(SomfyDirection, self.content[0])
 
     # The movement duration in the units of 10ms
     def get_tens_of_ms(self) -> int:
         return self.content[2] << 8 | self.content[1]
 
     def as_dict(self):
         return {"direction": self.get_direction(), "tens_of_ms": self.get_tens_of_ms()}
 
     @staticmethod
     def make(direction: int, tens_of_ms: int) -> 'CtrlMoveForcedPayload':
         return CtrlMoveForcedPayload([direction, tens_of_ms & 0xFF, tens_of_ms >> 8 & 0xFF])
 
 
-class RelativeMoveFunction(EnumWithMissing):
+class RelativeMoveFunction(IntEnumWithStr):
     MOVE_NEXT_IP_DOWN = 0x00
     MOVE_NEXT_IP_UP = 0x01
     MOVE_NUM_PULSES_DOWN = 0x02
     MOVE_NUM_PULSES_UP = 0x03
     MOVE_TENS_OF_MS_DOWN = 0x04
     MOVE_TENS_OF_MS_UP = 0x05
 
 
 class CtrlMoveRelativePayload(SomfyPayload):
     expected_lengths = [4]
 
-    def get_function(self) -> RelativeMoveFunction:
-        return RelativeMoveFunction(self.content[0])
+    def get_function(self) -> RelativeMoveFunction | int:
+        return enum_or_int(RelativeMoveFunction, self.content[0])
 
     def get_parameter(self) -> int:
         return self.content[2] >> 8 | self.content[1]
 
     def as_dict(self):
         return {"function": self.get_function(), "parameter": self.get_parameter()}
 
     @staticmethod
-    def make(function: RelativeMoveFunction, parameter: int) -> 'CtrlMoveRelativePayload':
-        return CtrlMoveRelativePayload([function, parameter & 0xFF, parameter >> 8 & 0xFF, 0])
+    def make(func: RelativeMoveFunction | int, parameter: int) -> 'CtrlMoveRelativePayload':
+        return CtrlMoveRelativePayload([func, parameter & 0xFF, parameter >> 8 & 0xFF, 0])
 
 
-class SetLimitsFunction(EnumWithMissing):
+class SetLimitsFunction(IntEnumWithStr):
     SET_AT_CURRENT = 0x01
     SET_AT_PULSE_COUNT = 0x02  # At the specified pulse count
     ADJUST_BY_TENS_OF_MS = 0x04  # Adjust up or down by N*10 milliseconds
     ADJUST_BY_PULSE_COUNT = 0x05  # Adjust up or down by N pulses
 
 
 class SetMotorLimitsPayload(SomfyPayload):
     expected_lengths = [4]
 
-    def get_function(self) -> SetLimitsFunction:
-        return SetLimitsFunction(self.content[0])
+    def get_function(self) -> SetLimitsFunction | int:
+        return enum_or_int(SetLimitsFunction, self.content[0])
 
-    def get_direction(self) -> SomfyDirection:
-        return SomfyDirection(self.content[1])
+    def get_direction(self) -> SomfyDirection | int:
+        return enum_or_int(SomfyDirection, self.content[1])
 
     def get_parameter(self) -> int:
         return self.content[3] << 8 | self.content[2]
 
-    # @override
+    @override
     def as_dict(self):
         return {"function": self.get_function(), "direction": self.get_direction(), "parameter": self.get_parameter()}
 
     @staticmethod
     def make(lower: int) -> 'SetMotorLimitsPayload':
         return SetMotorLimitsPayload([0, 0, lower & 0xFF, lower >> 8 & 0xFF])
 
@@ -576,39 +579,39 @@
 
     def get_reserved(self) -> int:
         return self.content[1] << 8 | self.content[0] & 0xFF
 
     def get_limit(self) -> int:
         return self.content[3] << 8 | self.content[2] & 0xFF
 
-    # @override
+    @override
     def as_dict(self):
         return {"reserved": self.get_reserved(), "limit": self.get_limit()}
 
     @staticmethod
     def make(limit: int) -> 'PostMotorLimitsPayload':
         return PostMotorLimitsPayload([0, 0, limit & 0xFF, limit >> 8 & 0xFF])
 
 
-class MotorRotationDirection(EnumWithMissing):
+class MotorRotationDirection(IntEnumWithStr):
     STANDARD = 0x00
     REVERSED = 0x01
 
 
 class MotorRotationDirectionPayload(SomfyPayload):
     expected_lengths = [1]
 
-    def get_direction(self) -> MotorRotationDirection:
-        return MotorRotationDirection(self.content[0])
+    def get_direction(self) -> MotorRotationDirection | int:
+        return enum_or_int(MotorRotationDirection, self.content[0])
 
     def as_dict(self):
         return {"direction": self.get_direction()}
 
     @staticmethod
-    def make(direction: MotorRotationDirection) -> 'MotorRotationDirectionPayload':
+    def make(direction: MotorRotationDirection | int) -> 'MotorRotationDirectionPayload':
         return MotorRotationDirectionPayload([direction])
 
 
 def register_documented_payloads():
     dp = dict[int, type]({
         SomfyMessageId.GET_NODE_ADDR: EmptyPayload,
         SomfyMessageId.POST_NODE_ADDR: EmptyPayload,
```

### Comparing `python_somfy-1.0.0/somfy/recognizer.py` & `python_somfy-1.1.0/somfy/recognizer.py`

 * *Files identical despite different names*

### Comparing `python_somfy-1.0.0/tests/test_decoding.py` & `python_somfy-1.1.0/tests/test_decoding.py`

 * *Files identical despite different names*

