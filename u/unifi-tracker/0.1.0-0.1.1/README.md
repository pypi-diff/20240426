# Comparing `tmp/unifi_tracker-0.1.0.tar.gz` & `tmp/unifi_tracker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifi_tracker-0.1.0.tar", last modified: Sun Jan 28 20:16:30 2024, max compression
+gzip compressed data, was "unifi_tracker-0.1.1.tar", last modified: Fri Apr 26 03:27:58 2024, max compression
```

## Comparing `unifi_tracker-0.1.0.tar` & `unifi_tracker-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2024-01-28 20:16:30.715900 unifi_tracker-0.1.0/
--rw-r--r--   0 joelp     (1000) joelp     (1000)     1071 2024-01-27 18:14:32.000000 unifi_tracker-0.1.0/LICENSE
--rw-r--r--   0 joelp     (1000) joelp     (1000)     7114 2024-01-28 20:16:30.715900 unifi_tracker-0.1.0/PKG-INFO
--rw-r--r--   0 joelp     (1000) joelp     (1000)     6545 2024-01-28 20:10:54.000000 unifi_tracker-0.1.0/README.md
--rw-r--r--   0 joelp     (1000) joelp     (1000)      103 2024-01-27 18:14:32.000000 unifi_tracker-0.1.0/pyproject.toml
--rw-r--r--   0 joelp     (1000) joelp     (1000)      694 2024-01-28 20:16:30.715900 unifi_tracker-0.1.0/setup.cfg
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2024-01-28 20:16:30.711900 unifi_tracker-0.1.0/src/
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2024-01-28 20:16:30.711900 unifi_tracker-0.1.0/src/unifi_tracker/
--rw-r--r--   0 joelp     (1000) joelp     (1000)      160 2024-01-28 20:10:54.000000 unifi_tracker-0.1.0/src/unifi_tracker/__init__.py
--rw-r--r--   0 joelp     (1000) joelp     (1000)    10011 2024-01-28 20:10:54.000000 unifi_tracker-0.1.0/src/unifi_tracker/unifi_tracker.py
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2024-01-28 20:16:30.711900 unifi_tracker-0.1.0/src/unifi_tracker.egg-info/
--rw-r--r--   0 joelp     (1000) joelp     (1000)     7114 2024-01-28 20:16:30.000000 unifi_tracker-0.1.0/src/unifi_tracker.egg-info/PKG-INFO
--rw-r--r--   0 joelp     (1000) joelp     (1000)      346 2024-01-28 20:16:30.000000 unifi_tracker-0.1.0/src/unifi_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 joelp     (1000) joelp     (1000)        1 2024-01-28 20:16:30.000000 unifi_tracker-0.1.0/src/unifi_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 joelp     (1000) joelp     (1000)       14 2024-01-28 20:16:30.000000 unifi_tracker-0.1.0/src/unifi_tracker.egg-info/top_level.txt
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2024-01-28 20:16:30.711900 unifi_tracker-0.1.0/tests/
--rw-r--r--   0 joelp     (1000) joelp     (1000)     2230 2024-01-28 20:10:54.000000 unifi_tracker-0.1.0/tests/test_diff.py
--rw-r--r--   0 joelp     (1000) joelp     (1000)     2899 2024-01-28 20:10:54.000000 unifi_tracker-0.1.0/tests/test_diff_by_ap.py
--rw-r--r--   0 joelp     (1000) joelp     (1000)     2100 2024-01-12 21:29:24.000000 unifi_tracker-0.1.0/tests/test_property_setters.py
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2024-04-26 03:27:58.014599 unifi_tracker-0.1.1/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     1071 2024-04-26 03:19:55.000000 unifi_tracker-0.1.1/LICENSE
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     7430 2024-04-26 03:27:58.014599 unifi_tracker-0.1.1/PKG-INFO
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     6861 2024-04-26 03:24:40.000000 unifi_tracker-0.1.1/README.md
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      103 2024-01-27 18:14:32.000000 unifi_tracker-0.1.1/pyproject.toml
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      694 2024-04-26 03:27:58.018599 unifi_tracker-0.1.1/setup.cfg
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2024-04-26 03:27:58.014599 unifi_tracker-0.1.1/src/
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2024-04-26 03:27:58.014599 unifi_tracker-0.1.1/src/unifi_tracker/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      160 2024-04-26 03:18:48.000000 unifi_tracker-0.1.1/src/unifi_tracker/__init__.py
+-rw-r--r--   0 joelp     (1000) joelp     (1000)    10099 2024-02-29 00:48:35.000000 unifi_tracker-0.1.1/src/unifi_tracker/unifi_tracker.py
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2024-04-26 03:27:58.014599 unifi_tracker-0.1.1/src/unifi_tracker.egg-info/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     7430 2024-04-26 03:27:58.000000 unifi_tracker-0.1.1/src/unifi_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      346 2024-04-26 03:27:58.000000 unifi_tracker-0.1.1/src/unifi_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 joelp     (1000) joelp     (1000)        1 2024-04-26 03:27:58.000000 unifi_tracker-0.1.1/src/unifi_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 joelp     (1000) joelp     (1000)       14 2024-04-26 03:27:58.000000 unifi_tracker-0.1.1/src/unifi_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2024-04-26 03:27:58.014599 unifi_tracker-0.1.1/tests/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     2230 2024-01-28 20:10:54.000000 unifi_tracker-0.1.1/tests/test_diff.py
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     2899 2024-01-28 20:10:54.000000 unifi_tracker-0.1.1/tests/test_diff_by_ap.py
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     2100 2024-01-12 21:29:24.000000 unifi_tracker-0.1.1/tests/test_property_setters.py
```

### Comparing `unifi_tracker-0.1.0/LICENSE` & `unifi_tracker-0.1.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Joel Pothering
+Copyright (c) 2024 Joel Pothering
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `unifi_tracker-0.1.0/PKG-INFO` & `unifi_tracker-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifi_tracker
-Version: 0.1.0
+Version: 0.1.1
 Summary: Track the comings and goings of WiFi clients on multiple Unifi APs and generate a diff between scans.
 Home-page: https://github.com/idatum/unifi_tracker
 Author: Joel P.
 Author-email: joelp@live.com
 Project-URL: Bug Tracker, https://github.com/idatum/unifi_tracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,15 +30,15 @@
 The Python module ```unifi_tracker``` has the functionality to query each AP using SSH by remotely executing a Unifi utility ```mca-dump```. Only SSH key auth is supported.
 
 Python Package Index:
 https://pypi.org/project/unifi-tracker/
 
 Example application:
 - 
-https://github.com/idatum/unifi_tracker/blob/main/app/device_tracker.py provides an example intended for use with HA. It's a simple service using ```unifi_tracker```:
+https://github.com/idatum/unifi_tracker/blob/main/app/device_tracker.py provides an example intended for use with the HA MQTT integration. It's a simple service using ```unifi_tracker```:
 
 1. Periodically return client info from all APs.
 2. Either union all client MACs from all APs or group client MACs by AP hostname.
 3. Do a diff between the previous and current set of MAC addresses.
 4. Publish diff to MQTT (Mosquitto) for processing in HA using the MQTT service.
 
 A few key notes:
@@ -48,15 +48,15 @@
 mqtt:
   device_tracker:
     - name: "my_phone_north"
       state_topic: "device_tracker/unifi_tracker/northAP/xx:xx:xx:xx:xx:xx"
     - name: "my_phone_south"
       state_topic: "device_tracker/unifi_tracker/southAP/xx:xx:xx:xx:xx:xx"
   ```
