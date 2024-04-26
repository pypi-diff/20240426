# Comparing `tmp/mqtt_spb_wrapper-1.0.19.tar.gz` & `tmp/mqtt_spb_wrapper-1.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt_spb_wrapper-1.0.19.tar", last modified: Sat Feb 25 09:45:12 2023, max compression
+gzip compressed data, was "mqtt_spb_wrapper-1.0.20.tar", last modified: Fri Apr 26 18:41:39 2024, max compression
```

## Comparing `mqtt_spb_wrapper-1.0.19.tar` & `mqtt_spb_wrapper-1.0.20.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 09:45:12.610216 mqtt_spb_wrapper-1.0.19/
--rw-rw-rw-   0        0        0    14476 2023-02-25 09:35:37.000000 mqtt_spb_wrapper-1.0.19/LICENSE
--rw-rw-rw-   0        0        0     7701 2023-02-25 09:45:12.605335 mqtt_spb_wrapper-1.0.19/PKG-INFO
--rw-rw-rw-   0        0        0     7199 2023-02-25 09:35:37.000000 mqtt_spb_wrapper-1.0.19/README.md
--rw-rw-rw-   0        0        0     1207 2023-02-25 09:44:40.000000 mqtt_spb_wrapper-1.0.19/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-25 09:45:12.611193 mqtt_spb_wrapper-1.0.19/setup.cfg
--rw-rw-rw-   0        0        0       55 2023-02-25 09:35:37.000000 mqtt_spb_wrapper-1.0.19/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-25 09:45:12.550715 mqtt_spb_wrapper-1.0.19/src/
-drwxrwxrwx   0        0        0        0 2023-02-25 09:45:12.571184 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/
--rw-rw-rw-   0        0        0      425 2023-02-25 09:35:37.000000 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/__init__.py
--rw-rw-rw-   0        0        0    33799 2023-02-25 09:44:34.000000 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/mqtt_spb_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-02-25 09:45:12.601432 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/spb_core/
--rw-rw-rw-   0        0        0      299 2023-02-25 09:35:37.000000 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/spb_core/__init__.py
--rw-rw-rw-   0        0        0    12488 2023-02-25 09:35:37.000000 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/spb_core/sparkplug_b.py
--rw-rw-rw-   0        0        0    56950 2023-02-25 09:35:37.000000 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/spb_core/sparkplug_b_pb2.py
--rw-rw-rw-   0        0        0     2324 2023-02-25 09:35:37.000000 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/spb_core/sparkplug_b_tools.py
-drwxrwxrwx   0        0        0        0 2023-02-25 09:45:12.587768 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper.egg-info/
--rw-rw-rw-   0        0        0     7701 2023-02-25 09:45:12.000000 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2023-02-25 09:45:12.000000 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 09:45:12.000000 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-02-25 09:45:12.000000 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-02-25 09:45:12.000000 mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 jfe03      (502) staff       (20)        0 2024-04-26 18:41:39.350477 mqtt_spb_wrapper-1.0.20/
+-rw-r--r--   0 jfe03      (502) staff       (20)    14476 2023-02-25 15:15:33.000000 mqtt_spb_wrapper-1.0.20/LICENSE
+-rw-r--r--   0 jfe03      (502) staff       (20)     7561 2024-04-26 18:41:39.350169 mqtt_spb_wrapper-1.0.20/PKG-INFO
+-rw-r--r--   0 jfe03      (502) staff       (20)     7009 2024-04-26 16:55:24.000000 mqtt_spb_wrapper-1.0.20/README.md
+-rw-r--r--   0 jfe03      (502) staff       (20)     1207 2024-04-26 18:40:42.000000 mqtt_spb_wrapper-1.0.20/pyproject.toml
+-rw-r--r--   0 jfe03      (502) staff       (20)       38 2024-04-26 18:41:39.350525 mqtt_spb_wrapper-1.0.20/setup.cfg
+-rw-r--r--   0 jfe03      (502) staff       (20)       55 2023-02-25 15:15:35.000000 mqtt_spb_wrapper-1.0.20/setup.py
+drwxr-xr-x   0 jfe03      (502) staff       (20)        0 2024-04-26 18:41:39.344029 mqtt_spb_wrapper-1.0.20/src/
+drwxr-xr-x   0 jfe03      (502) staff       (20)        0 2024-04-26 18:41:39.346278 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/
+-rw-r--r--   0 jfe03      (502) staff       (20)      425 2023-02-25 15:15:33.000000 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/__init__.py
+-rw-r--r--   0 jfe03      (502) staff       (20)    35593 2024-04-26 18:37:23.000000 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/mqtt_spb_wrapper.py
+drwxr-xr-x   0 jfe03      (502) staff       (20)        0 2024-04-26 18:41:39.349341 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/spb_core/
+-rw-r--r--   0 jfe03      (502) staff       (20)      299 2023-02-25 15:15:33.000000 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/spb_core/__init__.py
+-rw-r--r--   0 jfe03      (502) staff       (20)    12488 2023-02-25 15:15:33.000000 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/spb_core/sparkplug_b.py
+-rw-r--r--   0 jfe03      (502) staff       (20)    56950 2023-02-25 15:19:23.000000 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/spb_core/sparkplug_b_pb2.py
+-rw-r--r--   0 jfe03      (502) staff       (20)     2324 2023-02-25 15:19:35.000000 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/spb_core/sparkplug_b_tools.py
+drwxr-xr-x   0 jfe03      (502) staff       (20)        0 2024-04-26 18:41:39.349824 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper.egg-info/
+-rw-r--r--   0 jfe03      (502) staff       (20)     7561 2024-04-26 18:41:39.000000 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 jfe03      (502) staff       (20)      521 2024-04-26 18:41:39.000000 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 jfe03      (502) staff       (20)        1 2024-04-26 18:41:39.000000 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 jfe03      (502) staff       (20)       34 2024-04-26 18:41:39.000000 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper.egg-info/requires.txt
+-rw-r--r--   0 jfe03      (502) staff       (20)       17 2024-04-26 18:41:39.000000 mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper.egg-info/top_level.txt
```

### Comparing `mqtt_spb_wrapper-1.0.19/LICENSE` & `mqtt_spb_wrapper-1.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `mqtt_spb_wrapper-1.0.19/PKG-INFO` & `mqtt_spb_wrapper-1.0.20/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,204 +1,190 @@
-Metadata-Version: 2.1
-Name: mqtt_spb_wrapper
-Version: 1.0.19
-Summary: MQTT Sparkplug B v1.0 Wrapper
-Author: Javier FG
-Project-URL: Homepage, https://github.com/javier-fg/mqtt-spb-wrapper
-Keywords: sparkplug,mqtt,ecliplse,tahu,iiot,iot
-Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python Sparkplug B Wrapper
-
-This python module implements an easy way to create Sparkplug B entities on Python, abstracting one level up the already existing python Eclipse Tahu Sparkplug B v1.0 core modules.
-
-The *mqtt-spb-wrapper* python module provides the following high level objects to handle generic Sparkplug B entities in an easy way:
-
-- **MqttSpbEntityEdgeNode** - End of Network (EoN) entity 
-  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD as well as to the STATUS messages from the SCADA application.
-- **MqttSpbEntityDevice** - End of Network Device (EoND) entity 
-  - This entity that can publish DDATA, DBIRTH, DDEATH messages and subscribe to its own commands DCMD as well as to the STATUS messages from the SCADA application.
-- **MqttSpbEntityApplication** - Application entity 
-  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD, to the STATUS messages from the SCADA application as well as to all other messages from the Sparkplug B Domain ID.
-- **MqttSpbEntityScada** - SCADA entity 
-  - This entity can publish NDATA, NBIRTH, NDEATH messages as well as to send commands to all EoN and EoND (NCMD, DCMD), and subscribe to all other messages from the Sparkplug B Domain ID.
-
-Other helper classes:
-
-- **MqttSpbPayload**
-  - Class to decode the Sparkplug B binary payloads ( Google protobuf format )
-- **MqttSpbTopic** 
-  - Class to parse, decode and handle MQTT Sparkplug B topics.
-
-## Examples
-
-The repository includes a folder with some basic examples for the different type of entities, **see the folder /examples** in this repository for more examples.
-
-### Basic EoN Device
-
-The following code shows how to create an EoND entity that transmit some simple data.
-
-```python
-import time
-from mqtt_spb_wrapper import *
-
-_DEBUG = True  # Enable debug messages
-
-print("--- Sparkplug B example - End of Node Device - Simple")
-
-
-def callback_command(payload):
-    print("DEVICE received CMD: %s" % (payload))
-
-
-def callback_message(topic, payload):
-    print("Received MESSAGE: %s - %s" % (topic, payload))
-
-
-# Create the spB entity object
-group_name = "Group-001"
-edge_node_name = "Gateway-001"
-device_name = "SimpleEoND-01"
-
-device = MqttSpbEntityDevice(group_name, edge_node_name, device_name, _DEBUG)
-
-device.on_message = callback_message  # Received messages
-device.on_command = callback_command  # Callback for received commands
-
-# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
-
-# Attributes
-device.attribures.set_value("description", "Simple EoN Device node")
-device.attribures.set_value("type", "Simulated-EoND-device")
-device.attribures.set_value("version", "0.01")
-
-# Data / Telemetry
-device.data.set_value("value", 0)
-
-# Commands
-device.commands.set_value("rebirth", False)
-
-# Connect to the broker --------------------------------------------
-_connected = False
-while not _connected:
-    print("Trying to connect to broker...")
-    _connected = device.connect("localhost8", 1883)
-    if not _connected:
-        print("  Error, could not connect. Trying again in a few seconds ...")
-        time.sleep(3)
-
-# Send birth message
-device.publish_birth()
-
-
-# Send some telemetry values ---------------------------------------
-value = 0  # Simple counter
-for i in range(5):
-    # Update the data value
-    device.data.set_value("value", value)
-
-    # Send data values
-    print("Sending data - value : %d" % value)
-    device.publish_data()
-
-    # Increase counter
-    value += 1
-
-    # Sleep some time
-    time.sleep(5)
-
-# Disconnect device -------------------------------------------------
-# After disconnection the MQTT broker will send the entity DEATH message.
-print("Disconnecting device")
-device.disconnect()
-
-print("Application finished !")
-```
-
-
-
-### Basic Listener Application
-
-The following code shows how to create an application entity to listen to all Sparkplug B messages on a given group.
-
-```python
-import time
-from mqtt_spb_wrapper import *
-
-_DEBUG = True  # Enable debug messages
-
-print("--- Sparkplug B example - Application Entity Listener")
-
-
-def callback_app_message(topic, payload):
-    print("APP received MESSAGE: %s - %s" % (topic, payload))
-
-
-def callback_app_command(payload):
-    print("APP received CMD: %s" % payload)
-
-
-domain_name = "Domain-001"
-app_entity_name = "ListenApp01"
-
-app = MqttSpbEntityApplication(domain_name, app_entity_name, debug_info=_DEBUG)
-
-# Set callbacks
-app.on_message = callback_app_message
-app.on_command = callback_app_command
-
-# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
-
-# Attributes
-app.attribures.set_value("description", "Test application")
-
-# Commands
-app.commands.set_value("rebirth", False)
-
-# Connect to the broker----------------------------------------------------------------
-_connected = False
-while not _connected:
-    print("Trying to connect to broker...")
-    _connected = app.connect("localhost8", 1883)
-    if not _connected:
-        print("  Error, could not connect. Trying again in a few seconds ...")
-        time.sleep(3)
-
-# Send birth message
-app.publish_birth()
-
-
-# Loop forever, messages and commands will be handeled by the callbacks
-while True:
-    time.sleep(1000)
-```
-
-
-
-## Eclipse Sparkplug B v1.0
-
-Sparkplug is a specification for MQTT enabled devices and applications to send and receive messages in a stateful way. While MQTT is stateful by nature it doesn't ensure that all data on a receiving MQTT application is current or valid. Sparkplug provides a mechanism for ensuring that remote device or application data is current and valid. The main Sparkplug B features include:
-
-- Complex data types using templates
-- Datasets
-- Richer metrics with the ability to add property metadata for each metric
-- Metric alias support to maintain rich metric naming while keeping bandwidth usage to a minimum
-- Historical data
-- File data
-
-Sparkplug B Specification: [https://www.eclipse.org/tahu/spec/Sparkplug%20Topic%20Namespace%20and%20State%20ManagementV2.2-with%20appendix%20B%20format%20-%20Eclipse.pdf](https://www.eclipse.org/tahu/spec/Sparkplug Topic Namespace and State ManagementV2.2-with appendix B format - Eclipse.pdf)
-
-
-
-## Eclipse Tahu spB v1.0 implementation
-
-Eclipse Tahu provide client libraries and reference implementations in various languages and for various devices to show how the device/remote application must connect and disconnect from the MQTT server using the Sparkplug specification explained below.  This includes device lifecycle messages such as the required birth and last will & testament messages that must be sent to ensure the device lifecycle state and data integrity.
-
-The *mqtt-spb-wrapper* python module uses the open source Sparkplug core function from Eclipse Tahu repository, located at: https://github.com/eclipse/tahu (The current release used is v0.5.15 ).
-
-For more information visit : https://github.com/eclipse/tahu
-
+# Python Sparkplug B Wrapper
+
+This python module implements an easy way to create Sparkplug B entities on Python, abstracting one level up the already existing python Eclipse Tahu Sparkplug B v1.0 core modules.
+
+The *mqtt-spb-wrapper* python module provides the following high level objects to handle generic Sparkplug B entities in an easy way:
+
+- **MqttSpbEntityEdgeNode** - End of Network (EoN) entity 
+  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD as well as to the STATUS messages from the SCADA application.
+- **MqttSpbEntityDevice** - End of Network Device (EoND) entity 
+  - This entity that can publish DDATA, DBIRTH, DDEATH messages and subscribe to its own commands DCMD as well as to the STATUS messages from the SCADA application.
+- **MqttSpbEntityApplication** - Application entity 
+  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD, to the STATUS messages from the SCADA application as well as to all other messages from the Sparkplug B Domain ID.
+- **MqttSpbEntityScada** - SCADA entity 
+  - This entity can publish NDATA, NBIRTH, NDEATH messages as well as to send commands to all EoN and EoND (NCMD, DCMD), and subscribe to all other messages from the Sparkplug B Domain ID.
+
+Other helper classes:
+
+- **MqttSpbPayload**
+  - Class to decode the Sparkplug B binary payloads ( Google protobuf format )
+- **MqttSpbTopic** 
+  - Class to parse, decode and handle MQTT Sparkplug B topics.
+
+## Examples
+
+The repository includes a folder with some basic examples for the different type of entities, **see the folder /examples** in this repository for more examples.
+
+### Basic EoN Device
+
+The following code shows how to create an EoND entity that transmit some simple data.
+
+```python
+import time
+from mqtt_spb_wrapper import *
+
+_DEBUG = True  # Enable debug messages
+
+print("--- Sparkplug B example - End of Node Device - Simple")
+
+
+def callback_command(payload):
+    print("DEVICE received CMD: %s" % (payload))
+
+
+def callback_message(topic, payload):
+    print("Received MESSAGE: %s - %s" % (topic, payload))
+
+
+# Create the spB entity object
+group_name = "Group-001"
+edge_node_name = "Gateway-001"
+device_name = "SimpleEoND-01"
+
+device = MqttSpbEntityDevice(group_name, edge_node_name, device_name, _DEBUG)
+
+device.on_message = callback_message  # Received messages
+device.on_command = callback_command  # Callback for received commands
+
+# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
+
+# Attributes
+device.attributes.set_value("description", "Simple EoN Device node")
+device.attributes.set_value("type", "Simulated-EoND-device")
+device.attributes.set_value("version", "0.01")
+
+# Data / Telemetry
+device.data.set_value("value", 0)
+
+# Commands
+device.commands.set_value("rebirth", False)
+
+# Connect to the broker --------------------------------------------
+_connected = False
+while not _connected:
+    print("Trying to connect to broker...")
+    _connected = device.connect("localhost8", 1883)
+    if not _connected:
+        print("  Error, could not connect. Trying again in a few seconds ...")
+        time.sleep(3)
+
+# Send birth message
+device.publish_birth()
+
+
+# Send some telemetry values ---------------------------------------
+value = 0  # Simple counter
+for i in range(5):
+    # Update the data value
+    device.data.set_value("value", value)
+
+    # Send data values
+    print("Sending data - value : %d" % value)
+    device.publish_data()
+
+    # Increase counter
+    value += 1
+
+    # Sleep some time
+    time.sleep(5)
+
+# Disconnect device -------------------------------------------------
+# After disconnection the MQTT broker will send the entity DEATH message.
+print("Disconnecting device")
+device.disconnect()
+
+print("Application finished !")
+```
+
+
+
+### Basic Listener Application
+
+The following code shows how to create an application entity to listen to all Sparkplug B messages on a given group.
+
+```python
+import time
+from mqtt_spb_wrapper import *
+
+_DEBUG = True  # Enable debug messages
+
+print("--- Sparkplug B example - Application Entity Listener")
+
+
+def callback_app_message(topic, payload):
+    print("APP received MESSAGE: %s - %s" % (topic, payload))
+
+
+def callback_app_command(payload):
+    print("APP received CMD: %s" % payload)
+
+
+domain_name = "Domain-001"
+app_entity_name = "ListenApp01"
+
+app = MqttSpbEntityApplication(domain_name, app_entity_name, debug_info=_DEBUG)
+
+# Set callbacks
+app.on_message = callback_app_message
+app.on_command = callback_app_command
+
+# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
+
+# Attributes
+app.attributes.set_value("description", "Test application")
+
+# Commands
+app.commands.set_value("rebirth", False)
+
+# Connect to the broker----------------------------------------------------------------
+_connected = False
+while not _connected:
+    print("Trying to connect to broker...")
+    _connected = app.connect("localhost8", 1883)
+    if not _connected:
+        print("  Error, could not connect. Trying again in a few seconds ...")
+        time.sleep(3)
+
+# Send birth message
+app.publish_birth()
+
+
+# Loop forever, messages and commands will be handeled by the callbacks
+while True:
+    time.sleep(1000)
+```
+
+
+
+## Eclipse Sparkplug B v1.0
+
+Sparkplug is a specification for MQTT enabled devices and applications to send and receive messages in a stateful way. While MQTT is stateful by nature it doesn't ensure that all data on a receiving MQTT application is current or valid. Sparkplug provides a mechanism for ensuring that remote device or application data is current and valid. The main Sparkplug B features include:
+
+- Complex data types using templates
+- Datasets
+- Richer metrics with the ability to add property metadata for each metric
+- Metric alias support to maintain rich metric naming while keeping bandwidth usage to a minimum
+- Historical data
+- File data
+
+Sparkplug B Specification: [https://www.eclipse.org/tahu/spec/Sparkplug%20Topic%20Namespace%20and%20State%20ManagementV2.2-with%20appendix%20B%20format%20-%20Eclipse.pdf](https://www.eclipse.org/tahu/spec/Sparkplug Topic Namespace and State ManagementV2.2-with appendix B format - Eclipse.pdf)
+
+
+
+## Eclipse Tahu spB v1.0 implementation
+
+Eclipse Tahu provide client libraries and reference implementations in various languages and for various devices to show how the device/remote application must connect and disconnect from the MQTT server using the Sparkplug specification explained below.  This includes device lifecycle messages such as the required birth and last will & testament messages that must be sent to ensure the device lifecycle state and data integrity.
+
+The *mqtt-spb-wrapper* python module uses the open source Sparkplug core function from Eclipse Tahu repository, located at: https://github.com/eclipse/tahu (The current release used is v0.5.15 ).
+
+For more information visit : https://github.com/eclipse/tahu
+
```

