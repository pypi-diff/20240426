# Comparing `tmp/pts_fault_injection-0.1.0.tar.gz` & `tmp/pts_fault_injection-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_fault_injection-0.1.0.tar", last modified: Thu Apr 18 13:26:39 2024, max compression
+gzip compressed data, was "dist/pts_fault_injection-0.1.1.tar", last modified: Fri Apr 26 10:08:45 2024, max compression
```

## Comparing `pts_fault_injection-0.1.0.tar` & `pts_fault_injection-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     4002 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      969 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4002 2024-04-18 13:26:38.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 13:26:38.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-18 13:26:38.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-18 13:26:38.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     3470 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/pts_fault_injection/
--rw-rw-rw-   0 root         (0) root         (0)    32907 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/pts_fault_injection/fib_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     8261 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/pts_fault_injection/cmb_box.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/pts_fault_injection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7658 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/pts_fault_injection/load_box.py
--rw-rw-rw-   0 root         (0) root         (0)     7764 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/pts_fault_injection/CANFWupdate.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 10:08:45.000000 pts_fault_injection-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     4002 2024-04-26 10:08:45.000000 pts_fault_injection-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      969 2024-04-26 10:08:36.000000 pts_fault_injection-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 10:08:45.000000 pts_fault_injection-0.1.1/pts_fault_injection.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4002 2024-04-26 10:08:45.000000 pts_fault_injection-0.1.1/pts_fault_injection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-04-26 10:08:45.000000 pts_fault_injection-0.1.1/pts_fault_injection.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 10:08:45.000000 pts_fault_injection-0.1.1/pts_fault_injection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-26 10:08:45.000000 pts_fault_injection-0.1.1/pts_fault_injection.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-26 10:08:45.000000 pts_fault_injection-0.1.1/pts_fault_injection.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-04-26 10:08:36.000000 pts_fault_injection-0.1.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3470 2024-04-26 10:08:36.000000 pts_fault_injection-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 10:08:45.000000 pts_fault_injection-0.1.1/pts_fault_injection/
+-rw-rw-rw-   0 root         (0) root         (0)    33267 2024-04-26 10:08:36.000000 pts_fault_injection-0.1.1/pts_fault_injection/fib_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     8261 2024-04-26 10:08:36.000000 pts_fault_injection-0.1.1/pts_fault_injection/cmb_box.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-26 10:08:36.000000 pts_fault_injection-0.1.1/pts_fault_injection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7658 2024-04-26 10:08:36.000000 pts_fault_injection-0.1.1/pts_fault_injection/load_box.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2024-04-26 10:08:36.000000 pts_fault_injection-0.1.1/pts_fault_injection/CANFWupdate.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 10:08:45.000000 pts_fault_injection-0.1.1/setup.cfg
```

### Comparing `pts_fault_injection-0.1.0/PKG-INFO` & `pts_fault_injection-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts_fault_injection
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.1.0/setup.py` & `pts_fault_injection-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_fault_injection",
-    version="0.1.0",
+    version="0.1.1",
     author="Pass testing Solutions GmbH",
     description="Fault Injection box Diagnostics package Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/pts-fault-injection-box",
     license="MIT",
```

### Comparing `pts_fault_injection-0.1.0/pts_fault_injection.egg-info/PKG-INFO` & `pts_fault_injection-0.1.1/pts_fault_injection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts-fault-injection
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.1.0/LICENSE.txt` & `pts_fault_injection-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.1.0/README.md` & `pts_fault_injection-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.1.0/pts_fault_injection/fib_controller.py` & `pts_fault_injection-0.1.1/pts_fault_injection/fib_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         "StandardSignal2": StandardSignalCard.test_standard_signal_card2,
         "StandardSignal3": StandardSignalCard.test_standard_signal_card3,
         "StandardSignal4": StandardSignalCard.test_standard_signal_card4,
         "BusSignal": BusSignalCard.test_bus_signal_card,
         "HVSignal": HVSignalCard.test_hv_signal_card,
     }
     if card in funcs:
-        logging.debug(f"TESTING BOARD {card}")
+        print(f"TESTING BOARD {card}")
         funcs[card]()
     else:
         raise Exception(f"Signal Card {card} not present.")
 
 
 class FaultInjectionController(object):
     """
@@ -192,14 +192,23 @@
     def oc_all_relays(self) -> None:
         """
         Open Circuits all relays on the signal cards (except HV signal card)
         """
         # Get number and send command
         self.set_multiple_relays("oc", True, list(range(1, 50))+list(range(51, 61)))
 
+    def reset_all(self) -> None:
+        """
+        Resets all relays on the signal cards to boot up state
+        """
+        logging.debug("Using broadcast ID " + hex(broadcast_id))
+        msg = can.Message(arbitration_id=broadcast_id, data=[ord('R'), ord('E'), ord('B'), 0, 0, 0, 0, 0],
+                          is_extended_id=False)
+        self.bus.send(msg)
+
     def send_card_can_message(self, card: int, data: bin) -> None:
         """
         Creates a can message out of the state and sends it to the can connector for a signal card
         :param card: int: 0-5 for the Signal Cards
         :param data: CAN Message is RC_Cntrl, ID 0x210
         Signals :
             RC_mux -> FIB Card (0-7) multiplexer
```

### Comparing `pts_fault_injection-0.1.0/pts_fault_injection/cmb_box.py` & `pts_fault_injection-0.1.1/pts_fault_injection/cmb_box.py`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.1.0/pts_fault_injection/load_box.py` & `pts_fault_injection-0.1.1/pts_fault_injection/load_box.py`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.1.0/pts_fault_injection/CANFWupdate.py` & `pts_fault_injection-0.1.1/pts_fault_injection/CANFWupdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 else:
     print("You Have not specified an input HEX file\nDo you want to download one from the Internet? (Y/N)")
     res = input()
     while res not in ('Y', 'N'):
         print("Could not interpret the input, try again or cancel with ctrl-c")
         res = input()
     if res == 'Y':
-        with urllib.request.urlopen('http://hil-common-firmware.s3.us-east-2.amazonaws.com/?list-type=2') as response:
+        with urllib.request.urlopen('http://hil-common-firmware.s3.us-east-2.amazonaws.com/?list-type=2&prefix=hil-common-firmware/') as response:
             dom = xml.dom.minidom.parseString(response.read())
             files = parse_s3_index_response(dom)
 
         print("Following Files have been found Online:")
         idx = 1
         for file in files:
             print(str(idx) + " - " + str(file))
```

