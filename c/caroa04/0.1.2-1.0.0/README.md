# Comparing `tmp/caroa04-0.1.2.tar.gz` & `tmp/caroa04-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caroa04-0.1.2.tar", last modified: Mon Apr 15 08:20:45 2024, max compression
+gzip compressed data, was "caroa04-1.0.0.tar", last modified: Fri Apr 26 12:38:51 2024, max compression
```

## Comparing `caroa04-0.1.2.tar` & `caroa04-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 08:20:45.072304 caroa04-0.1.2/
--rw-rw-rw-   0        0        0      179 2024-04-14 17:26:49.000000 caroa04-0.1.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3870 2024-04-14 17:26:49.000000 caroa04-0.1.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2024-04-14 17:26:49.000000 caroa04-0.1.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1102 2024-04-14 17:26:49.000000 caroa04-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      273 2024-04-14 17:26:49.000000 caroa04-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4025 2024-04-15 08:20:45.071306 caroa04-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2874 2024-04-15 08:20:21.000000 caroa04-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-15 08:20:45.054492 caroa04-0.1.2/docs/
--rw-rw-rw-   0        0        0      628 2024-04-14 17:26:49.000000 caroa04-0.1.2/docs/Makefile
--rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-0.1.2/docs/authors.rst
--rw-rw-rw-   0        0        0     4990 2024-04-14 19:01:23.000000 caroa04-0.1.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2024-04-14 17:26:49.000000 caroa04-0.1.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-0.1.2/docs/history.rst
--rw-rw-rw-   0        0        0      324 2024-04-14 17:26:49.000000 caroa04-0.1.2/docs/index.rst
--rw-rw-rw-   0        0        0     1169 2024-04-14 17:26:49.000000 caroa04-0.1.2/docs/installation.rst
--rwxrwxrwx   0        0        0      805 2024-04-14 17:26:49.000000 caroa04-0.1.2/docs/make.bat
--rw-rw-rw-   0        0        0       28 2024-04-14 17:26:49.000000 caroa04-0.1.2/docs/readme.rst
--rw-rw-rw-   0        0        0       76 2024-04-14 17:26:49.000000 caroa04-0.1.2/docs/usage.rst
--rw-rw-rw-   0        0        0     1598 2024-04-15 08:20:21.000000 caroa04-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 08:20:45.072304 caroa04-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 08:20:44.983681 caroa04-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 08:20:45.059306 caroa04-0.1.2/src/caroa04/
--rw-rw-rw-   0        0        0      140 2024-04-14 17:26:49.000000 caroa04-0.1.2/src/caroa04/__init__.py
--rw-rw-rw-   0        0        0    15137 2024-04-15 08:20:21.000000 caroa04-0.1.2/src/caroa04/canmessage.py
--rw-rw-rw-   0        0        0     5184 2024-04-15 08:20:21.000000 caroa04-0.1.2/src/caroa04/caroa04.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:20:45.069306 caroa04-0.1.2/src/caroa04.egg-info/
--rw-rw-rw-   0        0        0     4025 2024-04-15 08:20:44.000000 caroa04-0.1.2/src/caroa04.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-15 08:20:44.000000 caroa04-0.1.2/src/caroa04.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 08:20:44.000000 caroa04-0.1.2/src/caroa04.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-15 08:20:44.000000 caroa04-0.1.2/src/caroa04.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 08:20:44.000000 caroa04-0.1.2/src/caroa04.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 08:20:45.068305 caroa04-0.1.2/tests/
--rw-rw-rw-   0        0        0       38 2024-04-14 17:26:49.000000 caroa04-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     7429 2024-04-15 08:20:21.000000 caroa04-0.1.2/tests/test_caroa04.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.086998 caroa04-1.0.0/
+-rw-rw-rw-   0        0        0      179 2024-04-14 17:26:49.000000 caroa04-1.0.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3870 2024-04-14 17:26:49.000000 caroa04-1.0.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2024-04-14 17:26:49.000000 caroa04-1.0.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1102 2024-04-14 17:26:49.000000 caroa04-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2024-04-14 17:26:49.000000 caroa04-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4948 2024-04-26 12:38:51.086998 caroa04-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3797 2024-04-26 12:37:44.000000 caroa04-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.078535 caroa04-1.0.0/docs/
+-rw-rw-rw-   0        0        0      628 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     4990 2024-04-14 19:01:23.000000 caroa04-1.0.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/history.rst
+-rw-rw-rw-   0        0        0      324 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1169 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      805 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       76 2024-04-14 17:26:49.000000 caroa04-1.0.0/docs/usage.rst
+-rw-rw-rw-   0        0        0     1598 2024-04-26 12:38:09.000000 caroa04-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 12:38:51.086998 caroa04-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.064518 caroa04-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.080541 caroa04-1.0.0/src/caroa04/
+-rw-rw-rw-   0        0        0      140 2024-04-14 17:26:49.000000 caroa04-1.0.0/src/caroa04/__init__.py
+-rw-rw-rw-   0        0        0    14337 2024-04-26 10:46:42.000000 caroa04-1.0.0/src/caroa04/canmessage.py
+-rw-rw-rw-   0        0        0     5977 2024-04-26 12:37:57.000000 caroa04-1.0.0/src/caroa04/caroa04.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.085999 caroa04-1.0.0/src/caroa04.egg-info/
+-rw-rw-rw-   0        0        0     4948 2024-04-26 12:38:51.000000 caroa04-1.0.0/src/caroa04.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-26 12:38:51.000000 caroa04-1.0.0/src/caroa04.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 12:38:51.000000 caroa04-1.0.0/src/caroa04.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-26 12:38:51.000000 caroa04-1.0.0/src/caroa04.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 12:38:51.000000 caroa04-1.0.0/src/caroa04.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 12:38:51.083998 caroa04-1.0.0/tests/
+-rw-rw-rw-   0        0        0       38 2024-04-14 17:26:49.000000 caroa04-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     6899 2024-04-26 12:37:44.000000 caroa04-1.0.0/tests/test_caroa04.py
```

### Comparing `caroa04-0.1.2/CONTRIBUTING.rst` & `caroa04-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.2/LICENSE` & `caroa04-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.2/PKG-INFO` & `caroa04-1.0.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: caroa04
-Version: 0.1.2
-Summary: Library to control the CAROA04 CAN-IO expander device from eletechsup.
-Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
-Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
-License: MIT license
-Project-URL: bugs, https://github.com/supermete/caroa04/issues
-Project-URL: changelog, https://github.com/supermete/caroa04/blob/master/changelog.md
-Project-URL: homepage, https://github.com/supermete/caroa04
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: python-can>=3.3.0
-Requires-Dist: numpy>=1.24.0
-Provides-Extra: dev
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-
 =======
 caroa04
 =======
 
 
 .. image:: https://img.shields.io/pypi/v/caroa04.svg
         :target: https://pypi.python.org/pypi/caroa04