-Using the option to group clients by AP, this creates 2 entities for a single phone WiFi client MAC address, for the northAP and the southAP hostname APs. You can then associate both with a single user in ```SettingsPeople/Select the devices that belong to this person```.
+Using the option to group clients by AP, this creates 2 entities for a single phone WiFi client MAC address, for the northAP and the southAP hostname APs. You can then associate both with a single user in ```Settings/People/Select the devices that belong to this person```. Or, create 2 People entities, one for the northAP and one for the southAP, so you can do presence detection per AP coverage area.
 
 Starting with HA 2022.9, MQTT tracked devices are no longer defined under the ```device_tracker``` platform, and are now under ```mqtt```. With this change, there is no longer a  ```consider_home``` parameter that will work with MQTT. You now need to publish a payload of "not_home". Note that presence state will now be "unknown" until an associated MQTT message is published. This may need to be accounted for in any HA automations.
 
 Consider using the --maxIdleTime option for ```device_tracker.py``` to delay a change to "away", similar to the old behavior of ```consider_home```. Also, I recommend using the ```sshTimeout``` option to avoid potentially hanging on the SSH channel if the AP is rebooted (e.g. firmware update).
 
 If any one AP fails to return output from ```mca-dump```, the entire diff will fail. Note that clients can roam, switching from one AP to another, and if you want to know which client is connected to which AP, use the group clients by AP option.
 
