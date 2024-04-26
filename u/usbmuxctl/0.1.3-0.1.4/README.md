# Comparing `tmp/usbmuxctl-0.1.3.tar.gz` & `tmp/usbmuxctl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usbmuxctl-0.1.3.tar", last modified: Mon Feb 27 17:04:30 2023, max compression
+gzip compressed data, was "usbmuxctl-0.1.4.tar", last modified: Fri Apr 26 07:51:14 2024, max compression
```

## Comparing `usbmuxctl-0.1.3.tar` & `usbmuxctl-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-02-27 17:04:30.674426 usbmuxctl-0.1.3/
--rw-rw-r--   0 chris     (1000) chris     (1000)    26530 2021-07-16 06:52:01.000000 usbmuxctl-0.1.3/COPYING
--rw-rw-r--   0 chris     (1000) chris     (1000)      167 2021-07-16 06:52:01.000000 usbmuxctl-0.1.3/MANIFEST.in
--rw-r--r--   0 chris     (1000) chris     (1000)    13423 2023-02-27 17:04:30.674426 usbmuxctl-0.1.3/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)    10733 2023-02-27 10:34:06.000000 usbmuxctl-0.1.3/README.rst
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-02-27 17:04:30.670426 usbmuxctl-0.1.3/contrib/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-02-27 17:04:30.670426 usbmuxctl-0.1.3/contrib/udev/
--rw-rw-r--   0 chris     (1000) chris     (1000)      115 2021-07-16 06:52:01.000000 usbmuxctl-0.1.3/contrib/udev/99-usbmux.rules
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-02-27 17:04:30.670426 usbmuxctl-0.1.3/contrib/windows/
--rw-r--r--   0 chris     (1000) chris     (1000)  2056446 2023-02-27 10:34:06.000000 usbmuxctl-0.1.3/contrib/windows/libusb_USB-Mux_driver_installer.zip
--rw-r--r--   0 chris     (1000) chris     (1000)     3782 2023-02-27 10:34:06.000000 usbmuxctl-0.1.3/fastentrypoints.py
--rw-r--r--   0 chris     (1000) chris     (1000)       32 2023-02-27 10:34:06.000000 usbmuxctl-0.1.3/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      225 2023-02-27 17:04:30.674426 usbmuxctl-0.1.3/setup.cfg
--rwxr-xr-x   0 chris     (1000) chris     (1000)      749 2023-02-27 16:28:10.000000 usbmuxctl-0.1.3/setup.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-02-27 17:04:30.674426 usbmuxctl-0.1.3/usbmuxctl/
--rw-r--r--   0 chris     (1000) chris     (1000)      887 2023-02-27 10:34:06.000000 usbmuxctl-0.1.3/usbmuxctl/__init__.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)    17330 2023-02-27 16:26:40.000000 usbmuxctl-0.1.3/usbmuxctl/__main__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-02-27 17:04:30.674426 usbmuxctl-0.1.3/usbmuxctl/firmware/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2021-07-16 06:52:01.000000 usbmuxctl-0.1.3/usbmuxctl/firmware/__init__.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)    12356 2021-07-16 06:52:01.000000 usbmuxctl-0.1.3/usbmuxctl/firmware/umx-T03_0.1.2.bin
--rw-r--r--   0 chris     (1000) chris     (1000)     1276 2023-02-27 10:34:06.000000 usbmuxctl-0.1.3/usbmuxctl/firmware/version.py
--rw-r--r--   0 chris     (1000) chris     (1000)    13851 2023-02-27 10:34:06.000000 usbmuxctl-0.1.3/usbmuxctl/update.py
--rw-r--r--   0 chris     (1000) chris     (1000)    13093 2023-02-27 10:34:06.000000 usbmuxctl-0.1.3/usbmuxctl/usbmuxctl.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-02-27 17:04:30.674426 usbmuxctl-0.1.3/usbmuxctl.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)    13423 2023-02-27 17:04:30.000000 usbmuxctl-0.1.3/usbmuxctl.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      549 2023-02-27 17:04:30.000000 usbmuxctl-0.1.3/usbmuxctl.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2023-02-27 17:04:30.000000 usbmuxctl-0.1.3/usbmuxctl.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       55 2023-02-27 17:04:30.000000 usbmuxctl-0.1.3/usbmuxctl.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       16 2023-02-27 17:04:30.000000 usbmuxctl-0.1.3/usbmuxctl.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       10 2023-02-27 17:04:30.000000 usbmuxctl-0.1.3/usbmuxctl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:51:14.789386 usbmuxctl-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:51:14.777386 usbmuxctl-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:51:14.781386 usbmuxctl-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/.github/workflows/check-and-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26530 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-26 07:51:14.789386 usbmuxctl-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:51:14.777386 usbmuxctl-0.1.4/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:51:14.781386 usbmuxctl-0.1.4/contrib/udev/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/contrib/udev/99-usbmux.rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:51:14.781386 usbmuxctl-0.1.4/contrib/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)  2056446 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/contrib/windows/libusb_USB-Mux_driver_installer.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:51:14.785386 usbmuxctl-0.1.4/debian/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/debian/control
+-rwxr-xr-x   0 runner    (1001) docker     (127)      112 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/debian/usbmuxctl.udev
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 07:51:14.789386 usbmuxctl-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:51:14.785386 usbmuxctl-0.1.4/usbmuxctl/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/usbmuxctl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17243 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/usbmuxctl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:51:14.785386 usbmuxctl-0.1.4/usbmuxctl/firmware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/usbmuxctl/firmware/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12356 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/usbmuxctl/firmware/umx-T03_0.1.2.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/usbmuxctl/firmware/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13888 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/usbmuxctl/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-04-26 07:51:06.000000 usbmuxctl-0.1.4/usbmuxctl/usbmuxctl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:51:14.785386 usbmuxctl-0.1.4/usbmuxctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-26 07:51:14.000000 usbmuxctl-0.1.4/usbmuxctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-26 07:51:14.000000 usbmuxctl-0.1.4/usbmuxctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:51:14.000000 usbmuxctl-0.1.4/usbmuxctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 07:51:14.000000 usbmuxctl-0.1.4/usbmuxctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 07:51:14.000000 usbmuxctl-0.1.4/usbmuxctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 07:51:14.000000 usbmuxctl-0.1.4/usbmuxctl.egg-info/top_level.txt
```

### Comparing `usbmuxctl-0.1.3/COPYING` & `usbmuxctl-0.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `usbmuxctl-0.1.3/README.rst` & `usbmuxctl-0.1.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -229,23 +229,24 @@
 Contributing
 ------------
 
 Thank you for considering a contribution to this project!
 Changes should be submitted via a
 `Github pull request <https://github.com/linux-automation/usbmuxctl/pulls>`_.
 
