# Comparing `tmp/robothub-2.5.9.tar.gz` & `tmp/robothub-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robothub-2.5.9.tar", last modified: Thu Apr 18 12:30:37 2024, max compression
+gzip compressed data, was "robothub-2.6.0.tar", last modified: Fri Apr 26 21:08:50 2024, max compression
```

## Comparing `robothub-2.5.9.tar` & `robothub-2.6.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.141693 robothub-2.5.9/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-04-18 12:30:20.000000 robothub-2.5.9/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       35 2024-04-18 12:30:20.000000 robothub-2.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-18 12:30:37.141693 robothub-2.5.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)      942 2024-04-18 12:30:20.000000 robothub-2.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:30:37.141693 robothub-2.5.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-04-18 12:30:20.000000 robothub-2.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.133694 robothub-2.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.133694 robothub-2.5.9/src/robothub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      656 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5804 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/frame_buffer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20074 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/live_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/live_view_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.137694 robothub-2.5.9/src/robothub/replay/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/capture_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/captures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/replay_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    33998 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/replay_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/replay/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.137694 robothub-2.5.9/src/robothub/robothub_core_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/_event_typechecks.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/_stop_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9383 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/robothub_core_wrapper/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-18 12:30:20.000000 robothub-2.5.9/src/robothub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.141693 robothub-2.5.9/src/robothub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-18 12:30:37.000000 robothub-2.5.9/src/robothub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-18 12:30:37.000000 robothub-2.5.9/src/robothub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:30:37.000000 robothub-2.5.9/src/robothub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 12:30:37.000000 robothub-2.5.9/src/robothub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:37.137694 robothub-2.5.9/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:20.000000 robothub-2.5.9/tests/test_callback.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:20.000000 robothub-2.5.9/tests/test_hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:30:20.000000 robothub-2.5.9/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:50.127305 robothub-2.6.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-04-26 21:08:32.000000 robothub-2.6.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       35 2024-04-26 21:08:32.000000 robothub-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-26 21:08:50.123305 robothub-2.6.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)      942 2024-04-26 21:08:32.000000 robothub-2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:08:50.127305 robothub-2.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-04-26 21:08:32.000000 robothub-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:50.119305 robothub-2.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:50.119305 robothub-2.6.0/src/robothub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      656 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5804 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/frame_buffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20074 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/live_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/live_view_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:50.123305 robothub-2.6.0/src/robothub/replay/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/replay/capture_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/replay/captures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/replay/replay_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34331 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/replay/replay_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/replay/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:50.123305 robothub-2.6.0/src/robothub/robothub_core_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/_event_typechecks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/_stop_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9383 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/robothub_core_wrapper/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-26 21:08:32.000000 robothub-2.6.0/src/robothub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:50.123305 robothub-2.6.0/src/robothub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-26 21:08:50.000000 robothub-2.6.0/src/robothub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-26 21:08:50.000000 robothub-2.6.0/src/robothub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:08:50.000000 robothub-2.6.0/src/robothub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 21:08:50.000000 robothub-2.6.0/src/robothub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:50.123305 robothub-2.6.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:32.000000 robothub-2.6.0/tests/test_callback.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:32.000000 robothub-2.6.0/tests/test_hub_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:08:32.000000 robothub-2.6.0/tests/test_manager.py
```

### Comparing `robothub-2.5.9/LICENSE` & `robothub-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/PKG-INFO` & `robothub-2.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub
-Version: 2.5.9
+Version: 2.6.0
 Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub-2.5.9/README.md` & `robothub-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/setup.py` & `robothub-2.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the requirements from requirements.txt
 # with open('requirements.txt') as f:
 #     requirements = f.read().splitlines()
 
 setup(
     name='robothub',
-    version='2.5.9',
+    version='2.6.0',
     description='RobotHub integration library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.luxonis.com/',
     license='MIT',
     keywords='robothub camera robot hub connect agent depthai sdk',
     author='Luxonis',
```

### Comparing `robothub-2.5.9/src/robothub/__init__.py` & `robothub-2.6.0/src/robothub/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 
 # Import symbols from robothub_core and make them available under the robothub namespace
 try:
     import robothub_core as robothub
 except ImportError:
     import robothub.robothub_core_wrapper as robothub
 
-__version__ = "2.5.9"
+__version__ = "2.6.0"
 
 # Setup logging for the module
 # setup_logger(__name__)
```

### Comparing `robothub-2.5.9/src/robothub/application.py` & `robothub-2.6.0/src/robothub/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,16 +83,17 @@
         DEVICE_MXID = self._device_mxid
         self._device_ip = self.__rh_device.oak["ipAddress"]
         
         self._device_product_name = (
             self.__rh_device.oak.get("name", None)
             or self.__rh_device.oak.get("productName", None)
             or self._device_mxid)
-        
+
         self.__device_state = robothub_core.DeviceState.DISCONNECTED
+        self.__report_device_info()
 
         # run __manage_device in the main thread when developing locally - enables the usa of cv2.imshow()
         if LOCAL_DEV is True:
             return
 
         self.__device_thread = Thread(
             target=self.__manage_device,
@@ -133,37 +134,41 @@
             self._close_device()
             logger.info(f"Device {self._device_product_name}: thread stopped.")
 
     def _report_info_and_stats(self) -> None:
         """
         Report device info and stats every 30 seconds.
         """
-        product_name = self._device_product_name
         while app_is_running() and self.device_is_running:
-            try:
-                device_info = get_device_details(self.__get_dai_device(), self.__device_state)
-                robothub_core.AGENT.publish_device_info(device_info)
-            except Exception as e:
-                logger.debug(f"Device {product_name}: could not report info with error: {e}.")
+            self.__report_device_info()
+            self.__report_device_stats()
+            self._device_stop_event.wait(30)
 
-            try:
-                device_stats = get_device_performance_metrics(self.__get_dai_device())
-                robothub_core.AGENT.publish_device_stats(device_stats)
-            except Exception as e:
-                logger.debug(f"Device {product_name}: could not report stats with error: {e}.")
+    def __report_device_info(self) -> None:
+        try:
+            device_info = get_device_details(self._get_dai_device(), self.__device_state)
+            robothub_core.AGENT.publish_device_info(device_info)
+        except Exception as e:
+            logger.error(f"Device {self._device_product_name}: could not report info with error: {e}.")
 
-            self._device_stop_event.wait(30)
+    def __report_device_stats(self) -> None:
+        try:
+            device_stats = get_device_performance_metrics(self._get_dai_device())
+            robothub_core.AGENT.publish_device_stats(device_stats)
+        except Exception as e:
+            logger.error(f"Device {self._device_product_name}: could not report stats with error: {e}.")
 
     def _connect(self) -> None:
         """
         Connect to the device. This method is called in a separate thread.
         """
         give_up_time = time.monotonic() + 30
 
         self.__device_state = robothub_core.DeviceState.CONNECTING
+        self.__report_device_info()
         product_name = self._device_product_name
         logger.info(f"Establishing connection with Device {product_name}...")
         while self.running and time.monotonic() < give_up_time:
             logger.debug(
                 f"Device {product_name}: remaining time to connect - {give_up_time - time.monotonic()} seconds."
             )
             try:
@@ -171,19 +176,21 @@
                                     
             except Exception as e:
                 # If device can't be connected to on first try, wait 5 seconds and try again.
                 logger.error(f"Device {product_name}: error while trying to connect - {e}.")
                 self.wait(5)
             else:
                 self.__device_state = robothub_core.DeviceState.CONNECTED
+                self.__report_device_info()
                 logger.info(f"Device {product_name}: successfully connected.")
                 return
 
         logger.error(f"Device {product_name}: could not manage to connect within 30s timeout.")
         self.__device_state = robothub_core.DeviceState.DISCONNECTED
+        self.__report_device_info()
         return
 
     def _close_device(self):
         """
         Close the device gracefully. If the device is not running, this method does nothing.
         """
         with contextlib.suppress(Exception):
@@ -205,16 +212,17 @@
         """
         if not self._device:
             logger.warning("Device is not initialized and cannot be restarted.")
             return
 
         self._device_stop_event.set()
 
-    def __get_dai_device(self) -> depthai.Device:
-        return self._device.device
+    @abstractmethod
+    def _get_dai_device(self) -> depthai.Device:
+        pass
 
     @abstractmethod
     def _manage_device_inner(self):
         pass
 
     @abstractmethod
     def _acquire_device(self):
@@ -265,15 +273,15 @@
     def _start_replay(self):
         for replay in ReplayCamera.replay_camera_instances:
             replay.start_polling(self._device)
 
     def _acquire_device(self) -> depthai.Device:
         return depthai.Device(depthai.DeviceInfo(self._device_ip or self._device_mxid))
 
-    def __get_dai_device(self) -> depthai.Device:
+    def _get_dai_device(self) -> depthai.Device:
         return self._device
 
     @abstractmethod
     def setup_pipeline(self) -> depthai.Pipeline:
         pass
 
     @abstractmethod
```

### Comparing `robothub-2.5.9/src/robothub/decorators.py` & `robothub-2.6.0/src/robothub/decorators.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/events.py` & `robothub-2.6.0/src/robothub/events.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/frame_buffer.py` & `robothub-2.6.0/src/robothub/frame_buffer.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/live_view.py` & `robothub-2.6.0/src/robothub/live_view.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/live_view_utils.py` & `robothub-2.6.0/src/robothub/live_view_utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/replay/capture_manager.py` & `robothub-2.6.0/src/robothub/replay/capture_manager.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/replay/captures.py` & `robothub-2.6.0/src/robothub/replay/captures.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/replay/replay_builder.py` & `robothub-2.6.0/src/robothub/replay/replay_builder.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/replay/replay_camera.py` & `robothub-2.6.0/src/robothub/replay/replay_camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,28 +208,30 @@
                 raw_img_frame = create_img_frame(
                     data=to_planar(frame, (self._raw_width, self._raw_height)),
                     width=self._raw_width,
                     height=self._raw_height,
                     type=dai.ImgFrame.Type.BGR888p,
                     sequence_number=sequence_number,
                     timestamp=timestamp,
+                    camera_socket=self._camera_socket,
                 )
                 self._raw_queue.send(raw_img_frame)
             if self._use_nv12_frame:
                 isp_frame = cv2.resize(frame, (self._isp_width, self._isp_height))
                 isp_nv12_frame = BGR2YUV_NV12(isp_frame)
                 video_nv12_frame = None
                 if self._isp_queue is not None:
                     isp_img_frame = create_img_frame(
                         data=isp_nv12_frame,
                         width=self._isp_width,
                         height=self._isp_height,
                         type=dai.ImgFrame.Type.NV12,
                         sequence_number=sequence_number,
                         timestamp=timestamp,
+                        camera_socket=self._camera_socket,
                     )
                     self._isp_queue.send(isp_img_frame)
                 if self._video_queue is not None:
                     if self._video_width == self._isp_width and self._video_height == self._isp_height:
                         video_nv12_frame = isp_nv12_frame
                     else:
                         video_frame = cv2.resize(frame, (self._video_width, self._video_height))
@@ -237,14 +239,15 @@
                     video_img_frame = create_img_frame(
                         data=video_nv12_frame,
                         width=self._video_width,
                         height=self._video_height,
                         type=dai.ImgFrame.Type.NV12,
                         sequence_number=sequence_number,
                         timestamp=timestamp,
+                        camera_socket=self._camera_socket,
                     )
                     self._video_queue.send(video_img_frame)
                 if self._still_queue is not None and self._send_capture_still:
                     if self._still_width == self._isp_width and self._still_height == self._isp_height:
                         still_nv12_frame = isp_nv12_frame
                     elif video_nv12_frame is not None and self._still_width == self._video_width and self._still_height == self._video_width:
                         still_nv12_frame = video_nv12_frame
@@ -255,14 +258,15 @@
                     video_img_frame = create_img_frame(
                         data=still_nv12_frame,
                         width=self._video_width,
                         height=self._video_height,
                         type=dai.ImgFrame.Type.NV12,
                         sequence_number=sequence_number,
                         timestamp=timestamp,
+                        camera_socket=self._camera_socket,
                     )
                     self._still_queue.send(video_img_frame)
 
             if self._preview_queue is not None:
                 preview_frame = frame
                 # crop when preview aspect ratio is different to video aspect ratio
                 if self._preview_crop_needed is None:
@@ -276,14 +280,15 @@
                 preview_img_frame = create_img_frame(
                     data=to_planar(preview_frame, (self._preview_width, self._preview_height)),
                     width=self._preview_width,
                     height=self._preview_height,
                     type=dai.ImgFrame.Type.BGR888p,
                     sequence_number=sequence_number,
                     timestamp=timestamp,
+                    camera_socket=self._camera_socket,
                 )
                 if self._preview_queue is not None:
                     self._preview_queue.send(preview_img_frame)
 
             sequence_number += 1
 
             process_time = time.monotonic() - start
@@ -677,26 +682,28 @@
                 raw_img_frame = create_img_frame(
                     data=to_planar(frame, (self._raw_width, self._raw_height)),
                     width=self._raw_width,
                     height=self._raw_height,
                     type=dai.ImgFrame.Type.BGR888p,
                     sequence_number=sequence_number,
                     timestamp=timestamp,
+                    camera_socket=self._camera_socket,
                 )
                 self._raw_queue.send(raw_img_frame)
 
             if self._out_queue is not None:
                 preview_frame = cv2.resize(frame, (self._out_width, self._out_height))
                 preview_img_frame = create_img_frame(
                     data=to_planar(preview_frame, (self._out_width, self._out_height)),
                     width=self._out_width,
                     height=self._out_height,
                     type=dai.ImgFrame.Type.BGR888p,
                     sequence_number=sequence_number,
                     timestamp=timestamp,
+                    camera_socket=self._camera_socket,
                 )
                 self._out_queue.send(preview_img_frame)
 
             sequence_number += 1
 
             process_time = time.monotonic() - start
             if process_time > 1.0 / self._fps:
@@ -718,16 +725,16 @@
             self._stop_event.set()
             self._thread.join()
 
     @property
     def replay_is_running(self) -> bool:
         return not self._stop_event.is_set()
 
-    def getBoardSocket(self) -> dai.CameraBoardSocket:
-        raise NotImplementedError("This function is not yet implemented")
+    def getBoardSocket(self) -> dai.CameraBoardSocket | None:
+        return self._camera_socket
 
     def getCamId(self) -> int:
         raise NotImplementedError("This function is not yet implemented")
 
     def getCamera(self) -> str:
         raise NotImplementedError("This function is not yet implemented")
 
@@ -755,15 +762,15 @@
     def getResolutionSize(self) -> Tuple[int, int]:
         raise NotImplementedError("This function is not yet implemented")
 
     def getResolutionWidth(self) -> int:
         raise NotImplementedError("This function is not yet implemented")
 
     def setBoardSocket(self, boardSocket: dai.CameraBoardSocket) -> None:
-        raise NotImplementedError("This function is not yet implemented")
+        self._camera_socket = boardSocket
 
     def setCamId(self, arg0: int) -> None:
         raise NotImplementedError("This function is not yet implemented")
 
     def setCamera(self, name: str) -> None:
         raise NotImplementedError("This function is not yet implemented")
```

### Comparing `robothub-2.5.9/src/robothub/replay/utils.py` & `robothub-2.6.0/src/robothub/replay/utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/robothub_core_wrapper/__init__.py` & `robothub-2.6.0/src/robothub/robothub_core_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/robothub_core_wrapper/_event_typechecks.py` & `robothub-2.6.0/src/robothub/robothub_core_wrapper/_event_typechecks.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/robothub_core_wrapper/app.py` & `robothub-2.6.0/src/robothub/robothub_core_wrapper/app.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/robothub_core_wrapper/client.py` & `robothub-2.6.0/src/robothub/robothub_core_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/robothub_core_wrapper/communicator.py` & `robothub-2.6.0/src/robothub/robothub_core_wrapper/communicator.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/robothub_core_wrapper/device.py` & `robothub-2.6.0/src/robothub/robothub_core_wrapper/device.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/robothub_core_wrapper/events.py` & `robothub-2.6.0/src/robothub/robothub_core_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/robothub_core_wrapper/globals.py` & `robothub-2.6.0/src/robothub/robothub_core_wrapper/globals.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/robothub_core_wrapper/streams.py` & `robothub-2.6.0/src/robothub/robothub_core_wrapper/streams.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.9/src/robothub/utils.py` & `robothub-2.6.0/src/robothub/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,31 +60,36 @@
 
 
 def get_device_details(device: depthai.Device, state: robothub_core.DeviceState) -> Dict[str, Any]:
     """
     Returns a dictionary with information about the device.
     """
     info = {
-        'mxid': device.getMxId(),
+        'mxid': 'unknown',
+        'state': state.value,
         'protocol': 'unknown',
         'platform': 'unknown',
         'product_name': 'unknown',
         'board_name': 'unknown',
         'board_rev': 'unknown',
-        'bootloader_version': 'unknown',
-        'usb_speed': 'unknown',
-        'state': state.value
+        'bootloader_version': 'unknown'
     }
 
-    device_info = try_or_default(device.getDeviceInfo)
+    if device is None:
+        return info
+
+    mxid = try_or_default(device.getMxId)
+    bootloader_version = device.getBootloaderVersion()  # can be None
     calibration = try_or_default(device.readFactoryCalibration) or try_or_default(device.readCalibration2)
     eeprom_data = try_or_default(calibration.getEepromData)
+    device_info = try_or_default(device.getDeviceInfo)
+
+    if mxid:
+        info['mxid'] = mxid
 
-    info['usb_speed'] = device.getUsbSpeed().name.lower()
-    bootloader_version = device.getBootloaderVersion()  # can be None
     if bootloader_version:
         info['bootloader_version'] = bootloader_version.toStringSemver()
 
     if eeprom_data:
         info['product_name'] = eeprom_data.productName
         info['board_name'] = eeprom_data.boardName
         info['board_rev'] = eeprom_data.boardRev
```

### Comparing `robothub-2.5.9/src/robothub.egg-info/PKG-INFO` & `robothub-2.6.0/src/robothub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub
-Version: 2.5.9
+Version: 2.6.0
 Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub-2.5.9/src/robothub.egg-info/SOURCES.txt` & `robothub-2.6.0/src/robothub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