@@ -78,14 +78,19 @@
 
 Summary
 -
 Works fine generally, and allows me to more freely innovate and be less dependent on another component for running HA for my home automation.
 
 History
 -
+### v0.1.1
+- Log handled vs raised exceptions differently.
+- Explicitly set callback_api_version.
+- Improve client hostname logging.
+- Consistent mac upper casing.
 ### v0.1.0
 - Functionality to group clients by AP hostname.
 - Optimization: filter client properties to save memory.
 - Improved tests.
 ### v0.0.9
 - Bug fix: Apply ```--sshTimeout``` arg value to ```timeout``` parameter of ```paramiko.client.SSHClient exec_command()```; use local scope for Queue variable.
 ### v0.0.8
```

### Comparing `unifi_tracker-0.1.0/README.md` & `unifi_tracker-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 The Python module ```unifi_tracker``` has the functionality to query each AP using SSH by remotely executing a Unifi utility ```mca-dump```. Only SSH key auth is supported.
 
 Python Package Index:
 https://pypi.org/project/unifi-tracker/
 
 Example application:
 - 
-https://github.com/idatum/unifi_tracker/blob/main/app/device_tracker.py provides an example intended for use with HA. It's a simple service using ```unifi_tracker```:
+https://github.com/idatum/unifi_tracker/blob/main/app/device_tracker.py provides an example intended for use with the HA MQTT integration. It's a simple service using ```unifi_tracker```:
 
 1. Periodically return client info from all APs.
 2. Either union all client MACs from all APs or group client MACs by AP hostname.
 3. Do a diff between the previous and current set of MAC addresses.
 4. Publish diff to MQTT (Mosquitto) for processing in HA using the MQTT service.
 
 A few key notes:
@@ -33,15 +33,15 @@
 mqtt:
   device_tracker:
     - name: "my_phone_north"
       state_topic: "device_tracker/unifi_tracker/northAP/xx:xx:xx:xx:xx:xx"
     - name: "my_phone_south"
       state_topic: "device_tracker/unifi_tracker/southAP/xx:xx:xx:xx:xx:xx"
   ```
-Using the option to group clients by AP, this creates 2 entities for a single phone WiFi client MAC address, for the northAP and the southAP hostname APs. You can then associate both with a single user in ```SettingsPeople/Select the devices that belong to this person```.
+Using the option to group clients by AP, this creates 2 entities for a single phone WiFi client MAC address, for the northAP and the southAP hostname APs. You can then associate both with a single user in ```Settings/People/Select the devices that belong to this person```. Or, create 2 People entities, one for the northAP and one for the southAP, so you can do presence detection per AP coverage area.
 
 Starting with HA 2022.9, MQTT tracked devices are no longer defined under the ```device_tracker``` platform, and are now under ```mqtt```. With this change, there is no longer a  ```consider_home``` parameter that will work with MQTT. You now need to publish a payload of "not_home". Note that presence state will now be "unknown" until an associated MQTT message is published. This may need to be accounted for in any HA automations.
 
 Consider using the --maxIdleTime option for ```device_tracker.py``` to delay a change to "away", similar to the old behavior of ```consider_home```. Also, I recommend using the ```sshTimeout``` option to avoid potentially hanging on the SSH channel if the AP is rebooted (e.g. firmware update).
 
 If any one AP fails to return output from ```mca-dump```, the entire diff will fail. Note that clients can roam, switching from one AP to another, and if you want to know which client is connected to which AP, use the group clients by AP option.
 
@@ -63,14 +63,19 @@
 
 Summary
 -
 Works fine generally, and allows me to more freely innovate and be less dependent on another component for running HA for my home automation.
 
 History
 -
+### v0.1.1
+- Log handled vs raised exceptions differently.
+- Explicitly set callback_api_version.
+- Improve client hostname logging.
+- Consistent mac upper casing.
 ### v0.1.0
 - Functionality to group clients by AP hostname.
 - Optimization: filter client properties to save memory.
 - Improved tests.
 ### v0.0.9
 - Bug fix: Apply ```--sshTimeout``` arg value to ```timeout``` parameter of ```paramiko.client.SSHClient exec_command()```; use local scope for Queue variable.
 ### v0.0.8
```