-We use the `black <https://black.readthedocs.io/en/stable/>`_ code formatter,
-please run `black` when contributing changes:
+We use the `ruff <https://docs.astral.sh/ruff/>`_ code formatter and linter,
+please run `ruff format` and `ruff check` when contributing changes:
 
 .. code-block:: bash
 
-    $ python3 -m pip install black
-    $ black *.py usbmuxctl/
-    All done! ✨ 🍰 ✨
-    8 files left unchanged.
+    $ python3 -m pip install ruff
+    $ ruff format
+    6 files left unchanged
+    $ ruff check
+    All checks passed!
 
 This project uses the `Developer's Certificate of Origin 1.1
 <https://developercertificate.org/>`_ with the same `process
 <https://www.kernel.org/doc/html/latest/process/submitting-patches.html#sign-your-work-the-developer-s-certificate-of-origin>`_
 as used for the Linux kernel:
 
   Developer's Certificate of Origin 1.1
@@ -274,15 +275,15 @@
       maintained indefinitely and may be redistributed consistent with
       this project or the open source license(s) involved.
 
 Then you just add a line (using ``git commit -s``) saying:
 
   Signed-off-by: Random J Developer <random@developer.example.org>
 
-using your real name (sorry, no pseudonyms or anonymous contributions).
+using a known identity (sorry, no anonymous contributions).
 
 .. |license| image:: https://img.shields.io/badge/license-LGPLv2.1-blue.svg
     :alt: LGPLv2.1
     :target: https://raw.githubusercontent.com/linux-automation/usbmuxctl/master/COPYING
 
 .. |pypi| image:: https://img.shields.io/pypi/v/usbmuxctl.svg
     :alt: pypi.org
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `usbmuxctl-0.1.3/contrib/windows/libusb_USB-Mux_driver_installer.zip` & `usbmuxctl-0.1.4/contrib/windows/libusb_USB-Mux_driver_installer.zip`

 * *Files identical despite different names*