@@ -63,14 +35,16 @@
 
     $ pip install caroao4
 
 
 Usage
 -----
 
+You can instantiate a CaroA04 object and start it to communicate with the device as follows.
+
 .. code-block:: python
 
     from caroa04 import CaroA04
 
     caro = CaroA04()
     caro.start(0xE0, 'pcan', 250000, 'PCAN_USBBUS1')  # start communication
 
@@ -84,18 +58,39 @@
     print(caro.node_id.phys)  # read current address code
     caro.node_id.phys = 0xE1  # set address code (will require device power cycle)
 
     caro.shutdown()  # free the bus
 
 ..
 
+In order to share the bus with other participants, you can assign the bus attribute of the CaroA04 object before starting it.
+You should simply then add CaroA04's listener to the existing bus' notifier.
+
+.. code-block:: python
+
+    import canopen
+    from caroa04 import CaroA04
+
+    nw = canopen.Network()
+    nw.connect(interface='pcan', bitrate=250000, channel='PCAN_USBBUS1')
+
+
+    caro = CaroA04()
+    caro.bus = nw.bus  # use the bus already started by canopen
+    nw.notifier.add_listener(caro.listener)  # add listener so that we can receive messages
+
+    caro.start(0xE0, 'pcan')  # start communication
+    caro.shutdown()  # free the bus
+
+..
+
 Features
 --------
 