### Comparing `unifi_tracker-0.1.0/setup.cfg` & `unifi_tracker-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unifi_tracker
-version = 0.1.0
+version = 0.1.1
 author = Joel P.
 author_email = joelp@live.com
 description = Track the comings and goings of WiFi clients on multiple Unifi APs and generate a diff between scans.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/idatum/unifi_tracker
 project_urls =
```

### Comparing `unifi_tracker-0.1.0/src/unifi_tracker/unifi_tracker.py` & `unifi_tracker-0.1.1/src/unifi_tracker/unifi_tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,30 +100,31 @@
         '''Retrieve clients from a Unifi AP'''
         ap_clients = []
         out, err = self.exec_ssh_cmdline(user=ssh_username, host=ap_host, cmdline=self.UNIFI_CMDLINE)
         jresult = json.loads(out.decode('utf-8'))
         ap_hostname = jresult.get('hostname')
         if not jresult or self.UNIFI_SSID_TABLE not in jresult:
             _LOGGER.debug(f"{err}")
-            raise UnifiTrackerException(f"No results for AP address {ap_host}")
+            raise UnifiTrackerException(f"No results for AP {ap_host}") from None
         for ssid in jresult[self.UNIFI_SSID_TABLE]:
             if self.UNIFI_CLIENT_TABLE not in ssid:
                 _LOGGER.debug(jresult)
-                raise UnifiTrackerException(f"No client table {ap_host}")
+                raise UnifiTrackerException(f"No client table {ap_host} {err}") from None
             ap_clients += ssid.get(self.UNIFI_CLIENT_TABLE)
         return (ap_hostname, ap_clients)
 
     def get_client_props(self, client, ap_hostname):
         client = {p: client[p] if p in client else None for p in self._client_props}
         client['ap_hostname'] = ap_hostname
         return client
 
     def get_client_display_name(self, client):
-        mac = client['mac']
-        return f"{client['hostname']} ({mac})" if 'hostname' in client else mac
+        mac = client['mac'].upper()
+        hostname = client['hostname'] if 'hostname' in client else None
+        return f"{hostname} ({mac})" if hostname is not None else mac
 
     def get_ap_mac_clients(self, ssh_username: str, ap_host: str):
         '''MAC to client JSON from a Unifi AP'''
         _LOGGER.debug(f'Scanning {ap_host}.')
         ap_clients = self.get_ap_clients(ssh_username=ssh_username, ap_host=ap_host)
         return {client.get('mac').upper(): self.get_client_props(client, ap_clients[0]) for client in ap_clients[1]}