### Comparing `usbmuxctl-0.1.3/usbmuxctl/__init__.py` & `usbmuxctl-0.1.4/usbmuxctl/__init__.py`

 * *Files identical despite different names*

### Comparing `usbmuxctl-0.1.3/usbmuxctl/__main__.py` & `usbmuxctl-0.1.4/usbmuxctl/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,81 +31,71 @@
 
 
 class ConnectionNotPossible(Exception):
     pass
 
 
 artwork = {}
-artwork[
-    "DUT-Host Device-Host"
-] = """                                     +-----------------------+
+artwork["DUT-Host Device-Host"] = """                                     +-----------------------+
                                      | USB-Mux               |
                                   +--|                       |
                                   |  | SN:   {:11s}     |
                                   |  | Path: {:16s}|
                                   |  +-----------------------+
        VCC: {:1.2f}V    +---------+  |
 Host |>--------------|       1 |--+         ID: {}
                      |         |           VCC: {:1.2f}V
                      |  {:6} |---------------------|> DUT
                      |         |
                      |       3 |---------------------|> Device
                      +---------+           VCC: {:1.2f}V"""
 
-artwork[
-    "None"
-] = """                                     +-----------------------+
+artwork["None"] = """                                     +-----------------------+
                                      | USB-Mux               |
                                   +--|                       |
                                   |  | SN:   {:11s}     |
                                   |  | Path: {:16s}|
                                   |  +-----------------------+
        VCC: {:1.2f}V    +---------+  |
 Host |>--------------|       1 |--+         ID: {}
                      |         |           VCC: {:1.2f}V
                      |  {:6} |----x    ------------|> DUT
                      |         |
                      |       3 |----x    ------------|> Device
                      +---------+           VCC: {:1.2f}V"""
 
-artwork[
-    "DUT-Host"
-] = """                                     +-----------------------+
+artwork["DUT-Host"] = """                                     +-----------------------+
                                      | USB-Mux               |
                                   +--|                       |
                                   |  | SN:   {:11s}     |
                                   |  | Path: {:16s}|
                                   |  +-----------------------+
        VCC: {:1.2f}V    +---------+  |
 Host |>--------------|       1 |--+         ID: {}
                      |         |           VCC: {:1.2f}V
                      |  {:6} |---------------------|> DUT
                      |         |
                      |       3 |----x    ------------|> Device
                      +---------+           VCC: {:1.2f}V"""
 
-artwork[
-    "Device-Host"
-] = """                                     +-----------------------+
+artwork["Device-Host"] = """                                     +-----------------------+
                                      | USB-Mux               |
                                   +--|                       |
                                   |  | SN:   {:11s}     |
                                   |  | Path: {:16s}|
                                   |  +-----------------------+
        VCC: {:1.2f}V    +---------+  |
 Host |>--------------|       1 |--+         ID: {}
                      |         |           VCC: {:1.2f}V
                      |  {:6} |----x    ------------|> DUT
                      |         |
                      |       3 |---------------------|> Device
                      +---------+           VCC: {:1.2f}V"""
 
-artwork[
-    "DUT-Device"
-] = """                                     +-----------------------+
+artwork["DUT-Device"] = """                                     +-----------------------+
                                      | USB-Mux               |
                                   +--|                       |
                                   |  | SN:   {:11s}     |
                                   |  | Path: {:16s}|
                                   |  +-----------------------+
        VCC: {:1.2f}V    +---------+  |
 Host |>--------------|       1 |--+         ID: {}