### Comparing `mqtt_spb_wrapper-1.0.19/README.md` & `mqtt_spb_wrapper-1.0.20/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,190 +1,206 @@
-# Python Sparkplug B Wrapper
-
-This python module implements an easy way to create Sparkplug B entities on Python, abstracting one level up the already existing python Eclipse Tahu Sparkplug B v1.0 core modules.
-
-The *mqtt-spb-wrapper* python module provides the following high level objects to handle generic Sparkplug B entities in an easy way:
-
-- **MqttSpbEntityEdgeNode** - End of Network (EoN) entity 
-  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD as well as to the STATUS messages from the SCADA application.
-- **MqttSpbEntityDevice** - End of Network Device (EoND) entity 
-  - This entity that can publish DDATA, DBIRTH, DDEATH messages and subscribe to its own commands DCMD as well as to the STATUS messages from the SCADA application.
-- **MqttSpbEntityApplication** - Application entity 
-  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD, to the STATUS messages from the SCADA application as well as to all other messages from the Sparkplug B Domain ID.
-- **MqttSpbEntityScada** - SCADA entity 
-  - This entity can publish NDATA, NBIRTH, NDEATH messages as well as to send commands to all EoN and EoND (NCMD, DCMD), and subscribe to all other messages from the Sparkplug B Domain ID.
-
-Other helper classes:
-
-- **MqttSpbPayload**
-  - Class to decode the Sparkplug B binary payloads ( Google protobuf format )
-- **MqttSpbTopic** 
-  - Class to parse, decode and handle MQTT Sparkplug B topics.
-
-## Examples
-
-The repository includes a folder with some basic examples for the different type of entities, **see the folder /examples** in this repository for more examples.
-
-### Basic EoN Device
-
-The following code shows how to create an EoND entity that transmit some simple data.
-
-```python
-import time
-from mqtt_spb_wrapper import *
-
-_DEBUG = True  # Enable debug messages
-
-print("--- Sparkplug B example - End of Node Device - Simple")
-
-
-def callback_command(payload):
-    print("DEVICE received CMD: %s" % (payload))
-
-
-def callback_message(topic, payload):
-    print("Received MESSAGE: %s - %s" % (topic, payload))
-
-
-# Create the spB entity object
-group_name = "Group-001"
-edge_node_name = "Gateway-001"
-device_name = "SimpleEoND-01"
-
-device = MqttSpbEntityDevice(group_name, edge_node_name, device_name, _DEBUG)
-
-device.on_message = callback_message  # Received messages
-device.on_command = callback_command  # Callback for received commands
-
-# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
-
-# Attributes
-device.attribures.set_value("description", "Simple EoN Device node")
-device.attribures.set_value("type", "Simulated-EoND-device")
-device.attribures.set_value("version", "0.01")
-
-# Data / Telemetry
-device.data.set_value("value", 0)
-
-# Commands
-device.commands.set_value("rebirth", False)
-
-# Connect to the broker --------------------------------------------
-_connected = False
-while not _connected:
-    print("Trying to connect to broker...")
-    _connected = device.connect("localhost8", 1883)
-    if not _connected:
-        print("  Error, could not connect. Trying again in a few seconds ...")
-        time.sleep(3)
-
-# Send birth message
-device.publish_birth()
-
-
-# Send some telemetry values ---------------------------------------
-value = 0  # Simple counter
-for i in range(5):
-    # Update the data value
-    device.data.set_value("value", value)
-
-    # Send data values
-    print("Sending data - value : %d" % value)
-    device.publish_data()
-
-    # Increase counter
-    value += 1
-
-    # Sleep some time
-    time.sleep(5)
-
-# Disconnect device -------------------------------------------------
-# After disconnection the MQTT broker will send the entity DEATH message.
-print("Disconnecting device")
-device.disconnect()
-
-print("Application finished !")
-```
-
-
-
-### Basic Listener Application
-
-The following code shows how to create an application entity to listen to all Sparkplug B messages on a given group.
-
-```python
-import time
-from mqtt_spb_wrapper import *
-
-_DEBUG = True  # Enable debug messages
-
-print("--- Sparkplug B example - Application Entity Listener")
-
-
-def callback_app_message(topic, payload):
-    print("APP received MESSAGE: %s - %s" % (topic, payload))
-
-
-def callback_app_command(payload):
-    print("APP received CMD: %s" % payload)
-
-
-domain_name = "Domain-001"
-app_entity_name = "ListenApp01"
-
-app = MqttSpbEntityApplication(domain_name, app_entity_name, debug_info=_DEBUG)
-
-# Set callbacks
-app.on_message = callback_app_message
-app.on_command = callback_app_command
-
-# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
-
-# Attributes
-app.attribures.set_value("description", "Test application")
-
-# Commands
-app.commands.set_value("rebirth", False)
-
-# Connect to the broker----------------------------------------------------------------
-_connected = False
-while not _connected:
-    print("Trying to connect to broker...")
-    _connected = app.connect("localhost8", 1883)
-    if not _connected:
-        print("  Error, could not connect. Trying again in a few seconds ...")
-        time.sleep(3)
-
-# Send birth message
-app.publish_birth()
-
-
-# Loop forever, messages and commands will be handeled by the callbacks
-while True:
-    time.sleep(1000)
-```
-
-
-
-## Eclipse Sparkplug B v1.0
-
-Sparkplug is a specification for MQTT enabled devices and applications to send and receive messages in a stateful way. While MQTT is stateful by nature it doesn't ensure that all data on a receiving MQTT application is current or valid. Sparkplug provides a mechanism for ensuring that remote device or application data is current and valid. The main Sparkplug B features include:
-
-- Complex data types using templates
-- Datasets
-- Richer metrics with the ability to add property metadata for each metric
-- Metric alias support to maintain rich metric naming while keeping bandwidth usage to a minimum
-- Historical data
-- File data
-
-Sparkplug B Specification: [https://www.eclipse.org/tahu/spec/Sparkplug%20Topic%20Namespace%20and%20State%20ManagementV2.2-with%20appendix%20B%20format%20-%20Eclipse.pdf](https://www.eclipse.org/tahu/spec/Sparkplug Topic Namespace and State ManagementV2.2-with appendix B format - Eclipse.pdf)
-
-
-
-## Eclipse Tahu spB v1.0 implementation
-
-Eclipse Tahu provide client libraries and reference implementations in various languages and for various devices to show how the device/remote application must connect and disconnect from the MQTT server using the Sparkplug specification explained below.  This includes device lifecycle messages such as the required birth and last will & testament messages that must be sent to ensure the device lifecycle state and data integrity.
-
-The *mqtt-spb-wrapper* python module uses the open source Sparkplug core function from Eclipse Tahu repository, located at: https://github.com/eclipse/tahu (The current release used is v0.5.15 ).
-
-For more information visit : https://github.com/eclipse/tahu
-
+Metadata-Version: 2.1
+Name: mqtt_spb_wrapper
+Version: 1.0.20
+Summary: MQTT Sparkplug B v1.0 Wrapper
+Author: Javier FG
+Project-URL: Homepage, https://github.com/javier-fg/mqtt-spb-wrapper
+Keywords: sparkplug,mqtt,ecliplse,tahu,iiot,iot
+Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: paho_mqtt==1.6.1
+Requires-Dist: protobuf==3.20.3
+
+# Python Sparkplug B Wrapper
+
+This python module implements an easy way to create Sparkplug B entities on Python, abstracting one level up the already existing python Eclipse Tahu Sparkplug B v1.0 core modules.
+
+The *mqtt-spb-wrapper* python module provides the following high level objects to handle generic Sparkplug B entities in an easy way:
+
+- **MqttSpbEntityEdgeNode** - End of Network (EoN) entity 
+  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD as well as to the STATUS messages from the SCADA application.
+- **MqttSpbEntityDevice** - End of Network Device (EoND) entity 
+  - This entity that can publish DDATA, DBIRTH, DDEATH messages and subscribe to its own commands DCMD as well as to the STATUS messages from the SCADA application.
+- **MqttSpbEntityApplication** - Application entity 
+  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD, to the STATUS messages from the SCADA application as well as to all other messages from the Sparkplug B Domain ID.
+- **MqttSpbEntityScada** - SCADA entity 
+  - This entity can publish NDATA, NBIRTH, NDEATH messages as well as to send commands to all EoN and EoND (NCMD, DCMD), and subscribe to all other messages from the Sparkplug B Domain ID.
+
+Other helper classes:
+
+- **MqttSpbPayload**
+  - Class to decode the Sparkplug B binary payloads ( Google protobuf format )
+- **MqttSpbTopic** 
+  - Class to parse, decode and handle MQTT Sparkplug B topics.
+
+## Examples
+
+The repository includes a folder with some basic examples for the different type of entities, **see the folder /examples** in this repository for more examples.
+
+### Basic EoN Device
+
+The following code shows how to create an EoND entity that transmit some simple data.
+
+```python
+import time
+from mqtt_spb_wrapper import *
+
+_DEBUG = True  # Enable debug messages
+
+print("--- Sparkplug B example - End of Node Device - Simple")
+
+
+def callback_command(payload):
+    print("DEVICE received CMD: %s" % (payload))
+
+
+def callback_message(topic, payload):
+    print("Received MESSAGE: %s - %s" % (topic, payload))
+
+
+# Create the spB entity object
+group_name = "Group-001"
+edge_node_name = "Gateway-001"
+device_name = "SimpleEoND-01"
+
+device = MqttSpbEntityDevice(group_name, edge_node_name, device_name, _DEBUG)
+
+device.on_message = callback_message  # Received messages
+device.on_command = callback_command  # Callback for received commands
+
+# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
+
+# Attributes
+device.attributes.set_value("description", "Simple EoN Device node")
+device.attributes.set_value("type", "Simulated-EoND-device")
+device.attributes.set_value("version", "0.01")
+
+# Data / Telemetry
+device.data.set_value("value", 0)
+
+# Commands
+device.commands.set_value("rebirth", False)
+
+# Connect to the broker --------------------------------------------
+_connected = False
+while not _connected:
+    print("Trying to connect to broker...")
+    _connected = device.connect("localhost8", 1883)
+    if not _connected:
+        print("  Error, could not connect. Trying again in a few seconds ...")
+        time.sleep(3)
+
+# Send birth message
+device.publish_birth()
+
+
+# Send some telemetry values ---------------------------------------
+value = 0  # Simple counter
+for i in range(5):
+    # Update the data value
+    device.data.set_value("value", value)
+
+    # Send data values
+    print("Sending data - value : %d" % value)
+    device.publish_data()
+
+    # Increase counter
+    value += 1
+
+    # Sleep some time
+    time.sleep(5)
+
+# Disconnect device -------------------------------------------------
+# After disconnection the MQTT broker will send the entity DEATH message.
+print("Disconnecting device")
+device.disconnect()
+
+print("Application finished !")
+```
+
+
+
+### Basic Listener Application
+
+The following code shows how to create an application entity to listen to all Sparkplug B messages on a given group.
+
+```python
+import time
+from mqtt_spb_wrapper import *
+
+_DEBUG = True  # Enable debug messages
+
+print("--- Sparkplug B example - Application Entity Listener")
+
+
+def callback_app_message(topic, payload):
+    print("APP received MESSAGE: %s - %s" % (topic, payload))
+
+
+def callback_app_command(payload):
+    print("APP received CMD: %s" % payload)
+
+
+domain_name = "Domain-001"
+app_entity_name = "ListenApp01"
+
+app = MqttSpbEntityApplication(domain_name, app_entity_name, debug_info=_DEBUG)
+
+# Set callbacks
+app.on_message = callback_app_message
+app.on_command = callback_app_command
+
+# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
+
+# Attributes
+app.attributes.set_value("description", "Test application")
+
+# Commands
+app.commands.set_value("rebirth", False)
+
+# Connect to the broker----------------------------------------------------------------
+_connected = False
+while not _connected:
+    print("Trying to connect to broker...")
+    _connected = app.connect("localhost8", 1883)
+    if not _connected:
+        print("  Error, could not connect. Trying again in a few seconds ...")
+        time.sleep(3)
+
+# Send birth message
+app.publish_birth()
+
+
+# Loop forever, messages and commands will be handeled by the callbacks
+while True:
+    time.sleep(1000)
+```
+
+
+
+## Eclipse Sparkplug B v1.0
+
+Sparkplug is a specification for MQTT enabled devices and applications to send and receive messages in a stateful way. While MQTT is stateful by nature it doesn't ensure that all data on a receiving MQTT application is current or valid. Sparkplug provides a mechanism for ensuring that remote device or application data is current and valid. The main Sparkplug B features include:
+
+- Complex data types using templates
+- Datasets
+- Richer metrics with the ability to add property metadata for each metric
+- Metric alias support to maintain rich metric naming while keeping bandwidth usage to a minimum
+- Historical data
+- File data
+
+Sparkplug B Specification: [https://www.eclipse.org/tahu/spec/Sparkplug%20Topic%20Namespace%20and%20State%20ManagementV2.2-with%20appendix%20B%20format%20-%20Eclipse.pdf](https://www.eclipse.org/tahu/spec/Sparkplug Topic Namespace and State ManagementV2.2-with appendix B format - Eclipse.pdf)
+
+
+
+## Eclipse Tahu spB v1.0 implementation
+
+Eclipse Tahu provide client libraries and reference implementations in various languages and for various devices to show how the device/remote application must connect and disconnect from the MQTT server using the Sparkplug specification explained below.  This includes device lifecycle messages such as the required birth and last will & testament messages that must be sent to ensure the device lifecycle state and data integrity.
+
+The *mqtt-spb-wrapper* python module uses the open source Sparkplug core function from Eclipse Tahu repository, located at: https://github.com/eclipse/tahu (The current release used is v0.5.15 ).
+
+For more information visit : https://github.com/eclipse/tahu
+
```

### Comparing `mqtt_spb_wrapper-1.0.19/pyproject.toml` & `mqtt_spb_wrapper-1.0.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mqtt_spb_wrapper"
-version = "1.0.19"
+version = "1.0.20"
 description = "MQTT Sparkplug B v1.0 Wrapper"
 readme = "README.md"
 authors = [{ name = "Javier FG" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["sparkplug", "mqtt", "ecliplse", "tahu", "iiot", "iot"]
 dependencies = [
     "paho_mqtt==1.6.1",
-    "protobuf==3.20.1",
+    "protobuf==3.20.3",
 ]
 requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/javier-fg/mqtt-spb-wrapper"
 
 # Package distribution extracted from:
```

### Comparing `mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/mqtt_spb_wrapper.py` & `mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/mqtt_spb_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         self.entity_uid = None        # Generic attributes
         self.entity_class = None
         self.entity_subclass = None
 
         self.is_alive = True
         self.is_birth_published = False
 
-        self.attribures = self._ValuesGroup()
+        self.attributes = self._ValuesGroup()
         self.data = self._ValuesGroup()
         self.commands = self._ValuesGroup()
 
         self.on_command = None  # Callback function when a comand is received
         self.on_connect = None
         self.on_disconnect = None
         self.on_message = None
@@ -203,20 +203,20 @@
     def get_dictionary(self):
         temp = {}
         temp['spb_group_name'] = self._spb_group_name
         temp['spb_eon_name'] = self._spb_eon_name
         if self._spb_eon_device_name is not None:
             temp['spb_eon_device_name'] = self._spb_eon_device_name
         temp['data'] = self.data.get_dictionary()
-        temp['attributes'] = self.attribures.get_dictionary()
+        temp['attributes'] = self.attributes.get_dictionary()
         temp['commands'] = self.commands.get_dictionary()
         return temp
 
     def is_empty(self):
-        if self.data.is_empty() and self.attribures.is_empty() and self.commands.is_empty():
+        if self.data.is_empty() and self.attributes.is_empty() and self.commands.is_empty():
             return True
         return False
 
     @property
     def spb_group_name(self):
         return self._spb_group_name
 
@@ -258,16 +258,16 @@
 
         if self._spb_eon_device_name is None:  # EoN type
             payload = getNodeBirthPayload()
         else:  # Device
             payload = getDeviceBirthPayload()
 
         # Attributes
-        if not self.attribures.is_empty():
-            for item in self.attribures.values:
+        if not self.attributes.is_empty():
+            for item in self.attributes.values:
                 name = "ATTR/" + item.name
                 addMetric(payload, name, None, self._spb_data_type(item.value), item.value, item.timestamp)
 
         # Data
         if not self.data.is_empty():
             for item in self.data.values:
                 name = "DATA/" + item.name
@@ -290,15 +290,15 @@
         if payload is not None:
 
             # Iterate over the metrics to update the data fields
             for field in payload.get('metrics', []):
 
                 if field['name'].startswith("ATTR/"):
                     field['name'] = field['name'][5:]
-                    self.attribures.set_value(field['name'], field['value'], field['timestamp'])  # update field
+                    self.attributes.set_value(field['name'], field['value'], field['timestamp'])  # update field
 
                 elif field['name'].startswith("CMD/"):
                     field['name'] = field['name'][4:]
                     self.commands.set_value(field['name'], field['value'], field['timestamp'])  # update field
 
                 elif field['name'].startswith("DATA/"):
                     field['name'] = field['name'][5:]
@@ -330,47 +330,47 @@
 
             #Iterate over the metrics to update the data fields
             for field in payload.get('metrics', []):
                 self.data.set_value(field['name'], field['value'], field['timestamp']) # update field
 
         return payload
 
-    def publish_birth(self):
+    def publish_birth(self, QoS=0):
 
         if not self.is_connected():  # If not connected
             logger.warning("%s - Could not send publish_birth(), not connected to MQTT server" % self._entity_domain)
             return False
 
         if self.is_empty():  # If no data (Data, attributes, commands )
             logger.warning(
                 "%s - Could not send publish_birth(), entity doesn't have data ( attributes, data, commands )" % self._entity_domain)
             return False
 
         # If it is a type entity SCADA, change the BIRTH certificate
         if self._entity_is_scada:
             topic = "spBv1.0/" + self.spb_group_name + "/STATE/" + self._spb_eon_name
             self._loopback_topic = topic
-            self._mqtt.publish(topic, "ONLINE".encode("utf-8"), 0, True)
+            self._mqtt.publish(topic, "ONLINE".encode("utf-8"), QoS, True)
             logger.info("%s - Published STATE BIRTH message " % (self._entity_domain))
             return
 
         # Publish BIRTH message
         payload_bytes = self.serialize_payload_birth()
         if self._spb_eon_device_name is None:  # EoN
             topic = "spBv1.0/" + self.spb_group_name + "/NBIRTH/" + self._spb_eon_name
         else:
             topic = "spBv1.0/" + self.spb_group_name + "/DBIRTH/" + self._spb_eon_name + "/" + self._spb_eon_device_name
         self._loopback_topic = topic
-        self._mqtt.publish(topic, payload_bytes, 0, True)
+        self._mqtt.publish(topic, payload_bytes, QoS, True)
 
         logger.info("%s - Published BIRTH message" % (self._entity_domain))
 
         self.is_birth_published = True
 
-    def publish_data(self, send_all=False):
+    def publish_data(self, send_all=False, QoS=0):
         """
             Send the new updated data to the MQTT broker as a Sparkplug B DATA message.
 
         :param send_all: boolean    True: Send all data fields, False: send only updated field values.
         :return:                    result
         """
 
@@ -390,15 +390,15 @@
             payload_bytes = self.serialize_payload_data(send_all)   # Get the data payload
 
             if self._spb_eon_device_name is None:  # EoN
                 topic = "spBv1.0/" + self.spb_group_name + "/NDATA/" + self._spb_eon_name
             else:
                 topic = "spBv1.0/" + self.spb_group_name + "/DDATA/" + self._spb_eon_name + "/" + self._spb_eon_device_name
             self._loopback_topic = topic
-            self._mqtt.publish(topic, payload_bytes, 0, False)
+            self._mqtt.publish(topic, payload_bytes, QoS, False)
 
             logger.info("%s - Published DATA message %s" % (self._entity_domain, topic))
             return True
 
         logger.warning("%s - Could not publish DATA message, may be data no new data values?" % (self._entity_domain))
         return False
 
@@ -407,14 +407,15 @@
                 port=1883,
                 user="",
                 password="",
 				use_tls=False,
                 tls_ca_path="",
                 tls_cert_path="",
                 tls_key_path="",
+                tls_insecure=False,
                 timeout=5):
 
         # If we are already connected, then exit
         if self.is_connected():
             return True
 
         # MQTT Client configuration
@@ -425,22 +426,28 @@
         self._mqtt.on_disconnect = self._mqtt_on_disconnect
         self._mqtt.on_message = self._mqtt_on_message
 
         if user != "":
             self._mqtt.username_pw_set(user, password)
 
         # If client certificates are provided
-        if tls_cert_path and tls_cert_path and tls_key_path:
+        if tls_ca_path and tls_cert_path and tls_key_path:
             logger.debug("Setting CA client certificates")
-            import ssl
-            self._mqtt.tls_set(ca_certs=tls_cert_path, certfile=tls_cert_path, keyfile=tls_key_path, cert_reqs=ssl.CERT_NONE)
-            # self._mqtt.tls_insecure_set(True)
+
+            if tls_insecure:
+                logger.debug("Setting CA client certificates - IMPORTANT CA insecure mode ( use only for testing )")
+                import ssl
+                self._mqtt.tls_set(ca_certs=tls_ca_path, certfile=tls_cert_path, keyfile=tls_key_path, cert_reqs=ssl.CERT_NONE)
+                self._mqtt.tls_insecure_set(True)
+            else:
+                logger.debug("Setting CA client certificates")
+                self._mqtt.tls_set(ca_certs=tls_ca_path, certfile=tls_cert_path, keyfile=tls_key_path)
 
         #If only CA is proviced.
-        elif tls_cert_path:
+        elif tls_ca_path:
             logger.debug("Setting CA certificate")
             self._mqtt.tls_set(ca_certs=tls_ca_path)
 
         # If TLS is enabled
         else:
             if use_tls:
                 self._mqtt.tls_set()    # Enable TLS encryption
@@ -473,19 +480,35 @@
         _timeout = time.time() + timeout
         while not self.is_connected() and _timeout > time.time():
             time.sleep(0.1)
 
         # Return if we connected successfully
         return self.is_connected()
 
-    def disconnect(self):
+    def disconnect(self, skip_death_publish=False):
 
         logger.info("%s - Disconnecting from MQTT server" % (self._entity_domain))
 
         if self._mqtt is not None:
+
+            # Send the DEATH message
+            if not skip_death_publish:
+                if self._entity_is_scada:  # If it is a type entity SCADA, change the DEATH certificate
+                    topic = "spBv1.0/" + self.spb_group_name + "/STATE/" + self._spb_eon_name
+                    self._mqtt.publish(topic, "OFFLINE".encode("utf-8"), 0, False)
+                else:  # Normal node
+                    payload = getNodeDeathPayload()
+                    payload_bytes = bytearray(payload.SerializeToString())
+                    if self._spb_eon_device_name is None:  # EoN
+                        topic = "spBv1.0/" + self.spb_group_name + "/NDEATHx/" + self._spb_eon_name
+                    else:
+                        topic = "spBv1.0/" + self.spb_group_name + "/DDEATHx/" + self._spb_eon_name + "/" + self._spb_eon_device_name
+                    self._mqtt.publish(topic, payload_bytes, 0, False)  # Set message
+
+            # Disconnect from MQTT broker
             self._mqtt.loop_stop()
             time.sleep(0.1)
             self._mqtt.disconnect()
             time.sleep(0.1)
         self._mqtt = None
 
     def is_connected(self):
@@ -529,15 +552,15 @@
 
     def _mqtt_on_message(self, client, userdata, msg):
 
         # Check if loopback message
         if self._loopback_topic == msg.topic:
                 return
 
-        msg_ts_rx = int(round(datetime.datetime.now().utcnow().timestamp() * 1000))  # Save the current timestamp
+        msg_ts_rx = int(datetime.datetime.utcnow().timestamp() * 1000)  # Save the current timestamp
 
         logger.info("%s - Message received  %s" % (self._entity_domain, msg.topic))
 
         # Parse the topic namespace ------------------------------------------------
         topic = MqttSpbTopic(msg.topic)  # Parse and get the topic object
 
         # Check that the namespace and group are correct
@@ -608,15 +631,15 @@
                     self.on_command(payload)
 
     class _ValueItem:
         def __init__(self, name, value, timestamp=None):
             self.name = name
             self._value = value
             if timestamp is None:
-                self._timestamp = int(datetime.datetime.now().utcnow().timestamp() * 1000)
+                self._timestamp = int(datetime.datetime.utcnow().timestamp() * 1000)
             else:
                 self._timestamp = timestamp
             self.is_updated = True
 
         def __str__(self):
             return str(self.get_dictionary())
 
@@ -708,26 +731,35 @@
             return False
 
         def clear(self):
             self.values = []
 
         def set_value(self, name, value, timestamp=None):
 
+            # If value is set to None, ignore the update
+            if value is None:
+                return False
+
             # If exist update the value, otherwise add the element.
             for item in self.values:
                 if item.name == name:
                     item.value = value
                     item.timestamp = timestamp  # If timestamp is none, the current time will be used.
                     return True
 
             # item was not found, then add it to the list.
             self.values.append(MqttSpbEntityDevice._ValueItem(name, value, timestamp))
-
             return True
 
+        def remove_value(self, name):
+            # If exist remove the value by its name.
+            original_count = len(self.values)
+            self.values = [value for value in self.values if value.name != name]
+            return len(self.values) < original_count
+
         def set_dictionary(self, values: dict, timestamp=None):
             """
                 Import a list of values based on a dictionary FieldName:FieldValue
             :param values:      Dictionary with fields-values
             :param timestamp:   Timestamp value in ms
             :return:            Result
             """
```

### Comparing `mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/spb_core/sparkplug_b.py` & `mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/spb_core/sparkplug_b.py`

 * *Files identical despite different names*

### Comparing `mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/spb_core/sparkplug_b_pb2.py` & `mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/spb_core/sparkplug_b_pb2.py`

 * *Files identical despite different names*

### Comparing `mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper/spb_core/sparkplug_b_tools.py` & `mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper/spb_core/sparkplug_b_tools.py`

 * *Files identical despite different names*

### Comparing `mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper.egg-info/PKG-INFO` & `mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,204 +1,206 @@
-Metadata-Version: 2.1
-Name: mqtt-spb-wrapper
-Version: 1.0.19
-Summary: MQTT Sparkplug B v1.0 Wrapper
-Author: Javier FG
-Project-URL: Homepage, https://github.com/javier-fg/mqtt-spb-wrapper
-Keywords: sparkplug,mqtt,ecliplse,tahu,iiot,iot
-Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python Sparkplug B Wrapper
-
-This python module implements an easy way to create Sparkplug B entities on Python, abstracting one level up the already existing python Eclipse Tahu Sparkplug B v1.0 core modules.
-
-The *mqtt-spb-wrapper* python module provides the following high level objects to handle generic Sparkplug B entities in an easy way:
-
-- **MqttSpbEntityEdgeNode** - End of Network (EoN) entity 
-  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD as well as to the STATUS messages from the SCADA application.
-- **MqttSpbEntityDevice** - End of Network Device (EoND) entity 
-  - This entity that can publish DDATA, DBIRTH, DDEATH messages and subscribe to its own commands DCMD as well as to the STATUS messages from the SCADA application.
-- **MqttSpbEntityApplication** - Application entity 
-  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD, to the STATUS messages from the SCADA application as well as to all other messages from the Sparkplug B Domain ID.
-- **MqttSpbEntityScada** - SCADA entity 
-  - This entity can publish NDATA, NBIRTH, NDEATH messages as well as to send commands to all EoN and EoND (NCMD, DCMD), and subscribe to all other messages from the Sparkplug B Domain ID.
-
-Other helper classes:
-
-- **MqttSpbPayload**
-  - Class to decode the Sparkplug B binary payloads ( Google protobuf format )
-- **MqttSpbTopic** 
-  - Class to parse, decode and handle MQTT Sparkplug B topics.
-
-## Examples
-
-The repository includes a folder with some basic examples for the different type of entities, **see the folder /examples** in this repository for more examples.
-
-### Basic EoN Device
-
-The following code shows how to create an EoND entity that transmit some simple data.
-
-```python
-import time
-from mqtt_spb_wrapper import *
-
-_DEBUG = True  # Enable debug messages
-
-print("--- Sparkplug B example - End of Node Device - Simple")
-
-
-def callback_command(payload):
-    print("DEVICE received CMD: %s" % (payload))
-
-
-def callback_message(topic, payload):
-    print("Received MESSAGE: %s - %s" % (topic, payload))
-
-
-# Create the spB entity object
-group_name = "Group-001"
-edge_node_name = "Gateway-001"
-device_name = "SimpleEoND-01"
-
-device = MqttSpbEntityDevice(group_name, edge_node_name, device_name, _DEBUG)
-
-device.on_message = callback_message  # Received messages
-device.on_command = callback_command  # Callback for received commands
-
-# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
-
-# Attributes
-device.attribures.set_value("description", "Simple EoN Device node")
-device.attribures.set_value("type", "Simulated-EoND-device")
-device.attribures.set_value("version", "0.01")
-
-# Data / Telemetry
-device.data.set_value("value", 0)
-
-# Commands
-device.commands.set_value("rebirth", False)
-
-# Connect to the broker --------------------------------------------
-_connected = False
-while not _connected:
-    print("Trying to connect to broker...")
-    _connected = device.connect("localhost8", 1883)
-    if not _connected:
-        print("  Error, could not connect. Trying again in a few seconds ...")
-        time.sleep(3)
-
-# Send birth message
-device.publish_birth()
-
-
-# Send some telemetry values ---------------------------------------
-value = 0  # Simple counter
-for i in range(5):
-    # Update the data value
-    device.data.set_value("value", value)
-
-    # Send data values
-    print("Sending data - value : %d" % value)
-    device.publish_data()
-
-    # Increase counter
-    value += 1
-
-    # Sleep some time
-    time.sleep(5)
-
-# Disconnect device -------------------------------------------------
-# After disconnection the MQTT broker will send the entity DEATH message.
-print("Disconnecting device")
-device.disconnect()
-
-print("Application finished !")
-```
-
-
-
-### Basic Listener Application
-
-The following code shows how to create an application entity to listen to all Sparkplug B messages on a given group.
-
-```python
-import time
-from mqtt_spb_wrapper import *
-
-_DEBUG = True  # Enable debug messages
-
-print("--- Sparkplug B example - Application Entity Listener")
-
-
-def callback_app_message(topic, payload):
-    print("APP received MESSAGE: %s - %s" % (topic, payload))
-
-
-def callback_app_command(payload):
-    print("APP received CMD: %s" % payload)
-
-
-domain_name = "Domain-001"
-app_entity_name = "ListenApp01"
-
-app = MqttSpbEntityApplication(domain_name, app_entity_name, debug_info=_DEBUG)
-
-# Set callbacks
-app.on_message = callback_app_message
-app.on_command = callback_app_command
-
-# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
-
-# Attributes
-app.attribures.set_value("description", "Test application")
-
-# Commands
-app.commands.set_value("rebirth", False)
-
-# Connect to the broker----------------------------------------------------------------
-_connected = False
-while not _connected:
-    print("Trying to connect to broker...")
-    _connected = app.connect("localhost8", 1883)
-    if not _connected:
-        print("  Error, could not connect. Trying again in a few seconds ...")
-        time.sleep(3)
-
-# Send birth message
-app.publish_birth()
-
-
-# Loop forever, messages and commands will be handeled by the callbacks
-while True:
-    time.sleep(1000)
-```
-
-
-
-## Eclipse Sparkplug B v1.0
-
-Sparkplug is a specification for MQTT enabled devices and applications to send and receive messages in a stateful way. While MQTT is stateful by nature it doesn't ensure that all data on a receiving MQTT application is current or valid. Sparkplug provides a mechanism for ensuring that remote device or application data is current and valid. The main Sparkplug B features include:
-
-- Complex data types using templates
-- Datasets
-- Richer metrics with the ability to add property metadata for each metric
-- Metric alias support to maintain rich metric naming while keeping bandwidth usage to a minimum
-- Historical data
-- File data
-
-Sparkplug B Specification: [https://www.eclipse.org/tahu/spec/Sparkplug%20Topic%20Namespace%20and%20State%20ManagementV2.2-with%20appendix%20B%20format%20-%20Eclipse.pdf](https://www.eclipse.org/tahu/spec/Sparkplug Topic Namespace and State ManagementV2.2-with appendix B format - Eclipse.pdf)
-
-
-
-## Eclipse Tahu spB v1.0 implementation
-
-Eclipse Tahu provide client libraries and reference implementations in various languages and for various devices to show how the device/remote application must connect and disconnect from the MQTT server using the Sparkplug specification explained below.  This includes device lifecycle messages such as the required birth and last will & testament messages that must be sent to ensure the device lifecycle state and data integrity.
-
-The *mqtt-spb-wrapper* python module uses the open source Sparkplug core function from Eclipse Tahu repository, located at: https://github.com/eclipse/tahu (The current release used is v0.5.15 ).
-
-For more information visit : https://github.com/eclipse/tahu
-
+Metadata-Version: 2.1
+Name: mqtt_spb_wrapper
+Version: 1.0.20
+Summary: MQTT Sparkplug B v1.0 Wrapper
+Author: Javier FG
+Project-URL: Homepage, https://github.com/javier-fg/mqtt-spb-wrapper
+Keywords: sparkplug,mqtt,ecliplse,tahu,iiot,iot
+Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: paho_mqtt==1.6.1
+Requires-Dist: protobuf==3.20.3
+
+# Python Sparkplug B Wrapper
+
+This python module implements an easy way to create Sparkplug B entities on Python, abstracting one level up the already existing python Eclipse Tahu Sparkplug B v1.0 core modules.
+
+The *mqtt-spb-wrapper* python module provides the following high level objects to handle generic Sparkplug B entities in an easy way:
+
+- **MqttSpbEntityEdgeNode** - End of Network (EoN) entity 
+  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD as well as to the STATUS messages from the SCADA application.
+- **MqttSpbEntityDevice** - End of Network Device (EoND) entity 
+  - This entity that can publish DDATA, DBIRTH, DDEATH messages and subscribe to its own commands DCMD as well as to the STATUS messages from the SCADA application.
+- **MqttSpbEntityApplication** - Application entity 
+  - This entity can publish NDATA, NBIRTH, NDEATH messages and subscribe to its own commands NCMD, to the STATUS messages from the SCADA application as well as to all other messages from the Sparkplug B Domain ID.
+- **MqttSpbEntityScada** - SCADA entity 
+  - This entity can publish NDATA, NBIRTH, NDEATH messages as well as to send commands to all EoN and EoND (NCMD, DCMD), and subscribe to all other messages from the Sparkplug B Domain ID.
+
+Other helper classes:
+
+- **MqttSpbPayload**
+  - Class to decode the Sparkplug B binary payloads ( Google protobuf format )
+- **MqttSpbTopic** 
+  - Class to parse, decode and handle MQTT Sparkplug B topics.
+
+## Examples
+
+The repository includes a folder with some basic examples for the different type of entities, **see the folder /examples** in this repository for more examples.
+
+### Basic EoN Device
+
+The following code shows how to create an EoND entity that transmit some simple data.
+
+```python
+import time
+from mqtt_spb_wrapper import *
+
+_DEBUG = True  # Enable debug messages
+
+print("--- Sparkplug B example - End of Node Device - Simple")
+
+
+def callback_command(payload):
+    print("DEVICE received CMD: %s" % (payload))
+
+
+def callback_message(topic, payload):
+    print("Received MESSAGE: %s - %s" % (topic, payload))
+
+
+# Create the spB entity object
+group_name = "Group-001"
+edge_node_name = "Gateway-001"
+device_name = "SimpleEoND-01"
+
+device = MqttSpbEntityDevice(group_name, edge_node_name, device_name, _DEBUG)
+
+device.on_message = callback_message  # Received messages
+device.on_command = callback_command  # Callback for received commands
+
+# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
+
+# Attributes
+device.attributes.set_value("description", "Simple EoN Device node")
+device.attributes.set_value("type", "Simulated-EoND-device")
+device.attributes.set_value("version", "0.01")
+
+# Data / Telemetry
+device.data.set_value("value", 0)
+
+# Commands
+device.commands.set_value("rebirth", False)
+
+# Connect to the broker --------------------------------------------
+_connected = False
+while not _connected:
+    print("Trying to connect to broker...")
+    _connected = device.connect("localhost8", 1883)
+    if not _connected:
+        print("  Error, could not connect. Trying again in a few seconds ...")
+        time.sleep(3)
+
+# Send birth message
+device.publish_birth()
+
+
+# Send some telemetry values ---------------------------------------
+value = 0  # Simple counter
+for i in range(5):
+    # Update the data value
+    device.data.set_value("value", value)
+
+    # Send data values
+    print("Sending data - value : %d" % value)
+    device.publish_data()
+
+    # Increase counter
+    value += 1
+
+    # Sleep some time
+    time.sleep(5)
+
+# Disconnect device -------------------------------------------------
+# After disconnection the MQTT broker will send the entity DEATH message.
+print("Disconnecting device")
+device.disconnect()
+
+print("Application finished !")
+```
+
+
+
+### Basic Listener Application
+
+The following code shows how to create an application entity to listen to all Sparkplug B messages on a given group.
+
+```python
+import time
+from mqtt_spb_wrapper import *
+
+_DEBUG = True  # Enable debug messages
+
+print("--- Sparkplug B example - Application Entity Listener")
+
+
+def callback_app_message(topic, payload):
+    print("APP received MESSAGE: %s - %s" % (topic, payload))
+
+
+def callback_app_command(payload):
+    print("APP received CMD: %s" % payload)
+
+
+domain_name = "Domain-001"
+app_entity_name = "ListenApp01"
+
+app = MqttSpbEntityApplication(domain_name, app_entity_name, debug_info=_DEBUG)
+
+# Set callbacks
+app.on_message = callback_app_message
+app.on_command = callback_app_command
+
+# Set the device Attributes, Data and Commands that will be sent on the DBIRTH message --------------------------
+
+# Attributes
+app.attributes.set_value("description", "Test application")
+
+# Commands
+app.commands.set_value("rebirth", False)
+
+# Connect to the broker----------------------------------------------------------------
+_connected = False
+while not _connected:
+    print("Trying to connect to broker...")
+    _connected = app.connect("localhost8", 1883)
+    if not _connected:
+        print("  Error, could not connect. Trying again in a few seconds ...")
+        time.sleep(3)
+
+# Send birth message
+app.publish_birth()
+
+
+# Loop forever, messages and commands will be handeled by the callbacks
+while True:
+    time.sleep(1000)
+```
+
+
+
+## Eclipse Sparkplug B v1.0
+
+Sparkplug is a specification for MQTT enabled devices and applications to send and receive messages in a stateful way. While MQTT is stateful by nature it doesn't ensure that all data on a receiving MQTT application is current or valid. Sparkplug provides a mechanism for ensuring that remote device or application data is current and valid. The main Sparkplug B features include:
+
+- Complex data types using templates
+- Datasets
+- Richer metrics with the ability to add property metadata for each metric
+- Metric alias support to maintain rich metric naming while keeping bandwidth usage to a minimum
+- Historical data
+- File data
+
+Sparkplug B Specification: [https://www.eclipse.org/tahu/spec/Sparkplug%20Topic%20Namespace%20and%20State%20ManagementV2.2-with%20appendix%20B%20format%20-%20Eclipse.pdf](https://www.eclipse.org/tahu/spec/Sparkplug Topic Namespace and State ManagementV2.2-with appendix B format - Eclipse.pdf)
+
+
+
+## Eclipse Tahu spB v1.0 implementation
+
+Eclipse Tahu provide client libraries and reference implementations in various languages and for various devices to show how the device/remote application must connect and disconnect from the MQTT server using the Sparkplug specification explained below.  This includes device lifecycle messages such as the required birth and last will & testament messages that must be sent to ensure the device lifecycle state and data integrity.
+
+The *mqtt-spb-wrapper* python module uses the open source Sparkplug core function from Eclipse Tahu repository, located at: https://github.com/eclipse/tahu (The current release used is v0.5.15 ).
+
+For more information visit : https://github.com/eclipse/tahu
+
```

### Comparing `mqtt_spb_wrapper-1.0.19/src/mqtt_spb_wrapper.egg-info/SOURCES.txt` & `mqtt_spb_wrapper-1.0.20/src/mqtt_spb_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