```

### Comparing `unifi_tracker-0.1.0/src/unifi_tracker.egg-info/PKG-INFO` & `unifi_tracker-0.1.1/src/unifi_tracker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifi_tracker
-Version: 0.1.0
+Version: 0.1.1
 Summary: Track the comings and goings of WiFi clients on multiple Unifi APs and generate a diff between scans.
 Home-page: https://github.com/idatum/unifi_tracker
 Author: Joel P.
 Author-email: joelp@live.com
 Project-URL: Bug Tracker, https://github.com/idatum/unifi_tracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,15 +30,15 @@
 The Python module ```unifi_tracker``` has the functionality to query each AP using SSH by remotely executing a Unifi utility ```mca-dump```. Only SSH key auth is supported.
 
 Python Package Index:
 https://pypi.org/project/unifi-tracker/
 
 Example application:
 - 
-https://github.com/idatum/unifi_tracker/blob/main/app/device_tracker.py provides an example intended for use with HA. It's a simple service using ```unifi_tracker```:
+https://github.com/idatum/unifi_tracker/blob/main/app/device_tracker.py provides an example intended for use with the HA MQTT integration. It's a simple service using ```unifi_tracker```:
 
 1. Periodically return client info from all APs.
 2. Either union all client MACs from all APs or group client MACs by AP hostname.
 3. Do a diff between the previous and current set of MAC addresses.
 4. Publish diff to MQTT (Mosquitto) for processing in HA using the MQTT service.
 
 A few key notes:
@@ -48,15 +48,15 @@
 mqtt:
   device_tracker:
     - name: "my_phone_north"
       state_topic: "device_tracker/unifi_tracker/northAP/xx:xx:xx:xx:xx:xx"
     - name: "my_phone_south"
       state_topic: "device_tracker/unifi_tracker/southAP/xx:xx:xx:xx:xx:xx"
   ```
-Using the option to group clients by AP, this creates 2 entities for a single phone WiFi client MAC address, for the northAP and the southAP hostname APs. You can then associate both with a single user in ```SettingsPeople/Select the devices that belong to this person```.
+Using the option to group clients by AP, this creates 2 entities for a single phone WiFi client MAC address, for the northAP and the southAP hostname APs. You can then associate both with a single user in ```Settings/People/Select the devices that belong to this person```. Or, create 2 People entities, one for the northAP and one for the southAP, so you can do presence detection per AP coverage area.
 
 Starting with HA 2022.9, MQTT tracked devices are no longer defined under the ```device_tracker``` platform, and are now under ```mqtt```. With this change, there is no longer a  ```consider_home``` parameter that will work with MQTT. You now need to publish a payload of "not_home". Note that presence state will now be "unknown" until an associated MQTT message is published. This may need to be accounted for in any HA automations.
 
 Consider using the --maxIdleTime option for ```device_tracker.py``` to delay a change to "away", similar to the old behavior of ```consider_home```. Also, I recommend using the ```sshTimeout``` option to avoid potentially hanging on the SSH channel if the AP is rebooted (e.g. firmware update).
 
 If any one AP fails to return output from ```mca-dump```, the entire diff will fail. Note that clients can roam, switching from one AP to another, and if you want to know which client is connected to which AP, use the group clients by AP option.
 
@@ -78,14 +78,19 @@
 
 Summary
 -
 Works fine generally, and allows me to more freely innovate and be less dependent on another component for running HA for my home automation.
 
 History
 -
+### v0.1.1
+- Log handled vs raised exceptions differently.
+- Explicitly set callback_api_version.
+- Improve client hostname logging.
+- Consistent mac upper casing.
 ### v0.1.0
 - Functionality to group clients by AP hostname.
 - Optimization: filter client properties to save memory.
 - Improved tests.
 ### v0.0.9
 - Bug fix: Apply ```--sshTimeout``` arg value to ```timeout``` parameter of ```paramiko.client.SSHClient exec_command()```; use local scope for Queue variable.
 ### v0.0.8
```

### Comparing `unifi_tracker-0.1.0/tests/test_diff.py` & `unifi_tracker-0.1.1/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `unifi_tracker-0.1.0/tests/test_diff_by_ap.py` & `unifi_tracker-0.1.1/tests/test_diff_by_ap.py`

 * *Files identical despite different names*

### Comparing `unifi_tracker-0.1.0/tests/test_property_setters.py` & `unifi_tracker-0.1.1/tests/test_property_setters.py`

 * *Files identical despite different names*