@@ -182,18 +172,15 @@
         print(json.dumps(res))
     else:
         print("Serial      | USB-Path           | Host-DUT Lock? | Connections")
         print("----------- | ------------------ | -------------- | -----------")
         for d in Mux.find_devices():
             mux = Mux(path=d["path"])
             status = mux.get_status()
-            if status["data_links"] == "":
-                connections = "None"
-            else:
-                connections = status["data_links"]
+            connections = status["data_links"] if status["data_links"] != "" else "None"
             lock = "locked" if status["dut_power_lockout"] else "unlocked"
 
             messages = _ui_messages(status)
             print(f"{d['serial']:11} | {d['path']:18} | {lock:14} | {connections:14} {messages}")
 
 
 def show_status(status, raw=False):
@@ -388,25 +375,25 @@
             mux = find_umux(args)
             mux.update_software()
         except UmuxNotFound:
             result["error"] = True
             result["errormessage"] = "Failed to connect to device: Failed to find the defined USB-Mux"
         except DfuUtilNotFoundError:
             result["error"] = True
-            result[
-                "errormessage"
-            ] = "Could not find tool 'dfu-util'. Please install using your package manager and re-run this command."
+            result["errormessage"] = (
+                "Could not find tool 'dfu-util'. Please install using your package manager and re-run this command."
+            )
         except DfuUtilFailedError as e:
             result["error"] = True
             result["errormessage"] = f"'dfu-util' failed: '{e}'. Please check the log above for hints how to fix this."
         except usb.core.USBError as err:
             if err.errno == errno.EACCES:
                 result["error"] = True
                 result["errormessage"] = (
-                    "'dfu-util' failed. This probably happend because of "
+                    "'dfu-util' failed. This probably happened because of "
                     + f"insufficient permissions: {err} "
                     + "Disconnect and reconnect the USB-Mux."
                 )
             else:
                 result["error"] = True
                 result["errormessage"] = f"Unhandled USBError: {err}"
```

### Comparing `usbmuxctl-0.1.3/usbmuxctl/firmware/umx-T03_0.1.2.bin` & `usbmuxctl-0.1.4/usbmuxctl/firmware/umx-T03_0.1.2.bin`

 * *Files identical despite different names*

### Comparing `usbmuxctl-0.1.3/usbmuxctl/firmware/version.py` & `usbmuxctl-0.1.4/usbmuxctl/firmware/version.py`

 * *Files identical despite different names*

### Comparing `usbmuxctl-0.1.3/usbmuxctl/update.py` & `usbmuxctl-0.1.4/usbmuxctl/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         ret = self._cmd_in(_DfuCommand.DFU_GETSTATUS, 0, 6)
         ret = self.parse_dfu_status(ret)
         self.log.debug("get_status: %s", ret)
         return ret
 
     def _check_status(self):
         """Wrapper for _get_status.
-        Returns the device status and thows DFUException if bStatus is not OK"""
+        Returns the device status and throws DFUException if bStatus is not OK"""
 
         status = self._get_status()
         if status["bStatus"] != _bStatus.OK:
             raise DFUException(status)
         return status
 
     def _clear_status(self):
@@ -222,32 +222,32 @@
         self.log.debug("Abort")
         self._cmd_out(_DfuCommand.DFU_ABORT, 0)
         self._check_status()
 
     def _set_address(self, address):
         """DFU internal command
         Set the address to read, write, execute"""
-        self.log.debug("Set Adress: %x", address)
+        self.log.debug("Set Address: %x", address)
         self._cmd_out(_DfuCommand.DFU_DNLOAD, 0, struct.pack("<BI", 0x21, address))
         self._check_status()
 
     def _read_mem(self, length):
         """DFU internal command
         Reads length number of bytes from memory.
         The address is set by the set_address() command."""
         self.log.debug("Reading memory length: %d", length)
 
         ret = self._cmd_in(_DfuCommand.DFU_UPLOAD, 2, length)
 
-        self.log.debug("Data receving: %s", "".join(f"{i:02X}" for i in ret))
+        self.log.debug("Data receiving: %s", "".join(f"{i:02X}" for i in ret))
         return ret, self._check_status()
 
     def _get_cmd(self):
         """DFU internal command