-* This library uses the python-can library to communicate with the device.
+* This library uses the python-can library to communicate with the device. Please refer to its documentation to know about all the CAN interfaces that can be used with this library (https://python-can.readthedocs.io/en/stable/)
 * The device has 4 digital outputs and 4 digital inputs. Hence the signals can be read/written by using the attributes of the CaroA04 class:
     * do1, do2, do3, do4 : digital output 1 to digital output 4
     * di1, di2, di3, di4 : digital input 1 to digital input 4
     * bitrate, node_id : bitrate and address code of the device
 * Each signal has a raw value and a physical value. For example, the device does not understand a bitrate in bps. It expects an enumeration that it will interpret. So it can either be set by writing its physical value (bitrate.phys = 250000) or by writing its raw value (bitrate.raw) as follows:
     * 0: 5 kbps
     * 1: 10 kbps
```

### Comparing `caroa04-0.1.2/docs/Makefile` & `caroa04-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.2/docs/conf.py` & `caroa04-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.2/docs/installation.rst` & `caroa04-1.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.2/docs/make.bat` & `caroa04-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.2/pyproject.toml` & `caroa04-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caroa04"
-version = "0.1.2"
+version = "1.0.0"
 description = "Library to control the CAROA04 CAN-IO expander device from eletechsup."
 readme = "README.rst"
 requires-python = ">=3.8"
 authors = [
   {name = "Rodolphe Mete Soyding", email = "r.soyding@gmail.com"}
 ]
 maintainers = [
```

### Comparing `caroa04-0.1.2/src/caroa04/canmessage.py` & `caroa04-1.0.0/src/caroa04/canmessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,16 +355,16 @@
 
     @property
     def node_id(self):
         return self._node_id
 
     @node_id.setter
     def node_id(self, value):
-        self.read_id = (self.read_id & 0xFFFFFF00) | value
-        self.write_id = (self.write_id & 0xFFFFFF00) | value
+        self.read_id = (self.read_id & 0x700) | value
+        self.write_id = (self.write_id & 0x700) | value
         self._node_id = value
 
     def write(self):
         """
         Sends message with the write identifier.
         :return: None
         """
@@ -375,22 +375,15 @@
                 self.cmd_byte.raw = self.tx_cmd_byte
 
             message = can.Message(arbitration_id=self.write_id,
                                   data=self.payload,
                                   is_extended_id=self.is_extended)
             logging.debug(message)
             self.bus.send(message)
-
-            self.bus.set_filters([{"can_id": self.write_id, "can_mask": 0x7ff, "extended": False}])
-            sts = self.bus.recv(5)
-            if sts is not None and sts.arbitration_id == self.write_id and sts.dlc > 0:
-                self.update_payload(sts.data)
-            else:
-                logging.warning('Could not get a response from the device')
-            self.bus.set_filters()
+            self.bus.recv(1)
 
     def read(self):
         """
         Sends message with the read identifier and updates the signals with the received response.
         :return: None
         """
         if self.bus is not None:
@@ -398,30 +391,22 @@
                 self.cmd_byte.raw = self.rx_cmd_byte
 
             message = can.Message(arbitration_id=self.read_id,
                                   data=self.payload,
                                   is_extended_id=self.is_extended)
             logging.debug(message)
             self.bus.send(message)
-
-            self.bus.set_filters([{"can_id": self.read_id, "can_mask": 0x7ff, "extended": False}])
-            sts = self.bus.recv(5)
-            if sts is not None and sts.arbitration_id == self.read_id and sts.dlc > 0:
-                logging.debug(sts)
-                self.update_payload(sts.data)
-            else:
-                logging.warning('Could not get a response from the device')
-            self.bus.set_filters()
+            self.bus.recv(1)
 
 
 if __name__ == "__main__":
     msg_3c2 = CanMessage(0x3c2)
     csm_fail = CanSignal(startbit=8, length=1)
     sig1 = CanSignal(startbit=0, length=8)
     msg_3c2.add(csm_fail)
     msg_3c2.add(sig1)
 
     csm_fail.raw = 1
     sig1.raw = 0xff
 
     print(csm_fail.raw)
-    print(msg_3c2.payload)
+    print(msg_3c2.payload)
```

### Comparing `caroa04-0.1.2/src/caroa04/caroa04.py` & `caroa04-1.0.0/src/caroa04/caroa04.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 sys.path.append(str(pathlib.Path(__file__).parent))
 
 from canmessage import CanMessageRW, XCanSignal, BOOL, ENUM
 
 logging.basicConfig(level=logging.INFO)
 
 __author__ = "R. Soyding"
-__version__ = "0.1.2"
+__version__ = "1.0.0"
 
 MSGID_DO_WRITE = 0x100
 MSGID_DO_READ = 0x200
 MSGID_DI_READ = 0x300
 MSGID_PARAM = 0x700
 DEFAULT_NODEID = 0xE0
 
@@ -50,14 +50,15 @@
     It is, together with the bitrate, also a signal that can be set by the user. However, changing the bitrate or
     address code will only take effect after power cyclcing the device. Then the communication needs to be stopped and
     restarted with the new address code/bitrate.
     """
     def __init__(self):
         self._node_id = DEFAULT_NODEID
         self.bus = None
+        self.notifier = None
 
         self.message_do = CanMessageRW(self._node_id, MSGID_DO_READ, MSGID_DO_WRITE, dlc=8)
         self.message_di = CanMessageRW(self._node_id, MSGID_DI_READ, MSGID_DI_READ, dlc=8)
         self.message_bitrate = CanMessageRW(self._node_id,
                                             MSGID_PARAM,
                                             MSGID_PARAM,
                                             rx_cmd_byte=GET_BAUDRATE_CMD,
@@ -118,36 +119,47 @@
         self.message_di.node_id = node_id
         self.message_do.node_id = node_id
         self.message_bitrate.node_id = node_id
         self.message_nodeid.node_id = node_id
 
         if self.bus is None:
             self.bus = can.Bus(interface=interface, channel=channel, bitrate=bitrate)
-            self.message_do.bus = self.bus
-            self.message_di.bus = self.bus
-            self.message_nodeid.bus = self.bus
-            self.message_bitrate.bus = self.bus
+            self.notifier = can.Notifier(self.bus, [self.listener], timeout=2.0)
 
-    def stop(self):
-        """Stops any ongoing thread - unused"""
-        pass
+        self.message_do.bus = self.bus
+        self.message_di.bus = self.bus
+        self.message_nodeid.bus = self.bus
+        self.message_bitrate.bus = self.bus
+
+    def listener(self, msg):
+        if msg.arbitration_id in (self.message_do.read_id, self.message_do.write_id):
+            logging.debug(f"Response from caroA04> {msg}")
+            self.message_do.update_payload(msg.data)
+        elif msg.arbitration_id in (self.message_di.read_id, self.message_di.write_id):
+            logging.info(msg)
+            self.message_di.update_payload(msg.data)
+        elif msg.arbitration_id in (self.message_bitrate.read_id, self.message_bitrate.write_id):
+            logging.info(msg)
+            self.message_bitrate.update_payload(msg.data)
+        elif msg.arbitration_id in (self.message_nodeid.read_id, self.message_nodeid.write_id):
+            logging.info(msg)
+            self.message_nodeid.update_payload(msg.data)
 
-    def shutdown(self):
+    def stop(self):
+        """Stops any ongoing thread"""
+        if self.notifier is not None:
+            self.notifier.stop()
         if self.bus is not None:
             self.bus.shutdown()  # free the port
             self.bus = None
-            self.message_do.bus = None
-            self.message_di.bus = None
-            self.message_nodeid.bus = None
-            self.message_bitrate.bus = None
+        self.message_do.bus = None
+        self.message_di.bus = None
+        self.message_nodeid.bus = None
+        self.message_bitrate.bus = None
 
 
 if __name__ == "__main__":
     caro = CaroA04()
     caro.start(0xE0, 'pcan', 250000, 'PCAN_USBBUS2')
-    print(caro.do1.phys)
     caro.do1.phys = True
     print(caro.do1.phys)
-    time.sleep(0.5)
     caro.do1.phys = False
-    print(caro.do1.phys)
-    caro.shutdown()
```

### Comparing `caroa04-0.1.2/src/caroa04.egg-info/PKG-INFO` & `caroa04-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caroa04
-Version: 0.1.2
+Version: 1.0.0
 Summary: Library to control the CAROA04 CAN-IO expander device from eletechsup.
 Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/supermete/caroa04/issues
 Project-URL: changelog, https://github.com/supermete/caroa04/blob/master/changelog.md
 Project-URL: homepage, https://github.com/supermete/caroa04
@@ -63,14 +63,16 @@
 
     $ pip install caroao4
 
 
 Usage
 -----
 
+You can instantiate a CaroA04 object and start it to communicate with the device as follows.
+
 .. code-block:: python
 
     from caroa04 import CaroA04
 
     caro = CaroA04()
     caro.start(0xE0, 'pcan', 250000, 'PCAN_USBBUS1')  # start communication
 
@@ -84,18 +86,39 @@
     print(caro.node_id.phys)  # read current address code
     caro.node_id.phys = 0xE1  # set address code (will require device power cycle)
 
     caro.shutdown()  # free the bus
 
 ..
 
+In order to share the bus with other participants, you can assign the bus attribute of the CaroA04 object before starting it.
+You should simply then add CaroA04's listener to the existing bus' notifier.
+
+.. code-block:: python
+
+    import canopen
+    from caroa04 import CaroA04
+
+    nw = canopen.Network()
+    nw.connect(interface='pcan', bitrate=250000, channel='PCAN_USBBUS1')
+
+
+    caro = CaroA04()
+    caro.bus = nw.bus  # use the bus already started by canopen
+    nw.notifier.add_listener(caro.listener)  # add listener so that we can receive messages
+
+    caro.start(0xE0, 'pcan')  # start communication
+    caro.shutdown()  # free the bus
+
+..
+
 Features
 --------
 
-* This library uses the python-can library to communicate with the device.
+* This library uses the python-can library to communicate with the device. Please refer to its documentation to know about all the CAN interfaces that can be used with this library (https://python-can.readthedocs.io/en/stable/)
 * The device has 4 digital outputs and 4 digital inputs. Hence the signals can be read/written by using the attributes of the CaroA04 class:
     * do1, do2, do3, do4 : digital output 1 to digital output 4
     * di1, di2, di3, di4 : digital input 1 to digital input 4
     * bitrate, node_id : bitrate and address code of the device
 * Each signal has a raw value and a physical value. For example, the device does not understand a bitrate in bps. It expects an enumeration that it will interpret. So it can either be set by writing its physical value (bitrate.phys = 250000) or by writing its raw value (bitrate.raw) as follows:
     * 0: 5 kbps
     * 1: 10 kbps
```

### Comparing `caroa04-0.1.2/src/caroa04.egg-info/SOURCES.txt` & `caroa04-1.0.0/src/caroa04.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caroa04-0.1.2/tests/test_caroa04.py` & `caroa04-1.0.0/tests/test_caroa04.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-import threading
 import pytest
 import can
 
 from src.caroa04.caroa04 import CaroA04, MSGID_DO_READ, MSGID_DO_WRITE, MSGID_DI_READ
 from src.caroa04.canmessage import CanMessage, CanSignal, BOOL
 
 
 class VirtualDevice:
     """
     This class aims to simulate the device.
     It will respond to the messages sent by the library, and keep track of the signal's value to answer properly.
     """
     def __init__(self):
-        self._bus = None
-        self._thread = threading.Thread()
-        self._stop_thread = threading.Event()
+        self.bus = None
+        self.notifier = None
         self.message_do_set = CanMessage(MSGID_DO_WRITE)
         self.message_do_get = CanMessage(MSGID_DO_READ)
         self.message_di = CanMessage(MSGID_DI_READ)
         self.do1 = CanSignal(startbit=0, length=1, type=BOOL)
         self.do2 = CanSignal(startbit=1, length=1, type=BOOL)
         self.do3 = CanSignal(startbit=2, length=1, type=BOOL)
         self.do4 = CanSignal(startbit=3, length=1, type=BOOL)
@@ -53,50 +51,42 @@
         )
 
     def start(self, node_id):
         self.message_do_set.arbitration_id = (self.message_do_set.arbitration_id & 0x700) | node_id
         self.message_do_get.arbitration_id = (self.message_do_get.arbitration_id & 0x700) | node_id
         self.message_di.arbitration_id = (self.message_di.arbitration_id & 0x700) | node_id
 
-        if self._bus is None:
-            self._bus = can.interface.Bus(interface='virtual')
-            if not self._thread.is_alive():
-                self._stop_thread.clear()
-                self.__thread = threading.Thread(target=self._emit, daemon=True)
-                self.__thread.start()
-
-    def _emit(self):
-        while not self._stop_thread.is_set():
-            sts = self._bus.recv(1)
-            if sts is not None:
-                if sts.arbitration_id == self.message_do_get.arbitration_id:
-                    # read request received, respond with the last values set with message_do_set
-                    self._bus.send(can.Message(arbitration_id=self.message_do_get.arbitration_id,
-                                               data=self.message_do_set.payload,
-                                               is_extended_id=False))
-                elif sts.arbitration_id == self.message_do_set.arbitration_id:
-                    # write request received, respond with empty message
-                    self.message_do_get.update_payload(sts.data)
-                    self._bus.send(can.Message(arbitration_id=self.message_do_set.arbitration_id,
-                                               data=sts.data,
-                                               is_extended_id=False))
-                elif sts.arbitration_id == self.message_di.arbitration_id:
-                    # read DI request received, respond with the DI message
-                    self._bus.send(can.Message(arbitration_id=self.message_di.arbitration_id,
-                                               data=self.message_di.payload,
-                                               is_extended_id=False))
+        if self.bus is None:
+            self.bus = can.interface.Bus(interface='virtual')
+            self.notifier = can.Notifier(self.bus, [self.listener], timeout=2.0)
+
+    def listener(self, msg):
+        if msg.arbitration_id == self.message_do_get.arbitration_id:
+            # read request received, respond with the last values set with message_do_set
+            self.bus.send(can.Message(arbitration_id=self.message_do_get.arbitration_id,
+                                      data=self.message_do_set.payload,
+                                      is_extended_id=False))
+        elif msg.arbitration_id == self.message_do_set.arbitration_id:
+            # write request received, respond with empty message
+            self.message_do_get.update_payload(msg.data)
+            self.bus.send(can.Message(arbitration_id=self.message_do_set.arbitration_id,
+                                      data=msg.data,
+                                      is_extended_id=False))
+        elif msg.arbitration_id == self.message_di.arbitration_id:
+            # read DI request received, respond with the DI message
+            self.bus.send(can.Message(arbitration_id=self.message_di.arbitration_id,
+                                      data=self.message_di.payload,
+                                      is_extended_id=False))
 
     def stop(self):
-        self._stop_thread.set()
-        if self._thread.is_alive():
-            self._thread.join()
-
-    def shutdown(self):
-        self._bus.shutdown()
-        self._bus = None
+        if self.notifier is not None:
+            self.notifier.stop()
+        if self.bus is not None:
+            self.bus.shutdown()
+            self.bus = None
 
 
 class TestVirtualCanIoExp1:
     @pytest.fixture(scope="class")
     def caro(self):
         return CaroA04()
 
@@ -109,17 +99,15 @@
         """Fixture to execute asserts before and after a sccenario is run"""
         caro.start(0xE0, 'virtual')
         virtualdevice.start(0xE0)
 
         yield
 
         caro.stop()
-        caro.shutdown()
         virtualdevice.stop()
-        virtualdevice.shutdown()
 
     def test_do1(self, caro, virtualdevice):
         assert caro.do1.phys is False, "Initial value of DO1 is wrong"
         caro.do1.phys = True
         assert virtualdevice.do1.phys is True, "DO1 write message not sent"
         caro.do1.phys = False
         assert virtualdevice.do1.phys is False, "Value of DO1 is wrong"
```