-        Requests a list of supportet commands from the DFU device"""
+        Requests a list of supported commands from the DFU device"""
         raise NotImplementedError()
 
     def _write_mem(self):
         """DFU internal command"""
         raise NotImplementedError()
 
     def _erase(self):
@@ -263,15 +263,15 @@
         Executes the code at the address set by set_address()"""
         self.log.debug("Leaving DFU mode")
 
         self._cmd_out(_DfuCommand.DFU_DNLOAD, 0, b"")
         status = self._check_status()
 
         if status["bState"] != _bState.dfuMANIFEST:
-            self.log.error("Leave dfu command faild")
+            self.log.error("Leave dfu command failed")
             raise DFUException(status)
 
     def read_at_addr_len(self, addr, length):
         """Read data from the DFU device.
 
         Arguments:
             addr   -- address to the first byte to read
@@ -355,54 +355,54 @@
 
     try:
         output = subprocess.check_output([DFU_UTIL_CMD, "-V"])
         output = output.decode("utf-8") + "\n"
         dfu_version, *_ = output.split("\n")
 
         return dfu_version
-    except FileNotFoundError:
-        raise DfuUtilNotFoundError("dfu-util not found. Might not be installed.")
+    except FileNotFoundError as e:
+        raise DfuUtilNotFoundError("dfu-util not found. Might not be installed.") from e
 
 
 def dfu_util_flash_firmware(firmware_path, usb_path):
     """Flash firmware to USB-Mux in DFU mode.
     This uses the command line tool dfu-util so that must be installed.
 
     Arguments:
     firmware_path -- Path to the firmware file as string
     usb_path      -- USB path to USB device (example: 1-2.2.1)
 
-    Throws an Exception if dfu-util is not installed oder dfu-util failed"""
+    Throws an Exception if dfu-util is not installed or dfu-util failed"""
     try:
         res = subprocess.run(
             [DFU_UTIL_CMD, "-d", "0483:df11", "-a", "0", "-D", firmware_path, "-s", "0x8000000", "--path", usb_path]
         )
         if res.returncode != 0:
             raise DfuUtilFailedError(f"dfu-util failed with: {res}")
-    except FileNotFoundError:
-        raise DfuUtilNotFoundError("dfu-util not found. Might not be installed.")
+    except FileNotFoundError as e:
+        raise DfuUtilNotFoundError("dfu-util not found. Might not be installed.") from e
 
 
 def dfu_util_flash_config(file_path, usb_path):
     """Flash config to USB-Mux in DFU mode.
     This uses the command line tool dfu-util so that must be installed.
 
     Arguments:
     firmware_path -- Path to the config file as string
     usb_path      -- USB path to USB device (example: 1-2.2.1)
 
-    Throws an Exception if dfu-util is not installed oder dfu-util failed"""
+    Throws an Exception if dfu-util is not installed or dfu-util failed"""
     try:
         res = subprocess.run(
             [DFU_UTIL_CMD, "-d", "0483:df11", "-a", "0", "-D", file_path, "-s", "0x8007c00", "--path", usb_path]
         )
         if res.returncode != 0:
             raise Exception(f"dfu-util failed with: {res}")
-    except FileNotFoundError:
-        raise Exception("dfu-util not found. Might not be installed.")
+    except FileNotFoundError as e:
+        raise Exception("dfu-util not found. Might not be installed.") from e
 
 
 def _find_dfu_device(search_path):
     try:
         dfu = DFU(path=search_path)
     except TooManyDFUDevicesFound as e:
         print("Found more then one DFU Device.")
@@ -496,15 +496,15 @@
         "--path",
         "-p",
         help="USB Path to USB device (1-4.1)",
     )
     parser.add_argument(
         "--serial",
         "-s",
-        help="USBMux serial numer (00001.00020)",
+        help="USBMux serial number (00001.00020)",
     )
     parser.add_argument(
         "-v",
         help="Be verbose",
         action="store_true",
     )
     args = parser.parse_args()
```

### Comparing `usbmuxctl-0.1.3/usbmuxctl/usbmuxctl.py` & `usbmuxctl-0.1.4/usbmuxctl/usbmuxctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
+import contextlib
 import errno
 import struct
 from sys import stderr
 from time import sleep
 
 import usb.core
 
@@ -70,15 +71,15 @@
     _USB_IDs = [
         {
             # This is our actual Linux Automation GmbH Vendor ID and our actual Product ID.
             "VENDORID": 0x33F7,
             "PRODUCTID": 0x0001,
         },
         {
-            # This is a _fake_ Vendor-ID and Product-ID that we have choosen by throwing dice during
+            # This is a _fake_ Vendor-ID and Product-ID that we have chosen by throwing dice during
             # development. This ID is only for the transition phase. There should be no USB-Muxes
             # in the wild using this ID!
             "VENDORID": 0x5824,
             "PRODUCTID": 0x27DD,
         },
     ]
 
@@ -173,16 +174,16 @@
                     "The protocol version reported by the USB-Mux is not supported by this control tool."
                 )
             self._proto_version = "".join(str(x) for x in proto_version)
             if self._proto_version not in ["00000000"]:
                 raise ProtocolVersionMismatch(
                     "The protocol version reported by the USB-Mux is not supported by this control tool."
                 )
-        except ValueError:
-            raise NoPrivileges("Could not communicate with USB-device. Check privileges, maybe add udev-rule")
+        except ValueError as e:
+            raise NoPrivileges("Could not communicate with USB-device. Check privileges, maybe add udev-rule") from e
 
         # read sw version
         self.sw_version = str(self._send_cmd(self._SW_VERSION), "utf-8")
         self.sw_version_num = version.version_from_string(self.sw_version)
 
     def _send_cmd(self, cmd, arg=0):
         """
@@ -292,18 +293,16 @@
         To resume normal operation the USB-Mux must be either reset
         using the DFU-Mode or power cycled.
         """
         self._connect_power(0)
         self._connect_data(0)
 
         sleep(0.1)
-        try:
+        with contextlib.suppress(usb.core.USBError):
             self._send_cmd(self._DFU)
-        except usb.core.USBError:
-            pass
 
     def connect(self, links, id_pull_low=None):
         """
         Applies a connection between ports of the USB-Mux.
 
         Before switching to a new connection all current connections
         are being removed and this methods gives the USB-Mux about 0.5 s to settle.
@@ -346,15 +345,15 @@
 
     def __str__(self):
         path = path_from_usb_dev(self._dev)
         path = f"Connected to:\n- ID:   {self._dev.serial_number}\n- Path: {path}\n- Name: {self._dev.product}"
         return path
 
     def is_software_up_to_date(self):
-        return version.FIRMWARE_VERSION <= self.sw_version_num
+        return self.sw_version_num >= version.FIRMWARE_VERSION
 
     def update_software(self):
         """Updates the usbmux software"""
 
         from .update import (
             DFU,
             dfu_util_flash_firmware,
```

### Comparing `usbmuxctl-0.1.3/usbmuxctl.egg-info/SOURCES.txt` & `usbmuxctl-0.1.4/usbmuxctl.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 COPYING
 MANIFEST.in
+Makefile
 README.rst
-fastentrypoints.py
 pyproject.toml
-setup.cfg
-setup.py
+.github/workflows/check-and-publish.yaml
 contrib/udev/99-usbmux.rules
 contrib/windows/libusb_USB-Mux_driver_installer.zip
+debian/changelog
+debian/compat
+debian/control
+debian/rules
+debian/usbmuxctl.udev
 usbmuxctl/__init__.py
 usbmuxctl/__main__.py
 usbmuxctl/update.py
 usbmuxctl/usbmuxctl.py
 usbmuxctl.egg-info/PKG-INFO
 usbmuxctl.egg-info/SOURCES.txt
 usbmuxctl.egg-info/dependency_links.txt
```

